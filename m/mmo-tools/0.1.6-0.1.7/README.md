# Comparing `tmp/mmo_tools-0.1.6.tar.gz` & `tmp/mmo_tools-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmo_tools-0.1.6.tar", last modified: Sun May  5 09:01:13 2024, max compression
+gzip compressed data, was "mmo_tools-0.1.7.tar", last modified: Tue May 14 13:16:14 2024, max compression
```

## Comparing `mmo_tools-0.1.6.tar` & `mmo_tools-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 09:01:13.097372 mmo_tools-0.1.6/
--rw-rw-rw-   0        0        0     6191 2024-05-05 09:01:13.095372 mmo_tools-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     4757 2024-05-05 08:50:07.000000 mmo_tools-0.1.6/README.md
--rw-rw-rw-   0        0        0       42 2024-05-05 09:01:13.097372 mmo_tools-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1235 2024-05-05 09:00:58.000000 mmo_tools-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-05 09:01:13.072737 mmo_tools-0.1.6/src/
-drwxrwxrwx   0        0        0        0 2024-05-05 09:01:13.082360 mmo_tools-0.1.6/src/mmo_tools/
--rw-rw-rw-   0        0        0      304 2024-05-05 08:46:45.000000 mmo_tools-0.1.6/src/mmo_tools/__init__.py
--rw-rw-rw-   0        0        0     4675 2024-05-05 09:00:52.000000 mmo_tools-0.1.6/src/mmo_tools/core.py
--rw-rw-rw-   0        0        0     1852 2024-05-05 08:47:13.000000 mmo_tools-0.1.6/src/mmo_tools/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-05 09:01:13.094373 mmo_tools-0.1.6/src/mmo_tools.egg-info/
--rw-rw-rw-   0        0        0     6191 2024-05-05 09:01:13.000000 mmo_tools-0.1.6/src/mmo_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2024-05-05 09:01:13.000000 mmo_tools-0.1.6/src/mmo_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 09:01:13.000000 mmo_tools-0.1.6/src/mmo_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-05 09:01:13.000000 mmo_tools-0.1.6/src/mmo_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 13:16:14.949289 mmo_tools-0.1.7/
+-rw-rw-rw-   0        0        0     3646 2024-05-14 13:16:14.948289 mmo_tools-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2428 2024-05-14 13:12:43.000000 mmo_tools-0.1.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-14 13:16:14.949289 mmo_tools-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1235 2024-05-14 13:15:39.000000 mmo_tools-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 13:16:14.931289 mmo_tools-0.1.7/src/
+drwxrwxrwx   0        0        0        0 2024-05-14 13:16:14.933288 mmo_tools-0.1.7/src/mmo_tools/
+-rw-rw-rw-   0        0        0      304 2024-05-05 08:46:45.000000 mmo_tools-0.1.7/src/mmo_tools/__init__.py
+-rw-rw-rw-   0        0        0     5402 2024-05-14 13:01:39.000000 mmo_tools-0.1.7/src/mmo_tools/core.py
+-rw-rw-rw-   0        0        0     1852 2024-05-05 08:47:13.000000 mmo_tools-0.1.7/src/mmo_tools/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-14 13:16:14.948289 mmo_tools-0.1.7/src/mmo_tools.egg-info/
+-rw-rw-rw-   0        0        0     3646 2024-05-14 13:16:14.000000 mmo_tools-0.1.7/src/mmo_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2024-05-14 13:16:14.000000 mmo_tools-0.1.7/src/mmo_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 13:16:14.000000 mmo_tools-0.1.7/src/mmo_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-14 13:16:14.000000 mmo_tools-0.1.7/src/mmo_tools.egg-info/top_level.txt
```

### Comparing `mmo_tools-0.1.6/setup.py` & `mmo_tools-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
     name='mmo_tools',  # Tên thư viện của bạn
-    version='0.1.6',  # Phiên bản đầu tiên
+    version='0.1.7',  # Phiên bản đầu tiên
     packages=find_packages('src'),  # Tìm tất cả các packages trong thư mục src
     package_dir={'': 'src'},  # Chỉ định thư mục chứa các packages
     author='Lam Dinh',
     author_email='ldl.contact.booking@gmail.com',
     description='Thư Viện Hỗ Trợ Viết Tool Facebook Nhanh',
     long_description=open('README.md','r',encoding='utf-8').read(),  # Đọc nội dung README nếu có
     long_description_content_type='text/markdown',  # Định dạng của long description
```

### Comparing `mmo_tools-0.1.6/src/mmo_tools/core.py` & `mmo_tools-0.1.7/src/mmo_tools/core.py`

 * *Files 9% similar despite different names*

```diff
@@ -117,14 +117,35 @@
         ip , port , user , pass_proxy = map(str,proxy.split(":"))
         https = {
             "https":f"http://{user}:{pass_proxy}@{ip}:{ port}",
             "http":f"http://{user}:{pass_proxy}@{ip}:{ port}"
             }
     return https
 
+
+def cookie_confirm_auth_2fa(session:requests,code:str,fb_dtsg:str):
+    
+    """
+        Request confirm 2fa next link account
+
+        * input : / 
+                - session : Session account facebook
+                - code    : 8-digit code
+                - fb_stg  : Auth fb_stg , example : NAcMyHWHPkEy***3873369
+        
+        * output : /
+                - Bool True : confirm success
+                - Bool False : confirm error
+    """
+    return '"codeConfirmed":true' in session.post(
+        "https://business.facebook.com/security/twofactor/reauth/enter/",
+        data   = "approvals_code={}&save_device=true&__a=1&fb_dtsg={}".format(code,fb_dtsg),
+        timeout= 60
+        ).text
+    
 def check_facebook_account(fbid):
     """
         return  / live : 1
                 / die  : 0
     """
     try:
         response = requests.get(f'https://graph.facebook.com/{str(fbid)}/picture?redirect=0')
```

### Comparing `mmo_tools-0.1.6/src/mmo_tools/utils.py` & `mmo_tools-0.1.7/src/mmo_tools/utils.py`

 * *Files identical despite different names*

