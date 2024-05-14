# Comparing `tmp/libwiipy-0.2.2.tar.gz` & `tmp/libwiipy-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libwiipy-0.2.2.tar", last modified: Wed May  1 03:09:12 2024, max compression
+gzip compressed data, was "libwiipy-0.2.3.tar", last modified: Tue May 14 14:29:43 2024, max compression
```

## Comparing `libwiipy-0.2.2.tar` & `libwiipy-0.2.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 campbell  (1000) campbell  (1000)        0 2024-05-01 03:09:12.989026 libwiipy-0.2.2/
--rw-r--r--   0 campbell  (1000) campbell  (1000)     1056 2024-02-06 23:30:14.000000 libwiipy-0.2.2/LICENSE
--rw-r--r--   0 campbell  (1000) campbell  (1000)     4600 2024-05-01 03:09:12.989026 libwiipy-0.2.2/PKG-INFO
--rw-r--r--   0 campbell  (1000) campbell  (1000)     3942 2024-04-04 03:07:12.000000 libwiipy-0.2.2/README.md
--rw-r--r--   0 campbell  (1000) campbell  (1000)      753 2024-05-01 03:08:41.000000 libwiipy-0.2.2/pyproject.toml
--rw-r--r--   0 campbell  (1000) campbell  (1000)       38 2024-05-01 03:09:12.989026 libwiipy-0.2.2/setup.cfg
-drwxr-xr-x   0 campbell  (1000) campbell  (1000)        0 2024-05-01 03:09:12.982360 libwiipy-0.2.2/src/
-drwxr-xr-x   0 campbell  (1000) campbell  (1000)        0 2024-05-01 03:09:12.985693 libwiipy-0.2.2/src/libWiiPy/
--rw-r--r--   0 campbell  (1000) campbell  (1000)      350 2024-04-04 01:06:05.000000 libwiipy-0.2.2/src/libWiiPy/__init__.py
--rw-r--r--   0 campbell  (1000) campbell  (1000)     1086 2024-04-14 16:45:16.000000 libwiipy-0.2.2/src/libWiiPy/commonkeys.py
--rw-r--r--   0 campbell  (1000) campbell  (1000)    16468 2024-04-03 22:17:05.000000 libwiipy-0.2.2/src/libWiiPy/content.py
--rw-r--r--   0 campbell  (1000) campbell  (1000)     4264 2024-04-07 00:18:51.000000 libwiipy-0.2.2/src/libWiiPy/crypto.py
--rw-r--r--   0 campbell  (1000) campbell  (1000)     7824 2024-05-01 03:08:41.000000 libwiipy-0.2.2/src/libWiiPy/nus.py
--rw-r--r--   0 campbell  (1000) campbell  (1000)     1181 2024-04-03 22:17:05.000000 libwiipy-0.2.2/src/libWiiPy/shared.py
--rw-r--r--   0 campbell  (1000) campbell  (1000)    11921 2024-04-03 22:17:05.000000 libwiipy-0.2.2/src/libWiiPy/ticket.py
--rw-r--r--   0 campbell  (1000) campbell  (1000)     9216 2024-04-14 16:53:37.000000 libwiipy-0.2.2/src/libWiiPy/title.py
--rw-r--r--   0 campbell  (1000) campbell  (1000)    13730 2024-04-27 01:34:39.000000 libwiipy-0.2.2/src/libWiiPy/tmd.py
--rw-r--r--   0 campbell  (1000) campbell  (1000)     1938 2024-04-03 22:17:05.000000 libwiipy-0.2.2/src/libWiiPy/types.py
--rw-r--r--   0 campbell  (1000) campbell  (1000)    12515 2024-04-05 05:06:09.000000 libwiipy-0.2.2/src/libWiiPy/wad.py
-drwxr-xr-x   0 campbell  (1000) campbell  (1000)        0 2024-05-01 03:09:12.989026 libwiipy-0.2.2/src/libWiiPy.egg-info/
--rw-r--r--   0 campbell  (1000) campbell  (1000)     4600 2024-05-01 03:09:12.000000 libwiipy-0.2.2/src/libWiiPy.egg-info/PKG-INFO
--rw-r--r--   0 campbell  (1000) campbell  (1000)      460 2024-05-01 03:09:12.000000 libwiipy-0.2.2/src/libWiiPy.egg-info/SOURCES.txt
--rw-r--r--   0 campbell  (1000) campbell  (1000)        1 2024-05-01 03:09:12.000000 libwiipy-0.2.2/src/libWiiPy.egg-info/dependency_links.txt
--rw-r--r--   0 campbell  (1000) campbell  (1000)       22 2024-05-01 03:09:12.000000 libwiipy-0.2.2/src/libWiiPy.egg-info/requires.txt
--rw-r--r--   0 campbell  (1000) campbell  (1000)        9 2024-05-01 03:09:12.000000 libwiipy-0.2.2/src/libWiiPy.egg-info/top_level.txt
+drwxr-xr-x   0 campbell  (1000) campbell  (1000)        0 2024-05-14 14:29:43.650597 libwiipy-0.2.3/
+-rw-r--r--   0 campbell  (1000) campbell  (1000)     1056 2024-04-09 02:52:36.000000 libwiipy-0.2.3/LICENSE
+-rw-r--r--   0 campbell  (1000) campbell  (1000)     4595 2024-05-14 14:29:43.650597 libwiipy-0.2.3/PKG-INFO
+-rw-r--r--   0 campbell  (1000) campbell  (1000)     3937 2024-05-08 12:41:32.000000 libwiipy-0.2.3/README.md
+-rw-r--r--   0 campbell  (1000) campbell  (1000)      753 2024-05-03 18:28:56.000000 libwiipy-0.2.3/pyproject.toml
+-rw-r--r--   0 campbell  (1000) campbell  (1000)       38 2024-05-14 14:29:43.650597 libwiipy-0.2.3/setup.cfg
+drwxr-xr-x   0 campbell  (1000) campbell  (1000)        0 2024-05-14 14:29:43.647264 libwiipy-0.2.3/src/
+drwxr-xr-x   0 campbell  (1000) campbell  (1000)        0 2024-05-14 14:29:43.650597 libwiipy-0.2.3/src/libWiiPy/
+-rw-r--r--   0 campbell  (1000) campbell  (1000)      372 2024-05-03 18:58:04.000000 libwiipy-0.2.3/src/libWiiPy/__init__.py
+-rw-r--r--   0 campbell  (1000) campbell  (1000)     1086 2024-04-09 02:52:36.000000 libwiipy-0.2.3/src/libWiiPy/commonkeys.py
+-rw-r--r--   0 campbell  (1000) campbell  (1000)    16251 2024-05-06 23:31:05.000000 libwiipy-0.2.3/src/libWiiPy/content.py
+-rw-r--r--   0 campbell  (1000) campbell  (1000)     5691 2024-05-06 23:24:32.000000 libwiipy-0.2.3/src/libWiiPy/crypto.py
+-rw-r--r--   0 campbell  (1000) campbell  (1000)     9365 2024-05-06 23:21:29.000000 libwiipy-0.2.3/src/libWiiPy/nus.py
+-rw-r--r--   0 campbell  (1000) campbell  (1000)     2030 2024-05-06 23:31:05.000000 libwiipy-0.2.3/src/libWiiPy/shared.py
+-rw-r--r--   0 campbell  (1000) campbell  (1000)    11237 2024-05-06 23:21:29.000000 libwiipy-0.2.3/src/libWiiPy/ticket.py
+-rw-r--r--   0 campbell  (1000) campbell  (1000)     9216 2024-05-01 03:07:22.000000 libwiipy-0.2.3/src/libWiiPy/title.py
+-rw-r--r--   0 campbell  (1000) campbell  (1000)    13750 2024-05-09 15:17:24.000000 libwiipy-0.2.3/src/libWiiPy/tmd.py
+-rw-r--r--   0 campbell  (1000) campbell  (1000)     1938 2024-04-09 02:52:36.000000 libwiipy-0.2.3/src/libWiiPy/types.py
+-rw-r--r--   0 campbell  (1000) campbell  (1000)    11975 2024-05-06 23:34:18.000000 libwiipy-0.2.3/src/libWiiPy/wad.py
+drwxr-xr-x   0 campbell  (1000) campbell  (1000)        0 2024-05-14 14:29:43.650597 libwiipy-0.2.3/src/libWiiPy.egg-info/
+-rw-r--r--   0 campbell  (1000) campbell  (1000)     4595 2024-05-14 14:29:43.000000 libwiipy-0.2.3/src/libWiiPy.egg-info/PKG-INFO
+-rw-r--r--   0 campbell  (1000) campbell  (1000)      460 2024-05-14 14:29:43.000000 libwiipy-0.2.3/src/libWiiPy.egg-info/SOURCES.txt
+-rw-r--r--   0 campbell  (1000) campbell  (1000)        1 2024-05-14 14:29:43.000000 libwiipy-0.2.3/src/libWiiPy.egg-info/dependency_links.txt
+-rw-r--r--   0 campbell  (1000) campbell  (1000)       22 2024-05-14 14:29:43.000000 libwiipy-0.2.3/src/libWiiPy.egg-info/requires.txt
+-rw-r--r--   0 campbell  (1000) campbell  (1000)        9 2024-05-14 14:29:43.000000 libwiipy-0.2.3/src/libWiiPy.egg-info/top_level.txt
```

### Comparing `libwiipy-0.2.2/LICENSE` & `libwiipy-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `libwiipy-0.2.2/PKG-INFO` & `libwiipy-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libWiiPy
-Version: 0.2.2
+Version: 0.2.3
 Summary: A modern Python library for handling files used by the Wii
 Author-email: NinjaCheetah <ninjacheetah@ncxprogramming.com>, Lillian Skinner <lillian@randommeaninglesscharacters.com>
 Project-URL: Homepage, https://github.com/NinjaCheetah/libWiiPy
 Project-URL: Issues, https://github.com/NinjaCheetah/libWiipy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -22,15 +22,15 @@
 
 **Note:** While libWiiPy is directly inspired by libWiiSharp and aims to have feature parity with it, no code from either libWiiSharp or Wii.py was used in the making of this library. All code is original and is written by [@NinjaCheetah](https://github.com/NinjaCheetah), [@rvtr](https://github.com/rvtr), and any other GitHub contributors.
 
 # Features
 This list will expand as libWiiPy is developed, but these features are currently available:
 - TMD, ticket, and WAD parsing
 - WAD content extraction, decryption, re-encryption, and packing
-- Downloading free titles from the NUS
+- Downloading titles from the NUS
 
 # Usage
 A wiki, and in the future a potential documenation site, is being worked on, and can be accessed [here](https://github.com/NinjaCheetah/libWiiPy/wiki). It is currently fairly barebones, but it will be improved in the future.
 
 The easiest way to get libWiiPy for your project is to install the latest version of the library from PyPI, as shown below. 
 ```sh
 pip install -U libWiiPy
@@ -43,35 +43,35 @@
 ```
 Please be aware that because libWiiPy is in a very early state right now, many features may be subject to change, and methods and properties available now have the potential to disappear in the future.
 
 # Building
 To build this package locally, the steps are quite simple, and should apply to all platforms. Make sure you've set up your `venv` first!
 
 First, install the dependencies from `requirements.txt`:
-```py
+```sh
 pip install -r requirements.txt
 ```
 
 Then, build the package using the Python `build` module:
-```py
+```sh
 python -m build
 ```
 
 And that's all! You'll find your compiled pip package in `dist/`.
 
 # Special Thanks
-This project wouldn't be possible without the amazing people behind its predecessors and all of the people who have contributed to the documentation of the Wii's inner workings over at [Wiibrew](https://wiibrew.org).
+This project wouldn't be possible without the amazing people behind its predecessors and all of the people who have contributed to the documentation of the Wii's inner workings over at [WiiBrew](https://wiibrew.org).
 
 ## Special Thanks for the Inspiration and Previous Projects
 - Xuzz, SquidMan, megazig, Matt_P, Omega and The Lemon Man for creating Wii.py
 - Leathl for creating libWiiSharp
 - TheShadowEevee for maintaining libWiiSharp
 
-## Special Thanks to Wiibrew Contributors
-Thank you to all of the contributors to the documentation on the Wiibrew pages that make this all understandable! Some of the key articles referenced are as follows:
+## Special Thanks to WiiBrew Contributors
+Thank you to all of the contributors to the documentation on the WiiBrew pages that make this all understandable! Some of the key articles referenced are as follows:
 - [Title metadata](https://wiibrew.org/wiki/Title_metadata), for the documentation on how a TMD is structured
 - [WAD files](https://wiibrew.org/wiki/WAD_files), for the documentation on how a WAD is structured
 - [IOS history](https://wiibrew.org/wiki/IOS_history), for the documentation on IOS TIDs and how IOS is versioned
 
 ### One additional special thanks to [@DamiDoop](https://github.com/DamiDoop)!
 She made the very cool banner you can see at the top of this README, and has also helped greatly with my sanity throughout debugging this library.
```

### Comparing `libwiipy-0.2.2/README.md` & `libwiipy-0.2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 **Note:** While libWiiPy is directly inspired by libWiiSharp and aims to have feature parity with it, no code from either libWiiSharp or Wii.py was used in the making of this library. All code is original and is written by [@NinjaCheetah](https://github.com/NinjaCheetah), [@rvtr](https://github.com/rvtr), and any other GitHub contributors.
 
 # Features
 This list will expand as libWiiPy is developed, but these features are currently available:
 - TMD, ticket, and WAD parsing
 - WAD content extraction, decryption, re-encryption, and packing
-- Downloading free titles from the NUS
+- Downloading titles from the NUS
 
 # Usage
 A wiki, and in the future a potential documenation site, is being worked on, and can be accessed [here](https://github.com/NinjaCheetah/libWiiPy/wiki). It is currently fairly barebones, but it will be improved in the future.
 
 The easiest way to get libWiiPy for your project is to install the latest version of the library from PyPI, as shown below. 
 ```sh
 pip install -U libWiiPy
@@ -27,35 +27,35 @@
 ```
 Please be aware that because libWiiPy is in a very early state right now, many features may be subject to change, and methods and properties available now have the potential to disappear in the future.
 
 # Building
 To build this package locally, the steps are quite simple, and should apply to all platforms. Make sure you've set up your `venv` first!
 
 First, install the dependencies from `requirements.txt`:
-```py
+```sh
 pip install -r requirements.txt
 ```
 
 Then, build the package using the Python `build` module:
-```py
+```sh
 python -m build
 ```
 
 And that's all! You'll find your compiled pip package in `dist/`.
 
 # Special Thanks
-This project wouldn't be possible without the amazing people behind its predecessors and all of the people who have contributed to the documentation of the Wii's inner workings over at [Wiibrew](https://wiibrew.org).
+This project wouldn't be possible without the amazing people behind its predecessors and all of the people who have contributed to the documentation of the Wii's inner workings over at [WiiBrew](https://wiibrew.org).
 
 ## Special Thanks for the Inspiration and Previous Projects
 - Xuzz, SquidMan, megazig, Matt_P, Omega and The Lemon Man for creating Wii.py
 - Leathl for creating libWiiSharp
 - TheShadowEevee for maintaining libWiiSharp
 
-## Special Thanks to Wiibrew Contributors
-Thank you to all of the contributors to the documentation on the Wiibrew pages that make this all understandable! Some of the key articles referenced are as follows:
+## Special Thanks to WiiBrew Contributors
+Thank you to all of the contributors to the documentation on the WiiBrew pages that make this all understandable! Some of the key articles referenced are as follows:
 - [Title metadata](https://wiibrew.org/wiki/Title_metadata), for the documentation on how a TMD is structured
 - [WAD files](https://wiibrew.org/wiki/WAD_files), for the documentation on how a WAD is structured
 - [IOS history](https://wiibrew.org/wiki/IOS_history), for the documentation on IOS TIDs and how IOS is versioned
 
 ### One additional special thanks to [@DamiDoop](https://github.com/DamiDoop)!
 She made the very cool banner you can see at the top of this README, and has also helped greatly with my sanity throughout debugging this library.
```

### Comparing `libwiipy-0.2.2/pyproject.toml` & `libwiipy-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "libWiiPy"
-version = "0.2.2"
+version = "0.2.3"
 authors = [
     { name="NinjaCheetah", email="ninjacheetah@ncxprogramming.com" },
     { name="Lillian Skinner", email="lillian@randommeaninglesscharacters.com" }
 ]
 description = "A modern Python library for handling files used by the Wii"
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `libwiipy-0.2.2/src/libWiiPy/commonkeys.py` & `libwiipy-0.2.3/src/libWiiPy/commonkeys.py`

 * *Files identical despite different names*

### Comparing `libwiipy-0.2.2/src/libWiiPy/content.py` & `libwiipy-0.2.3/src/libWiiPy/content.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,29 +75,26 @@
         content list matches the raw data.
 
         Returns
         -------
         bytes
             The full WAD file as bytes.
         """
-        # Open the stream and begin writing data to it.
-        with io.BytesIO() as content_region_data:
-            for content in self.content_list:
-                # Calculate padding after this content before the next one.
-                padding_bytes = 0
-                if (len(content) % 64) != 0:
-                    padding_bytes = 64 - (len(content) % 64)
-                # Write content data, then the padding afterward if necessary.
-                content_region_data.write(content)
-                if padding_bytes > 0:
-                    content_region_data.write(b'\x00' * padding_bytes)
-            content_region_data.seek(0x0)
-            content_region_raw = content_region_data.read()
+        content_region_data = b''
+        for content in self.content_list:
+            # Calculate padding after this content before the next one.
+            padding_bytes = 0
+            if (len(content) % 64) != 0:
+                padding_bytes = 64 - (len(content) % 64)
+            # Write content data, then the padding afterward if necessary.
+            content_region_data += content
+            if padding_bytes > 0:
+                content_region_data += b'\x00' * padding_bytes
         # Return the raw ContentRegion for the data contained in the object.
-        return content_region_raw
+        return content_region_data
 
     def get_enc_content_by_index(self, index: int) -> bytes:
         """
         Gets an individual content from the content region based on the provided index, in encrypted form.
 
         Parameters
         ----------
```

### Comparing `libwiipy-0.2.2/src/libWiiPy/nus.py` & `libwiipy-0.2.3/src/libWiiPy/nus.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,72 +1,80 @@
 # "nus.py" from libWiiPy by NinjaCheetah & Contributors
 # https://github.com/NinjaCheetah/libWiiPy
 #
 # See https://wiibrew.org/wiki/NUS for details about the NUS
 
-import io
 import requests
 import hashlib
 from typing import List
 from .title import Title
 from .tmd import TMD
 from .ticket import Ticket
 
+nus_endpoint = ["http://nus.cdn.shop.wii.com/ccs/download/", "http://ccs.cdn.wup.shop.nintendo.net/ccs/download/"]
 
-def download_title(title_id: str, title_version: int = None) -> Title:
+
+def download_title(title_id: str, title_version: int = None, wiiu_endpoint: bool = False) -> Title:
     """
     Download an entire title and all of its contents, then load the downloaded components into a Title object for
     further use. This method is NOT recommended for general use, as it has absolutely no verbosity. It is instead
     recommended to call the individual download methods instead to provide more flexibility and output.
 
     Parameters
     ----------
     title_id : str
         The Title ID of the title to download.
     title_version : int, option
         The version of the title to download. Defaults to latest if not set.
+    wiiu_endpoint : bool, option
+        Whether the Wii U endpoint for the NUS should be used or not. This increases download speeds. Defaults to False.
 
     Returns
     -------
     Title
         A Title object containing all the data from the downloaded title.
     """
     # First, create the new title.
     title = Title()
     # Download and load the TMD, Ticket, and certs.
-    title.load_tmd(download_tmd(title_id, title_version))
-    title.load_ticket(download_ticket(title_id))
-    title.wad.set_cert_data(download_cert())
+    title.load_tmd(download_tmd(title_id, title_version, wiiu_endpoint))
+    title.load_ticket(download_ticket(title_id, wiiu_endpoint))
+    title.wad.set_cert_data(download_cert(wiiu_endpoint))
     # Download all contents
     title.load_content_records()
-    title.content.content_list = download_contents(title_id, title.tmd)
+    title.content.content_list = download_contents(title_id, title.tmd, wiiu_endpoint)
     # Return the completed title.
     return title
 
 
-def download_tmd(title_id: str, title_version: int = None) -> bytes:
+def download_tmd(title_id: str, title_version: int = None, wiiu_endpoint: bool = False) -> bytes:
     """
     Downloads the TMD of the Title specified in the object. Will download the latest version by default, or another
     version if it was manually specified in the object.
 
     Parameters
     ----------
     title_id : str
         The Title ID of the title to download the TMD for.
     title_version : int, option
         The version of the TMD to download. Defaults to latest if not set.
+    wiiu_endpoint : bool, option
+        Whether the Wii U endpoint for the NUS should be used or not. This increases download speeds. Defaults to False.
 
     Returns
     -------
     bytes
         The TMD file from the NUS.
     """
     # Build the download URL. The structure is download/<TID>/tmd for latest and download/<TID>/tmd.<version> for
     # when a specific version is requested.
-    tmd_url = "http://nus.cdn.shop.wii.com/ccs/download/" + title_id + "/tmd"
+    if wiiu_endpoint is False:
+        tmd_url = nus_endpoint[0] + title_id + "/tmd"
+    else:
+        tmd_url = nus_endpoint[1] + title_id + "/tmd"
     # Add the version to the URL if one was specified.
     if title_version is not None:
         tmd_url += "." + str(title_version)
     # Make the request.
     tmd_request = requests.get(url=tmd_url, headers={'User-Agent': 'wii libnup/1.0'}, stream=True)
     # Handle a 404 if the TID/version doesn't exist.
     if tmd_request.status_code != 200:
@@ -77,118 +85,137 @@
     # Use a TMD object to load the data and then return only the actual TMD.
     tmd_temp = TMD()
     tmd_temp.load(raw_tmd)
     tmd = tmd_temp.dump()
     return tmd
 
 
-def download_ticket(title_id: str) -> bytes:
+def download_ticket(title_id: str, wiiu_endpoint: bool = False) -> bytes:
     """
     Downloads the Ticket of the Title specified in the object. This will only work if the Title ID specified is for
     a free title.
 
     Parameters
     ----------
     title_id : str
         The Title ID of the title to download the Ticket for.
+    wiiu_endpoint : bool, option
+        Whether the Wii U endpoint for the NUS should be used or not. This increases download speeds. Defaults to False.
 
     Returns
     -------
     bytes
         The Ticket file from the NUS.
     """
     # Build the download URL. The structure is download/<TID>/cetk, and cetk will only exist if this is a free
     # title.
-    ticket_url = "http://nus.cdn.shop.wii.com/ccs/download/" + title_id + "/cetk"
+    if wiiu_endpoint is False:
+        ticket_url = nus_endpoint[0] + title_id + "/cetk"
+    else:
+        ticket_url = nus_endpoint[1] + title_id + "/cetk"
     # Make the request.
     ticket_request = requests.get(url=ticket_url, headers={'User-Agent': 'wii libnup/1.0'}, stream=True)
     if ticket_request.status_code != 200:
         raise ValueError("The requested Title ID does not exist, or refers to a non-free title. Tickets can only"
                          " be downloaded for titles that are free on the NUS.")
     # Save the raw cetk file.
     cetk = ticket_request.content
     # Use a Ticket object to load only the Ticket data from cetk and return it.
     ticket_temp = Ticket()
     ticket_temp.load(cetk)
     ticket = ticket_temp.dump()
     return ticket
 
 
-def download_cert() -> bytes:
+def download_cert(wiiu_endpoint: bool = False) -> bytes:
     """
     Downloads the signing certificate used by all WADs. This uses System Menu 4.3U as the source.
 
+    Parameters
+    ----------
+    wiiu_endpoint : bool, option
+        Whether the Wii U endpoint for the NUS should be used or not. This increases download speeds. Defaults to False.
+
     Returns
     -------
     bytes
         The cert file.
     """
     # Download the TMD and cetk for the System Menu 4.3U.
-    tmd = requests.get(url='http://nus.cdn.shop.wii.com/ccs/download/0000000100000002/tmd.513',
-                       headers={'User-Agent': 'wii libnup/1.0'}, stream=True).content
-    cetk = requests.get(url='http://nus.cdn.shop.wii.com/ccs/download/0000000100000002/cetk',
-                        headers={'User-Agent': 'wii libnup/1.0'}, stream=True).content
+    if wiiu_endpoint is False:
+        tmd_url = nus_endpoint[0] + "0000000100000002/tmd.513"
+        cetk_url = nus_endpoint[0] + "0000000100000002/cetk"
+    else:
+        tmd_url = nus_endpoint[1] + "0000000100000002/tmd.513"
+        cetk_url = nus_endpoint[1] + "0000000100000002/cetk"
+    tmd = requests.get(url=tmd_url, headers={'User-Agent': 'wii libnup/1.0'}, stream=True).content
+    cetk = requests.get(url=cetk_url, headers={'User-Agent': 'wii libnup/1.0'}, stream=True).content
     # Assemble the certificate.
-    with io.BytesIO() as cert_data:
-        # Certificate Authority data.
-        cert_data.write(cetk[0x2A4 + 768:])
-        # Certificate Policy data.
-        cert_data.write(tmd[0x328:0x328 + 768])
-        # XS data.
-        cert_data.write(cetk[0x2A4:0x2A4 + 768])
-        cert_data.seek(0x0)
-        cert = cert_data.read()
+    cert = b''
+    # Certificate Authority data.
+    cert += cetk[0x2A4 + 768:]
+    # Certificate Policy data.
+    cert += tmd[0x328:0x328 + 768]
+    # XS data.
+    cert += cetk[0x2A4:0x2A4 + 768]
     # Since the cert is always the same, check the hash to make sure nothing went wildly wrong.
     if hashlib.sha1(cert).hexdigest() != "ace0f15d2a851c383fe4657afc3840d6ffe30ad0":
         raise Exception("An unknown error has occurred downloading and creating the certificate.")
     return cert
 
 
-def download_content(title_id: str, content_id: int) -> bytes:
+def download_content(title_id: str, content_id: int, wiiu_endpoint: bool = False) -> bytes:
     """
     Downloads a specified content for the title specified in the object.
 
     Parameters
     ----------
     title_id : str
         The Title ID of the title to download content from.
     content_id : int
         The Content ID of the content you wish to download.
+    wiiu_endpoint : bool, option
+        Whether the Wii U endpoint for the NUS should be used or not. This increases download speeds. Defaults to False.
 
     Returns
     -------
     bytes
         The downloaded content.
     """
     # Build the download URL. The structure is download/<TID>/<Content ID>.
     content_id_hex = hex(content_id)[2:]
     if len(content_id_hex) < 2:
         content_id_hex = "0" + content_id_hex
-    content_url = "http://nus.cdn.shop.wii.com/ccs/download/" + title_id + "/000000" + content_id_hex
+    if wiiu_endpoint is False:
+        content_url = nus_endpoint[0] + title_id + "/000000" + content_id_hex
+    else:
+        content_url = nus_endpoint[1] + title_id + "/000000" + content_id_hex
     # Make the request.
     content_request = requests.get(url=content_url, headers={'User-Agent': 'wii libnup/1.0'}, stream=True)
     if content_request.status_code != 200:
         raise ValueError("The requested Title ID does not exist, or an invalid Content ID is present in the"
                          " content records provided.\n Failed while downloading Content ID: 000000" +
                          content_id_hex)
     content_data = content_request.content
     return content_data
 
 
-def download_contents(title_id: str, tmd: TMD) -> List[bytes]:
+def download_contents(title_id: str, tmd: TMD, wiiu_endpoint: bool = False) -> List[bytes]:
     """
     Downloads all the contents for the title specified in the object. This requires a TMD to already be available
     so that the content records can be accessed.
 
     Parameters
     ----------
     title_id : str
         The Title ID of the title to download content from.
     tmd : TMD
         The TMD that matches the title that the contents being downloaded are from.
+    wiiu_endpoint : bool, option
+        Whether the Wii U endpoint for the NUS should be used or not. This increases download speeds. Defaults to False.
 
     Returns
     -------
     List[bytes]
         A list of all the downloaded contents.
     """
     # Retrieve the content records from the TMD.
@@ -197,10 +224,10 @@
     content_ids = []
     for content_record in content_records:
         content_ids.append(content_record.content_id)
     # Iterate over that list and download each content in it, then add it to the array of contents.
     content_list = []
     for content_id in content_ids:
         # Call self.download_content() for each Content ID.
-        content = download_content(title_id, content_id)
+        content = download_content(title_id, content_id, wiiu_endpoint)
         content_list.append(content)
     return content_list
```

### Comparing `libwiipy-0.2.2/src/libWiiPy/ticket.py` & `libwiipy-0.2.3/src/libWiiPy/ticket.py`

 * *Files 18% similar despite different names*

```diff
@@ -95,18 +95,17 @@
             ticket_data.seek(0x1D0)
             self.ticket_id = ticket_data.read(8)
             # Console ID.
             ticket_data.seek(0x1D8)
             self.console_id = int.from_bytes(ticket_data.read(4))
             # Title ID.
             ticket_data.seek(0x1DC)
-            self.title_id = ticket_data.read(8)
+            self.title_id = binascii.hexlify(ticket_data.read(8))
             # Title ID (as a string).
-            title_id_hex = binascii.hexlify(self.title_id)
-            self.title_id_str = str(title_id_hex.decode())
+            self.title_id_str = str(self.title_id.decode())
             # Unknown data 1.
             ticket_data.seek(0x1E4)
             self.unknown1 = ticket_data.read(2)
             # Title version.
             ticket_data.seek(0x1E6)
             title_version_high = int.from_bytes(ticket_data.read(1)) * 256
             ticket_data.seek(0x1E7)
@@ -143,76 +142,70 @@
         dumped data, and triggers load() again to ensure that the raw data and object match.
 
         Returns
         -------
         bytes
             The full Ticket file as bytes.
         """
-        # Open the stream and begin writing to it.
-        with io.BytesIO() as ticket_data:
-            # Signature type.
-            ticket_data.write(self.signature_type)
-            # Signature data.
-            ticket_data.write(self.signature)
-            # Padding to 64 bytes.
-            ticket_data.write(b'\x00' * 60)
-            # Signature issuer.
-            ticket_data.write(str.encode(self.signature_issuer))
-            # ECDH data.
-            ticket_data.write(self.ecdh_data)
-            # Ticket version.
-            ticket_data.write(int.to_bytes(self.ticket_version, 1))
-            # Reserved (all \0x00).
-            ticket_data.write(b'\x00\x00')
-            # Title Key.
-            ticket_data.write(self.title_key_enc)
-            # Unknown (write \0x00).
-            ticket_data.write(b'\x00')
-            # Ticket ID.
-            ticket_data.write(self.ticket_id)
-            # Console ID.
-            ticket_data.write(int.to_bytes(self.console_id, 4))
-            # Title ID.
-            ticket_data.write(self.title_id)
-            # Unknown data 1.
-            ticket_data.write(self.unknown1)
-            # Title version.
-            title_version_high = round(self.title_version / 256)
-            ticket_data.write(int.to_bytes(title_version_high, 1))
-            title_version_low = self.title_version % 256
-            ticket_data.write(int.to_bytes(title_version_low, 1))
-            # Permitted titles mask.
-            ticket_data.write(self.permitted_titles)
-            # Permit mask.
-            ticket_data.write(self.permit_mask)
-            # Title Export allowed.
-            ticket_data.write(int.to_bytes(self.title_export_allowed, 1))
-            # Common Key index.
-            ticket_data.write(int.to_bytes(self.common_key_index, 1))
-            # Unknown data 2.
-            ticket_data.write(self.unknown2)
-            # Content access permissions.
-            ticket_data.write(self.content_access_permissions)
-            # Padding (always \x00).
-            ticket_data.write(b'\x00\x00')
-            # Iterate over Title Limit objects, write them back into raw data, then add them to the Ticket.
-            for title_limit in range(len(self.title_limits_list)):
-                title_limit_data = io.BytesIO()
-                # Write all fields from the title limit entry.
-                title_limit_data.write(int.to_bytes(self.title_limits_list[title_limit].limit_type, 4))
-                title_limit_data.write(int.to_bytes(self.title_limits_list[title_limit].maximum_usage, 4))
-                # Seek to the start and write the entry to the Ticket.
-                title_limit_data.seek(0x0)
-                ticket_data.write(title_limit_data.read())
-                title_limit_data.close()
-            # Set the Ticket attribute of the object to the new raw Ticket.
-            ticket_data.seek(0x0)
-            ticket_data_raw = ticket_data.read()
+        ticket_data = b''
+        # Signature type.
+        ticket_data += self.signature_type
+        # Signature data.
+        ticket_data += self.signature
+        # Padding to 64 bytes.
+        ticket_data += b'\x00' * 60
+        # Signature issuer.
+        ticket_data += str.encode(self.signature_issuer)
+        # ECDH data.
+        ticket_data += self.ecdh_data
+        # Ticket version.
+        ticket_data += int.to_bytes(self.ticket_version, 1)
+        # Reserved (all \0x00).
+        ticket_data += b'\x00\x00'
+        # Title Key.
+        ticket_data += self.title_key_enc
+        # Unknown (write \0x00).
+        ticket_data += b'\x00'
+        # Ticket ID.
+        ticket_data += self.ticket_id
+        # Console ID.
+        ticket_data += int.to_bytes(self.console_id, 4)
+        # Title ID.
+        ticket_data += binascii.unhexlify(self.title_id)
+        # Unknown data 1.
+        ticket_data += self.unknown1
+        # Title version.
+        title_version_high = round(self.title_version / 256)
+        ticket_data += int.to_bytes(title_version_high, 1)
+        title_version_low = self.title_version % 256
+        ticket_data += int.to_bytes(title_version_low, 1)
+        # Permitted titles mask.
+        ticket_data += self.permitted_titles
+        # Permit mask.
+        ticket_data += self.permit_mask
+        # Title Export allowed.
+        ticket_data += int.to_bytes(self.title_export_allowed, 1)
+        # Common Key index.
+        ticket_data += int.to_bytes(self.common_key_index, 1)
+        # Unknown data 2.
+        ticket_data += self.unknown2
+        # Content access permissions.
+        ticket_data += self.content_access_permissions
+        # Padding (always \x00).
+        ticket_data += b'\x00\x00'
+        # Iterate over Title Limit objects, write them back into raw data, then add them to the Ticket.
+        for title_limit in range(len(self.title_limits_list)):
+            title_limit_data = b''
+            # Write all fields from the title limit entry.
+            title_limit_data += int.to_bytes(self.title_limits_list[title_limit].limit_type, 4)
+            title_limit_data += int.to_bytes(self.title_limits_list[title_limit].maximum_usage, 4)
+            # Write the entry to the ticket.
+            ticket_data += title_limit_data
         # Return the raw TMD for the data contained in the object.
-        return ticket_data_raw
+        return ticket_data
 
     def get_title_id(self) -> str:
         """
         Gets the Title ID of the ticket's associated title.
 
         Returns
         -------
```

### Comparing `libwiipy-0.2.2/src/libWiiPy/title.py` & `libwiipy-0.2.3/src/libWiiPy/title.py`

 * *Files identical despite different names*

### Comparing `libwiipy-0.2.2/src/libWiiPy/tmd.py` & `libwiipy-0.2.3/src/libWiiPy/tmd.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,34 +31,36 @@
     """
     def __init__(self):
         self.blob_header: bytes = b''
         self.sig_type: int = 0
         self.sig: bytes = b''
         self.issuer: bytes = b''  # Follows the format "Root-CA%08x-CP%08x"
         self.tmd_version: int = 0  # This seems to always be 0 no matter what?
-        self.ca_crl_version: int = 0
-        self.signer_crl_version: int = 0
+        self.ca_crl_version: int = 0  # Certificate Authority Certificate Revocation List version
+        self.signer_crl_version: int = 0  # Certificate Policy Certificate Revocation List version
         self.vwii: int = 0  # Whether the title is for the vWii. 0 = No, 1 = Yes
         self.ios_tid: str = ""  # The Title ID of the IOS version the associated title runs on.
         self.ios_version: int = 0  # The IOS version the associated title runs on.
         self.title_id: str = ""  # The Title ID of the associated title.
         self.content_type: str = ""  # The type of content contained within the associated title.
         self.group_id: int = 0  # The ID of the publisher of the associated title.
         self.region: int = 0  # The ID of the region of the associated title.
-        self.ratings: bytes = b''
+        self.ratings: bytes = b''  # The parental controls rating of the associated title.
+        self.reserved1: bytes = b''  # Unknown data labeled "Reserved" on WiiBrew.
         self.ipc_mask: bytes = b''
+        self.reserved2: bytes = b''  # Other "Reserved" data from WiiBrew.
         self.access_rights: bytes = b''
         self.title_version: int = 0  # The version of the associated title.
         self.num_contents: int = 0  # The number of contents contained in the associated title.
-        self.boot_index: int = 0
+        self.boot_index: int = 0  # The content index that contains the bootable executable.
         self.content_records: List[ContentRecord] = []
 
     def load(self, tmd: bytes) -> None:
         """
-        Loads raw TMD data and sets all attributes of the WAD object. This allows for manipulating an already
+        Loads raw TMD data and sets all attributes of the TMD object. This allows for manipulating an already
         existing TMD.
 
         Parameters
         ----------
         tmd : bytes
             The data for the TMD you wish to load.
         """
@@ -70,18 +72,18 @@
             self.blob_header = tmd_data.read(320)
             # Signing certificate issuer.
             tmd_data.seek(0x140)
             self.issuer = tmd_data.read(64)
             # TMD version, seems to usually be 0, but I've seen references to other numbers.
             tmd_data.seek(0x180)
             self.tmd_version = int.from_bytes(tmd_data.read(1))
-            # Root certificate crl version.
+            # Certificate Authority CRL version.
             tmd_data.seek(0x181)
             self.ca_crl_version = int.from_bytes(tmd_data.read(1))
-            # Signer crl version.
+            # Certificate Policy CRL version.
             tmd_data.seek(0x182)
             self.signer_crl_version = int.from_bytes(tmd_data.read(1))
             # If this is a vWii title or not.
             tmd_data.seek(0x183)
             self.vwii = int.from_bytes(tmd_data.read(1))
             # TID of the IOS to use for the title, set to 0 if this title is the IOS, set to boot2 version if boot2.
             tmd_data.seek(0x184)
@@ -99,37 +101,43 @@
             tmd_data.seek(0x194)
             content_type_bin = tmd_data.read(4)
             content_type_hex = binascii.hexlify(content_type_bin)
             self.content_type = str(content_type_hex.decode())
             # Publisher of the title.
             tmd_data.seek(0x198)
             self.group_id = int.from_bytes(tmd_data.read(2))
-            # Region of the title, 0 = JAP, 1 = USA, 2 = EUR, 3 = NONE, 4 = KOR.
+            # Region of the title, 0 = JAP, 1 = USA, 2 = EUR, 3 = WORLD, 4 = KOR.
             tmd_data.seek(0x19C)
             region_hex = tmd_data.read(2)
             self.region = int.from_bytes(region_hex)
-            # Likely the localized content rating for the title. (ESRB, CERO, PEGI, etc.)
+            # Content rating of the title for parental controls. Likely based on ESRB, CERO, PEGI, etc. rating.
             tmd_data.seek(0x19E)
             self.ratings = tmd_data.read(16)
+            # "Reserved" data 1.
+            tmd_data.seek(0x1AE)
+            self.reserved1 = tmd_data.read(12)
             # IPC mask.
             tmd_data.seek(0x1BA)
             self.ipc_mask = tmd_data.read(12)
+            # "Reserved" data 2.
+            tmd_data.seek(0x1C6)
+            self.reserved2 = tmd_data.read(18)
             # Access rights of the title; DVD-video access and AHBPROT.
             tmd_data.seek(0x1D8)
             self.access_rights = tmd_data.read(4)
             # Calculate the version number by multiplying 0x1DC by 256 and adding 0x1DD.
             tmd_data.seek(0x1DC)
             title_version_high = int.from_bytes(tmd_data.read(1)) * 256
             tmd_data.seek(0x1DD)
             title_version_low = int.from_bytes(tmd_data.read(1))
             self.title_version = title_version_high + title_version_low
             # The number of contents listed in the TMD.
             tmd_data.seek(0x1DE)
             self.num_contents = int.from_bytes(tmd_data.read(2))
-            # Content index in content list that contains the boot file.
+            # The content index that contains the bootable executable.
             tmd_data.seek(0x1E0)
             self.boot_index = int.from_bytes(tmd_data.read(2))
             # Get content records for the number of contents in num_contents.
             self.content_records = []
             for content in range(0, self.num_contents):
                 tmd_data.seek(0x1E4 + (36 * content))
                 content_record_hdr = struct.unpack(">LHH4x4s20s", tmd_data.read(36))
@@ -144,101 +152,95 @@
         and triggers load() again to ensure that the raw data and object match.
 
         Returns
         -------
         bytes
             The full TMD file as bytes.
         """
-        # Open the stream and begin writing to it.
-        with io.BytesIO() as tmd_data:
-            # Signed blob header.
-            tmd_data.write(self.blob_header)
-            # Signing certificate issuer.
-            tmd_data.write(self.issuer)
-            # TMD version.
-            tmd_data.write(int.to_bytes(self.tmd_version, 1))
-            # Root certificate crl version.
-            tmd_data.write(int.to_bytes(self.ca_crl_version, 1))
-            # Signer crl version.
-            tmd_data.write(int.to_bytes(self.signer_crl_version, 1))
-            # If this is a vWii title or not.
-            tmd_data.write(int.to_bytes(self.vwii, 1))
-            # IOS Title ID.
-            tmd_data.write(binascii.unhexlify(self.ios_tid))
-            # Title's Title ID.
-            tmd_data.write(binascii.unhexlify(self.title_id))
-            # Content type.
-            tmd_data.write(binascii.unhexlify(self.content_type))
-            # Group ID.
-            tmd_data.write(int.to_bytes(self.group_id, 2))
-            # 2 bytes of zero for reasons.
-            tmd_data.write(b'\x00\x00')
-            # Region.
-            tmd_data.write(int.to_bytes(self.region, 2))
-            # Ratings.
-            tmd_data.write(self.ratings)
-            # Reserved (all \x00).
-            tmd_data.write(b'\x00' * 12)
-            # IPC mask.
-            tmd_data.write(self.ipc_mask)
-            # Reserved (all \x00).
-            tmd_data.write(b'\x00' * 18)
-            # Access rights.
-            tmd_data.write(self.access_rights)
-            # Title version.
-            title_version_high = round(self.title_version / 256)
-            tmd_data.write(int.to_bytes(title_version_high, 1))
-            title_version_low = self.title_version % 256
-            tmd_data.write(int.to_bytes(title_version_low, 1))
-            # Number of contents.
-            tmd_data.write(int.to_bytes(self.num_contents, 2))
-            # Boot index.
-            tmd_data.write(int.to_bytes(self.boot_index, 2))
-            # Minor version. Unused so write \x00.
-            tmd_data.write(b'\x00\x00')
-            # Iterate over content records, write them back into raw data, then add them to the TMD.
-            for content_record in range(self.num_contents):
-                content_data = io.BytesIO()
-                # Write all fields from the content record.
-                content_data.write(int.to_bytes(self.content_records[content_record].content_id, 4))
-                content_data.write(int.to_bytes(self.content_records[content_record].index, 2))
-                content_data.write(int.to_bytes(self.content_records[content_record].content_type, 2))
-                content_data.write(int.to_bytes(self.content_records[content_record].content_size, 8))
-                content_data.write(binascii.unhexlify(self.content_records[content_record].content_hash))
-                # Seek to the start and write the record to the TMD.
-                content_data.seek(0x0)
-                tmd_data.write(content_data.read())
-                content_data.close()
-            # Set the TMD attribute of the object to the new raw TMD.
-            tmd_data.seek(0x0)
-            tmd_data_raw = tmd_data.read()
+        tmd_data = b''
+        # Signed blob header.
+        tmd_data += self.blob_header
+        # Signing certificate issuer.
+        tmd_data += self.issuer
+        # TMD version.
+        tmd_data += int.to_bytes(self.tmd_version, 1)
+        # Certificate Authority CRL version.
+        tmd_data += int.to_bytes(self.ca_crl_version, 1)
+        # Certificate Policy CRL version.
+        tmd_data += int.to_bytes(self.signer_crl_version, 1)
+        # If this is a vWii title or not.
+        tmd_data += int.to_bytes(self.vwii, 1)
+        # IOS Title ID.
+        tmd_data += binascii.unhexlify(self.ios_tid)
+        # Title's Title ID.
+        tmd_data += binascii.unhexlify(self.title_id)
+        # Content type.
+        tmd_data += binascii.unhexlify(self.content_type)
+        # Group ID.
+        tmd_data += int.to_bytes(self.group_id, 2)
+        # 2 bytes of zero for reasons.
+        tmd_data += b'\x00\x00'
+        # Region.
+        tmd_data += int.to_bytes(self.region, 2)
+        # Parental Controls Ratings.
+        tmd_data += self.ratings
+        # "Reserved" 1.
+        tmd_data += self.reserved1
+        # IPC mask.
+        tmd_data += self.ipc_mask
+        # "Reserved" 2.
+        tmd_data += self.reserved2
+        # Access rights.
+        tmd_data += self.access_rights
+        # Title version.
+        title_version_high = round(self.title_version / 256)
+        tmd_data += int.to_bytes(title_version_high, 1)
+        title_version_low = self.title_version % 256
+        tmd_data += int.to_bytes(title_version_low, 1)
+        # Number of contents.
+        tmd_data += int.to_bytes(self.num_contents, 2)
+        # Boot index.
+        tmd_data += int.to_bytes(self.boot_index, 2)
+        # Minor version. Unused so write \x00.
+        tmd_data += b'\x00\x00'
+        # Iterate over content records, write them back into raw data, then add them to the TMD.
+        for content_record in range(self.num_contents):
+            content_data = b''
+            # Write all fields from the content record.
+            content_data += int.to_bytes(self.content_records[content_record].content_id, 4)
+            content_data += int.to_bytes(self.content_records[content_record].index, 2)
+            content_data += int.to_bytes(self.content_records[content_record].content_type, 2)
+            content_data += int.to_bytes(self.content_records[content_record].content_size, 8)
+            content_data += binascii.unhexlify(self.content_records[content_record].content_hash)
+            # Write the record to the TMD.
+            tmd_data += content_data
         # Return the raw TMD for the data contained in the object.
-        return tmd_data_raw
+        return tmd_data
 
     def get_title_region(self) -> str:
         """
         Gets the region of the TMD's associated title.
 
         Can be one of several possible values:
-        'JAP', 'USA', 'EUR', 'NONE', or 'KOR'.
+        'JAP', 'USA', 'EUR', 'WORLD', or 'KOR'.
 
         Returns
         -------
         str
             The region of the title.
         """
         match self.region:
             case 0:
                 return "JAP"
             case 1:
                 return "USA"
             case 2:
                 return "EUR"
             case 3:
-                return "NONE"
+                return "WORLD"
             case 4:
                 return "KOR"
 
     def get_is_vwii_title(self) -> bool:
         """
         Gets whether the TMD is designed for the vWii or not.
```

### Comparing `libwiipy-0.2.2/src/libWiiPy/types.py` & `libwiipy-0.2.3/src/libWiiPy/types.py`

 * *Files identical despite different names*

### Comparing `libwiipy-0.2.2/src/libWiiPy/wad.py` & `libwiipy-0.2.3/src/libWiiPy/wad.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # "wad.py" from libWiiPy by NinjaCheetah & Contributors
 # https://github.com/NinjaCheetah/libWiiPy
 #
 # See https://wiibrew.org/wiki/WAD_files for details about the WAD format
 
 import io
 import binascii
-from .shared import align_value, pad_bytes_stream
+from .shared import align_value, pad_bytes
 
 
 class WAD:
     """
     A WAD object that allows for either loading and editing an existing WAD or creating a new WAD from raw data.
 
     Attributes
     ----------
     wad_type : str
-        The type of WAD, either ib for boot2 or Is for normal installable WADs. libWiiPy only supports Is currently.
+        The type of WAD, either ib for boot2 or Is for normal installable WADs.
     wad_cert_size : int
         The size of the WAD's certificate.
     wad_crl_size : int
         The size of the WAD's crl.
     wad_tik_size : int
         The size of the WAD's Ticket.
     wad_tmd_size : int
@@ -56,16 +56,16 @@
 
         Parameters
         ----------
         wad_data : bytes
             The data for the WAD you wish to load.
         """
         with io.BytesIO(wad_data) as wad_data:
-            # Read the first 8 bytes of the file to ensure that it's a WAD. This will currently reject boot2 WADs, but
-            # this tool cannot handle them correctly right now anyway.
+            # Read the first 8 bytes of the file to ensure that it's a WAD. Has two possible valid values for the two
+            # different types of WADs that might be encountered.
             wad_data.seek(0x0)
             wad_magic_bin = wad_data.read(8)
             wad_magic_hex = binascii.hexlify(wad_magic_bin)
             wad_magic = str(wad_magic_hex.decode())
             if wad_magic != "0000002049730000" and wad_magic != "0000002069620000":
                 raise TypeError("This does not appear to be a valid WAD file.")
             # ====================================================================================
@@ -136,58 +136,54 @@
         the WAD object.
 
         Returns
         -------
         bytes
             The full WAD file as bytes.
         """
-        # Open the stream and begin writing data to it.
-        with io.BytesIO() as wad_data:
-            # Lead-in data.
-            wad_data.write(b'\x00\x00\x00\x20')
-            # WAD type.
-            wad_data.write(str.encode(self.wad_type))
-            # WAD version.
-            wad_data.write(self.wad_version)
-            # WAD cert size.
-            wad_data.write(int.to_bytes(self.wad_cert_size, 4))
-            # WAD crl size.
-            wad_data.write(int.to_bytes(self.wad_crl_size, 4))
-            # WAD ticket size.
-            wad_data.write(int.to_bytes(self.wad_tik_size, 4))
-            # WAD TMD size.
-            wad_data.write(int.to_bytes(self.wad_tmd_size, 4))
-            # WAD content size.
-            wad_data.write(int.to_bytes(self.wad_content_size, 4))
-            # WAD meta size.
-            wad_data.write(int.to_bytes(self.wad_meta_size, 4))
-            wad_data = pad_bytes_stream(wad_data)
-            # Retrieve the cert data and write it out.
-            wad_data.write(self.get_cert_data())
-            wad_data = pad_bytes_stream(wad_data)
-            # Retrieve the crl data and write it out.
-            wad_data.write(self.get_crl_data())
-            wad_data = pad_bytes_stream(wad_data)
-            # Retrieve the ticket data and write it out.
-            wad_data.write(self.get_ticket_data())
-            wad_data = pad_bytes_stream(wad_data)
-            # Retrieve the TMD data and write it out.
-            wad_data.write(self.get_tmd_data())
-            wad_data = pad_bytes_stream(wad_data)
-            # Retrieve the meta/footer data and write it out.
-            wad_data.write(self.get_meta_data())
-            wad_data = pad_bytes_stream(wad_data)
-            # Retrieve the content data and write it out.
-            wad_data.write(self.get_content_data())
-            wad_data = pad_bytes_stream(wad_data)
-            # Seek to the beginning and save this as the WAD data for the object.
-            wad_data.seek(0x0)
-            wad_data_raw = wad_data.read()
+        wad_data = b''
+        # Lead-in data.
+        wad_data += b'\x00\x00\x00\x20'
+        # WAD type.
+        wad_data += str.encode(self.wad_type)
+        # WAD version.
+        wad_data += self.wad_version
+        # WAD cert size.
+        wad_data += int.to_bytes(self.wad_cert_size, 4)
+        # WAD crl size.
+        wad_data += int.to_bytes(self.wad_crl_size, 4)
+        # WAD ticket size.
+        wad_data += int.to_bytes(self.wad_tik_size, 4)
+        # WAD TMD size.
+        wad_data += int.to_bytes(self.wad_tmd_size, 4)
+        # WAD content size.
+        wad_data += int.to_bytes(self.wad_content_size, 4)
+        # WAD meta size.
+        wad_data += int.to_bytes(self.wad_meta_size, 4)
+        wad_data = pad_bytes(wad_data)
+        # Retrieve the cert data and write it out.
+        wad_data += self.get_cert_data()
+        wad_data = pad_bytes(wad_data)
+        # Retrieve the crl data and write it out.
+        wad_data += self.get_crl_data()
+        wad_data = pad_bytes(wad_data)
+        # Retrieve the ticket data and write it out.
+        wad_data += self.get_ticket_data()
+        wad_data = pad_bytes(wad_data)
+        # Retrieve the TMD data and write it out.
+        wad_data += self.get_tmd_data()
+        wad_data = pad_bytes(wad_data)
+        # Retrieve the meta/footer data and write it out.
+        wad_data += self.get_meta_data()
+        wad_data = pad_bytes(wad_data)
+        # Retrieve the content data and write it out.
+        wad_data += self.get_content_data()
+        wad_data = pad_bytes(wad_data)
         # Return the raw WAD file for the data contained in the object.
-        return wad_data_raw
+        return wad_data
 
     def get_wad_type(self) -> str:
         """
         Gets the type of the WAD.
 
         Returns
         -------
```

### Comparing `libwiipy-0.2.2/src/libWiiPy.egg-info/PKG-INFO` & `libwiipy-0.2.3/src/libWiiPy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libWiiPy
-Version: 0.2.2
+Version: 0.2.3
 Summary: A modern Python library for handling files used by the Wii
 Author-email: NinjaCheetah <ninjacheetah@ncxprogramming.com>, Lillian Skinner <lillian@randommeaninglesscharacters.com>
 Project-URL: Homepage, https://github.com/NinjaCheetah/libWiiPy
 Project-URL: Issues, https://github.com/NinjaCheetah/libWiipy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -22,15 +22,15 @@
 
 **Note:** While libWiiPy is directly inspired by libWiiSharp and aims to have feature parity with it, no code from either libWiiSharp or Wii.py was used in the making of this library. All code is original and is written by [@NinjaCheetah](https://github.com/NinjaCheetah), [@rvtr](https://github.com/rvtr), and any other GitHub contributors.
 
 # Features
 This list will expand as libWiiPy is developed, but these features are currently available:
 - TMD, ticket, and WAD parsing
 - WAD content extraction, decryption, re-encryption, and packing
-- Downloading free titles from the NUS
+- Downloading titles from the NUS
 
 # Usage
 A wiki, and in the future a potential documenation site, is being worked on, and can be accessed [here](https://github.com/NinjaCheetah/libWiiPy/wiki). It is currently fairly barebones, but it will be improved in the future.
 
 The easiest way to get libWiiPy for your project is to install the latest version of the library from PyPI, as shown below. 
 ```sh
 pip install -U libWiiPy
@@ -43,35 +43,35 @@
 ```
 Please be aware that because libWiiPy is in a very early state right now, many features may be subject to change, and methods and properties available now have the potential to disappear in the future.
 
 # Building
 To build this package locally, the steps are quite simple, and should apply to all platforms. Make sure you've set up your `venv` first!
 
 First, install the dependencies from `requirements.txt`:
-```py
+```sh
 pip install -r requirements.txt
 ```
 
 Then, build the package using the Python `build` module:
-```py
+```sh
 python -m build
 ```
 
 And that's all! You'll find your compiled pip package in `dist/`.
 
 # Special Thanks
-This project wouldn't be possible without the amazing people behind its predecessors and all of the people who have contributed to the documentation of the Wii's inner workings over at [Wiibrew](https://wiibrew.org).
+This project wouldn't be possible without the amazing people behind its predecessors and all of the people who have contributed to the documentation of the Wii's inner workings over at [WiiBrew](https://wiibrew.org).
 
 ## Special Thanks for the Inspiration and Previous Projects
 - Xuzz, SquidMan, megazig, Matt_P, Omega and The Lemon Man for creating Wii.py
 - Leathl for creating libWiiSharp
 - TheShadowEevee for maintaining libWiiSharp
 
-## Special Thanks to Wiibrew Contributors
-Thank you to all of the contributors to the documentation on the Wiibrew pages that make this all understandable! Some of the key articles referenced are as follows:
+## Special Thanks to WiiBrew Contributors
+Thank you to all of the contributors to the documentation on the WiiBrew pages that make this all understandable! Some of the key articles referenced are as follows:
 - [Title metadata](https://wiibrew.org/wiki/Title_metadata), for the documentation on how a TMD is structured
 - [WAD files](https://wiibrew.org/wiki/WAD_files), for the documentation on how a WAD is structured
 - [IOS history](https://wiibrew.org/wiki/IOS_history), for the documentation on IOS TIDs and how IOS is versioned
 
 ### One additional special thanks to [@DamiDoop](https://github.com/DamiDoop)!
 She made the very cool banner you can see at the top of this README, and has also helped greatly with my sanity throughout debugging this library.
```

