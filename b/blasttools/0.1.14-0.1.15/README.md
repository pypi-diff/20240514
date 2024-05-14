# Comparing `tmp/blasttools-0.1.14.tar.gz` & `tmp/blasttools-0.1.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blasttools-0.1.14.tar", max compression
+gzip compressed data, was "blasttools-0.1.15.tar", max compression
```

## Comparing `blasttools-0.1.14.tar` & `blasttools-0.1.15.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1068 2023-10-11 02:44:22.861784 blasttools-0.1.14/LICENSE
--rw-r--r--   0        0        0     2983 2024-05-09 01:30:40.236863 blasttools-0.1.14/README.md
--rw-r--r--   0        0        0        0 2023-10-11 02:44:42.585932 blasttools-0.1.14/blasttools/__init__.py
--rw-r--r--   0        0        0      290 2023-11-10 01:48:55.422665 blasttools-0.1.14/blasttools/__main__.py
--rw-r--r--   0        0        0    20571 2024-05-09 02:05:45.622412 blasttools-0.1.14/blasttools/blastapi.py
--rw-r--r--   0        0        0     8081 2024-05-09 01:32:30.185998 blasttools-0.1.14/blasttools/blastxml.py
--rw-r--r--   0        0        0     7355 2024-05-09 01:53:56.743166 blasttools-0.1.14/blasttools/cli.py
--rw-r--r--   0        0        0     2441 2023-12-06 01:23:32.917966 blasttools-0.1.14/blasttools/columns.py
--rw-r--r--   0        0        0      126 2024-04-19 05:53:19.292568 blasttools-0.1.14/blasttools/config.py
--rw-r--r--   0        0        0     1754 2024-05-09 02:10:12.165137 blasttools-0.1.14/blasttools/exact.py
--rw-r--r--   0        0        0     1207 2024-05-09 02:05:36.010314 blasttools-0.1.14/blasttools/options.py
--rw-r--r--   0        0        0    10301 2024-05-13 03:38:48.699691 blasttools-0.1.14/blasttools/plants.py
--rw-r--r--   0        0        0     8034 2024-05-13 03:38:48.535689 blasttools-0.1.14/blasttools/plants_ui.py
--rw-r--r--   0        0        0        0 2023-10-12 03:37:43.243775 blasttools-0.1.14/blasttools/py.typed
--rw-r--r--   0        0        0      409 2024-05-09 02:05:36.302317 blasttools-0.1.14/blasttools/translate.py
--rw-r--r--   0        0        0     1647 2024-05-09 02:05:36.370317 blasttools-0.1.14/blasttools/utils.py
--rw-r--r--   0        0        0      899 2024-05-13 03:37:58.035175 blasttools-0.1.14/pyproject.toml
--rw-r--r--   0        0        0     4035 1970-01-01 00:00:00.000000 blasttools-0.1.14/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-10-11 02:44:22.861784 blasttools-0.1.15/LICENSE
+-rw-r--r--   0        0        0     2983 2024-05-09 01:30:40.236863 blasttools-0.1.15/README.md
+-rw-r--r--   0        0        0        0 2023-10-11 02:44:42.585932 blasttools-0.1.15/blasttools/__init__.py
+-rw-r--r--   0        0        0      290 2023-11-10 01:48:55.422665 blasttools-0.1.15/blasttools/__main__.py
+-rw-r--r--   0        0        0    20571 2024-05-09 02:05:45.622412 blasttools-0.1.15/blasttools/blastapi.py
+-rw-r--r--   0        0        0     8081 2024-05-09 01:32:30.185998 blasttools-0.1.15/blasttools/blastxml.py
+-rw-r--r--   0        0        0     7355 2024-05-09 01:53:56.743166 blasttools-0.1.15/blasttools/cli.py
+-rw-r--r--   0        0        0     2441 2023-12-06 01:23:32.917966 blasttools-0.1.15/blasttools/columns.py
+-rw-r--r--   0        0        0      126 2024-04-19 05:53:19.292568 blasttools-0.1.15/blasttools/config.py
+-rw-r--r--   0        0        0     1754 2024-05-09 02:10:12.165137 blasttools-0.1.15/blasttools/exact.py
+-rw-r--r--   0        0        0     1207 2024-05-09 02:05:36.010314 blasttools-0.1.15/blasttools/options.py
+-rw-r--r--   0        0        0    10607 2024-05-14 06:12:46.350291 blasttools-0.1.15/blasttools/plants.py
+-rw-r--r--   0        0        0     8379 2024-05-14 06:11:15.617299 blasttools-0.1.15/blasttools/plants_ui.py
+-rw-r--r--   0        0        0        0 2023-10-12 03:37:43.243775 blasttools-0.1.15/blasttools/py.typed
+-rw-r--r--   0        0        0      409 2024-05-09 02:05:36.302317 blasttools-0.1.15/blasttools/translate.py
+-rw-r--r--   0        0        0     1647 2024-05-09 02:05:36.370317 blasttools-0.1.15/blasttools/utils.py
+-rw-r--r--   0        0        0      899 2024-05-14 06:14:09.647202 blasttools-0.1.15/pyproject.toml
+-rw-r--r--   0        0        0     4035 1970-01-01 00:00:00.000000 blasttools-0.1.15/PKG-INFO
```

### Comparing `blasttools-0.1.14/LICENSE` & `blasttools-0.1.15/LICENSE`

 * *Files identical despite different names*

### Comparing `blasttools-0.1.14/README.md` & `blasttools-0.1.15/README.md`

 * *Files identical despite different names*

### Comparing `blasttools-0.1.14/blasttools/blastapi.py` & `blasttools-0.1.15/blasttools/blastapi.py`

 * *Files identical despite different names*

### Comparing `blasttools-0.1.14/blasttools/blastxml.py` & `blasttools-0.1.15/blasttools/blastxml.py`

 * *Files identical despite different names*

### Comparing `blasttools-0.1.14/blasttools/cli.py` & `blasttools-0.1.15/blasttools/cli.py`

 * *Files identical despite different names*

### Comparing `blasttools-0.1.14/blasttools/columns.py` & `blasttools-0.1.15/blasttools/columns.py`

 * *Files identical despite different names*

### Comparing `blasttools-0.1.14/blasttools/exact.py` & `blasttools-0.1.15/blasttools/exact.py`

 * *Files identical despite different names*

### Comparing `blasttools-0.1.14/blasttools/options.py` & `blasttools-0.1.15/blasttools/options.py`

 * *Files identical despite different names*

### Comparing `blasttools-0.1.14/blasttools/plants.py` & `blasttools-0.1.15/blasttools/plants.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,26 +24,26 @@
 from .blastapi import fetch_seq as fetch_seq_raw
 from .blastapi import remove_files
 from .blastapi import safe_which
 
 PUB = "ensemblgenomes/pub/"
 TOP = PUB + "release-{release}/plants/"
 FASTAS_DIR = "ensemblgenomes/pub/release-{release}/plants/fasta/"
-PEP_DIR = TOP + "fasta/{plant}/pep"
-CDNA_DIR = TOP + "fasta/{plant}/cdna"
+TARGET_DIR = TOP + "fasta/{plant}/{seqtype}"
+
 FTPURL = "ftp.ebi.ac.uk"
 ENSEMBL = f"ftp://{FTPURL}/" + TOP + "fasta/{plant}/{seqtype}/{file}"
 SPECIES_TSV = "species_EnsemblPlants.txt"
 
 
 def blast_dir(release: int, *, kingdom: str = "plants") -> Path:
     return Path(f"ensembl{kingdom}-{release}")
 
 
-SeqType = Literal["pep", "cdna"]
+SeqType = Literal["pep", "cdna", "cds"]
 
 
 @dataclass
 class FileInfo:
     species: str
     fasta: str | None
 
@@ -71,20 +71,18 @@
     release: int,
     *,
     seqtype: SeqType = "pep",
 ) -> Iterator[FileInfo]:
     from .config import FTP_TIMEOUT
 
     tail = f".{seqtype}.all.fa.gz"
-    dirname = PEP_DIR if seqtype == "pep" else CDNA_DIR
     with ftplib.FTP(FTPURL, timeout=FTP_TIMEOUT) as ftp:
         ftp.login()
         for plant in plants:
-            dname = dirname.format(release=release, plant=plant)
-            print("looking in", dname, tail)
+            dname = TARGET_DIR.format(release=release, plant=plant, seqtype=seqtype)
             for n in ftp.nlst(dname):
                 print(n)
                 if n.endswith(tail):
                     yield FileInfo(plant, n[len(dname) + 1 :])
                     break
             else:
                 yield FileInfo(plant, None)
@@ -192,48 +190,64 @@
 
     with ftplib.FTP(FTPURL, timeout=FTP_TIMEOUT) as ftp:
         ftp.login()
         ftp.cwd(FASTAS_DIR.format(release=release))
         return list(ftp.nlst())
 
 
-def get_available_species(release: int, *, quiet: bool = False) -> pd.DataFrame | None:
+def get_available_species(
+    release: int,
+    *,
+    quiet: bool = False,
+    fail_early: bool = False,
+) -> pd.DataFrame | None:
     bd = blast_dir(release)
     sfile = bd / SPECIES_TSV
     if sfile.exists():
         return pd.read_csv(sfile, sep="\t", index_col=False)
+    if fail_early:
+        return None
     url = f"ftp://{FTPURL}/{TOP.format(release=release)}/{SPECIES_TSV}"
     resp = fetch_file(SPECIES_TSV, url, release, quiet=quiet)
     if resp.returncode or not sfile.exists():
         return None
     return pd.read_csv(sfile, sep="\t", index_col=False)
 
 
+def show_missing(plants: Sequence[str], release: int) -> list[str]:
+    df = get_available_species(release, quiet=True, fail_early=False)
+    if df is None:
+        return []
+    missing = [m for m in plants if m not in df["species"].to_list()]
+    return missing
+
+
 def fetch_fastas(
     plants: Sequence[str],
     release: int,
     *,
     seqtype: SeqType = "pep",
-) -> Path:
+) -> tuple[Path, int]:
     bd = blast_dir(release)
 
     bd.mkdir(parents=True, exist_ok=True)
-
+    failed = 0
     for info in find_fasta_names(plants, release, seqtype=seqtype):
         if info.fasta is None:
             click.echo(f"Can't find fasta for {info.species}!", err=True)
             continue
 
         if (bd / info.fasta).exists():
             continue
         click.echo(f"fetching {info.fasta}")
         r = fetch_fasta(info.species, info.fasta, release=release, seqtype=seqtype)
         if r.returncode:
+            failed += 1
             click.secho(f"failed to fetch {info.fasta}: {r}", fg="red", err=True)
-    return bd
+    return bd, failed
 
 
 def build(species: Sequence[str], release: int, *, path: str | None = None) -> bool:
     blastdir = blast_dir(release)
     if path is not None:
         blastdir = Path(path) / blastdir
     blastdir.mkdir(parents=True, exist_ok=True)
```

### Comparing `blasttools-0.1.14/blasttools/plants_ui.py` & `blasttools-0.1.15/blasttools/plants_ui.py`

 * *Files 7% similar despite different names*

```diff
@@ -167,34 +167,45 @@
         df.rename(columns=VALID, inplace=True)
     click.secho(f"writing {out}", fg="green")
     save_df(df, out, index=False)
 
 
 @plants.command(name="fasta-fetch")
 @click.option(
-    "--cdna",
-    is_flag=True,
-    help="download the cdna (instead of peptide) version",
+    "-s",
+    "--stype",
+    "seqtype",
+    type=click.Choice(["pep", "cdna", "cds"]),
+    default="pep",
+    help="download the cdna/cds (instead of peptide) version",
 )
 @click.argument("species", nargs=-1)
 @pass_config
-def fasta_fetch_cmd(cfg: Config, species: Sequence[str], cdna: bool) -> None:
+def fasta_fetch_cmd(cfg: Config, species: Sequence[str], seqtype: str) -> None:
     """Download fasta files from FTP site"""
-    from .plants import fetch_fastas
+    from typing import cast
+    from .plants import fetch_fastas, show_missing, SeqType
 
     if not species:
         return
-    download_dir = fetch_fastas(
+
+    missing = show_missing(species, cfg.release)
+    if missing:
+        click.secho(f"unknown species: {', '.join(missing)}", fg="red", err=True)
+        raise click.Abort()
+
+    download_dir, failed = fetch_fastas(
         species,
         release=cfg.release,
-        seqtype="cdna" if cdna else "pep",
+        seqtype=cast(SeqType, seqtype),
     )
-    dd = click.style(str(download_dir), fg="blue")
-    s = "s" if len(species) > 1 else ""
-    click.echo(f"downloaded file{s} into: {dd}/")
+    if failed == 0:
+        dd = click.style(str(download_dir), fg="blue")
+        s = "s" if len(species) > 1 else ""
+        click.echo(f"downloaded file{s} into: {dd}/")
 
 
 @plants.command("fasta-filenames")
 @click.option("-f", "--full", is_flag=True, help="show full URL to file")
 @click.argument("species", nargs=-1)
 @pass_config
 def fasta_filenames_cmd(
```

### Comparing `blasttools-0.1.14/blasttools/utils.py` & `blasttools-0.1.15/blasttools/utils.py`

 * *Files identical despite different names*

### Comparing `blasttools-0.1.14/pyproject.toml` & `blasttools-0.1.15/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "blasttools"
-version = "0.1.14"
+version = "0.1.15"
 description = "Commands for turning blast queries into pandas dataframes."
 authors = ["Ian Castleden <ian.castleden@uwa.edu.au>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/arabidopsis/blasttools"
 keywords = ["genomics", "bioinformatics"]
 classifiers = [
```

### Comparing `blasttools-0.1.14/PKG-INFO` & `blasttools-0.1.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blasttools
-Version: 0.1.14
+Version: 0.1.15
 Summary: Commands for turning blast queries into pandas dataframes.
 Home-page: https://github.com/arabidopsis/blasttools
 License: MIT
 Keywords: genomics,bioinformatics
 Author: Ian Castleden
 Author-email: ian.castleden@uwa.edu.au
 Requires-Python: >=3.9,<3.13
```

