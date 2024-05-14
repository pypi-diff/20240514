# Comparing `tmp/eurmlsdk-0.0.82.tar.gz` & `tmp/eurmlsdk-0.0.83.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/eurmlsdk-0.0.82.tar", last modified: Mon May 13 15:30:44 2024, max compression
+gzip compressed data, was "dist/eurmlsdk-0.0.83.tar", last modified: Tue May 14 07:16:28 2024, max compression
```

## Comparing `eurmlsdk-0.0.82.tar` & `eurmlsdk-0.0.83.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-13 15:30:44.000000 eurmlsdk-0.0.82/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       10 2024-05-09 09:42:44.000000 eurmlsdk-0.0.82/README.md
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-09 09:42:44.000000 eurmlsdk-0.0.82/MANIFEST.in
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-13 15:30:44.000000 eurmlsdk-0.0.82/eurmlsdk.egg-info/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)        9 2024-05-13 15:30:44.000000 eurmlsdk-0.0.82/eurmlsdk.egg-info/top_level.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)        1 2024-05-13 15:30:44.000000 eurmlsdk-0.0.82/eurmlsdk.egg-info/dependency_links.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       53 2024-05-13 15:30:44.000000 eurmlsdk-0.0.82/eurmlsdk.egg-info/entry_points.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      321 2024-05-13 15:30:44.000000 eurmlsdk-0.0.82/eurmlsdk.egg-info/SOURCES.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       79 2024-05-13 15:30:44.000000 eurmlsdk-0.0.82/eurmlsdk.egg-info/requires.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      383 2024-05-13 15:30:44.000000 eurmlsdk-0.0.82/eurmlsdk.egg-info/PKG-INFO
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-13 15:30:44.000000 eurmlsdk-0.0.82/setup.cfg
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      790 2024-05-13 15:28:12.000000 eurmlsdk-0.0.82/setup.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       16 2024-05-09 09:42:44.000000 eurmlsdk-0.0.82/LICENSE.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      383 2024-05-13 15:30:44.000000 eurmlsdk-0.0.82/PKG-INFO
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-13 15:30:44.000000 eurmlsdk-0.0.82/eurmlsdk/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)     3976 2024-05-13 15:30:02.000000 eurmlsdk-0.0.82/eurmlsdk/__main__.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)     6823 2024-05-13 14:29:39.000000 eurmlsdk-0.0.82/eurmlsdk/eur_sdk.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)    10466 2024-05-09 09:42:44.000000 eurmlsdk-0.0.82/eurmlsdk/base_class.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       31 2024-05-09 09:42:44.000000 eurmlsdk-0.0.82/eurmlsdk/__init__.py
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-14 07:16:28.000000 eurmlsdk-0.0.83/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       10 2024-05-09 09:42:44.000000 eurmlsdk-0.0.83/README.md
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-09 09:42:44.000000 eurmlsdk-0.0.83/MANIFEST.in
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-14 07:16:28.000000 eurmlsdk-0.0.83/eurmlsdk.egg-info/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)        9 2024-05-14 07:16:28.000000 eurmlsdk-0.0.83/eurmlsdk.egg-info/top_level.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)        1 2024-05-14 07:16:28.000000 eurmlsdk-0.0.83/eurmlsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       53 2024-05-14 07:16:28.000000 eurmlsdk-0.0.83/eurmlsdk.egg-info/entry_points.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      315 2024-05-14 07:16:28.000000 eurmlsdk-0.0.83/eurmlsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       79 2024-05-14 07:16:28.000000 eurmlsdk-0.0.83/eurmlsdk.egg-info/requires.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      383 2024-05-14 07:16:28.000000 eurmlsdk-0.0.83/eurmlsdk.egg-info/PKG-INFO
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-14 07:16:28.000000 eurmlsdk-0.0.83/setup.cfg
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      790 2024-05-14 07:16:12.000000 eurmlsdk-0.0.83/setup.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       16 2024-05-09 09:42:44.000000 eurmlsdk-0.0.83/LICENSE.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      383 2024-05-14 07:16:28.000000 eurmlsdk-0.0.83/PKG-INFO
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-14 07:16:28.000000 eurmlsdk-0.0.83/eurmlsdk/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)     4171 2024-05-14 07:16:17.000000 eurmlsdk-0.0.83/eurmlsdk/__main__.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)     5990 2024-05-14 07:12:17.000000 eurmlsdk-0.0.83/eurmlsdk/eur_sdk.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)     1230 2024-05-14 07:15:30.000000 eurmlsdk-0.0.83/eurmlsdk/yolo.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       33 2024-05-14 06:27:37.000000 eurmlsdk-0.0.83/eurmlsdk/__init__.py
```

### Comparing `eurmlsdk-0.0.82/setup.py` & `eurmlsdk-0.0.83/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='eurmlsdk',
-    version='0.0.82',
+    version='0.0.83',
     packages=find_packages(),
     description='eUR ML SDK',
     long_description=open('README.md').read(),
     install_requires=[
         'boto3',
         'numpy==1.24.3',
         'python-dotenv',
```

### Comparing `eurmlsdk-0.0.82/eurmlsdk/__main__.py` & `eurmlsdk-0.0.83/eurmlsdk/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,93 +1,96 @@
 from sys import argv,exit
 import os
 import logging
-from .eur_sdk import ModelYolo
+from .yolo import ModelYolo
 
 os.environ['TF_CPP_MIN_LOG_LEVEL'] = '2'  # Suppress TensorFlow info and warning logs
 logging.getLogger('tensorflow').setLevel(logging.ERROR)  # Suppress TensorFlow warning logs
 logging.getLogger('tensorflow.compiler.tf2tensorrt').setLevel(logging.ERROR)  # Suppress TensorFlow-TRT warning logs
 
 def list_commands():
     print("Available commands in eurmlsdk package are:")
     print("  deploy <model path> <hostname> <username> <password> : Uploads the model file and executes remote script")
     print("  help | --h                                           : Lists all commands available in eurmlsdk package")
     print("  predict <model path> <dataset path>                  : Predicts the labels and saves the predicted result")
     print("  validate <task> <model path>                         : Validates the model and returns the metrics using default dataset")
     print(" ")
     print("Options:")
-    print(" <dataset path> : Image or Video path (optional)")
+    print(" <dataset path> : Image or Video path")
     print(" <hostname>     : Remote Server hostname")
     print(" <model path>   : Model file path")
     print(" <password>     : Remote Server password")
-    print(" <task>         : Prediction task - 'seg' or 'pose' or 'detect' or 'classify'")
+    print(" <task>         : Validation task - 'seg' or 'pose' or 'detect' or 'classify'")
     print(" <username>     : Remote Server username")
 
 def main():
+    commands_list = ['deploy','help','--h','predict','validate']
     try:
-        if len(argv) == 1:
+        argLen = len(argv)
+        if argLen == 1:
             print("Model Zoo SDK")
             print("Package name: eurmlsdk")
-            print("Version: 0.0.76")
+            print("Version: 0.0.83")
             print("Run 'eurmlsdk help' or eurmlsdk --h to find the list of commands.")
             exit()
 
-        command = argv[1]        
+        command = argv[1]
+        if command not in commands_list:
+            print("Unknown command. Please find the list of commands")
+            list_commands()
+            exit()
+
         if command == "help" or command == "--h":
             list_commands()
-  
         elif command == "validate":
             taskList = ["seg", "pose", "classify", "detect"]
-            if len(argv) <4:
+            if argLen < 4:
                 print("Missing required arguments")
                 print("Usage: eurmlsdk validate <task> <model path>")
                 exit(1)
-            if len(argv) > 4:
+            if argLen > 4:
                 print("Too many arguments")
                 print("Usage: eurmlsdk validate <task> <model path>")
                 exit(1)
             if argv[2] not in taskList:
-                print("Please provide valid task")
+                print("Please provide valid task for validation")
                 exit(1)
             modelPath = argv[3]
             task = argv[2]
             yoloSDK = ModelYolo()
-            yoloSDK.validateModel(modelPath, task)
-            
+            yoloSDK.validate_model(modelPath, task)
         elif command == "predict":
-            if len(argv) <4:
+            if argLen < 4:
                 print("Missing required arguments")
                 print("Usage: eurmlsdk predict <model path> <dataset path>")
                 exit(1)
-            if len(argv) > 4:
+            if argLen > 4:
                 print("Too many arguments")
                 print("Usage: eurmlsdk predict <model path> <dataset path>")
                 exit(1)
             modelPath = argv[2]
             predictData = argv[3]
             yoloSDK = ModelYolo()
-            yoloSDK.predictModel(modelPath, predictData)
-        
+            yoloSDK.predict_model(modelPath, predictData)
         elif command == "deploy":
-            if len(argv) < 6:
+            if argLen < 6:
                 print("Missing required arguments")
                 print("Usage: eurmlsdk deploy <model path> <hostname> <username> <password>")
                 exit(1)
             if len(argv) > 6:
                 print("Too many arguments")
                 print("Usage: eurmlsdk deploy <model path> <hostname> <username> <password>")
                 exit(1)
             localPath = argv[2]
             hostname = argv[3]
             username = argv[4]
             password = argv[5]
             yoloSDK = ModelYolo()
             modelFile = localPath.split("/")[-1]
-            yoloSDK.deployModel(localPath,  hostname, username, password ,  modelFile)
-            
+            yoloSDK.deploy_model(localPath,  hostname, username, password ,  modelFile) 
         else:
             print("Unknown command. Please find the list of commands")
             list_commands()
     except KeyboardInterrupt:
         print("Exiting...")
         exit(130)
```

### Comparing `eurmlsdk-0.0.82/eurmlsdk/eur_sdk.py` & `eurmlsdk-0.0.83/eurmlsdk/eur_sdk.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,16 +15,16 @@
         with tqdm(total=total_size, unit='B', unit_scale=True, desc=remotepath) as pbar:
             def _callback(bytes_transferred, bytes_remaining):
                 pbar.update(bytes_transferred - pbar.n)
                 if callback:
                     callback(bytes_transferred, bytes_remaining)
             return super().put(localpath, remotepath, callback=_callback, confirm=confirm)
         
-class EurBaseSDK():  
-    def getModel(self, filepath) ->str:
+class EurBaseSDK():
+    def get_model(self, filepath) ->str:
         extension = filepath.split(".")
         if extension[1] != "pt" and extension[1] != "tflite":
             print("Not supported file path")
             return ""
         
         if os.path.exists(filepath):
             print("Model file exist and ready to load")
@@ -46,39 +46,47 @@
         except TimeoutError as err:
             print("Connection Timeout Error: ", err)
             exit(1)
         except Exception as err:
             print("Error: %s" % err)
             exit(1)
 
-    def uploadToRemote(self, ssh_client, local_path, remote_path):
-        print("Uploading model {} to {}".format(local_path, remote_path))
+    def upload_to_remote(self, ssh_client, local_path, remote_path):
+        print("Uploading file {} to {}".format(local_path, remote_path))
         sftp_progress_bar = SFTPWithProgressBar.from_transport(ssh_client.get_transport())
         sftp_progress_bar.put(local_path, remote_path)
-        print("Model upload successful")
+        print("File upload successful")
 
-    def uploadFile(self, ssh_client, local_path, remote_path, home_path):
+    def upload_file(self, ssh_client, local_path, remote_path, home_path):
         try:
             sftp = ssh_client.open_sftp()
-            print("Checking for model file in {}".format(home_path))
+            print("Checking for file in {}".format(home_path))
             sftp.stat(remote_path)
-            print('Model File already exists')
-            upload = input('Do you want to upload it again (y/n)? ')
+            print("File already exists")
+            upload = input("Do you want to upload it again (y/n)? ")
             while upload.lower() != 'y' and upload.lower() != 'n':
                 print("Your response ('{}') was not one of the expected responses: y, n".format(upload))
-                upload = input('Do you want to upload it again (y/n)? ')
+                upload = input("Do you want to upload it again (y/n)? ")
             if upload == 'y':
-                self.uploadToRemote(ssh_client, local_path, remote_path)
+                if not os.path.exists(local_path):
+                    print("File '{}' does not exist".format(local_path))
+                    print("Exiting...")
+                    sftp.close()
+                    ssh_client.close()
+                    exit(1)
+                self.upload_to_remote(ssh_client, local_path, remote_path)
             sftp.close()
         except IOError:
-            print("Model File does not exist")
-            self.uploadToRemote(ssh_client, local_path, remote_path)
+            print("File does not exist")
+            self.upload_to_remote(ssh_client, local_path, remote_path)
             sftp.close()
         except Exception as err:
-            print("Error uploading the model file: ", err)
+            print("Error uploading the file: ", err)
+            sftp.close()
+            ssh_client.close()
             exit(1)
 
     def execute_ssh_script(self, ssh_client, command):
         try:
             if command != "pwd":
                 print("Executing script")
             stdin, stdout, stderr = ssh_client.exec_command(f'{command}')
@@ -89,76 +97,41 @@
             if err:
                 print(err)
                 return ""
         except Exception as err:
             print("Error Executing the script: ", err)
             exit(1)
               
-    def deployModel(self, local_path, hostname, username, password, modelFile):
+    def deploy_model(self, local_path, hostname, username, password, modelFile):
         # Establish SSH connection
         ssh_client = self.connect_ssh_client(hostname, username, password)
         home_path = self.execute_ssh_script(ssh_client, 'pwd')
         if home_path == "":
             exit(1)
         remote_model_path = (f"{home_path}/{modelFile}").replace('\n', "").strip()
         script_path = (f'{home_path}/hello.py').replace('\n', "").strip()
-        self.uploadFile(ssh_client, local_path, remote_model_path, home_path)
+        self.upload_file(ssh_client, local_path, remote_model_path, home_path)
 
         print("Choose between static dataset or live feed for prediction.")
         static = input("Static dataset (y/n)? ")
         static_path = ''
         while(static.lower() != 'y' and static.lower() != 'n'):
             print("Your response ('{}') was not one of the expected responses: y, n".format(static))
             static = input("Static dataset (y/n)? ")
         if static.lower() == 'y':
             dataset_path = input("Enter img/video path: ")
             dataset_file = dataset_path.split("/")[-1]
             remote_dataset_path = (f"{home_path}/{dataset_file}").replace('\n', "").strip()
-            self.uploadFile(ssh_client, dataset_path, remote_dataset_path, home_path)
+            self.upload_file(ssh_client, dataset_path, remote_dataset_path, home_path)
             feedType = 'static'
             static_path = remote_dataset_path
         else:
-            feedType = 'live_feed'
+            feedType = "live_feed"
             # exit(1)
 
         script_command = f'python3 -m venv mlsdk-venv && source ./mlsdk-venv/bin/activate && pip install eurmlsdk --upgrade && python3 {script_path} {modelFile} {feedType} {static_path}'
         execute_script = self.execute_ssh_script(ssh_client, script_command)
         if execute_script != "":
             print(execute_script)
         # Close SSH connection
         ssh_client.close()
-        exit()
-
-class ModelYolo(EurBaseSDK):
-    def loadModel(self, modelPath) -> YOLO:
-        modelFile = self.getModel(modelPath)
-        if modelFile != "":
-            model = YOLO(modelPath)
-            return model 
-        else:
-            raise ModelNotFound()
-        
-    def predictModel(self, pathArg, dataSet):
-        try:
-            model = self.loadModel(pathArg)
-            print("Prediction started.....")
-            model.predict(dataSet, save=True)
-        except ModelNotFound as err:
-            print("Error :", err)
-            exit(1)
-        except Exception as err:
-            print("Error in Prediction :", err)
-            exit(1)
-
-    def validateModel(self, pathArg, task):
-        try: 
-            model = self.loadModel(pathArg)
-            print("Validation started........")
-            dataset = {
-                "seg" : "coco8-seg.yaml",
-                "pose" : "coco8-pose.yaml",
-            }
-            metrics = model.val(data=dataset.get(task, "coco8.yaml"))
-            print("Validated Metrics", metrics)
-        except ModelNotFound as err:
-            print("Error :", err)
-            exit(1)
+        exit()
```

