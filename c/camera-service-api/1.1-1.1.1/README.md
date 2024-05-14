# Comparing `tmp/camera_service_api-1.1.tar.gz` & `tmp/camera-service-api-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "camera_service_api-1.1.tar", last modified: Mon May 13 01:51:11 2024, max compression
+gzip compressed data, was "dist\camera-service-api-1.1.1.tar", last modified: Tue May 14 13:46:51 2024, max compression
```

## Comparing `camera_service_api-1.1.tar` & `camera-service-api-1.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 01:51:11.447154 camera_service_api-1.1/
--rw-rw-rw-   0        0        0     3280 2024-05-13 01:51:11.446152 camera_service_api-1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2689 2024-05-13 01:49:35.000000 camera_service_api-1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 01:51:11.445152 camera_service_api-1.1/camera_service_api.egg-info/
--rw-rw-rw-   0        0        0     3280 2024-05-13 01:51:11.000000 camera_service_api-1.1/camera_service_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      528 2024-05-13 01:51:11.000000 camera_service_api-1.1/camera_service_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 01:51:11.000000 camera_service_api-1.1/camera_service_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-13 01:51:11.000000 camera_service_api-1.1/camera_service_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-13 01:51:11.000000 camera_service_api-1.1/camera_service_api.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-13 01:51:11.437136 camera_service_api-1.1/services/
--rw-rw-rw-   0        0        0        0 2023-10-12 02:46:42.000000 camera_service_api-1.1/services/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 01:51:11.439164 camera_service_api-1.1/services/cameras/
--rw-rw-rw-   0        0        0        0 2023-10-12 02:46:42.000000 camera_service_api-1.1/services/cameras/__init__.py
--rw-rw-rw-   0        0        0     1399 2024-05-11 07:09:21.000000 camera_service_api-1.1/services/cameras/camera_service_api.py
--rw-rw-rw-   0        0        0      662 2024-05-11 06:32:02.000000 camera_service_api-1.1/services/cameras/models.py
-drwxrwxrwx   0        0        0        0 2024-05-13 01:51:11.444153 camera_service_api-1.1/services/grpc/
--rw-rw-rw-   0        0        0        0 2023-10-12 02:46:42.000000 camera_service_api-1.1/services/grpc/__init__.py
--rw-rw-rw-   0        0        0     2734 2024-05-11 07:06:20.000000 camera_service_api-1.1/services/grpc/camera_service_pb2.py
--rw-rw-rw-   0        0        0     7359 2024-05-11 07:06:20.000000 camera_service_api-1.1/services/grpc/camera_service_pb2_grpc.py
--rw-rw-rw-   0        0        0     1275 2024-05-11 05:23:15.000000 camera_service_api-1.1/services/grpc/grpcutilsc.py
--rw-rw-rw-   0        0        0     1523 2024-05-11 05:51:07.000000 camera_service_api-1.1/services/grpc/grpcutilss.py
--rw-rw-rw-   0        0        0     1628 2024-05-09 08:12:32.000000 camera_service_api-1.1/services/grpc/pb2utils.py
--rw-rw-rw-   0        0        0       42 2024-05-13 01:51:11.448154 camera_service_api-1.1/setup.cfg
--rw-rw-rw-   0        0        0     1021 2024-05-13 01:50:54.000000 camera_service_api-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 13:46:51.000000 camera-service-api-1.1.1/
+-rw-rw-rw-   0        0        0     4482 2024-05-14 13:46:51.000000 camera-service-api-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2689 2024-05-13 01:49:35.000000 camera-service-api-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 13:46:51.000000 camera-service-api-1.1.1/camera_service_api.egg-info/
+-rw-rw-rw-   0        0        0     4482 2024-05-14 13:46:51.000000 camera-service-api-1.1.1/camera_service_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      528 2024-05-14 13:46:51.000000 camera-service-api-1.1.1/camera_service_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 13:46:51.000000 camera-service-api-1.1.1/camera_service_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-14 13:46:51.000000 camera-service-api-1.1.1/camera_service_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-14 13:46:51.000000 camera-service-api-1.1.1/camera_service_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 13:46:51.000000 camera-service-api-1.1.1/services/
+-rw-rw-rw-   0        0        0        0 2023-10-12 02:46:42.000000 camera-service-api-1.1.1/services/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 13:46:51.000000 camera-service-api-1.1.1/services/cameras/
+-rw-rw-rw-   0        0        0        0 2023-10-12 02:46:42.000000 camera-service-api-1.1.1/services/cameras/__init__.py
+-rw-rw-rw-   0        0        0     1399 2024-05-11 07:09:21.000000 camera-service-api-1.1.1/services/cameras/camera_service_api.py
+-rw-rw-rw-   0        0        0      662 2024-05-11 06:32:02.000000 camera-service-api-1.1.1/services/cameras/models.py
+drwxrwxrwx   0        0        0        0 2024-05-14 13:46:51.000000 camera-service-api-1.1.1/services/grpc/
+-rw-rw-rw-   0        0        0        0 2023-10-12 02:46:42.000000 camera-service-api-1.1.1/services/grpc/__init__.py
+-rw-rw-rw-   0        0        0     2725 2024-05-14 13:30:07.000000 camera-service-api-1.1.1/services/grpc/camera_service_pb2.py
+-rw-rw-rw-   0        0        0     5866 2024-05-14 13:30:07.000000 camera-service-api-1.1.1/services/grpc/camera_service_pb2_grpc.py
+-rw-rw-rw-   0        0        0     1275 2024-05-11 05:23:15.000000 camera-service-api-1.1.1/services/grpc/grpcutilsc.py
+-rw-rw-rw-   0        0        0     1523 2024-05-11 05:51:07.000000 camera-service-api-1.1.1/services/grpc/grpcutilss.py
+-rw-rw-rw-   0        0        0     1628 2024-05-09 08:12:32.000000 camera-service-api-1.1.1/services/grpc/pb2utils.py
+-rw-rw-rw-   0        0        0       42 2024-05-14 13:46:51.000000 camera-service-api-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1040 2024-05-14 13:46:19.000000 camera-service-api-1.1.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `camera_service_api-1.1/PKG-INFO` & `camera-service-api-1.1.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,163 +1,162 @@
 Metadata-Version: 2.1
 Name: camera-service-api
-Version: 1.1
-Summary: Camera service grpc api
-Home-page: 
+Version: 1.1.1
+Summary: Camera service grpc api (for python3.7 )
+Home-page: UNKNOWN
 Author: L.K
 Author-email: L.K@idontwant.com
+License: UNKNOWN
+Description: # Camera service grpc API 
+        
+        ## Install 
+        
+        1. using pip install local package 
+          
+        ```bash
+        
+        pip install camera-service-api
+        
+        ```
+        
+        
+        ## Dependencies 
+        
+        - grpcio     1.63.0
+        - protobuf   5.26.1
+        
+        
+        ## API 
+        
+        
+        
+        ### Get API Instance  `create_camera_service_api`  
+        
+        - host , camera server host , e.g.  `localhost` 
+        - port , camera server port , e.g.  `6000`
+        
+        
+        ```python 
+        
+        # host 
+        api = create_camera_service_api(host, port)
+        
+        
+        ```
+        ### Get All camera meta infos `get_camera_metas`
+        
+        ```python
+        
+        def get_camera_metas(self) -> List[CameraMeta]:
+            ...     
+        
+        ```
+        
+        ```python
+        
+        metas = api.get_camera_metas()
+        for meta in metas:
+            print(f"Camera modelName: {meta.modelName} - deviceVersion: {meta.deviceVersion}")
+            print("get camera image serialNumber ", meta.serialNumber)
+            print("get info ", meta.info)
+        
+        
+        ```
+        
+        ### CameraMeta 
+        
+        - cameraType , camera type , `GIGE` | `u3v` 
+        - serialNumber : camera serial number , 
+        - modelName  : model name 
+        - manufactureName : manufacture name 
+        - deviceVersion :  device version 
+        - userDefinedName : name defined by user 
+        - info : Map[string,string] , ext info 
+        
+        
+        ### Get live image by serial number 
+        
+        input camera serial number and return live image (jpg), bytes.
+        and if return `None` means the camera maybe offline. 
+        
+        and using `try .. except` for catch `exception` 
+        
+        ```python
+        
+        def get_image(self, sn: str) -> bytes:
+            ...     
+        
+        ```
+        
+        Example: 
+        
+        ```python
+        
+        ...
+        body = api.get_image(meta.serialNumber)
+        print(" body : ", len(body)  )
+        
+        ...
+        
+        fopen = open('test.jpg', 'wb+')
+        fopen.write( body )
+        fopen.close()
+        
+        ...
+        
+        ```
+        
+        
+        ## Example 
+        
+        ```python
+        import time
+        
+        import grpc
+        
+        from services.cameras.camera_service_api import create_camera_service_api
+        
+        
+        max_test = 100
+        
+        def test_camera_api(host, port):
+            #
+            api = create_camera_service_api(host, port)
+            metas = api.get_camera_metas()
+            for meta in metas:
+                print(f"Camera modelName: {meta.modelName} - deviceVersion: {meta.deviceVersion}")
+                print("get camera image serialNumber ", meta.serialNumber)
+                print("get info ", meta.info)
+        
+                t1 = time.time()
+                try:
+                
+                    for i in range( max_test ):
+                        body = api.get_image(meta.serialNumber)
+                        print(" body : ", i, len(body)  )
+        
+                except Exception as e:
+                    print( e) 
+        
+                t2 = time.time()
+                tt = t2-t1
+                avg = tt / max_test
+                print( f" Try {max_test} times get image , using {tt} , avg {avg} ")
+        
+                # fopen = open('body.jpg'.encode('utf-8'), 'wb+')
+                # fopen.write( body, )
+                # fopen.close()
+        
+        # protect the entry point
+        if __name__ == '__main__':
+            print("GRPC Version : {} ".format(grpc.__version__))
+            test_camera_api("127.0.0.1", 6000)
+        
+        
+        
+        ```
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Requires-Dist: grpcio
-Requires-Dist: protobuf
-
-# Camera service grpc API 
-
-## Install 
-
-1. using pip install local package 
-  
-```bash
-
-pip install camera-service-api
-
-```
-
-
-## Dependencies 
-
-- grpcio     1.63.0
-- protobuf   5.26.1
-
-
-## API 
-
-
-
-### Get API Instance  `create_camera_service_api`  
-
-- host , camera server host , e.g.  `localhost` 
-- port , camera server port , e.g.  `6000`
-
-
-```python 
-
-# host 
-api = create_camera_service_api(host, port)
-
-
-```
-### Get All camera meta infos `get_camera_metas`
-
-```python
-
-def get_camera_metas(self) -> List[CameraMeta]:
-    ...     
-
-```
-
-```python
-
-metas = api.get_camera_metas()
-for meta in metas:
-    print(f"Camera modelName: {meta.modelName} - deviceVersion: {meta.deviceVersion}")
-    print("get camera image serialNumber ", meta.serialNumber)
-    print("get info ", meta.info)
-
-
-```
-
-### CameraMeta 
-
-- cameraType , camera type , `GIGE` | `u3v` 
-- serialNumber : camera serial number , 
-- modelName  : model name 
-- manufactureName : manufacture name 
-- deviceVersion :  device version 
-- userDefinedName : name defined by user 
-- info : Map[string,string] , ext info 
-
-
-### Get live image by serial number 
-
-input camera serial number and return live image (jpg), bytes.
-and if return `None` means the camera maybe offline. 
-
-and using `try .. except` for catch `exception` 
-
-```python
-
-def get_image(self, sn: str) -> bytes:
-    ...     
-
-```
-
-Example: 
-
-```python
-
-...
-body = api.get_image(meta.serialNumber)
-print(" body : ", len(body)  )
-
-...
-
-fopen = open('test.jpg', 'wb+')
-fopen.write( body )
-fopen.close()
-
-...
-
-```
-
-
-## Example 
-
-```python
-import time
-
-import grpc
-
-from services.cameras.camera_service_api import create_camera_service_api
-
-
-max_test = 100
-
-def test_camera_api(host, port):
-    #
-    api = create_camera_service_api(host, port)
-    metas = api.get_camera_metas()
-    for meta in metas:
-        print(f"Camera modelName: {meta.modelName} - deviceVersion: {meta.deviceVersion}")
-        print("get camera image serialNumber ", meta.serialNumber)
-        print("get info ", meta.info)
-
-        t1 = time.time()
-        try:
-        
-            for i in range( max_test ):
-                body = api.get_image(meta.serialNumber)
-                print(" body : ", i, len(body)  )
-
-        except Exception as e:
-            print( e) 
-
-        t2 = time.time()
-        tt = t2-t1
-        avg = tt / max_test
-        print( f" Try {max_test} times get image , using {tt} , avg {avg} ")
-
-        # fopen = open('body.jpg'.encode('utf-8'), 'wb+')
-        # fopen.write( body, )
-        # fopen.close()
-
-# protect the entry point
-if __name__ == '__main__':
-    print("GRPC Version : {} ".format(grpc.__version__))
-    test_camera_api("127.0.0.1", 6000)
-
-
-
-```
```

### Comparing `camera_service_api-1.1/README.md` & `camera-service-api-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `camera_service_api-1.1/camera_service_api.egg-info/PKG-INFO` & `camera-service-api-1.1.1/camera_service_api.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,163 +1,162 @@
 Metadata-Version: 2.1
 Name: camera-service-api
-Version: 1.1
-Summary: Camera service grpc api
-Home-page: 
+Version: 1.1.1
+Summary: Camera service grpc api (for python3.7 )
+Home-page: UNKNOWN
 Author: L.K
 Author-email: L.K@idontwant.com
+License: UNKNOWN
+Description: # Camera service grpc API 
+        
+        ## Install 
+        
+        1. using pip install local package 
+          
+        ```bash
+        
+        pip install camera-service-api
+        
+        ```
+        
+        
+        ## Dependencies 
+        
+        - grpcio     1.63.0
+        - protobuf   5.26.1
+        
+        
+        ## API 
+        
+        
+        
+        ### Get API Instance  `create_camera_service_api`  
+        
+        - host , camera server host , e.g.  `localhost` 
+        - port , camera server port , e.g.  `6000`
+        
+        
+        ```python 
+        
+        # host 
+        api = create_camera_service_api(host, port)
+        
+        
+        ```
+        ### Get All camera meta infos `get_camera_metas`
+        
+        ```python
+        
+        def get_camera_metas(self) -> List[CameraMeta]:
+            ...     
+        
+        ```
+        
+        ```python
+        
+        metas = api.get_camera_metas()
+        for meta in metas:
+            print(f"Camera modelName: {meta.modelName} - deviceVersion: {meta.deviceVersion}")
+            print("get camera image serialNumber ", meta.serialNumber)
+            print("get info ", meta.info)
+        
+        
+        ```
+        
+        ### CameraMeta 
+        
+        - cameraType , camera type , `GIGE` | `u3v` 
+        - serialNumber : camera serial number , 
+        - modelName  : model name 
+        - manufactureName : manufacture name 
+        - deviceVersion :  device version 
+        - userDefinedName : name defined by user 
+        - info : Map[string,string] , ext info 
+        
+        
+        ### Get live image by serial number 
+        
+        input camera serial number and return live image (jpg), bytes.
+        and if return `None` means the camera maybe offline. 
+        
+        and using `try .. except` for catch `exception` 
+        
+        ```python
+        
+        def get_image(self, sn: str) -> bytes:
+            ...     
+        
+        ```
+        
+        Example: 
+        
+        ```python
+        
+        ...
+        body = api.get_image(meta.serialNumber)
+        print(" body : ", len(body)  )
+        
+        ...
+        
+        fopen = open('test.jpg', 'wb+')
+        fopen.write( body )
+        fopen.close()
+        
+        ...
+        
+        ```
+        
+        
+        ## Example 
+        
+        ```python
+        import time
+        
+        import grpc
+        
+        from services.cameras.camera_service_api import create_camera_service_api
+        
+        
+        max_test = 100
+        
+        def test_camera_api(host, port):
+            #
+            api = create_camera_service_api(host, port)
+            metas = api.get_camera_metas()
+            for meta in metas:
+                print(f"Camera modelName: {meta.modelName} - deviceVersion: {meta.deviceVersion}")
+                print("get camera image serialNumber ", meta.serialNumber)
+                print("get info ", meta.info)
+        
+                t1 = time.time()
+                try:
+                
+                    for i in range( max_test ):
+                        body = api.get_image(meta.serialNumber)
+                        print(" body : ", i, len(body)  )
+        
+                except Exception as e:
+                    print( e) 
+        
+                t2 = time.time()
+                tt = t2-t1
+                avg = tt / max_test
+                print( f" Try {max_test} times get image , using {tt} , avg {avg} ")
+        
+                # fopen = open('body.jpg'.encode('utf-8'), 'wb+')
+                # fopen.write( body, )
+                # fopen.close()
+        
+        # protect the entry point
+        if __name__ == '__main__':
+            print("GRPC Version : {} ".format(grpc.__version__))
+            test_camera_api("127.0.0.1", 6000)
+        
+        
+        
+        ```
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Requires-Dist: grpcio
-Requires-Dist: protobuf
-
-# Camera service grpc API 
-
-## Install 
-
-1. using pip install local package 
-  
-```bash
-
-pip install camera-service-api
-
-```
-
-
-## Dependencies 
-
-- grpcio     1.63.0
-- protobuf   5.26.1
-
-
-## API 
-
-
-
-### Get API Instance  `create_camera_service_api`  
-
-- host , camera server host , e.g.  `localhost` 
-- port , camera server port , e.g.  `6000`
-
-
-```python 
-
-# host 
-api = create_camera_service_api(host, port)
-
-
-```
-### Get All camera meta infos `get_camera_metas`
-
-```python
-
-def get_camera_metas(self) -> List[CameraMeta]:
-    ...     
-
-```
-
-```python
-
-metas = api.get_camera_metas()
-for meta in metas:
-    print(f"Camera modelName: {meta.modelName} - deviceVersion: {meta.deviceVersion}")
-    print("get camera image serialNumber ", meta.serialNumber)
-    print("get info ", meta.info)
-
-
-```
-
-### CameraMeta 
-
-- cameraType , camera type , `GIGE` | `u3v` 
-- serialNumber : camera serial number , 
-- modelName  : model name 
-- manufactureName : manufacture name 
-- deviceVersion :  device version 
-- userDefinedName : name defined by user 
-- info : Map[string,string] , ext info 
-
-
-### Get live image by serial number 
-
-input camera serial number and return live image (jpg), bytes.
-and if return `None` means the camera maybe offline. 
-
-and using `try .. except` for catch `exception` 
-
-```python
-
-def get_image(self, sn: str) -> bytes:
-    ...     
-
-```
-
-Example: 
-
-```python
-
-...
-body = api.get_image(meta.serialNumber)
-print(" body : ", len(body)  )
-
-...
-
-fopen = open('test.jpg', 'wb+')
-fopen.write( body )
-fopen.close()
-
-...
-
-```
-
-
-## Example 
-
-```python
-import time
-
-import grpc
-
-from services.cameras.camera_service_api import create_camera_service_api
-
-
-max_test = 100
-
-def test_camera_api(host, port):
-    #
-    api = create_camera_service_api(host, port)
-    metas = api.get_camera_metas()
-    for meta in metas:
-        print(f"Camera modelName: {meta.modelName} - deviceVersion: {meta.deviceVersion}")
-        print("get camera image serialNumber ", meta.serialNumber)
-        print("get info ", meta.info)
-
-        t1 = time.time()
-        try:
-        
-            for i in range( max_test ):
-                body = api.get_image(meta.serialNumber)
-                print(" body : ", i, len(body)  )
-
-        except Exception as e:
-            print( e) 
-
-        t2 = time.time()
-        tt = t2-t1
-        avg = tt / max_test
-        print( f" Try {max_test} times get image , using {tt} , avg {avg} ")
-
-        # fopen = open('body.jpg'.encode('utf-8'), 'wb+')
-        # fopen.write( body, )
-        # fopen.close()
-
-# protect the entry point
-if __name__ == '__main__':
-    print("GRPC Version : {} ".format(grpc.__version__))
-    test_camera_api("127.0.0.1", 6000)
-
-
-
-```
```

### Comparing `camera_service_api-1.1/camera_service_api.egg-info/SOURCES.txt` & `camera-service-api-1.1.1/camera_service_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `camera_service_api-1.1/services/cameras/camera_service_api.py` & `camera-service-api-1.1.1/services/cameras/camera_service_api.py`

 * *Files identical despite different names*

### Comparing `camera_service_api-1.1/services/cameras/models.py` & `camera-service-api-1.1.1/services/cameras/models.py`

 * *Files identical despite different names*

### Comparing `camera_service_api-1.1/services/grpc/camera_service_pb2.py` & `camera-service-api-1.1.1/services/grpc/camera_service_pb2.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: services/grpc/camera-service.proto
-# Protobuf Python Version: 5.26.1
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -16,17 +16,17 @@
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"services/grpc/camera-service.proto\x12\x0cservice.grpc\x1a\x1bgoogle/protobuf/empty.proto\"\xf1\x01\n\nCameraMeta\x12\x14\n\x0cserialNumber\x18\x01 \x01(\t\x12\x11\n\tmodelName\x18\x02 \x01(\t\x12\x17\n\x0fmanufactureName\x18\x03 \x01(\t\x12\x15\n\rdeviceVersion\x18\x04 \x01(\t\x12\x17\n\x0fuserDefinedName\x18\x05 \x01(\t\x12\x12\n\ncameraType\x18\x06 \x01(\t\x12\x30\n\x04info\x18\x07 \x03(\x0b\x32\".service.grpc.CameraMeta.InfoEntry\x1a+\n\tInfoEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"5\n\x0b\x43\x61meraMetas\x12&\n\x04\x64\x61ta\x18\x01 \x03(\x0b\x32\x18.service.grpc.CameraMeta\"\x1c\n\tBytesBody\x12\x0f\n\x07\x63ontent\x18\x01 \x01(\x0c\"\x1c\n\x0bInputString\x12\r\n\x05value\x18\x01 \x01(\t2\xd3\x01\n\rCameraService\x12\x45\n\x0eGetCameraMetas\x12\x16.google.protobuf.Empty\x1a\x19.service.grpc.CameraMetas\"\x00\x12@\n\x08GetImage\x12\x19.service.grpc.InputString\x1a\x17.service.grpc.BytesBody\"\x00\x12\x39\n\x05Reset\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\"\x00\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'services.grpc.camera_service_pb2', _globals)
-if not _descriptor._USE_C_DESCRIPTORS:
-  DESCRIPTOR._loaded_options = None
-  _globals['_CAMERAMETA_INFOENTRY']._loaded_options = None
+if _descriptor._USE_C_DESCRIPTORS == False:
+  DESCRIPTOR._options = None
+  _globals['_CAMERAMETA_INFOENTRY']._options = None
   _globals['_CAMERAMETA_INFOENTRY']._serialized_options = b'8\001'
   _globals['_CAMERAMETA']._serialized_start=82
   _globals['_CAMERAMETA']._serialized_end=323
   _globals['_CAMERAMETA_INFOENTRY']._serialized_start=280
   _globals['_CAMERAMETA_INFOENTRY']._serialized_end=323
   _globals['_CAMERAMETAS']._serialized_start=325
   _globals['_CAMERAMETAS']._serialized_end=378
```

### Comparing `camera_service_api-1.1/services/grpc/grpcutilsc.py` & `camera-service-api-1.1.1/services/grpc/grpcutilsc.py`

 * *Files identical despite different names*

### Comparing `camera_service_api-1.1/services/grpc/grpcutilss.py` & `camera-service-api-1.1.1/services/grpc/grpcutilss.py`

 * *Files identical despite different names*

### Comparing `camera_service_api-1.1/services/grpc/pb2utils.py` & `camera-service-api-1.1.1/services/grpc/pb2utils.py`

 * *Files identical despite different names*

### Comparing `camera_service_api-1.1/setup.py` & `camera-service-api-1.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 with open("3rd.list.txt", "r") as fh:
     requirements = fh.readlines()
 
 pks = find_packages()  # .append('agent.py')
 print(pks)
 
 setup(name='camera-service-api',
-      version='1.1',  #
-      description='Camera service grpc api',  #
+      version='1.1.1',  #
+      description='Camera service grpc api (for python3.7 )',  #
       author='L.K',  #
       author_email='L.K@idontwant.com',  #
       url='',  #
       packages=pks,  # Python导入包的列表，我们使用find_packages() 来自动收集
       long_description=long_description,  #
       long_description_content_type="text/markdown",  #
```

