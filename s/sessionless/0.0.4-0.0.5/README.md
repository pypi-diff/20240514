# Comparing `tmp/sessionless-0.0.4.tar.gz` & `tmp/sessionless-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sessionless-0.0.4.tar", last modified: Sun Apr 28 14:24:15 2024, max compression
+gzip compressed data, was "sessionless-0.0.5.tar", last modified: Mon May 13 22:33:38 2024, max compression
```

## Comparing `sessionless-0.0.4.tar` & `sessionless-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 habsoomane   (501) staff       (20)        0 2024-04-28 14:24:15.848871 sessionless-0.0.4/
--rw-r--r--   0 habsoomane   (501) staff       (20)     3882 2024-04-28 14:24:15.847945 sessionless-0.0.4/PKG-INFO
--rw-r--r--   0 habsoomane   (501) staff       (20)     3274 2024-04-27 23:39:27.000000 sessionless-0.0.4/README.md
-drwxr-xr-x   0 habsoomane   (501) staff       (20)        0 2024-04-28 14:24:15.839877 sessionless-0.0.4/sessionless/
--rw-r--r--   0 habsoomane   (501) staff       (20)       59 2024-04-27 23:29:22.000000 sessionless-0.0.4/sessionless/__init__.py
--rw-r--r--   0 habsoomane   (501) staff       (20)     2273 2024-04-27 23:42:26.000000 sessionless-0.0.4/sessionless/modelsecp256k1.py
-drwxr-xr-x   0 habsoomane   (501) staff       (20)        0 2024-04-28 14:24:15.846876 sessionless-0.0.4/sessionless.egg-info/
--rw-r--r--   0 habsoomane   (501) staff       (20)     3882 2024-04-28 14:24:15.000000 sessionless-0.0.4/sessionless.egg-info/PKG-INFO
--rw-r--r--   0 habsoomane   (501) staff       (20)      291 2024-04-28 14:24:15.000000 sessionless-0.0.4/sessionless.egg-info/SOURCES.txt
--rw-r--r--   0 habsoomane   (501) staff       (20)        1 2024-04-28 14:24:15.000000 sessionless-0.0.4/sessionless.egg-info/dependency_links.txt
--rw-r--r--   0 habsoomane   (501) staff       (20)       15 2024-04-28 14:24:15.000000 sessionless-0.0.4/sessionless.egg-info/requires.txt
--rw-r--r--   0 habsoomane   (501) staff       (20)       17 2024-04-28 14:24:15.000000 sessionless-0.0.4/sessionless.egg-info/top_level.txt
--rw-r--r--   0 habsoomane   (501) staff       (20)       38 2024-04-28 14:24:15.849059 sessionless-0.0.4/setup.cfg
--rw-r--r--   0 habsoomane   (501) staff       (20)     1126 2024-04-27 23:01:41.000000 sessionless-0.0.4/setup.py
-drwxr-xr-x   0 habsoomane   (501) staff       (20)        0 2024-04-28 14:24:15.845574 sessionless-0.0.4/test/
--rw-r--r--   0 habsoomane   (501) staff       (20)       69 2024-04-27 23:23:43.000000 sessionless-0.0.4/test/__init__.py
--rw-r--r--   0 habsoomane   (501) staff       (20)     2761 2024-04-27 23:43:45.000000 sessionless-0.0.4/test/test_modelsecp256k1.py
+drwxr-xr-x   0 habsoomane   (501) staff       (20)        0 2024-05-13 22:33:38.346764 sessionless-0.0.5/
+-rw-r--r--   0 habsoomane   (501) staff       (20)     3910 2024-05-13 22:33:38.346226 sessionless-0.0.5/PKG-INFO
+-rw-r--r--   0 habsoomane   (501) staff       (20)     3274 2024-04-27 23:39:27.000000 sessionless-0.0.5/README.md
+drwxr-xr-x   0 habsoomane   (501) staff       (20)        0 2024-05-13 22:33:38.339732 sessionless-0.0.5/sessionless/
+-rw-r--r--   0 habsoomane   (501) staff       (20)       59 2024-04-27 23:29:22.000000 sessionless-0.0.5/sessionless/__init__.py
+-rw-r--r--   0 habsoomane   (501) staff       (20)     2948 2024-05-13 22:32:31.000000 sessionless-0.0.5/sessionless/modelsecp256k1.py
+drwxr-xr-x   0 habsoomane   (501) staff       (20)        0 2024-05-13 22:33:38.345603 sessionless-0.0.5/sessionless.egg-info/
+-rw-r--r--   0 habsoomane   (501) staff       (20)     3910 2024-05-13 22:33:38.000000 sessionless-0.0.5/sessionless.egg-info/PKG-INFO
+-rw-r--r--   0 habsoomane   (501) staff       (20)      291 2024-05-13 22:33:38.000000 sessionless-0.0.5/sessionless.egg-info/SOURCES.txt
+-rw-r--r--   0 habsoomane   (501) staff       (20)        1 2024-05-13 22:33:38.000000 sessionless-0.0.5/sessionless.egg-info/dependency_links.txt
+-rw-r--r--   0 habsoomane   (501) staff       (20)       28 2024-05-13 22:33:38.000000 sessionless-0.0.5/sessionless.egg-info/requires.txt
+-rw-r--r--   0 habsoomane   (501) staff       (20)       17 2024-05-13 22:33:38.000000 sessionless-0.0.5/sessionless.egg-info/top_level.txt
+-rw-r--r--   0 habsoomane   (501) staff       (20)       38 2024-05-13 22:33:38.346847 sessionless-0.0.5/setup.cfg
+-rw-r--r--   0 habsoomane   (501) staff       (20)     1143 2024-05-13 22:33:00.000000 sessionless-0.0.5/setup.py
+drwxr-xr-x   0 habsoomane   (501) staff       (20)        0 2024-05-13 22:33:38.344587 sessionless-0.0.5/test/
+-rw-r--r--   0 habsoomane   (501) staff       (20)       69 2024-04-27 23:23:43.000000 sessionless-0.0.5/test/__init__.py
+-rw-r--r--   0 habsoomane   (501) staff       (20)     2761 2024-04-27 23:43:45.000000 sessionless-0.0.5/test/test_modelsecp256k1.py
```

### Comparing `sessionless-0.0.4/PKG-INFO` & `sessionless-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: sessionless
-Version: 0.0.4
+Version: 0.0.5
 Summary: Sessionless is an attempt to make authentication handling easier for developers without traditional sessions.
 Author: Sessionless Team
 Author-email: zach@planetnine.app
 Keywords: authentication,cryptography,authenticate
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 Requires-Dist: secp256k1
 Requires-Dist: uuid
+Requires-Dist: pycryptodome
 
 <div align="center">
     <h1> Sessionless : Python</h1>
 </div>
 
 ## About
```

### Comparing `sessionless-0.0.4/README.md` & `sessionless-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `sessionless-0.0.4/sessionless/modelsecp256k1.py` & `sessionless-0.0.5/sessionless/modelsecp256k1.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 import secp256k1
 import pickle
 import uuid
+from Crypto.Hash import keccak
+
+class DigestableKeccak(): # I don't know if a class is the right way to do this
+    def digest(self, msg):
+        k = keccak.new(digest_bits=256)
+        k.update(msg)
+        return k
 
 class SessionlessSecp256k1():       
     def generateUUID(self):
         return uuid.uuid4().hex
     
     def generateKeys(self, saveKeys):
         try: 
@@ -18,33 +25,43 @@
         except Exception:
             raise TypeError("No default secure storage in python. Please provide a callable method to store private key.")
     
     async def sign(self, msg, getKey):
         try:
             privateKey = getKey()
             if not isinstance(msg, bytes):
-                msg = pickle.dumps(msg)
+                msg = msg.encode('ascii')
             privateKeyObj = secp256k1.PrivateKey()
             privateKeyObj.deserialize(privateKey)
-            deserializedSig = privateKeyObj.ecdsa_sign(msg)
+   
+            digestable_keccak = DigestableKeccak()
+            print(msg[0])
+            print(msg[1])
+            raw_msg = digestable_keccak.digest(msg)
+            deserializedSig = privateKeyObj.ecdsa_sign(raw_msg.digest(), raw=True)
+#            deserializedSig = privateKeyObj.ecdsa_sign(msg, digest=digestable_keccak.digest)
             sig = privateKeyObj.ecdsa_serialize_compact(deserializedSig)
             return sig.hex()
         except Exception:
             raise ValueError("Value not provided in correct format.")
         
     def verifySignature(self, signature, msg, publicKey):
         try:
             if not isinstance(msg, bytes):
-                msg = pickle.dumps(msg)
+                msg = msg.encode('ascii')
             sig = bytes.fromhex(signature)
             publicKeyObj = secp256k1.PublicKey()
             publicKeyObj.deserialize(bytes.fromhex(publicKey))
-            
+
+            digestable_keccak = DigestableKeccak()
+            raw_msg = digestable_keccak.digest(msg)
             signature = publicKeyObj.ecdsa_deserialize_compact(sig)
-            return publicKeyObj.ecdsa_verify(msg, signature)
+
+#            return publicKeyObj.ecdsa_verify(msg, signature)
+            return publicKeyObj.ecdsa_verify(raw_msg.digest(), signature, raw=True)
         except Exception:
             raise ValueError("Error with parameters. Please ensure values are provided in correct format.")
     
     def associate(self, primarySignature, primaryMsg, primaryPublicKey, secondarySignature, secondaryMsg, secondaryPublicKey ):
         try:
             return (self.verifySignature(primarySignature, primaryMsg, primaryPublicKey) and self.verifySignature(secondarySignature, secondaryMsg, secondaryPublicKey))
         except Exception:
```

### Comparing `sessionless-0.0.4/sessionless.egg-info/PKG-INFO` & `sessionless-0.0.5/sessionless.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: sessionless
-Version: 0.0.4
+Version: 0.0.5
 Summary: Sessionless is an attempt to make authentication handling easier for developers without traditional sessions.
 Author: Sessionless Team
 Author-email: zach@planetnine.app
 Keywords: authentication,cryptography,authenticate
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 Requires-Dist: secp256k1
 Requires-Dist: uuid
+Requires-Dist: pycryptodome
 
 <div align="center">
     <h1> Sessionless : Python</h1>
 </div>
 
 ## About
```

### Comparing `sessionless-0.0.4/setup.py` & `sessionless-0.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from setuptools import setup, find_packages
 
 def read_markdown_file(file_path):
     with open(file_path, 'r', encoding='utf-8') as file:
         markdown_content = file.read()
     return markdown_content
 
-VERSION = '0.0.4' 
+VERSION = '0.0.5' 
 DESCRIPTION = 'Sessionless is an attempt to make authentication handling easier for developers without traditional sessions.'
 LONG_DESCRIPTION = read_markdown_file("./README.md")
 
 # Setting up
 setup(
         name="sessionless", 
         version=VERSION,
         author="Sessionless Team",
         author_email="zach@planetnine.app",
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
         long_description_content_type="text/markdown",
         packages=find_packages(),
-        install_requires=["secp256k1", "uuid"],
+        install_requires=["secp256k1", "uuid", "pycryptodome"],
         keywords=['authentication', 'cryptography', 'authenticate'],
         classifiers= [
             "Development Status :: 3 - Alpha",
             "Intended Audience :: Developers",
             "Programming Language :: Python :: 3",
             "Operating System :: MacOS :: MacOS X",
             "Operating System :: Microsoft :: Windows",
         ]
-)
+)
```

### Comparing `sessionless-0.0.4/test/test_modelsecp256k1.py` & `sessionless-0.0.5/test/test_modelsecp256k1.py`

 * *Files identical despite different names*

