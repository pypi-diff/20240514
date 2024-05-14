# Comparing `tmp/ctrip-app-ui-0.4.3.tar.gz` & `tmp/ctrip-app-ui-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-app-ui-0.4.3.tar", last modified: Mon May 13 17:24:35 2024, max compression
+gzip compressed data, was "ctrip-app-ui-0.4.4.tar", last modified: Mon May 13 17:38:25 2024, max compression
```

## Comparing `ctrip-app-ui-0.4.3.tar` & `ctrip-app-ui-0.4.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 17:24:35.406988 ctrip-app-ui-0.4.3/
--rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.4.3/LICENSE
--rw-rw-rw-   0        0        0      474 2024-05-13 17:24:35.404992 ctrip-app-ui-0.4.3/PKG-INFO
--rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.4.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 17:24:35.390032 ctrip-app-ui-0.4.3/capp_ui/
--rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.4.3/capp_ui/__init__.py
--rw-rw-rw-   0        0        0      736 2024-05-06 07:02:29.000000 ctrip-app-ui-0.4.3/capp_ui/config.py
--rw-rw-rw-   0        0        0     4060 2024-05-07 16:57:27.000000 ctrip-app-ui-0.4.3/capp_ui/date_extend.py
--rw-rw-rw-   0        0        0     1664 2024-05-09 13:31:21.000000 ctrip-app-ui-0.4.3/capp_ui/device.py
--rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.4.3/capp_ui/dir.py
--rw-rw-rw-   0        0        0    64892 2024-05-13 17:22:07.000000 ctrip-app-ui-0.4.3/capp_ui/domain_service.py
--rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.4.3/capp_ui/fee.py
--rw-rw-rw-   0        0        0     3859 2024-05-11 16:34:35.000000 ctrip-app-ui-0.4.3/capp_ui/libs.py
--rw-rw-rw-   0        0        0    24821 2024-05-13 17:15:14.000000 ctrip-app-ui-0.4.3/capp_ui/mobile_terminals.py
--rw-rw-rw-   0        0        0     1719 2024-04-28 16:15:39.000000 ctrip-app-ui-0.4.3/capp_ui/platforms.py
--rw-rw-rw-   0        0        0      765 2024-04-28 16:02:26.000000 ctrip-app-ui-0.4.3/capp_ui/test.py
--rw-rw-rw-   0        0        0     5486 2024-05-11 03:13:30.000000 ctrip-app-ui-0.4.3/capp_ui/utils.py
--rw-rw-rw-   0        0        0     3023 2024-05-11 03:13:43.000000 ctrip-app-ui-0.4.3/capp_ui/validators.py
-drwxrwxrwx   0        0        0        0 2024-05-13 17:24:35.403995 ctrip-app-ui-0.4.3/ctrip_app_ui.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-13 17:24:35.000000 ctrip-app-ui-0.4.3/ctrip_app_ui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      460 2024-05-13 17:24:35.000000 ctrip-app-ui-0.4.3/ctrip_app_ui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 17:24:35.000000 ctrip-app-ui-0.4.3/ctrip_app_ui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-13 17:24:35.000000 ctrip-app-ui-0.4.3/ctrip_app_ui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-13 17:24:35.000000 ctrip-app-ui-0.4.3/ctrip_app_ui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 17:24:35.407987 ctrip-app-ui-0.4.3/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-13 17:24:26.000000 ctrip-app-ui-0.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 17:38:25.449829 ctrip-app-ui-0.4.4/
+-rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.4.4/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-05-13 17:38:25.448855 ctrip-app-ui-0.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.4.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 17:38:25.436865 ctrip-app-ui-0.4.4/capp_ui/
+-rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.4.4/capp_ui/__init__.py
+-rw-rw-rw-   0        0        0      736 2024-05-06 07:02:29.000000 ctrip-app-ui-0.4.4/capp_ui/config.py
+-rw-rw-rw-   0        0        0     4060 2024-05-07 16:57:27.000000 ctrip-app-ui-0.4.4/capp_ui/date_extend.py
+-rw-rw-rw-   0        0        0     1664 2024-05-09 13:31:21.000000 ctrip-app-ui-0.4.4/capp_ui/device.py
+-rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.4.4/capp_ui/dir.py
+-rw-rw-rw-   0        0        0    64845 2024-05-13 17:38:13.000000 ctrip-app-ui-0.4.4/capp_ui/domain_service.py
+-rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.4.4/capp_ui/fee.py
+-rw-rw-rw-   0        0        0     3859 2024-05-11 16:34:35.000000 ctrip-app-ui-0.4.4/capp_ui/libs.py
+-rw-rw-rw-   0        0        0    24821 2024-05-13 17:15:14.000000 ctrip-app-ui-0.4.4/capp_ui/mobile_terminals.py
+-rw-rw-rw-   0        0        0     1719 2024-04-28 16:15:39.000000 ctrip-app-ui-0.4.4/capp_ui/platforms.py
+-rw-rw-rw-   0        0        0      765 2024-04-28 16:02:26.000000 ctrip-app-ui-0.4.4/capp_ui/test.py
+-rw-rw-rw-   0        0        0     5486 2024-05-11 03:13:30.000000 ctrip-app-ui-0.4.4/capp_ui/utils.py
+-rw-rw-rw-   0        0        0     3023 2024-05-11 03:13:43.000000 ctrip-app-ui-0.4.4/capp_ui/validators.py
+drwxrwxrwx   0        0        0        0 2024-05-13 17:38:25.446837 ctrip-app-ui-0.4.4/ctrip_app_ui.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-13 17:38:25.000000 ctrip-app-ui-0.4.4/ctrip_app_ui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      460 2024-05-13 17:38:25.000000 ctrip-app-ui-0.4.4/ctrip_app_ui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 17:38:25.000000 ctrip-app-ui-0.4.4/ctrip_app_ui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-13 17:38:25.000000 ctrip-app-ui-0.4.4/ctrip_app_ui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-13 17:38:25.000000 ctrip-app-ui-0.4.4/ctrip_app_ui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 17:38:25.449829 ctrip-app-ui-0.4.4/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-13 17:38:21.000000 ctrip-app-ui-0.4.4/setup.py
```

### Comparing `ctrip-app-ui-0.4.3/LICENSE` & `ctrip-app-ui-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.3/capp_ui/config.py` & `ctrip-app-ui-0.4.4/capp_ui/config.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.3/capp_ui/date_extend.py` & `ctrip-app-ui-0.4.4/capp_ui/date_extend.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.3/capp_ui/device.py` & `ctrip-app-ui-0.4.4/capp_ui/device.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.3/capp_ui/dir.py` & `ctrip-app-ui-0.4.4/capp_ui/dir.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.3/capp_ui/domain_service.py` & `ctrip-app-ui-0.4.4/capp_ui/domain_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1170,16 +1170,15 @@
     # @SleepWait(wait_time=1)
     def select_more_payment(self) -> bool:
         """
         当【同意并支付】后，特殊情况下，会出现支付小弹框，这个时候需要先判断是否存在小框，如果存在，则切换到通用支付选择界面
         """
         flag = False
         try:
-            more_payment = self.device.get_po(type="android.view.ViewGroup", name="更多付款方式",
-                                              text="更多付款方式")
+            more_payment = self.device.get_po(type="android.view.ViewGroup", name="更多付款方式", desc="更多付款方式")
             if more_payment.exists() is True:
                 more_payment.click()
                 logger.warning("小弹框选择【更多付款方式】")
                 flag = True
         except (PocoNoSuchNodeException, Exception):
             try:
                 file_name = join_path([get_images_dir(), "更多付款方式.png"])
```

### Comparing `ctrip-app-ui-0.4.3/capp_ui/fee.py` & `ctrip-app-ui-0.4.4/capp_ui/fee.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.3/capp_ui/libs.py` & `ctrip-app-ui-0.4.4/capp_ui/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.3/capp_ui/mobile_terminals.py` & `ctrip-app-ui-0.4.4/capp_ui/mobile_terminals.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.3/capp_ui/platforms.py` & `ctrip-app-ui-0.4.4/capp_ui/platforms.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.3/capp_ui/test.py` & `ctrip-app-ui-0.4.4/capp_ui/test.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.3/capp_ui/utils.py` & `ctrip-app-ui-0.4.4/capp_ui/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.3/capp_ui/validators.py` & `ctrip-app-ui-0.4.4/capp_ui/validators.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.3/setup.py` & `ctrip-app-ui-0.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-app-ui',
-    version='0.4.3',
+    version='0.4.4',
     description='This is my ctrip app ui package',
     long_description='This is my ctrip app ui package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-app-ui',
     packages=find_packages(),
     install_requires=[
```

