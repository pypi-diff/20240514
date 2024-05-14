# Comparing `tmp/eurmlsdk-0.0.81.tar.gz` & `tmp/eurmlsdk-0.0.82.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/eurmlsdk-0.0.81.tar", last modified: Mon May 13 13:04:10 2024, max compression
+gzip compressed data, was "dist/eurmlsdk-0.0.82.tar", last modified: Mon May 13 15:30:44 2024, max compression
```

## Comparing `eurmlsdk-0.0.81.tar` & `eurmlsdk-0.0.82.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-13 13:04:10.000000 eurmlsdk-0.0.81/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       10 2024-05-09 09:42:44.000000 eurmlsdk-0.0.81/README.md
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-09 09:42:44.000000 eurmlsdk-0.0.81/MANIFEST.in
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-13 13:04:10.000000 eurmlsdk-0.0.81/eurmlsdk.egg-info/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)        9 2024-05-13 13:04:10.000000 eurmlsdk-0.0.81/eurmlsdk.egg-info/top_level.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)        1 2024-05-13 13:04:10.000000 eurmlsdk-0.0.81/eurmlsdk.egg-info/dependency_links.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       53 2024-05-13 13:04:10.000000 eurmlsdk-0.0.81/eurmlsdk.egg-info/entry_points.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      321 2024-05-13 13:04:10.000000 eurmlsdk-0.0.81/eurmlsdk.egg-info/SOURCES.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       79 2024-05-13 13:04:10.000000 eurmlsdk-0.0.81/eurmlsdk.egg-info/requires.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      383 2024-05-13 13:04:10.000000 eurmlsdk-0.0.81/eurmlsdk.egg-info/PKG-INFO
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-13 13:04:10.000000 eurmlsdk-0.0.81/setup.cfg
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      790 2024-05-13 13:03:59.000000 eurmlsdk-0.0.81/setup.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       16 2024-05-09 09:42:44.000000 eurmlsdk-0.0.81/LICENSE.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      383 2024-05-13 13:04:10.000000 eurmlsdk-0.0.81/PKG-INFO
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-13 13:04:10.000000 eurmlsdk-0.0.81/eurmlsdk/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)     3430 2024-05-13 11:38:36.000000 eurmlsdk-0.0.81/eurmlsdk/__main__.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)     6614 2024-05-13 12:12:20.000000 eurmlsdk-0.0.81/eurmlsdk/eur_sdk.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)    10466 2024-05-09 09:42:44.000000 eurmlsdk-0.0.81/eurmlsdk/base_class.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       31 2024-05-09 09:42:44.000000 eurmlsdk-0.0.81/eurmlsdk/__init__.py
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-13 15:30:44.000000 eurmlsdk-0.0.82/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       10 2024-05-09 09:42:44.000000 eurmlsdk-0.0.82/README.md
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-09 09:42:44.000000 eurmlsdk-0.0.82/MANIFEST.in
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-13 15:30:44.000000 eurmlsdk-0.0.82/eurmlsdk.egg-info/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)        9 2024-05-13 15:30:44.000000 eurmlsdk-0.0.82/eurmlsdk.egg-info/top_level.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)        1 2024-05-13 15:30:44.000000 eurmlsdk-0.0.82/eurmlsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       53 2024-05-13 15:30:44.000000 eurmlsdk-0.0.82/eurmlsdk.egg-info/entry_points.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      321 2024-05-13 15:30:44.000000 eurmlsdk-0.0.82/eurmlsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       79 2024-05-13 15:30:44.000000 eurmlsdk-0.0.82/eurmlsdk.egg-info/requires.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      383 2024-05-13 15:30:44.000000 eurmlsdk-0.0.82/eurmlsdk.egg-info/PKG-INFO
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-13 15:30:44.000000 eurmlsdk-0.0.82/setup.cfg
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      790 2024-05-13 15:28:12.000000 eurmlsdk-0.0.82/setup.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       16 2024-05-09 09:42:44.000000 eurmlsdk-0.0.82/LICENSE.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      383 2024-05-13 15:30:44.000000 eurmlsdk-0.0.82/PKG-INFO
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-13 15:30:44.000000 eurmlsdk-0.0.82/eurmlsdk/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)     3976 2024-05-13 15:30:02.000000 eurmlsdk-0.0.82/eurmlsdk/__main__.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)     6823 2024-05-13 14:29:39.000000 eurmlsdk-0.0.82/eurmlsdk/eur_sdk.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)    10466 2024-05-09 09:42:44.000000 eurmlsdk-0.0.82/eurmlsdk/base_class.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       31 2024-05-09 09:42:44.000000 eurmlsdk-0.0.82/eurmlsdk/__init__.py
```

### Comparing `eurmlsdk-0.0.81/setup.py` & `eurmlsdk-0.0.82/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='eurmlsdk',
-    version='0.0.81',
+    version='0.0.82',
     packages=find_packages(),
     description='eUR ML SDK',
     long_description=open('README.md').read(),
     install_requires=[
         'boto3',
         'numpy==1.24.3',
         'python-dotenv',
```

### Comparing `eurmlsdk-0.0.81/eurmlsdk/__main__.py` & `eurmlsdk-0.0.82/eurmlsdk/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,82 +4,92 @@
 from .eur_sdk import ModelYolo
 
 os.environ['TF_CPP_MIN_LOG_LEVEL'] = '2'  # Suppress TensorFlow info and warning logs
 logging.getLogger('tensorflow').setLevel(logging.ERROR)  # Suppress TensorFlow warning logs
 logging.getLogger('tensorflow.compiler.tf2tensorrt').setLevel(logging.ERROR)  # Suppress TensorFlow-TRT warning logs
 
 def list_commands():
-    print("Available commands in mlsdk package are:")
-    print("  deploy <model path> <hostname> <username> <password> : Uploads the model file in the Raspberry pi")
-    print("     <model path> : path to the model file")
-    print("     <hostname>   : hostname to connect to Raspberry pi")
-    print("     <username>   : username to connect to Raspberry pi")
-    print("     <password>   : password to connect to Raspberry pi")
-    print("  help | --h                : Lists all commands available in mlsdk package")
-    print("  predict <model path> <dataset> : Predicts the labels and saves the predicted image")
-    print("     <model path> : path to the model file")
-    print("     <dataset>    : sample dataset image")
-    print("  validate <dataType> <model path>     : Validates the model and returns the metrics using default dataset")
-    print("     <dataType>    : dataType can be of the string 'seg'  'pose' 'detect' 'classify' ")
+    print("Available commands in eurmlsdk package are:")
+    print("  deploy <model path> <hostname> <username> <password> : Uploads the model file and executes remote script")
+    print("  help | --h                                           : Lists all commands available in eurmlsdk package")
+    print("  predict <model path> <dataset path>                  : Predicts the labels and saves the predicted result")
+    print("  validate <task> <model path>                         : Validates the model and returns the metrics using default dataset")
+    print(" ")
+    print("Options:")
+    print(" <dataset path> : Image or Video path (optional)")
+    print(" <hostname>     : Remote Server hostname")
+    print(" <model path>   : Model file path")
+    print(" <password>     : Remote Server password")
+    print(" <task>         : Prediction task - 'seg' or 'pose' or 'detect' or 'classify'")
+    print(" <username>     : Remote Server username")
 
-def main(): 
-    if len(argv) == 1:
-        print("Model Zoo SDK")
-        print("Package name: eurmlsdk")
-        print("Version: 0.0.76")
-        print("Run 'eurmlsdk help' or eurmlsdk --h to find the list of commands.")
-        exit(1)
+def main():
+    try:
+        if len(argv) == 1:
+            print("Model Zoo SDK")
+            print("Package name: eurmlsdk")
+            print("Version: 0.0.76")
+            print("Run 'eurmlsdk help' or eurmlsdk --h to find the list of commands.")
+            exit()
 
-    command = argv[1]
-    if command == "help" or command == "--h":
-        list_commands()
-        exit(1)
-        
-    elif command == "validate":
-        taskList = ["seg", "pose", "classify", "detect"]
-        if len(argv) <4:
-            print("Please provide task type and model path")
-            exit(1)
-        elif argv[2] not in taskList:
-            print("Please provide valid task")
-            exit(1)
-        else:
+        command = argv[1]        
+        if command == "help" or command == "--h":
+            list_commands()
+  
+        elif command == "validate":
+            taskList = ["seg", "pose", "classify", "detect"]
+            if len(argv) <4:
+                print("Missing required arguments")
+                print("Usage: eurmlsdk validate <task> <model path>")
+                exit(1)
+            if len(argv) > 4:
+                print("Too many arguments")
+                print("Usage: eurmlsdk validate <task> <model path>")
+                exit(1)
+            if argv[2] not in taskList:
+                print("Please provide valid task")
+                exit(1)
             modelPath = argv[3]
             task = argv[2]
             yoloSDK = ModelYolo()
             yoloSDK.validateModel(modelPath, task)
-        exit(1)
-        
-    elif command == "predict":
-        if len(argv) <3:
-            print("Give the model file name or file file path")
-            exit(1)
-        elif len(argv) <4:
-            print("Please provide atlest one data set of images")
-            exit(1)                                                                                                                               
-        else:
+            
+        elif command == "predict":
+            if len(argv) <4:
+                print("Missing required arguments")
+                print("Usage: eurmlsdk predict <model path> <dataset path>")
+                exit(1)
+            if len(argv) > 4:
+                print("Too many arguments")
+                print("Usage: eurmlsdk predict <model path> <dataset path>")
+                exit(1)
             modelPath = argv[2]
             predictData = argv[3]
             yoloSDK = ModelYolo()
             yoloSDK.predictModel(modelPath, predictData)
-        exit(1)    
-    
-    elif command == "deploy":
-        if len(argv) < 6:
-            print("Missing required arguments")
-            print("Usage: eurmlsdk deploy <model path> <hostname> <username> <password>")
-        else:
+        
+        elif command == "deploy":
+            if len(argv) < 6:
+                print("Missing required arguments")
+                print("Usage: eurmlsdk deploy <model path> <hostname> <username> <password>")
+                exit(1)
+            if len(argv) > 6:
+                print("Too many arguments")
+                print("Usage: eurmlsdk deploy <model path> <hostname> <username> <password>")
+                exit(1)
             localPath = argv[2]
             hostname = argv[3]
             username = argv[4]
             password = argv[5]
             yoloSDK = ModelYolo()
             modelFile = localPath.split("/")[-1]
             yoloSDK.deployModel(localPath,  hostname, username, password ,  modelFile)
-        exit(1)
-        
-    else:
-        print("Unknown command. Please find the list of commands")
-        list_commands()
+            
+        else:
+            print("Unknown command. Please find the list of commands")
+            list_commands()
+    except KeyboardInterrupt:
+        print("Exiting...")
+        exit(130)
 
 if __name__ == "__main__":
-    main()
+    exit(main())
```

### Comparing `eurmlsdk-0.0.81/eurmlsdk/eur_sdk.py` & `eurmlsdk-0.0.82/eurmlsdk/eur_sdk.py`

 * *Files 6% similar despite different names*

```diff
@@ -98,34 +98,39 @@
         ssh_client = self.connect_ssh_client(hostname, username, password)
         home_path = self.execute_ssh_script(ssh_client, 'pwd')
         if home_path == "":
             exit(1)
         remote_model_path = (f"{home_path}/{modelFile}").replace('\n', "").strip()
         script_path = (f'{home_path}/hello.py').replace('\n', "").strip()
         self.uploadFile(ssh_client, local_path, remote_model_path, home_path)
+
         print("Choose between static dataset or live feed for prediction.")
         static = input("Static dataset (y/n)? ")
         static_path = ''
-        if static:
+        while(static.lower() != 'y' and static.lower() != 'n'):
+            print("Your response ('{}') was not one of the expected responses: y, n".format(static))
+            static = input("Static dataset (y/n)? ")
+        if static.lower() == 'y':
             dataset_path = input("Enter img/video path: ")
-            remote_dataset_path = (f"{home_path}/{dataset_path.split("/")[-1]}").replace('\n', "").strip()
+            dataset_file = dataset_path.split("/")[-1]
+            remote_dataset_path = (f"{home_path}/{dataset_file}").replace('\n', "").strip()
             self.uploadFile(ssh_client, dataset_path, remote_dataset_path, home_path)
             feedType = 'static'
             static_path = remote_dataset_path
         else:
             feedType = 'live_feed'
-            exit(1)
+            # exit(1)
+
         script_command = f'python3 -m venv mlsdk-venv && source ./mlsdk-venv/bin/activate && pip install eurmlsdk --upgrade && python3 {script_path} {modelFile} {feedType} {static_path}'
-        # self.execute_script(ssh_client, script_path , modelFile)
         execute_script = self.execute_ssh_script(ssh_client, script_command)
         if execute_script != "":
             print(execute_script)
         # Close SSH connection
         ssh_client.close()
-        exit(1)
+        exit()
 
 class ModelYolo(EurBaseSDK):
     def loadModel(self, modelPath) -> YOLO:
         modelFile = self.getModel(modelPath)
         if modelFile != "":
             model = YOLO(modelPath)
             return model
```

### Comparing `eurmlsdk-0.0.81/eurmlsdk/base_class.py` & `eurmlsdk-0.0.82/eurmlsdk/base_class.py`

 * *Files identical despite different names*

