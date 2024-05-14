# Comparing `tmp/process_time_azure_devops-0.0.5.tar.gz` & `tmp/process_time_azure_devops-0.0.7.tar.gz`

## Comparing `process_time_azure_devops-0.0.5.tar` & `process_time_azure_devops-0.0.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.5/azure-pipelines.yml
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.5/.github/workflows/pr.yml
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.5/.github/workflows/publish.yml
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.5/.idea/.gitignore
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.5/.idea/misc.xml
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.5/.idea/modules.xml
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.5/.idea/process-time-azure-devops.iml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.5/.idea/vcs.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.5/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.5/src/process_time_azure_devops/__init__.py
--rw-r--r--   0        0        0     2446 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.5/src/process_time_azure_devops/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.5/src/process_time_azure_devops/arts/__init__.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.5/src/process_time_azure_devops/arts/process_time_logo.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.5/src/process_time_azure_devops/models/ArgumentParseResult.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.5/src/process_time_azure_devops/models/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.5/src/process_time_azure_devops/parsers/__init__.py
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.5/src/process_time_azure_devops/parsers/get_last_attempt_to_deliver.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.5/tests/__init__.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.5/tests/generate_test_run.py
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.5/tests/test_get_last_attempt_to_deliver.py
--rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.5/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.5/LICENSE
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.5/README.md
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.7/azure-pipelines.yml
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.7/.github/workflows/pr.yml
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.7/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.7/.idea/.gitignore
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.7/.idea/misc.xml
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.7/.idea/modules.xml
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.7/.idea/process-time-azure-devops.iml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.7/.idea/vcs.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.7/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.7/src/process_time_azure_devops/__init__.py
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.7/src/process_time_azure_devops/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.7/src/process_time_azure_devops/arts/__init__.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.7/src/process_time_azure_devops/arts/process_time_logo.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.7/src/process_time_azure_devops/models/ArgumentParseResult.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.7/src/process_time_azure_devops/models/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.7/src/process_time_azure_devops/parsers/__init__.py
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.7/src/process_time_azure_devops/parsers/get_last_attempt_to_deliver.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.7/tests/__init__.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.7/tests/generate_test_run.py
+-rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.7/tests/test_get_last_attempt_to_deliver.py
+-rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.7/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.7/LICENSE
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.7/README.md
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.7/PKG-INFO
```

### Comparing `process_time_azure_devops-0.0.5/azure-pipelines.yml` & `process_time_azure_devops-0.0.7/azure-pipelines.yml`

 * *Files 11% similar despite different names*

```diff
@@ -29,11 +29,12 @@
     orgname="worldpwn"
     echo "orgname=$orgname"
     token=$(System.AccessToken)
     project="process-time"
     echo "project=$project"
     pipeline_id=2
     echo "pipeline_id=$pipeline_id"
-    python src/process_time_azure_devops/__main__.py --org "$orgname" --token "$token" --project "$project" --pipeline-id "$pipeline_id"
+    current_run_id=8
+    python src/process_time_azure_devops/__main__.py --org "$orgname" --token "$token" --project "$project" --pipeline-id "$pipeline_id" --current-run-id $current_run_id
   displayName: 'Test — Example Run Trunk Based'
   env:
     System.AccessToken: $(System.AccessToken)
```

### Comparing `process_time_azure_devops-0.0.5/.github/workflows/pr.yml` & `process_time_azure_devops-0.0.7/.github/workflows/pr.yml`

 * *Files identical despite different names*

### Comparing `process_time_azure_devops-0.0.5/.github/workflows/publish.yml` & `process_time_azure_devops-0.0.7/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `process_time_azure_devops-0.0.5/src/process_time_azure_devops/__main__.py` & `process_time_azure_devops-0.0.7/src/process_time_azure_devops/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,58 +1,73 @@
 from azure.devops.v7_1.pipelines.pipelines_client import PipelinesClient
+from azure.devops.v7_1.build.build_client import BuildClient
 from process_time_azure_devops.parsers.get_last_attempt_to_deliver import get_last_attempt_to_deliver
 from process_time_azure_devops.models.ArgumentParseResult import ArgumentParseResult
 from process_time_azure_devops.arts.process_time_logo import process_time_logo
 from msrest.authentication import BasicAuthentication
 import getopt
 import sys
 import json
 
 
 def display_help():
-    print('main.py --org <azure-devops-organization> --token <personal_access_token> --project <project> --pipeline-id <pipeline_id>')
+    print('main.py --org <azure-devops-organization> --token <personal_access_token> --project <project> '
+          '--pipeline-id <pipeline_id> --current-run-id <current_run_id>')
 
 
 def parse_arguments(argv) -> ArgumentParseResult:
     azure_devops_organization: str | None = None
     personal_access_token: str | None = None
     project: str | None = None
     pipeline_id: int | None = None
-    opts, args = getopt.getopt(argv, "h", ["org=", "token=", "project=", "pipeline-id=", "help"])
+    current_run_id: int | None = None
+    opts, args = getopt.getopt(argv, "h", ["org=", "token=", "project=", "pipeline-id=", "current-run-id=", "help"])
     for opt, arg in opts:
         if opt in ('-h', '--help'):
             display_help()
             sys.exit()
         elif opt in "--org":
             azure_devops_organization = arg
         elif opt in "--token":
             personal_access_token = arg
         elif opt in "--project":
             project = arg
         elif opt in "--pipeline-id":
             pipeline_id = int(arg)
+        elif opt in "--current-run-id":
+            current_run_id = int(arg)
 
     print('========== Arguments: ==========')
     print(f'Azure DevOps Organization: {azure_devops_organization}')
     print(f'Personal Access Token: {("*" * len(personal_access_token))[:7]}')
     print(f'Project: {project}')
     print(f'Pipeline ID: {pipeline_id}')
+    print(f'Current Run ID: {current_run_id}')
     print('================================')
-    return ArgumentParseResult(azure_devops_organization, personal_access_token, project, pipeline_id)
+    return ArgumentParseResult(azure_devops_organization, personal_access_token, project, pipeline_id, current_run_id)
 
 
 def calculate_process_tine(args: ArgumentParseResult) -> None:
     print('Calculating process time...')
     url = f'https://dev.azure.com/{args.azure_devops_organization}'
     print(f'Connecting to Azure DevOps Organization: {url}')
     credentials = BasicAuthentication('', args.personal_access_token)
+
+    # Get pipeline runs
     pipelines_client = PipelinesClient(url, credentials)
     runs = pipelines_client.list_runs(args.project, args.pipeline_id)
-    previous_attempt = get_last_attempt_to_deliver(runs)
+    previous_attempt = get_last_attempt_to_deliver(args.current_run_id, runs)
+    print('Previous attempt to deliver:')
     print(json.dumps(previous_attempt.as_dict(), sort_keys=True, indent=4))
+
+    # Get build info based on run
+    build_client = BuildClient(url, credentials)
+    build = build_client.get_build(args.project, previous_attempt.id)
+    print('Build info:')
+    print(json.dumps(build.as_dict(), sort_keys=True, indent=4))
     print('Process time calculated!')
 
 
 if __name__ == "__main__":
     print(process_time_logo)
     arguments = parse_arguments(sys.argv[1:])
     calculate_process_tine(arguments)
```

### Comparing `process_time_azure_devops-0.0.5/tests/test_get_last_attempt_to_deliver.py` & `process_time_azure_devops-0.0.7/tests/test_get_last_attempt_to_deliver.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,65 @@
 from process_time_azure_devops.parsers.get_last_attempt_to_deliver import get_last_attempt_to_deliver
 from tests.generate_test_run import generate_test_run
 
 
 def test_only_current_run_exist_should_return_current_run():
     current_run = generate_test_run(3, 'succeeded')
     pipelines = [current_run]
-    result = get_last_attempt_to_deliver(pipelines)
+    result = get_last_attempt_to_deliver(current_run.id, pipelines)
     assert result.id == current_run.id
 
 
 def test_previous_run_was_successful_return_current_run():
     current_run = generate_test_run(3, 'succeeded')
     previous_run = generate_test_run(2, 'succeeded')
     pipelines = [current_run, previous_run]
-    result = get_last_attempt_to_deliver(pipelines)
+    result = get_last_attempt_to_deliver(current_run.id, pipelines)
     assert result.id == current_run.id
 
 
 def test_previous_run_was_failed_but_no_more_runs_return_previous_run():
     current_run = generate_test_run(3, 'succeeded')
     previous_run = generate_test_run(2, 'failed')
     pipelines = [current_run, previous_run]
-    result = get_last_attempt_to_deliver(pipelines)
+    result = get_last_attempt_to_deliver(current_run.id, pipelines)
     assert result.id == previous_run.id
 
 
 def test_previous_run_was_failed_return_failed_before_successful():
     current_run = generate_test_run(3, 'succeeded')
     previous_run = generate_test_run(2, 'failed')
     previous_run2 = generate_test_run(1, 'succeeded')
     pipelines = [current_run, previous_run, previous_run2]
-    result = get_last_attempt_to_deliver(pipelines)
+    result = get_last_attempt_to_deliver(current_run.id, pipelines)
     assert result.id == previous_run.id
 
 
 def test_two_previous_runs_both_failed_return_last_failed_before_successful():
     current_run = generate_test_run(3, 'succeeded')
     previous_run = generate_test_run(2, 'failed')
     previous_run2 = generate_test_run(1, 'failed')
     previous_run3 = generate_test_run(0, 'succeeded')
     pipelines = [current_run, previous_run, previous_run2, previous_run3]
-    result = get_last_attempt_to_deliver(pipelines)
+    result = get_last_attempt_to_deliver(current_run.id, pipelines)
     assert result.id == previous_run2.id
+
+
+def test_pass_current_run_all_succeeded_should_return_current_run():
+    future_run = generate_test_run(4, 'succeeded')
+    current_run = generate_test_run(3, 'succeeded')
+    previous_run = generate_test_run(2, 'succeeded')
+    pipelines =[future_run, current_run, previous_run]
+    result = get_last_attempt_to_deliver(current_run.id, pipelines)
+    assert result.id == current_run.id
+
+
+def test_pass_current_run_with_previous_failed_and_future_should_return_before_successful():
+    future_run1 = generate_test_run(4, 'succeeded')
+    future_run2 = generate_test_run(4, 'succeeded')
+    current_run = generate_test_run(3, 'succeeded')
+    previous_run = generate_test_run(2, 'failed')
+    previous_run2 = generate_test_run(1, 'failed')
+    previous_run3 = generate_test_run(0, 'succeeded')
+    pipelines = [future_run1, future_run2, current_run, previous_run, previous_run2, previous_run3]
+    result = get_last_attempt_to_deliver(current_run.id, pipelines)
+    assert result.id == previous_run2.id
```

### Comparing `process_time_azure_devops-0.0.5/.gitignore` & `process_time_azure_devops-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `process_time_azure_devops-0.0.5/LICENSE` & `process_time_azure_devops-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `process_time_azure_devops-0.0.5/README.md` & `process_time_azure_devops-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `process_time_azure_devops-0.0.5/pyproject.toml` & `process_time_azure_devops-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/process_time_azure_devops"]
 
 [project]
 name = "process_time_azure_devops"
-version = "0.0.5"
+version = "0.0.7"
 authors = [
     { name="Andrei Kniazev" },
 ]
 description = "Will collect process time for projects that are hosted in Azure DevOps"
 readme = "README.md"
 requires-python = ">=3.8"
 license = "GPL-3.0-or-later"
```

### Comparing `process_time_azure_devops-0.0.5/PKG-INFO` & `process_time_azure_devops-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: process_time_azure_devops
-Version: 0.0.5
+Version: 0.0.7
 Summary: Will collect process time for projects that are hosted in Azure DevOps
 Project-URL: GitHub, https://github.com/worldpwn/process-time-azure-devops
 Project-URL: Issues, https://github.com/worldpwn/process-time-azure-devops/issues
 Author: Andrei Kniazev
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: process_time_azure_devops Version: 0.0.5 Summary:
+Metadata-Version: 2.3 Name: process_time_azure_devops Version: 0.0.7 Summary:
 Will collect process time for projects that are hosted in Azure DevOps Project-
 URL: GitHub, https://github.com/worldpwn/process-time-azure-devops Project-URL:
 Issues, https://github.com/worldpwn/process-time-azure-devops/issues Author:
 Andrei Kniazev License-Expression: GPL-3.0-or-later License-File: LICENSE
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Requires-Python: >=3.8 Provides-Extra: build Requires-Dist:
 azure-devops==7.1.0b4; extra == 'build' Requires-Dist: hatchling==1.24.2; extra
```

