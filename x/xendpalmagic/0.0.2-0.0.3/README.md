# Comparing `tmp/xendpalmagic-0.0.2.tar.gz` & `tmp/xendpalmagic-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xendpalmagic-0.0.2.tar", last modified: Fri Apr 12 17:51:10 2024, max compression
+gzip compressed data, was "xendpalmagic-0.0.3.tar", last modified: Mon May 13 23:07:59 2024, max compression
```

## Comparing `xendpalmagic-0.0.2.tar` & `xendpalmagic-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 joelogin  (1000) joelogin  (1004)        0 2024-04-12 17:51:10.810590 xendpalmagic-0.0.2/
--rw-r--r--   0 joelogin  (1000) joelogin  (1004)        0 2024-04-11 16:29:54.000000 xendpalmagic-0.0.2/LICENSE
--rw-r--r--   0 joelogin  (1000) joelogin  (1004)      161 2024-04-11 16:29:54.000000 xendpalmagic-0.0.2/MANIFEST.in
--rw-r--r--   0 joelogin  (1000) joelogin  (1004)     3227 2024-04-12 17:51:10.810590 xendpalmagic-0.0.2/PKG-INFO
--rw-r--r--   0 joelogin  (1000) joelogin  (1004)     2243 2024-04-12 17:49:31.000000 xendpalmagic-0.0.2/README.md
--rw-r--r--   0 joelogin  (1000) joelogin  (1004)        0 2024-04-11 16:29:54.000000 xendpalmagic-0.0.2/requirements.txt
--rw-r--r--   0 joelogin  (1000) joelogin  (1004)       38 2024-04-12 17:51:10.810590 xendpalmagic-0.0.2/setup.cfg
--rw-r--r--   0 joelogin  (1000) joelogin  (1004)     3271 2024-04-12 17:49:51.000000 xendpalmagic-0.0.2/setup.py
-drwxr-xr-x   0 joelogin  (1000) joelogin  (1004)        0 2024-04-12 17:51:10.807257 xendpalmagic-0.0.2/xendpalmagic/
--rw-r--r--   0 joelogin  (1000) joelogin  (1004)       94 2024-04-12 17:32:22.000000 xendpalmagic-0.0.2/xendpalmagic/__init__.py
--rw-r--r--   0 joelogin  (1000) joelogin  (1004)     3624 2024-04-11 16:29:54.000000 xendpalmagic-0.0.2/xendpalmagic/core.py
--rw-r--r--   0 joelogin  (1000) joelogin  (1004)     1281 2024-04-11 16:29:54.000000 xendpalmagic-0.0.2/xendpalmagic/exceptions.py
--rw-r--r--   0 joelogin  (1000) joelogin  (1004)    12673 2024-04-11 16:29:54.000000 xendpalmagic-0.0.2/xendpalmagic/signatures.py
-drwxr-xr-x   0 joelogin  (1000) joelogin  (1004)        0 2024-04-12 17:51:10.810590 xendpalmagic-0.0.2/xendpalmagic.egg-info/
--rw-r--r--   0 joelogin  (1000) joelogin  (1004)     3227 2024-04-12 17:51:10.000000 xendpalmagic-0.0.2/xendpalmagic.egg-info/PKG-INFO
--rw-r--r--   0 joelogin  (1000) joelogin  (1004)      299 2024-04-12 17:51:10.000000 xendpalmagic-0.0.2/xendpalmagic.egg-info/SOURCES.txt
--rw-r--r--   0 joelogin  (1000) joelogin  (1004)        1 2024-04-12 17:51:10.000000 xendpalmagic-0.0.2/xendpalmagic.egg-info/dependency_links.txt
--rw-r--r--   0 joelogin  (1000) joelogin  (1004)       13 2024-04-12 17:51:10.000000 xendpalmagic-0.0.2/xendpalmagic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:07:59.743962 xendpalmagic-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 23:07:51.000000 xendpalmagic-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-13 23:07:51.000000 xendpalmagic-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-05-13 23:07:59.743962 xendpalmagic-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-13 23:07:51.000000 xendpalmagic-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 23:07:51.000000 xendpalmagic-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 23:07:59.743962 xendpalmagic-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-05-13 23:07:51.000000 xendpalmagic-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:07:59.743962 xendpalmagic-0.0.3/xendpalmagic/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-13 23:07:51.000000 xendpalmagic-0.0.3/xendpalmagic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-05-13 23:07:51.000000 xendpalmagic-0.0.3/xendpalmagic/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-13 23:07:51.000000 xendpalmagic-0.0.3/xendpalmagic/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12673 2024-05-13 23:07:51.000000 xendpalmagic-0.0.3/xendpalmagic/signatures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:07:59.743962 xendpalmagic-0.0.3/xendpalmagic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-05-13 23:07:59.000000 xendpalmagic-0.0.3/xendpalmagic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-13 23:07:59.000000 xendpalmagic-0.0.3/xendpalmagic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 23:07:59.000000 xendpalmagic-0.0.3/xendpalmagic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-13 23:07:59.000000 xendpalmagic-0.0.3/xendpalmagic.egg-info/top_level.txt
```

### Comparing `xendpalmagic-0.0.2/PKG-INFO` & `xendpalmagic-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: xendpalmagic
-Version: 0.0.2
-Summary: Xendpal-magic: Advanced File Type Detection Library
+Version: 0.0.3
+Summary: Xendpalmagic: Advanced File Type Detection Library
 Author: joeygoesgrey
 Author-email: <mail@godfreydjoseph@gmail.com>
 License: MIT
 Keywords: file type detection,file signatures,MIME type,content analysis,python,file handling,file identification,magic numbers,file metadata
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -21,17 +21,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 
 ---
 
-# Xendpal-magic: Advanced File Type Detection Library
+# Xendpalmagic: Advanced File Type Detection Library
 
-Xendpal-magic is a comprehensive Python library designed to enhance file type detection through a multi-faceted approach. By combining file extensions, magic numbers, content analysis, and header parsing, Xendpal-magic offers unmatched accuracy and reliability for identifying a wide range of file formats.
+Xendpalmagic is a comprehensive Python library designed to enhance file type detection through a multi-faceted approach. By combining file extensions, magic numbers, content analysis, and header parsing, Xendpalmagic offers unmatched accuracy and reliability for identifying a wide range of file formats.
 
 ## Features
 
 - **Robust File Type Detection**: Utilizes magic numbers, content analysis, and header parsing for accurate file identification.
 - **Customizable Detection Strategies**: Tailor the detection process to prioritize speed, accuracy, or a balance of both.
 - **Extensive File Format Support**: Comes with a broad database of file signatures and MIME types, with the flexibility to add new ones.
 - **Developer-friendly**: Easy to integrate and use in any Python project requiring file handling capabilities.
@@ -49,26 +49,28 @@
 ```python
 from xendpalmagic import FileSignatureMatcher
 
 # Initialize the matcher
 matcher = FileSignatureMatcher()
 
 # Determine the file type of 'example.pdf'
-file_type = matcher.determine_file_type('path to file')
+file_type, method = matcher.determine_file_type('example.pdf')
 print(file_type)  # Outputs: 'application/pdf'
+
 ```
 
 ## Advanced Usage
 
 ### Custom Detection Strategy
 
 ```python
 matcher = FileSignatureMatcher(detection_method='signature', return_type='description')
-file_description = matcher.determine_file_type('path to file')
+file_description, method = matcher.determine_file_type('example.docx')
 print(file_description)  # Outputs: 'Microsoft Word document'
+
 ```
 
 ### Adding Custom File Signatures
 
 ```python
 matcher.add_custom_signature(
     extension='custom',
@@ -80,16 +82,16 @@
 
 ## Contributing
 
 Contributions are welcome! Please read our [Contributing Guide](CONTRIBUTING.md) for details on how to submit pull requests, report issues, and suggest improvements.
 
 ## License
 
-Xendpal-magic is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
+Xendpalmagic is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
 
 ## Acknowledgments
 
-- Special thanks to all [contributors](https://github.com/yourusername/xendpal-magic/contributors) who have helped shape Xendpalmagic into what it is today.
+- Special thanks to all [contributors](https://github.com/yourusername/xendpal-magic/contributors) who have helped shape Xendpal-magic into what it is today.
 
 ---
```

### Comparing `xendpalmagic-0.0.2/README.md` & `xendpalmagic-0.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 ---
 
-# Xendpal-magic: Advanced File Type Detection Library
+# Xendpalmagic: Advanced File Type Detection Library
 
-Xendpal-magic is a comprehensive Python library designed to enhance file type detection through a multi-faceted approach. By combining file extensions, magic numbers, content analysis, and header parsing, Xendpal-magic offers unmatched accuracy and reliability for identifying a wide range of file formats.
+Xendpalmagic is a comprehensive Python library designed to enhance file type detection through a multi-faceted approach. By combining file extensions, magic numbers, content analysis, and header parsing, Xendpalmagic offers unmatched accuracy and reliability for identifying a wide range of file formats.
 
 ## Features
 
 - **Robust File Type Detection**: Utilizes magic numbers, content analysis, and header parsing for accurate file identification.
 - **Customizable Detection Strategies**: Tailor the detection process to prioritize speed, accuracy, or a balance of both.
 - **Extensive File Format Support**: Comes with a broad database of file signatures and MIME types, with the flexibility to add new ones.
 - **Developer-friendly**: Easy to integrate and use in any Python project requiring file handling capabilities.
@@ -25,26 +25,28 @@
 ```python
 from xendpalmagic import FileSignatureMatcher
 
 # Initialize the matcher
 matcher = FileSignatureMatcher()
 
 # Determine the file type of 'example.pdf'
-file_type = matcher.determine_file_type('path to file')
+file_type, method = matcher.determine_file_type('example.pdf')
 print(file_type)  # Outputs: 'application/pdf'
+
 ```
 
 ## Advanced Usage
 
 ### Custom Detection Strategy
 
 ```python
 matcher = FileSignatureMatcher(detection_method='signature', return_type='description')
-file_description = matcher.determine_file_type('path to file')
+file_description, method = matcher.determine_file_type('example.docx')
 print(file_description)  # Outputs: 'Microsoft Word document'
+
 ```
 
 ### Adding Custom File Signatures
 
 ```python
 matcher.add_custom_signature(
     extension='custom',
@@ -56,16 +58,16 @@
 
 ## Contributing
 
 Contributions are welcome! Please read our [Contributing Guide](CONTRIBUTING.md) for details on how to submit pull requests, report issues, and suggest improvements.
 
 ## License
 
-Xendpal-magic is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
+Xendpalmagic is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
 
 ## Acknowledgments
 
-- Special thanks to all [contributors](https://github.com/yourusername/xendpal-magic/contributors) who have helped shape Xendpalmagic into what it is today.
+- Special thanks to all [contributors](https://github.com/yourusername/xendpal-magic/contributors) who have helped shape Xendpal-magic into what it is today.
 
 ---
```

### Comparing `xendpalmagic-0.0.2/setup.py` & `xendpalmagic-0.0.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.2'
-DESCRIPTION = 'Xendpal-magic: Advanced File Type Detection Library'
-LONG_DESCRIPTION = """Xendpal-magic is a cutting-edge Python library designed to elevate file type detection to new heights. Unlike traditional methods that rely solely on file extensions or basic signatures, Xendpal-magic introduces a multifaceted approach incorporating file extensions, magic numbers, content analysis, and header parsing to deliver unparalleled accuracy and reliability. This library stands out by offering customizable detection strategies, allowing users to tailor the detection process to their specific needs—whether prioritizing speed, accuracy, or a balance of both.
+VERSION = '0.0.3'
+DESCRIPTION = 'Xendpalmagic: Advanced File Type Detection Library'
+LONG_DESCRIPTION = """Xendpalmagic is a cutting-edge Python library designed to elevate file type detection to new heights. Unlike traditional methods that rely solely on file extensions or basic signatures, Xendpalmagic introduces a multifaceted approach incorporating file extensions, magic numbers, content analysis, and header parsing to deliver unparalleled accuracy and reliability. This library stands out by offering customizable detection strategies, allowing users to tailor the detection process to their specific needs—whether prioritizing speed, accuracy, or a balance of both.
 
-At the heart of Xendpal-magic lies a comprehensive database of file signatures and MIME types, covering a vast spectrum of file formats. From common image and document formats to more obscure or custom file types, Xendpal-magic ensures your application can identify and handle a wide array of files confidently. Furthermore, the library's extensible design means users can effortlessly add new signatures and MIME types, making it an ever-evolving tool that adapts to new file formats and industry standards.
+At the heart of Xendpalmagic lies a comprehensive database of file signatures and MIME types, covering a vast spectrum of file formats. From common image and document formats to more obscure or custom file types, Xendpalmagic ensures your application can identify and handle a wide array of files confidently. Furthermore, the library's extensible design means users can effortlessly add new signatures and MIME types, making it an ever-evolving tool that adapts to new file formats and industry standards.
 
-Designed with both ease of use and flexibility in mind, Xendpal-magic caters to developers looking for a simple solution to file type detection while also offering advanced features for those needing more control over the detection process. Whether you're building a content management system, a digital asset manager, or any application that requires robust file handling capabilities, Xendpal-magic is equipped to meet the challenge.
+Designed with both ease of use and flexibility in mind, Xendpalmagic caters to developers looking for a simple solution to file type detection while also offering advanced features for those needing more control over the detection process. Whether you're building a content management system, a digital asset manager, or any application that requires robust file handling capabilities, Xendpalmagic is equipped to meet the challenge.
 
 Embrace the future of file type detection with Xendpal-magic and unlock the potential to create more intelligent, efficient, and secure applications."""
 
 # Setting up
 setup(
     name="xendpalmagic",
     version=VERSION,
```

### Comparing `xendpalmagic-0.0.2/xendpalmagic/core.py` & `xendpalmagic-0.0.3/xendpalmagic/core.py`

 * *Files identical despite different names*

### Comparing `xendpalmagic-0.0.2/xendpalmagic/exceptions.py` & `xendpalmagic-0.0.3/xendpalmagic/exceptions.py`

 * *Files identical despite different names*

### Comparing `xendpalmagic-0.0.2/xendpalmagic/signatures.py` & `xendpalmagic-0.0.3/xendpalmagic/signatures.py`

 * *Files identical despite different names*

### Comparing `xendpalmagic-0.0.2/xendpalmagic.egg-info/PKG-INFO` & `xendpalmagic-0.0.3/xendpalmagic.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: xendpalmagic
-Version: 0.0.2
-Summary: Xendpal-magic: Advanced File Type Detection Library
+Version: 0.0.3
+Summary: Xendpalmagic: Advanced File Type Detection Library
 Author: joeygoesgrey
 Author-email: <mail@godfreydjoseph@gmail.com>
 License: MIT
 Keywords: file type detection,file signatures,MIME type,content analysis,python,file handling,file identification,magic numbers,file metadata
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -21,17 +21,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 
 ---
 
-# Xendpal-magic: Advanced File Type Detection Library
+# Xendpalmagic: Advanced File Type Detection Library
 
-Xendpal-magic is a comprehensive Python library designed to enhance file type detection through a multi-faceted approach. By combining file extensions, magic numbers, content analysis, and header parsing, Xendpal-magic offers unmatched accuracy and reliability for identifying a wide range of file formats.
+Xendpalmagic is a comprehensive Python library designed to enhance file type detection through a multi-faceted approach. By combining file extensions, magic numbers, content analysis, and header parsing, Xendpalmagic offers unmatched accuracy and reliability for identifying a wide range of file formats.
 
 ## Features
 
 - **Robust File Type Detection**: Utilizes magic numbers, content analysis, and header parsing for accurate file identification.
 - **Customizable Detection Strategies**: Tailor the detection process to prioritize speed, accuracy, or a balance of both.
 - **Extensive File Format Support**: Comes with a broad database of file signatures and MIME types, with the flexibility to add new ones.
 - **Developer-friendly**: Easy to integrate and use in any Python project requiring file handling capabilities.
@@ -49,26 +49,28 @@
 ```python
 from xendpalmagic import FileSignatureMatcher
 
 # Initialize the matcher
 matcher = FileSignatureMatcher()
 
 # Determine the file type of 'example.pdf'
-file_type = matcher.determine_file_type('path to file')
+file_type, method = matcher.determine_file_type('example.pdf')
 print(file_type)  # Outputs: 'application/pdf'
+
 ```
 
 ## Advanced Usage
 
 ### Custom Detection Strategy
 
 ```python
 matcher = FileSignatureMatcher(detection_method='signature', return_type='description')
-file_description = matcher.determine_file_type('path to file')
+file_description, method = matcher.determine_file_type('example.docx')
 print(file_description)  # Outputs: 'Microsoft Word document'
+
 ```
 
 ### Adding Custom File Signatures
 
 ```python
 matcher.add_custom_signature(
     extension='custom',
@@ -80,16 +82,16 @@
 
 ## Contributing
 
 Contributions are welcome! Please read our [Contributing Guide](CONTRIBUTING.md) for details on how to submit pull requests, report issues, and suggest improvements.
 
 ## License
 
-Xendpal-magic is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
+Xendpalmagic is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
 
 ## Acknowledgments
 
-- Special thanks to all [contributors](https://github.com/yourusername/xendpal-magic/contributors) who have helped shape Xendpalmagic into what it is today.
+- Special thanks to all [contributors](https://github.com/yourusername/xendpal-magic/contributors) who have helped shape Xendpal-magic into what it is today.
 
 ---
```

