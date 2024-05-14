# Comparing `tmp/jsonpath_rfc9535-0.1.1.tar.gz` & `tmp/jsonpath_rfc9535-0.1.2.tar.gz`

## Comparing `jsonpath_rfc9535-0.1.1.tar` & `jsonpath_rfc9535-0.1.2.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jsonpath_rfc9535-0.1.1/jsonpath_rfc9535/__about__.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 jsonpath_rfc9535-0.1.1/jsonpath_rfc9535/__init__.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 jsonpath_rfc9535-0.1.1/jsonpath_rfc9535/__main__.py
--rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 jsonpath_rfc9535-0.1.1/jsonpath_rfc9535/cli.py
--rw-r--r--   0        0        0     8480 2020-02-02 00:00:00.000000 jsonpath_rfc9535-0.1.1/jsonpath_rfc9535/environment.py
--rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 jsonpath_rfc9535-0.1.1/jsonpath_rfc9535/exceptions.py
--rw-r--r--   0        0        0    12845 2020-02-02 00:00:00.000000 jsonpath_rfc9535-0.1.1/jsonpath_rfc9535/filter_expressions.py
--rw-r--r--   0        0        0    14230 2020-02-02 00:00:00.000000 jsonpath_rfc9535-0.1.1/jsonpath_rfc9535/lex.py
--rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 jsonpath_rfc9535-0.1.1/jsonpath_rfc9535/node.py
--rw-r--r--   0        0        0    20958 2020-02-02 00:00:00.000000 jsonpath_rfc9535-0.1.1/jsonpath_rfc9535/parse.py
--rw-r--r--   0        0        0     4151 2020-02-02 00:00:00.000000 jsonpath_rfc9535-0.1.1/jsonpath_rfc9535/query.py
--rw-r--r--   0        0        0     5721 2020-02-02 00:00:00.000000 jsonpath_rfc9535-0.1.1/jsonpath_rfc9535/segments.py
--rw-r--r--   0        0        0     9994 2020-02-02 00:00:00.000000 jsonpath_rfc9535-0.1.1/jsonpath_rfc9535/selectors.py
--rw-r--r--   0        0        0     5614 2020-02-02 00:00:00.000000 jsonpath_rfc9535-0.1.1/jsonpath_rfc9535/tokens.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 jsonpath_rfc9535-0.1.1/jsonpath_rfc9535/function_extensions/__init__.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 jsonpath_rfc9535-0.1.1/jsonpath_rfc9535/function_extensions/count.py
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 jsonpath_rfc9535-0.1.1/jsonpath_rfc9535/function_extensions/filter_function.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 jsonpath_rfc9535-0.1.1/jsonpath_rfc9535/function_extensions/length.py
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 jsonpath_rfc9535-0.1.1/jsonpath_rfc9535/function_extensions/match.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 jsonpath_rfc9535-0.1.1/jsonpath_rfc9535/function_extensions/search.py
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 jsonpath_rfc9535-0.1.1/jsonpath_rfc9535/function_extensions/value.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jsonpath_rfc9535-0.1.1/jsonpath_rfc9535/utils/__init__.py
--rw-r--r--   0        0        0     4753 2020-02-02 00:00:00.000000 jsonpath_rfc9535-0.1.1/jsonpath_rfc9535/utils/nondeterministic_descent.py
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 jsonpath_rfc9535-0.1.1/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 jsonpath_rfc9535-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0     6547 2020-02-02 00:00:00.000000 jsonpath_rfc9535-0.1.1/README.md
--rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 jsonpath_rfc9535-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     7660 2020-02-02 00:00:00.000000 jsonpath_rfc9535-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jsonpath_rfc9535-0.1.2/jsonpath_rfc9535/__about__.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 jsonpath_rfc9535-0.1.2/jsonpath_rfc9535/__init__.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 jsonpath_rfc9535-0.1.2/jsonpath_rfc9535/__main__.py
+-rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 jsonpath_rfc9535-0.1.2/jsonpath_rfc9535/cli.py
+-rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 jsonpath_rfc9535-0.1.2/jsonpath_rfc9535/environment.py
+-rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 jsonpath_rfc9535-0.1.2/jsonpath_rfc9535/exceptions.py
+-rw-r--r--   0        0        0    12905 2020-02-02 00:00:00.000000 jsonpath_rfc9535-0.1.2/jsonpath_rfc9535/filter_expressions.py
+-rw-r--r--   0        0        0    14358 2020-02-02 00:00:00.000000 jsonpath_rfc9535-0.1.2/jsonpath_rfc9535/lex.py
+-rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 jsonpath_rfc9535-0.1.2/jsonpath_rfc9535/node.py
+-rw-r--r--   0        0        0    19557 2020-02-02 00:00:00.000000 jsonpath_rfc9535-0.1.2/jsonpath_rfc9535/parse.py
+-rw-r--r--   0        0        0     4138 2020-02-02 00:00:00.000000 jsonpath_rfc9535-0.1.2/jsonpath_rfc9535/query.py
+-rw-r--r--   0        0        0     6405 2020-02-02 00:00:00.000000 jsonpath_rfc9535-0.1.2/jsonpath_rfc9535/segments.py
+-rw-r--r--   0        0        0     9994 2020-02-02 00:00:00.000000 jsonpath_rfc9535-0.1.2/jsonpath_rfc9535/selectors.py
+-rw-r--r--   0        0        0     5506 2020-02-02 00:00:00.000000 jsonpath_rfc9535-0.1.2/jsonpath_rfc9535/tokens.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 jsonpath_rfc9535-0.1.2/jsonpath_rfc9535/function_extensions/__init__.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 jsonpath_rfc9535-0.1.2/jsonpath_rfc9535/function_extensions/_pattern.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 jsonpath_rfc9535-0.1.2/jsonpath_rfc9535/function_extensions/count.py
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 jsonpath_rfc9535-0.1.2/jsonpath_rfc9535/function_extensions/filter_function.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 jsonpath_rfc9535-0.1.2/jsonpath_rfc9535/function_extensions/length.py
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 jsonpath_rfc9535-0.1.2/jsonpath_rfc9535/function_extensions/match.py
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 jsonpath_rfc9535-0.1.2/jsonpath_rfc9535/function_extensions/search.py
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 jsonpath_rfc9535-0.1.2/jsonpath_rfc9535/function_extensions/value.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jsonpath_rfc9535-0.1.2/jsonpath_rfc9535/utils/__init__.py
+-rw-r--r--   0        0        0     5069 2020-02-02 00:00:00.000000 jsonpath_rfc9535-0.1.2/jsonpath_rfc9535/utils/nondeterministic_descent.py
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 jsonpath_rfc9535-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 jsonpath_rfc9535-0.1.2/LICENSE.txt
+-rw-r--r--   0        0        0     6533 2020-02-02 00:00:00.000000 jsonpath_rfc9535-0.1.2/README.md
+-rw-r--r--   0        0        0     4088 2020-02-02 00:00:00.000000 jsonpath_rfc9535-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     7682 2020-02-02 00:00:00.000000 jsonpath_rfc9535-0.1.2/PKG-INFO
```

### Comparing `jsonpath_rfc9535-0.1.1/jsonpath_rfc9535/__init__.py` & `jsonpath_rfc9535-0.1.2/jsonpath_rfc9535/__init__.py`

 * *Files identical despite different names*

### Comparing `jsonpath_rfc9535-0.1.1/jsonpath_rfc9535/cli.py` & `jsonpath_rfc9535-0.1.2/jsonpath_rfc9535/cli.py`

 * *Files identical despite different names*

### Comparing `jsonpath_rfc9535-0.1.1/jsonpath_rfc9535/environment.py` & `jsonpath_rfc9535-0.1.2/jsonpath_rfc9535/environment.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,15 +213,15 @@
                 ):
                     raise JSONPathTypeError(
                         f"{token.value}() argument {idx} must be of ValueType",
                         token=token,
                     )
             elif typ == ExpressionType.LOGICAL:
                 if not isinstance(
-                    arg, (FilterQuery, (LogicalExpression, ComparisonExpression))
+                    arg, (FilterQuery, LogicalExpression, ComparisonExpression)
                 ):
                     raise JSONPathTypeError(
                         f"{token.value}() argument {idx} must be of LogicalType",
                         token=token,
                     )
             elif typ == ExpressionType.NODES and not (
                 isinstance(arg, FilterQuery)
```

### Comparing `jsonpath_rfc9535-0.1.1/jsonpath_rfc9535/exceptions.py` & `jsonpath_rfc9535-0.1.2/jsonpath_rfc9535/exceptions.py`

 * *Files identical despite different names*

### Comparing `jsonpath_rfc9535-0.1.1/jsonpath_rfc9535/filter_expressions.py` & `jsonpath_rfc9535-0.1.2/jsonpath_rfc9535/filter_expressions.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,14 +182,15 @@
             and self.left == other.left
             and self.operator == other.operator
             and self.right == other.right
         )
 
     def evaluate(self, context: FilterContext) -> bool:
         """Evaluate the filter expression in the given _context_."""
+        # TODO: sort circuit eval of right if left is false
         return _compare(
             self.left.evaluate(context), self.operator, self.right.evaluate(context)
         )
 
 
 class ComparisonExpression(Expression):
     """A pair of expressions and a comparison operator."""
```

### Comparing `jsonpath_rfc9535-0.1.1/jsonpath_rfc9535/lex.py` & `jsonpath_rfc9535-0.1.2/jsonpath_rfc9535/lex.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 from .exceptions import JSONPathLexerError
 from .exceptions import JSONPathSyntaxError
 from .tokens import Token
 from .tokens import TokenType
 
 RE_WHITESPACE = re.compile(r"[ \n\r\t]+")
 RE_PROPERTY = re.compile(r"[\u0080-\uFFFFa-zA-Z_][\u0080-\uFFFFa-zA-Z0-9_-]*")
-RE_INDEX = re.compile(r"-?\d+")
+RE_INDEX = re.compile(r"-?[0-9]+")
 RE_INT = re.compile(r"-?[0-9]+")
-RE_EXPONENT = re.compile(r"e[+-]?\d+")
-RE_NEGATIVE_EXPONENT = re.compile(r"e-\d+")
+RE_EXPONENT = re.compile(r"e[+-]?[0-9]+")
+RE_NEGATIVE_EXPONENT = re.compile(r"e-[0-9]+")
 RE_FUNCTION_NAME = re.compile(r"[a-z][a-z_0-9]*")
 RE_AND = re.compile(r"&&")
 RE_OR = re.compile(r"\|\|")
 RE_TRUE = re.compile(r"true")
 RE_FALSE = re.compile(r"false")
 RE_NULL = re.compile(r"null")
 RE_ESCAPE = re.compile(r"\\[bfnrtu/]")
@@ -38,15 +38,15 @@
         self.filter_depth = 0
         """Filter nesting level."""
 
         self.paren_stack: List[int] = []
         """A running count of parentheses for each, possibly nested, function call.
         
         If the stack is empty, we are not in a function call. Remember that
-        function arguments can use arbitrarily nested in parentheses.
+        function arguments can be arbitrarily nested in parentheses.
         """
 
         self.tokens: List[Token] = []
         """Tokens resulting from scanning a JSONPath expression."""
 
         self.start = 0
         """Pointer to the start of the current token."""
@@ -154,17 +154,18 @@
         l.error(f"expected '$', found {c!r}")
         return None
 
     l.emit(TokenType.ROOT)
     return lex_segment
 
 
-def lex_segment(l: Lexer) -> Optional[StateFn]:  # noqa: D103
+def lex_segment(l: Lexer) -> Optional[StateFn]:  # noqa: D103, PLR0911
     if l.ignore_whitespace() and not l.peek():
         l.error("unexpected trailing whitespace")
+        return None
 
     c = l.next()
 
     if c == "":
         l.emit(TokenType.EOF)
         return None
 
@@ -277,28 +278,32 @@
             # Quoted dict/object key/property name
             return lex_double_quoted_string_inside_bracket_segment
 
         # default
         l.backup()
 
         if l.accept_match(RE_INDEX):
-            # Index selector of part of a slice selector.
+            # Index selector or part of a slice selector.
             l.emit(TokenType.INDEX)
             continue
 
         l.error(f"unexpected token {c!r} in bracketed selection")
         return None
 
 
 def lex_inside_filter(l: Lexer) -> Optional[StateFn]:  # noqa: D103, PLR0915, PLR0912, PLR0911
     while True:
         l.ignore_whitespace()
         c = l.next()
 
-        if c in ("", "]"):
+        if c == "":
+            l.error("unclosed bracketed selection")
+            return None
+
+        if c == "]":
             l.filter_depth -= 1
             if len(l.paren_stack) == 1:
                 l.error("unbalanced parentheses")
                 return None
 
             l.backup()
             return lex_inside_bracketed_segment
```

### Comparing `jsonpath_rfc9535-0.1.1/jsonpath_rfc9535/node.py` & `jsonpath_rfc9535-0.1.2/jsonpath_rfc9535/node.py`

 * *Files identical despite different names*

### Comparing `jsonpath_rfc9535-0.1.1/jsonpath_rfc9535/parse.py` & `jsonpath_rfc9535-0.1.2/jsonpath_rfc9535/parse.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """The default JSONPath parser."""
 
 from __future__ import annotations
 
 import json
-import re
 from typing import TYPE_CHECKING
 from typing import Callable
 from typing import Dict
 from typing import Iterable
 from typing import List
 from typing import Optional
 from typing import Tuple
@@ -47,49 +46,14 @@
 
 if TYPE_CHECKING:
     from .environment import JSONPathEnvironment
     from .tokens import TokenStream
 
 # ruff: noqa: D102
 
-INVALID_NAME_SELECTOR_CHARS = [
-    "\x00",
-    "\x01",
-    "\x02",
-    "\x03",
-    "\x04",
-    "\x05",
-    "\x06",
-    "\x07",
-    "\x08",
-    "\t",
-    "\n",
-    "\x0b",
-    "\x0c",
-    "\r",
-    "\x0e",
-    "\x0f",
-    "\x10",
-    "\x11",
-    "\x12",
-    "\x13",
-    "\x14",
-    "\x15",
-    "\x16",
-    "\x17",
-    "\x18",
-    "\x19",
-    "\x1a",
-    "\x1b",
-    "\x1c",
-    "\x1d",
-    "\x1e",
-    "\x1f",
-]
-
 
 class Parser:
     """A JSONPath expression parser bound to a `JSONPathEnvironment`."""
 
     PRECEDENCE_LOWEST = 1
     PRECEDENCE_LOGICAL_OR = 3
     PRECEDENCE_LOGICAL_AND = 4
@@ -98,30 +62,28 @@
 
     PRECEDENCES = {
         TokenType.AND: PRECEDENCE_LOGICAL_AND,
         TokenType.EQ: PRECEDENCE_RELATIONAL,
         TokenType.GE: PRECEDENCE_RELATIONAL,
         TokenType.GT: PRECEDENCE_RELATIONAL,
         TokenType.LE: PRECEDENCE_RELATIONAL,
-        TokenType.LG: PRECEDENCE_RELATIONAL,
         TokenType.LT: PRECEDENCE_RELATIONAL,
         TokenType.NE: PRECEDENCE_RELATIONAL,
         TokenType.NOT: PRECEDENCE_PREFIX,
         TokenType.OR: PRECEDENCE_LOGICAL_OR,
         TokenType.RPAREN: PRECEDENCE_LOWEST,
     }
 
     # Mapping of operator token to canonical string.
     BINARY_OPERATORS = {
         TokenType.AND: "&&",
         TokenType.EQ: "==",
         TokenType.GE: ">=",
         TokenType.GT: ">",
         TokenType.LE: "<=",
-        TokenType.LG: "<>",
         TokenType.LT: "<",
         TokenType.NE: "!=",
         TokenType.OR: "||",
     }
 
     COMPARISON_OPERATORS = frozenset(
         [
@@ -130,87 +92,69 @@
             ">",
             "<=",
             "<",
             "!=",
         ]
     )
 
-    PREFIX_OPERATORS = frozenset(
-        [
-            TokenType.NOT,
-        ]
-    )
-
-    _INVALID_NAME_SELECTOR_CHARS = f"[{''.join(INVALID_NAME_SELECTOR_CHARS)}]"
-    RE_INVALID_NAME_SELECTOR = re.compile(
-        rf'(?:(?!(?<!\\)"){_INVALID_NAME_SELECTOR_CHARS})'
-    )
-
     def __init__(self, *, env: JSONPathEnvironment) -> None:
         self.env = env
 
         self.token_map: Dict[TokenType, Callable[[TokenStream], Expression]] = {
             TokenType.DOUBLE_QUOTE_STRING: self.parse_string_literal,
             TokenType.FALSE: self.parse_boolean,
             TokenType.FLOAT: self.parse_float_literal,
             TokenType.FUNCTION: self.parse_function_extension,
             TokenType.INT: self.parse_integer_literal,
             TokenType.LPAREN: self.parse_grouped_expression,
             TokenType.NOT: self.parse_prefix_expression,
-            TokenType.NULL: self.parse_nil,
-            TokenType.ROOT: self.parse_root_path,
-            TokenType.CURRENT: self.parse_self_path,
+            TokenType.NULL: self.parse_null,
+            TokenType.ROOT: self.parse_root_query,
+            TokenType.CURRENT: self.parse_relative_query,
             TokenType.SINGLE_QUOTE_STRING: self.parse_string_literal,
             TokenType.TRUE: self.parse_boolean,
         }
 
-        self.list_item_map: Dict[TokenType, Callable[[TokenStream], Expression]] = {
-            TokenType.FALSE: self.parse_boolean,
-            TokenType.FLOAT: self.parse_float_literal,
-            TokenType.INT: self.parse_integer_literal,
-            TokenType.NULL: self.parse_nil,
-            TokenType.DOUBLE_QUOTE_STRING: self.parse_string_literal,
-            TokenType.SINGLE_QUOTE_STRING: self.parse_string_literal,
-            TokenType.TRUE: self.parse_boolean,
-        }
+        # TODO: can a function argument be a grouped expression?
+        # TODO: can a function argument contain a !?
 
         self.function_argument_map: Dict[
             TokenType, Callable[[TokenStream], Expression]
         ] = {
             TokenType.DOUBLE_QUOTE_STRING: self.parse_string_literal,
             TokenType.FALSE: self.parse_boolean,
             TokenType.FLOAT: self.parse_float_literal,
             TokenType.FUNCTION: self.parse_function_extension,
             TokenType.INT: self.parse_integer_literal,
-            TokenType.NULL: self.parse_nil,
-            TokenType.ROOT: self.parse_root_path,
-            TokenType.CURRENT: self.parse_self_path,
+            TokenType.NULL: self.parse_null,
+            TokenType.ROOT: self.parse_root_query,
+            TokenType.CURRENT: self.parse_relative_query,
             TokenType.SINGLE_QUOTE_STRING: self.parse_string_literal,
             TokenType.TRUE: self.parse_boolean,
         }
 
     def parse(self, stream: TokenStream) -> Iterable[JSONPathSegment]:
-        """Parse a JSONPath from a stream of tokens."""
+        """Parse a JSONPath expression from a stream of tokens."""
         stream.expect(TokenType.ROOT)
         stream.next_token()
-        yield from self.parse_path(stream, in_filter=False)
+        yield from self.parse_query(stream, in_filter=False)
 
         if stream.current.type_ != TokenType.EOF:
             raise JSONPathSyntaxError(
                 f"unexpected token {stream.current.value!r}",
                 token=stream.current,
             )
 
-    def parse_path(
+    def parse_query(
         self,
         stream: TokenStream,
         *,
         in_filter: bool = False,
     ) -> Iterable[JSONPathSegment]:
-        """Parse a top-level JSONPath, or one that is nested in a filter."""
+        """Parse a top-level JSONPath expression or a filter query."""
         while True:
             if stream.current.type_ == TokenType.DOUBLE_DOT:
                 tok = stream.next_token()
                 selectors = self.parse_selectors(stream)
                 yield JSONPathRecursiveDescentSegment(
                     env=self.env,
                     token=tok,
@@ -251,15 +195,15 @@
 
         if stream.current.type_ == TokenType.LBRACKET:
             return tuple(self.parse_bracketed_selection(stream))
 
         return ()
 
     def parse_slice(self, stream: TokenStream) -> SliceSelector:
-        """Parse a slice JSONPath expression from a stream of tokens."""
+        """Parse a slice selector."""
         tok = stream.current
         start: Optional[int] = None
         stop: Optional[int] = None
         step: Optional[int] = None
 
         def _maybe_index(token: Token) -> bool:
             if token.type_ == TokenType.INDEX:
@@ -284,15 +228,15 @@
             stream.next_token()
             if stream.current.type_ == TokenType.COLON:
                 stream.next_token()
         elif stream.current.type_ == TokenType.COLON:
             stream.expect(TokenType.COLON)
             stream.next_token()
 
-        # // 1 or ?
+        # 1 or ?
         if _maybe_index(stream.current):
             step = int(stream.current.value)
             stream.next_token()
 
         stream.push(stream.current)
 
         return SliceSelector(
@@ -300,15 +244,15 @@
             token=tok,
             start=start,
             stop=stop,
             step=step,
         )
 
     def parse_bracketed_selection(self, stream: TokenStream) -> List[JSONPathSelector]:  # noqa: PLR0912
-        """Parse a comma separated list JSONPath selectors from a stream of tokens."""
+        """Parse a comma separated list of JSONPath selectors."""
         tok = stream.next_token()  # Skip LBRACKET
         selectors: List[JSONPathSelector] = []
 
         while stream.current.type_ != TokenType.RBRACKET:
             if stream.current.type_ == TokenType.INDEX:
                 if stream.peek.type_ == TokenType.COLON:
                     selectors.append(self.parse_slice(stream))
@@ -327,20 +271,14 @@
                             index=int(stream.current.value),
                         )
                     )
             elif stream.current.type_ in (
                 TokenType.DOUBLE_QUOTE_STRING,
                 TokenType.SINGLE_QUOTE_STRING,
             ):
-                if self.RE_INVALID_NAME_SELECTOR.search(stream.current.value):
-                    raise JSONPathSyntaxError(
-                        f"invalid name selector {stream.current.value!r}",
-                        token=stream.current,
-                    )
-
                 selectors.append(
                     NameSelector(
                         env=self.env,
                         token=stream.current,
                         name=self._decode_string_literal(stream.current),
                     ),
                 )
@@ -411,15 +349,15 @@
         )
 
     def parse_boolean(self, stream: TokenStream) -> Expression:
         if stream.current.type_ == TokenType.TRUE:
             return BooleanLiteral(stream.current, True)  # noqa: FBT003
         return BooleanLiteral(stream.current, False)  # noqa: FBT003
 
-    def parse_nil(self, stream: TokenStream) -> Expression:
+    def parse_null(self, stream: TokenStream) -> Expression:
         return NullLiteral(stream.current, None)
 
     def parse_string_literal(self, stream: TokenStream) -> Expression:
         return StringLiteral(
             stream.current, value=self._decode_string_literal(stream.current)
         )
 
@@ -473,36 +411,37 @@
         stream.next_token()
 
         while stream.current.type_ != TokenType.RPAREN:
             if stream.current.type_ == TokenType.EOF:
                 raise JSONPathSyntaxError(
                     "unbalanced parentheses", token=stream.current
                 )
+            # TODO: only if binary op
             expr = self.parse_infix_expression(stream, expr)
 
         stream.expect(TokenType.RPAREN)
         return expr
 
-    def parse_root_path(self, stream: TokenStream) -> Expression:
+    def parse_root_query(self, stream: TokenStream) -> Expression:
         root = stream.next_token()
         assert root.type_ == TokenType.ROOT
         return RootFilterQuery(
             token=root,
             query=JSONPathQuery(
                 env=self.env,
-                segments=tuple(self.parse_path(stream, in_filter=True)),
+                segments=tuple(self.parse_query(stream, in_filter=True)),
             ),
         )
 
-    def parse_self_path(self, stream: TokenStream) -> Expression:
+    def parse_relative_query(self, stream: TokenStream) -> Expression:
         tok = stream.next_token()
         return RelativeFilterQuery(
             token=tok,
             query=JSONPathQuery(
-                env=self.env, segments=tuple(self.parse_path(stream, in_filter=True))
+                env=self.env, segments=tuple(self.parse_query(stream, in_filter=True))
             ),
         )
 
     def parse_function_extension(self, stream: TokenStream) -> Expression:
         function_arguments: List[Expression] = []
         tok = stream.next_token()
```

### Comparing `jsonpath_rfc9535-0.1.1/jsonpath_rfc9535/query.py` & `jsonpath_rfc9535-0.1.2/jsonpath_rfc9535/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
             a `Parser`.
 
     Attributes:
         env: The `JSONPathEnvironment` this query is bound to.
         segments: The `JSONPathSegment` instances that make up this query.
     """
 
-    __slots__ = ("env", "fake_root", "segments")
+    __slots__ = ("env", "segments")
 
     def __init__(
         self,
         *,
         env: JSONPathEnvironment,
         segments: Tuple[JSONPathSegment, ...],
     ) -> None:
```

### Comparing `jsonpath_rfc9535-0.1.1/jsonpath_rfc9535/segments.py` & `jsonpath_rfc9535-0.1.2/jsonpath_rfc9535/segments.py`

 * *Files 10% similar despite different names*

```diff
@@ -65,32 +65,25 @@
 
 
 class JSONPathRecursiveDescentSegment(JSONPathSegment):
     """The JSONPath recursive descent segment."""
 
     def resolve(self, nodes: Iterable[JSONPathNode]) -> Iterable[JSONPathNode]:
         """Select descendants of each node in _nodes_."""
-        # The nondeterministic visitor never generates a pre order traversal, so we
-        # still use the deterministic visitor 20% of the time, to cover all
-        # permutations.
-        #
-        # XXX: This feels like a bit of a hack.
         visitor = (
-            self._nondeterministic_visit
-            if self.env.nondeterministic and random.random() < 0.2  # noqa: S311, PLR2004
-            else self._visit
+            self._nondeterministic_visit if self.env.nondeterministic else self._visit
         )
 
         for node in nodes:
             for _node in visitor(node):
                 for selector in self.selectors:
                     yield from selector.resolve(_node)
 
     def _visit(self, node: JSONPathNode, depth: int = 1) -> Iterable[JSONPathNode]:
-        """Pre order node traversal."""
+        """Depth-first, pre-order node traversal."""
         if depth > self.env.max_recursion_depth:
             raise JSONPathRecursionError("recursion limit exceeded", token=self.token)
 
         yield node
 
         if isinstance(node.value, dict):
             for name, val in node.value.items():
@@ -110,56 +103,87 @@
                         root=node.root,
                     )
                     yield from self._visit(_node, depth + 1)
 
     def _nondeterministic_visit(
         self,
         root: JSONPathNode,
-        _: int = 1,
+        depth: int = 1,
     ) -> Iterable[JSONPathNode]:
-        def _children(node: JSONPathNode) -> Iterable[JSONPathNode]:
-            if isinstance(node.value, dict):
-                items = list(node.value.items())
-                random.shuffle(items)
-                for name, val in items:
-                    if isinstance(val, (dict, list)):
-                        yield JSONPathNode(
-                            value=val,
-                            location=node.location + (name,),
-                            root=node.root,
-                        )
-            elif isinstance(node.value, list):
-                for i, element in enumerate(node.value):
-                    if isinstance(element, (dict, list)):
-                        yield JSONPathNode(
-                            value=element,
-                            location=node.location + (i,),
-                            root=node.root,
-                        )
+        """Nondeterministic node traversal."""
+        # (node, depth) tuples
+        queue: Deque[Tuple[JSONPathNode, int]] = deque()
 
-        queue: Deque[JSONPathNode] = deque(_children(root))
+        # Visit the root node
         yield root
 
+        # Queue root's children
+        queue.extend([(child, depth) for child in _nondeterministic_children(root)])
+
         while queue:
-            _node = queue.popleft()
-            yield _node
-            # Visit child nodes now or queue them for later?
+            node, depth = queue.popleft()
+            yield node
+
+            if depth >= self.env.max_recursion_depth:
+                raise JSONPathRecursionError(
+                    "recursion limit exceeded", token=self.token
+                )
+
+            # Randomly choose to visit child nodes now or queue them for later?
             visit_children = random.choice([True, False])  # noqa: S311
-            for child in _children(_node):
+
+            for child in _nondeterministic_children(node):
                 if visit_children:
                     yield child
-                    queue.extend(_children(child))
+
+                    # Queue grandchildren by randomly interleaving them into the
+                    # queue while maintaining queue and grandchild order.
+                    grandchildren = [
+                        (child, depth + 2)
+                        for child in _nondeterministic_children(child)
+                    ]
+
+                    queue = deque(
+                        [
+                            next(n)
+                            for n in random.sample(
+                                [iter(queue)] * len(queue)
+                                + [iter(grandchildren)] * len(grandchildren),
+                                len(queue) + len(grandchildren),
+                            )
+                        ]
+                    )
                 else:
-                    queue.append(child)
+                    queue.append((child, depth + 1))
 
     def __str__(self) -> str:
         return f"..[{', '.join(str(itm) for itm in self.selectors)}]"
 
     def __eq__(self, __value: object) -> bool:
         return (
             isinstance(__value, JSONPathRecursiveDescentSegment)
             and self.selectors == __value.selectors
             and self.token == __value.token
         )
 
     def __hash__(self) -> int:
         return hash(("..", self.selectors, self.token))
+
+
+def _nondeterministic_children(node: JSONPathNode) -> Iterable[JSONPathNode]:
+    """Yield children of _node_ with nondeterministic object/dict iteration."""
+    if isinstance(node.value, dict):
+        items = list(node.value.items())
+        random.shuffle(items)
+        for name, val in items:
+            yield JSONPathNode(
+                value=val,
+                location=node.location + (name,),
+                root=node.root,
+            )
+    elif isinstance(node.value, list):
+        for i, element in enumerate(node.value):
+            yield JSONPathNode(
+                value=element,
+                location=node.location + (i,),
+                root=node.root,
+            )
```

### Comparing `jsonpath_rfc9535-0.1.1/jsonpath_rfc9535/selectors.py` & `jsonpath_rfc9535-0.1.2/jsonpath_rfc9535/selectors.py`

 * *Files identical despite different names*

### Comparing `jsonpath_rfc9535-0.1.1/jsonpath_rfc9535/tokens.py` & `jsonpath_rfc9535-0.1.2/jsonpath_rfc9535/tokens.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,45 +14,40 @@
 
 
 class TokenType(Enum):
     """JSONPath expression token types."""
 
     EOF = auto()
     ERROR = auto()
-    SKIP = auto()
+    INIT = auto()
 
     SHORTHAND_PROPERTY = auto()
     COLON = auto()
     COMMA = auto()
     DOT = auto()
     DOUBLE_DOT = auto()
     FILTER = auto()
     INDEX = auto()
     LBRACKET = auto()
     PROPERTY = auto()
     RBRACKET = auto()
     ROOT = auto()
-    SLICE = auto()
-    SLICE_START = auto()
-    SLICE_STEP = auto()
-    SLICE_STOP = auto()
     WILD = auto()
 
     AND = auto()
     CURRENT = auto()
     DOUBLE_QUOTE_STRING = auto()
     EQ = auto()
     FALSE = auto()
     FLOAT = auto()
     FUNCTION = auto()
     GE = auto()
     GT = auto()
     INT = auto()
     LE = auto()
-    LG = auto()
     LPAREN = auto()
     LT = auto()
     NE = auto()
     NOT = auto()
     NULL = auto()
     OP = auto()
     OR = auto()
@@ -113,15 +108,15 @@
 
 class TokenStream:
     """Step through or iterate a stream of tokens."""
 
     def __init__(self, token_iter: Iterable[Token]):
         self.iter = iter(token_iter)
         self._pushed: Deque[Token] = deque()
-        self.current = Token(TokenType.SKIP, "", -1, "")
+        self.current = Token(TokenType.INIT, "", -1, "")
         next(self)
 
     class TokenStreamIterator:
         """An iterable token stream."""
 
         def __init__(self, stream: TokenStream):
             self.stream = stream
```

### Comparing `jsonpath_rfc9535-0.1.1/jsonpath_rfc9535/function_extensions/count.py` & `jsonpath_rfc9535-0.1.2/jsonpath_rfc9535/function_extensions/count.py`

 * *Files identical despite different names*

### Comparing `jsonpath_rfc9535-0.1.1/jsonpath_rfc9535/function_extensions/filter_function.py` & `jsonpath_rfc9535-0.1.2/jsonpath_rfc9535/function_extensions/filter_function.py`

 * *Files identical despite different names*

### Comparing `jsonpath_rfc9535-0.1.1/jsonpath_rfc9535/function_extensions/length.py` & `jsonpath_rfc9535-0.1.2/jsonpath_rfc9535/function_extensions/length.py`

 * *Files identical despite different names*

### Comparing `jsonpath_rfc9535-0.1.1/jsonpath_rfc9535/function_extensions/match.py` & `jsonpath_rfc9535-0.1.2/jsonpath_rfc9535/function_extensions/match.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 """The standard `match` function extension."""
 
 import regex as re
+from iregexp_check import check
 
 from jsonpath_rfc9535.function_extensions import ExpressionType
 from jsonpath_rfc9535.function_extensions import FilterFunction
 
+from ._pattern import map_re
+
 
 class Match(FilterFunction):
     """The standard `match` function."""
 
     arg_types = [ExpressionType.VALUE, ExpressionType.VALUE]
     return_type = ExpressionType.LOGICAL
 
-    def __call__(self, string: str, pattern: str) -> bool:
+    def __call__(self, string: str, pattern: object) -> bool:
         """Return `True` if _string_ matches _pattern_, or `False` otherwise."""
+        if not isinstance(pattern, str) or not check(pattern):
+            return False
+
         try:
             # re.fullmatch caches compiled patterns internally
-            return bool(re.fullmatch(pattern, string))
+            return bool(re.fullmatch(map_re(pattern), string))
         except (TypeError, re.error):
             return False
```

### Comparing `jsonpath_rfc9535-0.1.1/jsonpath_rfc9535/function_extensions/search.py` & `jsonpath_rfc9535-0.1.2/jsonpath_rfc9535/function_extensions/search.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 """The standard `search` function extension."""
 
 import regex as re
+from iregexp_check import check
 
 from jsonpath_rfc9535.function_extensions import ExpressionType
 from jsonpath_rfc9535.function_extensions import FilterFunction
 
+from ._pattern import map_re
+
 
 class Search(FilterFunction):
     """The standard `search` function."""
 
     arg_types = [ExpressionType.VALUE, ExpressionType.VALUE]
     return_type = ExpressionType.LOGICAL
 
-    def __call__(self, string: str, pattern: str) -> bool:
+    def __call__(self, string: str, pattern: object) -> bool:
         """Return `True` if _string_ contains _pattern_, or `False` otherwise."""
+        if not isinstance(pattern, str) or not check(pattern):
+            return False
+
         try:
             # re.search caches compiled patterns internally
-            return bool(re.search(pattern, string))
+            return bool(re.search(map_re(pattern), string, re.VERSION1))
         except (TypeError, re.error):
             return False
```

### Comparing `jsonpath_rfc9535-0.1.1/jsonpath_rfc9535/function_extensions/value.py` & `jsonpath_rfc9535-0.1.2/jsonpath_rfc9535/function_extensions/value.py`

 * *Files identical despite different names*

### Comparing `jsonpath_rfc9535-0.1.1/jsonpath_rfc9535/utils/nondeterministic_descent.py` & `jsonpath_rfc9535-0.1.2/jsonpath_rfc9535/utils/nondeterministic_descent.py`

 * *Files 6% similar despite different names*

```diff
@@ -117,34 +117,42 @@
     while queue:
         _node = queue.popleft()
         yield _node
         queue.extend(_node.children)
 
 
 def nondeterministic_visit(root: AuxNode) -> Iterable[AuxNode]:
-    """Generate nodes rooted at _node_ from a nondeterministic traversal.
-
-    This tree visitor will never produce nodes in depth-first pre-order, so
-    use `pre_order_visit` in addition to `nondeterministic_visit` to get all
-    permutations. Or use `all_perms()`.
-    """
-    queue: Deque[AuxNode] = deque(root.children)
+    """Generate nodes rooted at _node_ from a nondeterministic traversal."""
     yield root
+    queue: Deque[AuxNode] = deque(root.children)
 
     while queue:
         _node = queue.popleft()
         yield _node
-        # Visit child nodes now or queue them for later?
+        # Randomly choose to visit child nodes now or queue them for later?
         visit_children = random.choice([True, False])
         for child in _node.children:
             if visit_children:
                 yield child
-                queue.extend(child.children)
+
+                # Queue grandchildren by randomly interleaving them into the
+                # queue while maintaining queue and grandchild order.
+                grandchildren = child.children
+
+                queue = deque(
+                    [
+                        next(n)
+                        for n in random.sample(
+                            [iter(queue)] * len(queue)
+                            + [iter(grandchildren)] * len(grandchildren),
+                            len(queue) + len(grandchildren),
+                        )
+                    ]
+                )
             else:
                 queue.append(child)
 
 
 def all_perms(root: AuxNode) -> List[Tuple[AuxNode, ...]]:
     """Return a list of valid permutations for the auxiliary tree _root_."""
     perms = {tuple(nondeterministic_visit(root)) for _ in range(1000)}
-    perms.add(tuple(pre_order_visit(root)))
     return sorted(perms, key=lambda t: str(t))
```

### Comparing `jsonpath_rfc9535-0.1.1/.gitignore` & `jsonpath_rfc9535-0.1.2/.gitignore`

 * *Files 11% similar despite different names*

```diff
@@ -80,8 +80,11 @@
 
 # Dev utils
 dev.py
 profile_.py
 
 # Test fixtures
 comparison_regression_suite.yaml
-cts.json
+cts.json
+
+# System
+.DS_Store
```

### Comparing `jsonpath_rfc9535-0.1.1/LICENSE.txt` & `jsonpath_rfc9535-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jsonpath_rfc9535-0.1.1/README.md` & `jsonpath_rfc9535-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 <p align="center">
 We follow <a href="https://datatracker.ietf.org/doc/html/rfc9535">RFC 9535</a> strictly and test against the <a href="https://github.com/jsonpath-standard/jsonpath-compliance-test-suite">JSONPath Compliance Test Suite</a>.
 </p>
 
 <p align="center">
   <a href="https://github.com/jg-rp/python-jsonpath-rfc9535/blob/main/LICENSE.txt">
-    <img src="https://img.shields.io/pypi/l/jsonpath-rfc9535?style=flat-square" alt="License">
+    <img src="https://img.shields.io/pypi/l/jsonpath-rfc9535.svg?style=flat-square" alt="License">
   </a>
   <a href="https://github.com/jg-rp/python-jsonpath-rfc9535/actions">
     <img src="https://img.shields.io/github/actions/workflow/status/jg-rp/python-jsonpath-rfc9535/tests.yaml?branch=main&label=tests&style=flat-square" alt="Tests">
   </a>
   <br>
   <a href="https://pypi.org/project/jsonpath-rfc9535">
     <img src="https://img.shields.io/pypi/v/jsonpath-rfc9535.svg?style=flat-square" alt="PyPi - Version">
@@ -93,15 +93,15 @@
 products = jsonpath.find("$..products.*", data).values()
 # ...
 ```
 
 ## Links
 
 - Change log: https://github.com/jg-rp/python-jsonpath-rfc9535/blob/main/CHANGELOG.md
-- PyPi: [TODO](https://pypi.org/project/jsonpath-rfc9535)
+- PyPi: https://pypi.org/project/jsonpath-rfc9535
 - Source code: https://github.com/jg-rp/python-jsonpath-rfc9535
 - Issue tracker: https://github.com/jg-rp/python-jsonpath-rfc9535/issues
 
 ## Related projects
 
 - [Python JSONPath](https://github.com/jg-rp/python-jsonpath) - Another Python package implementing JSONPath, but with additional features and customization options.
 - [JSON P3](https://github.com/jg-rp/json-p3) - RFC 9535 implemented in TypeScript.
@@ -198,11 +198,7 @@
 ```
 
 A `JSONPathQuery` has a `finditer(value)` method too, and `find(value)` is an alias for `apply(value)`.
 
 ## License
 
 `python-jsonpath-rfc9535` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
-
-```
-
-```
```

### Comparing `jsonpath_rfc9535-0.1.1/pyproject.toml` & `jsonpath_rfc9535-0.1.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
-dependencies = ["regex"]
+dependencies = ["regex", "iregexp-check>=0.1.3"]
 
 [project.urls]
 Documentation = "https://jg-rp.github.io/python-jsonpath-rfc9535/"
 Issues = "https://github.com/jg-rp/python-jsonpath-rfc9535/issues"
 Source = "https://github.com/jg-rp/python-jsonpath-rfc9535"
 
 [project.scripts]
```

### Comparing `jsonpath_rfc9535-0.1.1/PKG-INFO` & `jsonpath_rfc9535-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jsonpath-rfc9535
-Version: 0.1.1
+Version: 0.1.2
 Summary: RFC 9535 - JSONPath: Query Expressions for JSON in Python
 Project-URL: Documentation, https://jg-rp.github.io/python-jsonpath-rfc9535/
 Project-URL: Issues, https://github.com/jg-rp/python-jsonpath-rfc9535/issues
 Project-URL: Source, https://github.com/jg-rp/python-jsonpath-rfc9535
 Author-email: James Prior <jamesgr.prior@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -16,26 +16,27 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
+Requires-Dist: iregexp-check>=0.1.3
 Requires-Dist: regex
 Description-Content-Type: text/markdown
 
 <h1 align="center">RFC 9535 JSONPath: Query Expressions for JSON in Python</h1>
 
 <p align="center">
 We follow <a href="https://datatracker.ietf.org/doc/html/rfc9535">RFC 9535</a> strictly and test against the <a href="https://github.com/jsonpath-standard/jsonpath-compliance-test-suite">JSONPath Compliance Test Suite</a>.
 </p>
 
 <p align="center">
   <a href="https://github.com/jg-rp/python-jsonpath-rfc9535/blob/main/LICENSE.txt">
-    <img src="https://img.shields.io/pypi/l/jsonpath-rfc9535?style=flat-square" alt="License">
+    <img src="https://img.shields.io/pypi/l/jsonpath-rfc9535.svg?style=flat-square" alt="License">
   </a>
   <a href="https://github.com/jg-rp/python-jsonpath-rfc9535/actions">
     <img src="https://img.shields.io/github/actions/workflow/status/jg-rp/python-jsonpath-rfc9535/tests.yaml?branch=main&label=tests&style=flat-square" alt="Tests">
   </a>
   <br>
   <a href="https://pypi.org/project/jsonpath-rfc9535">
     <img src="https://img.shields.io/pypi/v/jsonpath-rfc9535.svg?style=flat-square" alt="PyPi - Version">
@@ -118,15 +119,15 @@
 products = jsonpath.find("$..products.*", data).values()
 # ...
 ```
 
 ## Links
 
 - Change log: https://github.com/jg-rp/python-jsonpath-rfc9535/blob/main/CHANGELOG.md
-- PyPi: [TODO](https://pypi.org/project/jsonpath-rfc9535)
+- PyPi: https://pypi.org/project/jsonpath-rfc9535
 - Source code: https://github.com/jg-rp/python-jsonpath-rfc9535
 - Issue tracker: https://github.com/jg-rp/python-jsonpath-rfc9535/issues
 
 ## Related projects
 
 - [Python JSONPath](https://github.com/jg-rp/python-jsonpath) - Another Python package implementing JSONPath, but with additional features and customization options.
 - [JSON P3](https://github.com/jg-rp/json-p3) - RFC 9535 implemented in TypeScript.
@@ -223,11 +224,7 @@
 ```
 
 A `JSONPathQuery` has a `finditer(value)` method too, and `find(value)` is an alias for `apply(value)`.
 
 ## License
 
 `python-jsonpath-rfc9535` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
-
-```
-
-```
```

