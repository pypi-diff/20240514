# Comparing `tmp/py-transgpt-1.4.tar.gz` & `tmp/py_transgpt-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-transgpt-1.4.tar", last modified: Sat Nov 11 23:51:56 2023, max compression
+gzip compressed data, was "py_transgpt-1.5.tar", last modified: Tue May 14 17:53:22 2024, max compression
```

## Comparing `py-transgpt-1.4.tar` & `py_transgpt-1.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-11 23:51:56.433292 py-transgpt-1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2023-11-11 23:51:40.000000 py-transgpt-1.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      157 2023-11-11 23:51:40.000000 py-transgpt-1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5126 2023-11-11 23:51:56.433292 py-transgpt-1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2023-11-11 23:51:40.000000 py-transgpt-1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      230 2023-11-11 23:51:40.000000 py-transgpt-1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       78 2023-11-11 23:51:56.433292 py-transgpt-1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     8800 2023-11-11 23:51:40.000000 py-transgpt-1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-11 23:51:56.429292 py-transgpt-1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-11 23:51:56.433292 py-transgpt-1.4/src/py_transgpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5126 2023-11-11 23:51:56.000000 py-transgpt-1.4/src/py_transgpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      467 2023-11-11 23:51:56.000000 py-transgpt-1.4/src/py_transgpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-11 23:51:56.000000 py-transgpt-1.4/src/py_transgpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      124 2023-11-11 23:51:56.000000 py-transgpt-1.4/src/py_transgpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-11-11 23:51:56.000000 py-transgpt-1.4/src/py_transgpt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-11 23:51:56.433292 py-transgpt-1.4/src/transgpt/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2023-11-11 23:51:40.000000 py-transgpt-1.4/src/transgpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2023-11-11 23:51:40.000000 py-transgpt-1.4/src/transgpt/_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4535 2023-11-11 23:51:40.000000 py-transgpt-1.4/src/transgpt/_trans_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2445 2023-11-11 23:51:40.000000 py-transgpt-1.4/src/transgpt/trans_baidu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3210 2023-11-11 23:51:40.000000 py-transgpt-1.4/src/transgpt/trans_chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2023-11-11 23:51:40.000000 py-transgpt-1.4/src/transgpt/trans_tencent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2023-11-11 23:51:40.000000 py-transgpt-1.4/src/transgpt/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-11 23:51:56.433292 py-transgpt-1.4/test/
--rw-r--r--   0 runner    (1001) docker     (127)     9224 2023-11-11 23:51:40.000000 py-transgpt-1.4/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:53:22.809898 py_transgpt-1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-14 17:53:18.000000 py_transgpt-1.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-14 17:53:18.000000 py_transgpt-1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-05-14 17:53:22.809898 py_transgpt-1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-05-14 17:53:18.000000 py_transgpt-1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-14 17:53:18.000000 py_transgpt-1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-14 17:53:22.809898 py_transgpt-1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8800 2024-05-14 17:53:18.000000 py_transgpt-1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:53:22.805898 py_transgpt-1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:53:22.809898 py_transgpt-1.5/src/py_transgpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-05-14 17:53:22.000000 py_transgpt-1.5/src/py_transgpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-14 17:53:22.000000 py_transgpt-1.5/src/py_transgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 17:53:22.000000 py_transgpt-1.5/src/py_transgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-14 17:53:22.000000 py_transgpt-1.5/src/py_transgpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-14 17:53:22.000000 py_transgpt-1.5/src/py_transgpt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:53:22.809898 py_transgpt-1.5/src/transgpt/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-14 17:53:18.000000 py_transgpt-1.5/src/transgpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-14 17:53:18.000000 py_transgpt-1.5/src/transgpt/_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-05-14 17:53:18.000000 py_transgpt-1.5/src/transgpt/_trans_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-05-14 17:53:18.000000 py_transgpt-1.5/src/transgpt/trans_baidu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-14 17:53:18.000000 py_transgpt-1.5/src/transgpt/trans_chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-05-14 17:53:18.000000 py_transgpt-1.5/src/transgpt/trans_tencent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-14 17:53:18.000000 py_transgpt-1.5/src/transgpt/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:53:22.809898 py_transgpt-1.5/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     9224 2024-05-14 17:53:18.000000 py_transgpt-1.5/test/test.py
```

### Comparing `py-transgpt-1.4/LICENSE.txt` & `py_transgpt-1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `py-transgpt-1.4/PKG-INFO` & `py_transgpt-1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-transgpt
-Version: 1.4
+Version: 1.5
 Summary: Platform translation interface encapsulation: ChatGPT, Baidu, Tencent
 Home-page: https://github.com/EXP-Codes/py-transgpt
 Author: EXP
 Author-email: exp.lqb@gmail.com
 Project-URL: Bug Reports, https://github.com/EXP-Codes/py-transgpt/issues
 Project-URL: Funding, https://github.com/EXP-Codes/py-transgpt/tree/master/imgs/donate-alipay.png
 Project-URL: Say Thanks!, https://github.com/EXP-Codes/py-transgpt/tree/master/imgs/donate-wechat.png
```

### Comparing `py-transgpt-1.4/README.md` & `py_transgpt-1.5/README.md`

 * *Files identical despite different names*

### Comparing `py-transgpt-1.4/setup.py` & `py_transgpt-1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='1.4',  # Required. eg. 1.2.3
+    version='1.5',  # Required. eg. 1.2.3
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='Platform translation interface encapsulation: ChatGPT, Baidu, Tencent',  # Optional
 
     # This is an optional longer description of your project that represents
```

### Comparing `py-transgpt-1.4/src/py_transgpt.egg-info/PKG-INFO` & `py_transgpt-1.5/src/py_transgpt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-transgpt
-Version: 1.4
+Version: 1.5
 Summary: Platform translation interface encapsulation: ChatGPT, Baidu, Tencent
 Home-page: https://github.com/EXP-Codes/py-transgpt
 Author: EXP
 Author-email: exp.lqb@gmail.com
 Project-URL: Bug Reports, https://github.com/EXP-Codes/py-transgpt/issues
 Project-URL: Funding, https://github.com/EXP-Codes/py-transgpt/tree/master/imgs/donate-alipay.png
 Project-URL: Say Thanks!, https://github.com/EXP-Codes/py-transgpt/tree/master/imgs/donate-wechat.png
```

### Comparing `py-transgpt-1.4/src/transgpt/_trans_base.py` & `py_transgpt-1.5/src/transgpt/_trans_base.py`

 * *Files identical despite different names*

### Comparing `py-transgpt-1.4/src/transgpt/trans_baidu.py` & `py_transgpt-1.5/src/transgpt/trans_baidu.py`

 * *Files identical despite different names*

### Comparing `py-transgpt-1.4/src/transgpt/trans_chatgpt.py` & `py_transgpt-1.5/src/transgpt/trans_chatgpt.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 HTTP_PROXY = "HTTP_PROXY"
 HTTPS_PROXY = "HTTPS_PROXY"
 
 # GPT 接口模型定义 https://platform.openai.com/docs/models/
 CHATGPT_35_TURBO = "gpt-3.5-turbo"
 CHATGPT_4 = "gpt-4" # 8K
 CHATGPT_4_TRUBO = "gpt-4-1106-preview"    # 128K
+CHATGPT_4o = "gpt-4o"    # 128K
 
 ARG_ROLE = 'role'
 ARG_OPENAI_MODEL = 'openai_model'
 ARG_PROXY_IP = 'proxy_ip'
 ARG_PROXY_PORT = 'proxy_port'
 
 class ChatgptTranslation(BaseTranslation) :
```

### Comparing `py-transgpt-1.4/src/transgpt/trans_tencent.py` & `py_transgpt-1.5/src/transgpt/trans_tencent.py`

 * *Files identical despite different names*

### Comparing `py-transgpt-1.4/src/transgpt/translate.py` & `py_transgpt-1.5/src/transgpt/translate.py`

 * *Files identical despite different names*

### Comparing `py-transgpt-1.4/test/test.py` & `py_transgpt-1.5/test/test.py`

 * *Files identical despite different names*

