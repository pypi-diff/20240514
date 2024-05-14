# Comparing `tmp/autopkg_wrapper-2024.5.1.tar.gz` & `tmp/autopkg_wrapper-2024.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autopkg_wrapper-2024.5.1.tar", max compression
+gzip compressed data, was "autopkg_wrapper-2024.5.2.tar", max compression
```

## Comparing `autopkg_wrapper-2024.5.1.tar` & `autopkg_wrapper-2024.5.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1602 2024-05-13 03:58:20.101243 autopkg_wrapper-2024.5.1/LICENSE
--rw-r--r--   0        0        0     1833 2024-05-13 03:58:20.101243 autopkg_wrapper-2024.5.1/README.md
--rw-r--r--   0        0        0       25 2024-05-13 03:58:42.681450 autopkg_wrapper-2024.5.1/autopkg_wrapper/__init__.py
--rwxr-xr-x   0        0        0    10410 2024-05-13 03:58:20.101243 autopkg_wrapper-2024.5.1/autopkg_wrapper/autopkg_wrapper.py
--rw-r--r--   0        0        0       22 2024-05-13 03:58:20.101243 autopkg_wrapper-2024.5.1/autopkg_wrapper/notifier/__init__.py
--rw-r--r--   0        0        0     1982 2024-05-13 03:58:20.101243 autopkg_wrapper-2024.5.1/autopkg_wrapper/notifier/slack.py
--rw-r--r--   0        0        0       22 2024-05-13 03:58:20.101243 autopkg_wrapper-2024.5.1/autopkg_wrapper/utils/__init__.py
--rw-r--r--   0        0        0     3934 2024-05-13 03:58:20.101243 autopkg_wrapper-2024.5.1/autopkg_wrapper/utils/args.py
--rw-r--r--   0        0        0     2975 2024-05-13 03:58:20.101243 autopkg_wrapper-2024.5.1/autopkg_wrapper/utils/git_functions.py
--rw-r--r--   0        0        0      324 2024-05-13 03:58:20.101243 autopkg_wrapper-2024.5.1/autopkg_wrapper/utils/logging.py
--rw-r--r--   0        0        0     1038 2024-05-13 03:58:42.673450 autopkg_wrapper-2024.5.1/pyproject.toml
--rw-r--r--   0        0        0     2659 1970-01-01 00:00:00.000000 autopkg_wrapper-2024.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1602 2024-05-14 06:41:08.056671 autopkg_wrapper-2024.5.2/LICENSE
+-rw-r--r--   0        0        0     1833 2024-05-14 06:41:08.056671 autopkg_wrapper-2024.5.2/README.md
+-rw-r--r--   0        0        0       25 2024-05-14 06:41:33.336877 autopkg_wrapper-2024.5.2/autopkg_wrapper/__init__.py
+-rwxr-xr-x   0        0        0    10575 2024-05-14 06:41:08.056671 autopkg_wrapper-2024.5.2/autopkg_wrapper/autopkg_wrapper.py
+-rw-r--r--   0        0        0       22 2024-05-14 06:41:08.056671 autopkg_wrapper-2024.5.2/autopkg_wrapper/notifier/__init__.py
+-rw-r--r--   0        0        0     1982 2024-05-14 06:41:08.056671 autopkg_wrapper-2024.5.2/autopkg_wrapper/notifier/slack.py
+-rw-r--r--   0        0        0       22 2024-05-14 06:41:08.056671 autopkg_wrapper-2024.5.2/autopkg_wrapper/utils/__init__.py
+-rw-r--r--   0        0        0     3934 2024-05-14 06:41:08.056671 autopkg_wrapper-2024.5.2/autopkg_wrapper/utils/args.py
+-rw-r--r--   0        0        0     2975 2024-05-14 06:41:08.056671 autopkg_wrapper-2024.5.2/autopkg_wrapper/utils/git_functions.py
+-rw-r--r--   0        0        0      324 2024-05-14 06:41:08.056671 autopkg_wrapper-2024.5.2/autopkg_wrapper/utils/logging.py
+-rw-r--r--   0        0        0     1038 2024-05-14 06:41:33.332877 autopkg_wrapper-2024.5.2/pyproject.toml
+-rw-r--r--   0        0        0     2659 1970-01-01 00:00:00.000000 autopkg_wrapper-2024.5.2/PKG-INFO
```

### Comparing `autopkg_wrapper-2024.5.1/LICENSE` & `autopkg_wrapper-2024.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `autopkg_wrapper-2024.5.1/README.md` & `autopkg_wrapper-2024.5.2/README.md`

 * *Files identical despite different names*

### Comparing `autopkg_wrapper-2024.5.1/autopkg_wrapper/autopkg_wrapper.py` & `autopkg_wrapper-2024.5.2/autopkg_wrapper/autopkg_wrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,16 +28,18 @@
 
     @property
     def name(self):
         name = self.filename.split(".")[0]
 
         return name
 
-    def verify_trust_info(self):
-        cmd = ["/usr/local/bin/autopkg", "verify-trust-info", self.filename, "-v"]
+    def verify_trust_info(self, debug):
+        verbose_output = ["-vvvv"]
+        cmd = ["/usr/local/bin/autopkg", "verify-trust-info", self.filename]
+        cmd = cmd + verbose_output if debug else cmd
         cmd = " ".join(cmd)
         logging.debug(f"cmd: {str(cmd)}")
 
         p = subprocess.Popen(
             cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True
         )
         (output, err) = p.communicate()
@@ -73,34 +75,35 @@
             munki_results = report_data["summary_results"].get(
                 "munki_importer_summary_result", {}
             )
             imported_items.extend(munki_results.get("data_rows", []))
 
         return {"imported": imported_items, "failed": failed_items}
 
-    def run(self):
+    def run(self, debug):
         if self.verified is False:
             self.error = True
             self.results["failed"] = True
             self.results["imported"] = ""
         else:
             report = Path("/tmp/autopkg.plist")
             report.touch(exist_ok=True)
 
             try:
                 post_processor_cmd = list(chain.from_iterable([("--post", processor) for processor in self.post_processors])) if self.post_processors else None
-                initial_cmd = [
+                verbose_output = ["-vvvv"]
+                cmd = [
                     "/usr/local/bin/autopkg",
                     "run",
                     self.filename,
-                    "-v",
                     "--report-plist",
                     str(report),
                 ]
-                cmd = initial_cmd + post_processor_cmd if post_processor_cmd else initial_cmd
+                cmd = cmd + post_processor_cmd if post_processor_cmd else cmd
+                cmd = cmd + verbose_output if debug else cmd
                 cmd = " ".join(cmd)
 
                 logging.debug(f"cmd: {str(cmd)}")
 
                 subprocess.check_call(cmd, shell=True)
 
             except subprocess.CalledProcessError:
@@ -241,49 +244,48 @@
             post_processors_list = [post_processor.strip() for post_processor in post_processors.split(" ") if post_processor.strip()]
 
     logging.info(f"Post Processors List: {post_processors_list}") if post_processors_list else None
 
     return post_processors_list
 
 
-def process_recipe(recipe, disable_recipe_trust_check):
+def process_recipe(recipe, disable_recipe_trust_check, debug):
     if disable_recipe_trust_check:
         logging.debug("Setting Recipe verification to None")
         recipe.verified = None
     else:
         logging.debug("Checking Recipe verification")
-        recipe.verify_trust_info()
+        recipe.verify_trust_info(debug)
 
     match recipe.verified:
         case False | None if disable_recipe_trust_check:
             logging.debug("Running Recipe without verification")
-            recipe.run()
+            recipe.run(debug)
         case True:
             logging.debug("Running Recipe after successful verification")
-            recipe.run()
+            recipe.run(debug)
         case False:
             recipe.update_trust_info()
 
     return recipe
 
 
 def main():
-    print("Hello World")
     args = setup_args()
     setup_logger(args.debug if args.debug else False)
     logging.info("Running autopkg_wrapper")
 
     override_repo_info = get_override_repo_info(args)
 
     post_processors_list = parse_post_processors(post_processors=args.post_processors)
     recipe_list = parse_recipe_list(recipes=args.recipes, recipe_file=args.recipe_file, post_processors=post_processors_list)
 
     for recipe in recipe_list:
         logging.info(f"Processing Recipe: {recipe.name}")
-        process_recipe(recipe=recipe, disable_recipe_trust_check=args.disable_recipe_trust_check)
+        process_recipe(recipe=recipe, disable_recipe_trust_check=args.disable_recipe_trust_check, debug=args.debug)
         update_recipe_repo(git_info=override_repo_info, recipe=recipe, disable_recipe_trust_check=args.disable_recipe_trust_check, args=args)
         slack.send_notification(recipe=recipe, token=args.slack_token) if args.slack_token else None
 
     recipe.pr_url = git.create_pull_request(git_info=override_repo_info, recipe=recipe) if args.create_pr else None
 
 
 if __name__ == "__main__":
```

### Comparing `autopkg_wrapper-2024.5.1/autopkg_wrapper/notifier/slack.py` & `autopkg_wrapper-2024.5.2/autopkg_wrapper/notifier/slack.py`

 * *Files identical despite different names*

### Comparing `autopkg_wrapper-2024.5.1/autopkg_wrapper/utils/args.py` & `autopkg_wrapper-2024.5.2/autopkg_wrapper/utils/args.py`

 * *Files identical despite different names*

### Comparing `autopkg_wrapper-2024.5.1/autopkg_wrapper/utils/git_functions.py` & `autopkg_wrapper-2024.5.2/autopkg_wrapper/utils/git_functions.py`

 * *Files identical despite different names*

### Comparing `autopkg_wrapper-2024.5.1/pyproject.toml` & `autopkg_wrapper-2024.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
     authors = ["James Smith <james@smithjw.me>"]
     description = "A package used to execute some autopkg functions, primarily within the context of a GitHub Actions runner."
     license = "BSD-3-Clause"
     name = "autopkg-wrapper"
     readme = "README.md"
     repository = "https://github.com/smithjw/autopkg-wrapper"
-    version = "2024.5.1"
+    version = "2024.5.2"
 
     [tool.poetry.scripts]
         # When built and installed by pip, the command autopkg_wrapper will be availble in to run within that environment
         autopkg-wrapper = "autopkg_wrapper.autopkg_wrapper:main"
         autopkg_wrapper = "autopkg_wrapper.autopkg_wrapper:main"
 
     [tool.poetry.dependencies]
```

### Comparing `autopkg_wrapper-2024.5.1/PKG-INFO` & `autopkg_wrapper-2024.5.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autopkg-wrapper
-Version: 2024.5.1
+Version: 2024.5.2
 Summary: A package used to execute some autopkg functions, primarily within the context of a GitHub Actions runner.
 Home-page: https://github.com/smithjw/autopkg-wrapper
 License: BSD-3-Clause
 Author: James Smith
 Author-email: james@smithjw.me
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: BSD License
```

