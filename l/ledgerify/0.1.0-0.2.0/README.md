# Comparing `tmp/ledgerify-0.1.0.tar.gz` & `tmp/ledgerify-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ledgerify-0.1.0.tar", max compression
+gzip compressed data, was "ledgerify-0.2.0.tar", max compression
```

## Comparing `ledgerify-0.1.0.tar` & `ledgerify-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    32471 2024-04-16 20:04:38.710816 ledgerify-0.1.0/LICENSE
--rw-r--r--   0        0        0      435 2024-04-16 21:48:59.099810 ledgerify-0.1.0/README.md
--rw-r--r--   0        0        0      640 2024-03-27 21:55:47.869310 ledgerify-0.1.0/pyproject.toml
--rwxr-xr-x   0        0        0    37964 2024-04-16 21:13:07.241266 ledgerify-0.1.0/src/ledgerify/ledgerify.py
--rw-r--r--   0        0        0      893 1970-01-01 00:00:00.000000 ledgerify-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    32471 2024-04-16 08:56:11.629078 ledgerify-0.2.0/LICENSE
+-rw-r--r--   0        0        0      681 2024-05-12 07:34:18.642073 ledgerify-0.2.0/README.md
+-rw-r--r--   0        0        0      640 2024-05-12 07:34:18.642073 ledgerify-0.2.0/pyproject.toml
+-rwxr-xr-x   0        0        0    39840 2024-05-14 11:44:20.646930 ledgerify-0.2.0/src/ledgerify/ledgerify.py
+-rw-r--r--   0        0        0     1139 1970-01-01 00:00:00.000000 ledgerify-0.2.0/PKG-INFO
```

### Comparing `ledgerify-0.1.0/LICENSE` & `ledgerify-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ledgerify-0.1.0/pyproject.toml` & `ledgerify-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ledgerify"
-version = "0.1.0"
+version = "0.2.0"
 description = "Ledger transactions importer"
 authors = ["Michal Goral <dev@goral.net.pl>"]
 license = "GPL-3.0"
 readme = "README.md"
 
 [tool.poetry.scripts]
 ledgerify = "ledgerify.ledgerify:main"
```

### Comparing `ledgerify-0.1.0/src/ledgerify/ledgerify.py` & `ledgerify-0.2.0/src/ledgerify/ledgerify.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 
 T = TypeVar("T")
 ConditionT = Optional[Callable[["Transaction"], bool]]
 Rule = Callable[["Transaction"], None]
 RuleList = List[Tuple[Rule, ConditionT]]
 Converter = Callable[[Any], T]
 Factory = Callable[[], T]
+LatestExtractor = Callable[[str], str]
 
 
 def eprint(*a, **kw):
     kw["file"] = sys.stderr
     print(*a, **kw)
 
 
@@ -372,14 +373,45 @@
             ret &= bool(other.description) and self.description == other.description
         if self.amount:
             ret &= bool(other.amount) and self.amount == other.amount
         if self.commodity:
             ret &= bool(other.commodity) and self.commodity == other.commodity
         return ret
 
+    # NOTE: this ISN'T commutative operation, i.e. results of lhs.cmp(rhs) and
+    # rhs.cmp(lhs) may differ!
+    #
+    # This is because lhs operand is treated as a template and if any of its
+    # fields isn't set, then rhs isn't checked against this field, but if it is
+    # set, then the corresponding field of rhs must be also set and equal.
+    def cmp(self, other, pattern_or_fn: str | LatestExtractor | None):
+        if not isinstance(other, Latest):
+            return NotImplemented
+
+        def extract(pattern_or_fn: str | LatestExtractor, what: str | None):
+            if what is None:
+                return None
+            if isinstance(pattern_or_fn, str):
+                m = re.search(pattern_or_fn, what)
+                return m[0] if m else None
+
+            ret = pattern_or_fn(what)
+            return str(ret) if ret is not None else None
+
+        ret = self.date == other.date
+        if pattern_or_fn is not None and self.description:
+            sdesc = extract(pattern_or_fn, self.description)
+            odesc = extract(pattern_or_fn, other.description)
+            ret &= odesc is not None and sdesc is not None and sdesc == odesc
+        if self.amount:
+            ret &= other.amount is not None and self.amount == other.amount
+        if self.commodity:
+            ret &= other.commodity is not None and self.commodity == other.commodity
+        return ret
+
 
 class SymbolSide(Enum):
     left = "left"
     right = "right"
     leftjoin = "leftjoin"
     rightjoin = "rightjoin"
 
@@ -839,14 +871,15 @@
 @dataclass
 class Config:
     source: Conversion[Optional[Path]] = Conversion(Path, default=None)
     filetype: Optional[str] = None  # helper to manually specify a filetype of source
     decimalmark: str = "."
     dateformat: Optional[str] = None
     timezone: Optional[str] = None
+    extractlatest: Optional[str] = r".*"
     default: DefaultTransaction = field(default_factory=DefaultTransaction)
     csv: CSV = field(default_factory=CSV)
 
     # TODO: annotate as RuleList, but it includes a type forward reference
     # ("Transaction"), which isn't defined yet and Conversion's get_type_hints
     # complains.
     _rules: List = field(default_factory=list, init=False, repr=False)
@@ -1153,25 +1186,32 @@
     if not args.latest:
         parentdir = cfg.source.parent if cfg.source else Path()
         source_name = cfg.source.name if cfg.source else "-"
         args.latest = parentdir / f".latest.{source_name}"
 
 
 def filter_latest(
-    transactions: List[Transaction], latest: List[Latest]
+    transactions: List[Transaction], latest: List[Latest], config: Config
 ) -> List[Transaction]:
     latest_copy = latest[:]
 
+    def find_latest(lhs):
+        for i, l in enumerate(latest_copy):
+            # note: order matters, see comment for Latest.cmp()
+            if l.cmp(lhs, config.extractlatest):
+                return i
+        raise ValueError(f"not found: {lhs}")
+
     def rule(transaction: Transaction):
         if latest_copy and transaction.date < latest_copy[0].date:
             return False
         elif latest_copy and transaction.date == latest_copy[0].date:
             cmp = Latest.from_transaction(transaction)
             try:
-                i = latest_copy.index(cmp)
+                i = find_latest(cmp)
                 del latest_copy[i]
             except ValueError:
                 return True
             else:
                 return False
         return True
 
@@ -1246,20 +1286,23 @@
     cfg.load(args.rules)
     override_config(cfg, args.options)
     validate_config(cfg, args)
 
     all_transactions = ordered_transactions(get_transactions(cfg))
 
     current_latest = read_latest(args.latest)
-    latest_transactions = filter_latest(all_transactions, current_latest)
+    latest_transactions = filter_latest(all_transactions, current_latest, cfg)
     new_latest = get_latest(latest_transactions)
 
     to_print = apply_rules(latest_transactions, cfg.rules)
 
-    write_latest(new_latest, args.latest)
+    if new_latest:
+        old_latest_left = [l for l in current_latest if l.date == new_latest[0].date]
+        write_latest(old_latest_left + new_latest, args.latest)
+
     # Print transactions ONLY when we're sure that ALL data is valid
     print_transactions(to_print)
 
     if not to_print:
         eprint("No transactions")
     else:
         eprint(f"Processed {len(to_print)} new transaction(s)")
```

