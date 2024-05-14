# Comparing `tmp/solar_registry-0.2.3.tar.gz` & `tmp/solar_registry-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solar_registry-0.2.3.tar", last modified: Mon May 13 12:04:09 2024, max compression
+gzip compressed data, was "solar_registry-0.2.4.tar", last modified: Tue May 14 07:31:00 2024, max compression
```

## Comparing `solar_registry-0.2.3.tar` & `solar_registry-0.2.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    11357 2024-05-13 12:03:48.924144 solar_registry-0.2.3/LICENSE
--rw-r--r--   0        0        0      682 2024-05-13 12:03:48.924144 solar_registry-0.2.3/README.md
--rw-r--r--   0        0        0     1182 2024-05-13 12:04:09.932246 solar_registry-0.2.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-13 12:03:48.924144 solar_registry-0.2.3/src/solar_registry/__init__.py
--rw-r--r--   0        0        0     1880 2024-05-13 12:03:48.924144 solar_registry-0.2.3/src/solar_registry/cli.py
--rw-r--r--   0        0        0        0 2024-05-13 12:03:48.924144 solar_registry-0.2.3/src/solar_registry/commands/__init__.py
--rw-r--r--   0        0        0     4928 2024-05-13 12:03:48.924144 solar_registry-0.2.3/src/solar_registry/commands/meta_merger.py
--rw-r--r--   0        0        0        0 2024-05-13 12:03:48.924144 solar_registry-0.2.3/src/solar_registry/model/__init__.py
--rw-r--r--   0        0        0     2051 2024-05-13 12:03:48.924144 solar_registry-0.2.3/src/solar_registry/model/test_tool.py
--rw-r--r--   0        0        0        0 2024-05-13 12:03:48.924144 solar_registry-0.2.3/src/solar_registry/service/__init__.py
--rw-r--r--   0        0        0     2517 2024-05-13 12:03:48.924144 solar_registry-0.2.3/src/solar_registry/service/generator.py
--rw-r--r--   0        0        0     2628 2024-05-13 12:03:48.924144 solar_registry-0.2.3/src/solar_registry/service/pr_generator.py
--rw-r--r--   0        0        0      505 2024-05-13 12:03:48.924144 solar_registry-0.2.3/src/solar_registry/service/testtool.py
--rw-r--r--   0        0        0     1625 2024-05-13 12:03:48.924144 solar_registry-0.2.3/src/solar_registry/service/validator.py
--rw-r--r--   0        0        0        0 2024-05-13 12:03:48.924144 solar_registry-0.2.3/src/solar_registry/util/__init__.py
--rw-r--r--   0        0        0      600 2024-05-13 12:03:48.924144 solar_registry-0.2.3/src/solar_registry/util/file.py
--rw-r--r--   0        0        0        0 2024-05-13 12:03:48.924144 solar_registry-0.2.3/tests/__init__.py
--rw-r--r--   0        0        0      680 2024-05-13 12:03:48.924144 solar_registry-0.2.3/tests/test_merger.py
--rw-r--r--   0        0        0      495 2024-05-13 12:03:48.924144 solar_registry-0.2.3/tests/test_pr_generator.py
--rw-r--r--   0        0        0      928 2024-05-13 12:03:48.924144 solar_registry-0.2.3/tests/test_testtool.py
--rw-r--r--   0        0        0      291 2024-05-13 12:03:48.924144 solar_registry-0.2.3/tests/test_validator.py
--rw-r--r--   0        0        0      731 2024-05-13 12:03:48.924144 solar_registry-0.2.3/tests/testdata/error_meta_file/pytest/testtool.yaml
--rw-r--r--   0        0        0      736 2024-05-13 12:03:48.924144 solar_registry-0.2.3/tests/testdata/error_version_file/pytest/testtool.yaml
--rw-r--r--   0        0        0     2820 2024-05-13 12:03:48.924144 solar_registry-0.2.3/tests/testdata/pytest/testtool.yaml
--rw-r--r--   0        0        0     3607 2024-05-13 12:03:48.924144 solar_registry-0.2.3/tests/testdata/stable_index_file_check/testtools/python/pytest/metadata.json
--rw-r--r--   0        0        0     2942 2024-05-13 12:03:48.928144 solar_registry-0.2.3/tests/testdata/stable_index_file_check/testtools/stable.index.json
--rw-r--r--   0        0        0     1462 1970-01-01 00:00:00.000000 solar_registry-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-14 07:30:40.762310 solar_registry-0.2.4/LICENSE
+-rw-r--r--   0        0        0      682 2024-05-14 07:30:40.762310 solar_registry-0.2.4/README.md
+-rw-r--r--   0        0        0     1182 2024-05-14 07:31:00.970325 solar_registry-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-14 07:30:40.762310 solar_registry-0.2.4/src/solar_registry/__init__.py
+-rw-r--r--   0        0        0     1880 2024-05-14 07:30:40.762310 solar_registry-0.2.4/src/solar_registry/cli.py
+-rw-r--r--   0        0        0        0 2024-05-14 07:30:40.762310 solar_registry-0.2.4/src/solar_registry/commands/__init__.py
+-rw-r--r--   0        0        0     4950 2024-05-14 07:30:40.762310 solar_registry-0.2.4/src/solar_registry/commands/meta_merger.py
+-rw-r--r--   0        0        0        0 2024-05-14 07:30:40.762310 solar_registry-0.2.4/src/solar_registry/model/__init__.py
+-rw-r--r--   0        0        0     2051 2024-05-14 07:30:40.762310 solar_registry-0.2.4/src/solar_registry/model/test_tool.py
+-rw-r--r--   0        0        0        0 2024-05-14 07:30:40.762310 solar_registry-0.2.4/src/solar_registry/service/__init__.py
+-rw-r--r--   0        0        0     2517 2024-05-14 07:30:40.762310 solar_registry-0.2.4/src/solar_registry/service/generator.py
+-rw-r--r--   0        0        0     2628 2024-05-14 07:30:40.762310 solar_registry-0.2.4/src/solar_registry/service/pr_generator.py
+-rw-r--r--   0        0        0      505 2024-05-14 07:30:40.762310 solar_registry-0.2.4/src/solar_registry/service/testtool.py
+-rw-r--r--   0        0        0     1998 2024-05-14 07:30:40.762310 solar_registry-0.2.4/src/solar_registry/service/validator.py
+-rw-r--r--   0        0        0        0 2024-05-14 07:30:40.762310 solar_registry-0.2.4/src/solar_registry/util/__init__.py
+-rw-r--r--   0        0        0      600 2024-05-14 07:30:40.762310 solar_registry-0.2.4/src/solar_registry/util/file.py
+-rw-r--r--   0        0        0        0 2024-05-14 07:30:40.762310 solar_registry-0.2.4/tests/__init__.py
+-rw-r--r--   0        0        0      680 2024-05-14 07:30:40.762310 solar_registry-0.2.4/tests/test_merger.py
+-rw-r--r--   0        0        0      495 2024-05-14 07:30:40.762310 solar_registry-0.2.4/tests/test_pr_generator.py
+-rw-r--r--   0        0        0      928 2024-05-14 07:30:40.762310 solar_registry-0.2.4/tests/test_testtool.py
+-rw-r--r--   0        0        0      291 2024-05-14 07:30:40.762310 solar_registry-0.2.4/tests/test_validator.py
+-rw-r--r--   0        0        0      731 2024-05-14 07:30:40.762310 solar_registry-0.2.4/tests/testdata/error_meta_file/pytest/testtool.yaml
+-rw-r--r--   0        0        0      736 2024-05-14 07:30:40.762310 solar_registry-0.2.4/tests/testdata/error_version_file/pytest/testtool.yaml
+-rw-r--r--   0        0        0     2778 2024-05-14 07:30:40.762310 solar_registry-0.2.4/tests/testdata/pytest/testtool.yaml
+-rw-r--r--   0        0        0     3607 2024-05-14 07:30:40.762310 solar_registry-0.2.4/tests/testdata/stable_index_file_check/testtools/python/pytest/metadata.json
+-rw-r--r--   0        0        0     2942 2024-05-14 07:30:40.762310 solar_registry-0.2.4/tests/testdata/stable_index_file_check/testtools/stable.index.json
+-rw-r--r--   0        0        0     1462 1970-01-01 00:00:00.000000 solar_registry-0.2.4/PKG-INFO
```

### Comparing `solar_registry-0.2.3/LICENSE` & `solar_registry-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.3/README.md` & `solar_registry-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.3/pyproject.toml` & `solar_registry-0.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "solar-registry"
-version = "0.2.3"
+version = "0.2.4"
 description = "Generate and merge meta data for testsolar test tools"
 authors = [
     { name = "asiazhang", email = "asiazhang2002@gmail.com" },
 ]
 dependencies = [
     "requests>=2.31.0",
     "pydantic>=2.7.1",
```

### Comparing `solar_registry-0.2.3/src/solar_registry/cli.py` & `solar_registry-0.2.4/src/solar_registry/cli.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.3/src/solar_registry/commands/meta_merger.py` & `solar_registry-0.2.4/src/solar_registry/commands/meta_merger.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,14 +122,15 @@
         logger.info("Merging meta history...")
         if not history.versions:
             history.versions = []
 
         for index, version in enumerate(history.versions):
             if version.meta.version == self.metadata.meta.version:
                 history.versions[index] = self.metadata
+                break
         else:
             history.versions.append(self.metadata)
 
         logger.info(
             f"Merge meta history result: {history.model_dump_json(by_alias=True, indent=2, exclude_none=True)}"
         )
```

### Comparing `solar_registry-0.2.3/src/solar_registry/model/test_tool.py` & `solar_registry-0.2.4/src/solar_registry/model/test_tool.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.3/src/solar_registry/service/generator.py` & `solar_registry-0.2.4/src/solar_registry/service/generator.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.3/src/solar_registry/service/pr_generator.py` & `solar_registry-0.2.4/src/solar_registry/service/pr_generator.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.3/src/solar_registry/service/validator.py` & `solar_registry-0.2.4/src/solar_registry/service/validator.py`

 * *Files 14% similar despite different names*

```diff
@@ -34,10 +34,16 @@
             for filename in filenames:
                 if filename != "stable.index.json":
                     metafile = Path(dir_path) / filename
                     logger.info(f"Validating tool meta file [{metafile}]")
                     with open(metafile) as f:
                         re = MetaDataHistory.model_validate_json(f.read())
                         if re.versions:
+                            # 检查versions中是否有重复版本
+                            all_versions = set(x.meta.version for x in re.versions)
+
+                            if len(all_versions) != len(re.versions):
+                                raise RuntimeError(f"去重之后的版本数目 [{len(all_versions)}] != 原始版本数目 [{len(re.versions)}]")
+
                             logger.info(
                                 f"✅ Validated tool [{re.versions[0].meta.name}] OK."
                             )
```

### Comparing `solar_registry-0.2.3/src/solar_registry/util/file.py` & `solar_registry-0.2.4/src/solar_registry/util/file.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.3/tests/test_merger.py` & `solar_registry-0.2.4/tests/test_merger.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.3/tests/test_testtool.py` & `solar_registry-0.2.4/tests/test_testtool.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 def test_validate_correct_pytest_tool():
     workdir = str((Path(__file__).parent / "testdata").resolve())
 
     tool = get_testtool("pytest", workdir)
 
     assert tool.name == "pytest"
-    assert tool.version == "0.1.3"
+    assert tool.version == "0.1.6"
 
 
 def test_validate_name_error():
     workdir = str((Path(__file__).parent / "testdata" / "error_meta_file").resolve())
 
     with pytest.raises(ValidationError) as ve:
         get_testtool("pytest", workdir)
```

### Comparing `solar_registry-0.2.3/tests/testdata/error_meta_file/pytest/testtool.yaml` & `solar_registry-0.2.4/tests/testdata/error_meta_file/pytest/testtool.yaml`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.3/tests/testdata/error_version_file/pytest/testtool.yaml` & `solar_registry-0.2.4/tests/testdata/error_version_file/pytest/testtool.yaml`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.3/tests/testdata/pytest/testtool.yaml` & `solar_registry-0.2.4/tests/testdata/pytest/testtool.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 schemaVersion: 1.0
 name: pytest
 lang: python
 langType: "INTERPRETED"
 description: Pytest测试工具
-version: '0.1.3'
+version: '0.1.6'
 defaultBaseImage: python:3.10 # 用户在 TestContainer 配置中未指定 baseImage 时的默认镜像
 scaffoldRepo: https://github.com/OpenTestSolar/testtool-scaffold-python-pytest/archive/refs/tags/0.1.0.tar.gz
-indexFile: https://raw.githubusercontent.com/OpenTestSolar/testtool-registry/main/testtools/stable.index.json
-versionFile: https://raw.githubusercontent.com/OpenTestSolar/testtool-registry/main/testtools/python/pytest/metadata.json
+indexFile: https://opentestsolar.github.io/testtool-registry/testtools/stable.index.json
+versionFile: https://opentestsolar.github.io/testtool-registry/testtools/python/pytest/metadata.json
 homePage: https://github.com/OpenTestSolar/testtool-python-pytest
 parameterDefs: # 用户 use 这个测试工具时可以配置的 with 参数
   - name: parseMode
     value: 加载用例的模式
     default: auto
     choices:
       - value: auto
```

### Comparing `solar_registry-0.2.3/tests/testdata/stable_index_file_check/testtools/python/pytest/metadata.json` & `solar_registry-0.2.4/tests/testdata/stable_index_file_check/testtools/python/pytest/metadata.json`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.3/tests/testdata/stable_index_file_check/testtools/stable.index.json` & `solar_registry-0.2.4/tests/testdata/stable_index_file_check/testtools/stable.index.json`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.3/PKG-INFO` & `solar_registry-0.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solar-registry
-Version: 0.2.3
+Version: 0.2.4
 Summary: Generate and merge meta data for testsolar test tools
 Author-Email: asiazhang <asiazhang2002@gmail.com>
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

