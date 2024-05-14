# Comparing `tmp/pyuftp-0.0.6.tar.gz` & `tmp/pyuftp-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyuftp-0.0.6.tar", last modified: Wed Jun 28 13:00:45 2023, max compression
+gzip compressed data, was "pyuftp-1.0.2.tar", last modified: Tue May 14 07:11:33 2024, max compression
```

## Comparing `pyuftp-0.0.6.tar` & `pyuftp-1.0.2.tar`

### file list

```diff
@@ -1,25 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:00:45.066634 pyuftp-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-28 13:00:31.000000 pyuftp-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-28 13:00:45.066634 pyuftp-0.0.6/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     1145 2023-06-28 13:00:31.000000 pyuftp-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-28 13:00:31.000000 pyuftp-0.0.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:00:45.066634 pyuftp-0.0.6/pyuftp/
--rwxr-xr-x   0 runner    (1001) docker     (123)       74 2023-06-28 13:00:31.000000 pyuftp-0.0.6/pyuftp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-28 13:00:45.066634 pyuftp-0.0.6/pyuftp/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7202 2023-06-28 13:00:31.000000 pyuftp-0.0.6/pyuftp/authenticate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-06-28 13:00:31.000000 pyuftp-0.0.6/pyuftp/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-28 13:00:31.000000 pyuftp-0.0.6/pyuftp/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11899 2023-06-28 13:00:31.000000 pyuftp-0.0.6/pyuftp/cp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-06-28 13:00:31.000000 pyuftp-0.0.6/pyuftp/share.py
--rw-r--r--   0 runner    (1001) docker     (123)     7911 2023-06-28 13:00:31.000000 pyuftp-0.0.6/pyuftp/uftp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-06-28 13:00:31.000000 pyuftp-0.0.6/pyuftp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:00:45.066634 pyuftp-0.0.6/pyuftp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-28 13:00:45.000000 pyuftp-0.0.6/pyuftp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-28 13:00:45.000000 pyuftp-0.0.6/pyuftp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 13:00:45.000000 pyuftp-0.0.6/pyuftp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-28 13:00:45.000000 pyuftp-0.0.6/pyuftp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 13:00:45.000000 pyuftp-0.0.6/pyuftp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-28 13:00:45.000000 pyuftp-0.0.6/pyuftp.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      190 2023-06-28 13:00:45.066634 pyuftp-0.0.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1062 2023-06-28 13:00:31.000000 pyuftp-0.0.6/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-06-28 13:00:31.000000 pyuftp-0.0.6/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:11:33.792507 pyuftp-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-14 07:11:25.000000 pyuftp-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-14 07:11:25.000000 pyuftp-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-05-14 07:11:33.792507 pyuftp-1.0.2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2247 2024-05-14 07:11:25.000000 pyuftp-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:11:33.788507 pyuftp-1.0.2/extras/
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-14 07:11:25.000000 pyuftp-1.0.2/extras/pyuftp
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-14 07:11:25.000000 pyuftp-1.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:11:33.792507 pyuftp-1.0.2/pyuftp/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       74 2024-05-14 07:11:25.000000 pyuftp-1.0.2/pyuftp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-14 07:11:33.796507 pyuftp-1.0.2/pyuftp/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10513 2024-05-14 07:11:25.000000 pyuftp-1.0.2/pyuftp/authenticate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14482 2024-05-14 07:11:25.000000 pyuftp-1.0.2/pyuftp/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-14 07:11:25.000000 pyuftp-1.0.2/pyuftp/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13822 2024-05-14 07:11:25.000000 pyuftp-1.0.2/pyuftp/cp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-14 07:11:25.000000 pyuftp-1.0.2/pyuftp/cryptutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-05-14 07:11:25.000000 pyuftp-1.0.2/pyuftp/pconnector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-05-14 07:11:25.000000 pyuftp-1.0.2/pyuftp/share.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13570 2024-05-14 07:11:25.000000 pyuftp-1.0.2/pyuftp/uftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9515 2024-05-14 07:11:25.000000 pyuftp-1.0.2/pyuftp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:11:33.792507 pyuftp-1.0.2/pyuftp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-05-14 07:11:33.000000 pyuftp-1.0.2/pyuftp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-14 07:11:33.000000 pyuftp-1.0.2/pyuftp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 07:11:33.000000 pyuftp-1.0.2/pyuftp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-14 07:11:33.000000 pyuftp-1.0.2/pyuftp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-14 07:11:33.000000 pyuftp-1.0.2/pyuftp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 07:11:33.000000 pyuftp-1.0.2/pyuftp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-14 07:11:25.000000 pyuftp-1.0.2/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      190 2024-05-14 07:11:33.792507 pyuftp-1.0.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1208 2024-05-14 07:11:25.000000 pyuftp-1.0.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83607 2024-05-14 07:11:25.000000 pyuftp-1.0.2/versioneer.py
```

### Comparing `pyuftp-0.0.6/LICENSE` & `pyuftp-1.0.2/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Copyright (c) 2011-2023
+Copyright (c) 2011-2024
 Forschungszentrum Jülich GmbH, ICM Warsaw, and other 
-contributors to UNICORE: http://www.unicore.eu
+contributors to UNICORE: https://www.unicore.eu
 
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are
 met:
```

### Comparing `pyuftp-0.0.6/PKG-INFO` & `pyuftp-1.0.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: pyuftp
-Version: 0.0.6
-Summary: UFTP (UNICORE FTP) commandline client
-Home-page: https://github.com/UNICORE-EU/pyuftp
-Author: Bernd Schuller
-Author-email: b.schuller@fz-juelich.de
-License: License :: OSI Approved :: BSD
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # PyUFTP, a commandline client for UFTP (UNICORE FTP) commandline client
 
 UFTP (UNICORE File Transfer Protocol) is a high-performance data
 streaming library and file transfer tool with sharing capabilities.
 It allows to transfer data from client to server (and vice versa),
 as well as providing data staging and third-party transfer between
 UFTP-enabled UNICORE sites.
@@ -25,18 +13,58 @@
 Commands include
 
 * authenticate  - Authenticate only, returning UFTPD address and one-time password
 * checksum      - Compute hashes for remote file(s) (MD5, SHA-1, SHA-256, SHA-512)
 * cp            - Download/upload file(s)
 * find          - List all files in a remote directory
 * info          - Gets info about the remote server
+* issue-token   - Get an authentication token from the Auth server
 * ls            - List a remote directory
 * mkdir         - Create a remote directory
 * rcp           - Server-server copy
 * rm            - Remove a remote file/directory
 * share         - List, create, update and delete shares
 
 ## Installation
 
 Install from PyPI with
 
-    pip install -U pyuftp
+    python3 -m pip install -U pyuftp
+
+### Commandline completion
+
+PyUFTP comes with a commandline completion script for Bash, but
+due to the limitations of a Python-based install, it might not get
+picked up automatically.
+
+If installing in a virtual environment (venv), you need
+to load it manually:
+
+    source $VIRTUAL_ENV/share/bash-completion/pyuftp
+
+You can also add this line to the venv activation script:
+
+    echo ". $VIRTUAL_ENV/share/bash-completion/pyuftp" >> $VIRTUAL_ENV/bin/activate
+
+When installing outside of a virtual environment, the completion script
+will be installed in 
+
+    ~/.local/share/bash-completion/completions/pyuftp
+
+and should be picked up automatically by Bash completion and loaded
+when you start a new shell.
+
+
+## Usage
+
+The commandline syntax is (mostly) the same as the Java version, have a look at the
+[documentation](https://uftp-docs.readthedocs.io/en/latest/user-docs/uftp-client/index.html).
+
+Try
+
+    pyuftp --help
+
+for a list of commands, and
+
+    pyuftp <command> --help
+
+to see the built-in help for each command.
```

### Comparing `pyuftp-0.0.6/pyuftp/base.py` & `pyuftp-1.0.2/pyuftp/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,223 +1,257 @@
-""" Base command class and a few general commands """
+""" 
+  Utility commands (ls, mkdir, ...) and helpers
+"""
 
-import pyuftp.authenticate
-import argparse, getpass, json, os, os.path, sys, threading
-from urllib.parse import urlparse
-
-class Base:
-    """ Base command class with support for common commandline args """
-
-    def __init__(self, password_source=None):
-        self.parser = argparse.ArgumentParser(prog="pyuftp",
-                                              description="A commandline client for UFTP (UNICORE FTP)")
-        self.args = None
-        self.is_verbose = False
-        self.credential = None
-        self.add_base_args()
-        self.add_command_args()
-        if password_source:
-            self.password_source = password_source
-        else:
-            self.password_source = getpass.getpass
+import pyuftp.base, pyuftp.uftp
 
-    def add_base_args(self):
-        self.parser.add_argument("-v", "--verbose",
-                            required=False,
-                            action="store_true",
-                            help="be verbose")
-        self.parser.add_argument("-t", "--token", help="authentication: bearer token")
-        self.parser.add_argument("-u", "--user", help="authentication: username[:password]")
-        self.parser.add_argument("-P", "--password", action="store_true",
-                            help="interactively query for password")
-        self.parser.add_argument("-i", "--identity", help="authentication: private key file")
+import fnmatch, os, os.path, stat, zlib
 
+class Ls(pyuftp.base.Base):
+    
     def add_command_args(self):
-        pass
+        self.parser.prog = "pyuftp ls"
+        self.parser.description = self.get_synopsis()
+        self.parser.add_argument("remoteURL", help="Remote UFTP URL")
 
-    def authenticate(self, endpoint, base_dir):
-        """ authenticate
-        Args:
-           endpoint - UFTP auth URL
-           base_dir - requested session base directory
-        Returns:
-           a tuple  (host, port, onetime_password)
-        """
-        self.verbose(f"Authenticating at {endpoint}, base dir: '{base_dir}'")
-        return pyuftp.authenticate.authenticate(endpoint, self.credential, base_dir)
+    def get_synopsis(self):
+        return """List a remote directory"""
 
     def run(self, args):
-        self.args = self.parser.parse_args(args)
-        self.is_verbose = self.args.verbose
-        self.create_credential()
+        super().run(args)
+        endpoint, base_dir, file_name = self.parse_url(self.args.remoteURL)
+        if endpoint is None:
+            raise ValueError(f"Does not seem to be a valid URL: {self.args.authURL}")
+        if file_name is None:
+            file_name = "."
+        host, port, onetime_pwd = self.authenticate(endpoint, base_dir)
+        self.verbose(f"Connecting to UFTPD {host}:{port}")
+        with pyuftp.uftp.open(host, port, onetime_pwd) as uftp:
+            entries = uftp.listdir(file_name)
+            width = 1
+            for entry in entries:
+                width = max(width, len(str(entry.size)))
+            for entry in entries:
+                print(entry.as_ls(width))
 
-    def get_synopsis(self):
-        return "N/A"
 
-    def create_credential(self):
-        username = None
-        password = None
-        identity = self.args.identity
-        token  = self.args.token
-        if self.args.user:
-            if ":" in self.args.user:
-                username, password = self.args.user.split(":",1)
-            else:
-                username = self.args.user
-        else:
-            username = os.getenv("UFTP_USER")
-            if not username:
-                username = os.getenv("USER")
-        if self.args.identity is None:
-            pwd_prompt = "Enter password: "
-        else:
-            pwd_prompt = "Enter passphrase for key: "
-        if self.args.password and password is None:
-            password = self.password_source(pwd_prompt)
-        try:
-            self.credential = pyuftp.authenticate.create_credential(username, password, token, identity)
-        except ValueError as e:
-            if self.args.identity is not None and password is None:
-                password = self.password_source(pwd_prompt)    
-                self.credential = pyuftp.authenticate.create_credential(username, password, token, identity)
-            else:
-                raise e
+class Mkdir(pyuftp.base.Base):
+    
+    def add_command_args(self):
+        self.parser.prog = "pyuftp mkdir"
+        self.parser.description = self.get_synopsis()
+        self.parser.add_argument("remoteURL", help="Remote UFTP URL")
 
-    def parse_url(self, url):
-        """ 
-        parses the given URL and returns a tuple consisting of
-         - auth endpoint URL (or None if URL is not a http(s) URL)
-         - base directory
-         - file name
-        as appropriate
-        """
-        parsed = urlparse(url)
-        service_path = parsed.path
-        endpoint = None
-        basedir = ""
-        filename = None
-        if ":" in service_path:
-            service_path, file_path = service_path.split(":",1)
-            if len(file_path)>0:
-                basedir = os.path.dirname(file_path)
-                filename = os.path.basename(file_path)
-        if service_path.endswith("/"):
-                service_path = service_path[:-1]
-        if parsed.scheme.lower().startswith("http"):
-            endpoint = f"{parsed.scheme}://{parsed.netloc}{service_path}"
-        return endpoint, basedir, filename
-
-    def verbose(self, msg):
-        if self.is_verbose:
-            print(msg)
+    def get_synopsis(self):
+        return """Create a remote directory"""
+
+    def run(self, args):
+        super().run(args)
+        endpoint, base_dir, file_name = self.parse_url(self.args.remoteURL)
+        if endpoint is None:
+            raise ValueError(f"Does not seem to be a valid URL: {self.args.authURL}")
+        host, port, onetime_pwd = self.authenticate(endpoint, base_dir)
+        self.verbose(f"Connecting to UFTPD {host}:{port}")
+        with pyuftp.uftp.open(host, port, onetime_pwd) as uftp:
+            uftp.mkdir(file_name)
 
-class Info(Base):
 
+class Rm(pyuftp.base.Base):
+    
     def add_command_args(self):
-        self.parser.prog = "pyuftp info"
+        self.parser.prog = "pyuftp rm"
         self.parser.description = self.get_synopsis()
-        self.parser.add_argument("authURL", help="Auth server URL")
-        self.parser.add_argument("-R", "--raw", help="print the JSON response from the server")
+        self.parser.add_argument("remoteURL", help="Remote UFTP URL")
 
     def get_synopsis(self):
-        return """Gets info about the remote server"""
+        return """Remove a remote file/directory"""
 
     def run(self, args):
         super().run(args)
-        endpoint, _, _ = self.parse_url(self.args.authURL)
+        endpoint, base_dir, file_name = self.parse_url(self.args.remoteURL)
         if endpoint is None:
             raise ValueError(f"Does not seem to be a valid URL: {self.args.authURL}")
-        auth_url = endpoint.split("/rest/auth")[0]+"/rest/auth"
-        self.verbose(f"Connecting to {auth_url}")
-        reply = pyuftp.authenticate.get_json(auth_url, self.credential)
-        if self.args.raw:
-            print(json.dumps(reply, indent=2))
-        else:
-            self.show_info(reply, auth_url)
-    
-    def show_info(self, reply, auth_url):
-        print(f"Client identity:    {reply['client']['dn']}")
-        print(f"Client auth method: {self.credential}")
-        print(f"Auth server type:   AuthServer v{reply['server'].get('version', 'n/a')}")
-        for key in reply:
-            if key in ['client', 'server']:
-                continue
-            server = reply[key]
-            print(f"Server: {key}")
-            print(f"  URL base:         {auth_url}/{key}")
-            print(f"  Description:      {server.get('description', 'N/A')}")
-            print(f"  Remote user info: uid={server.get('uid', 'N/A')};gid={server.get('gid', 'N/A')}")
-            if str(server["dataSharing"]["enabled"]).lower() == 'true':
-                sharing = "enabled"
+        if file_name is None:
+            file_name = "."
+        host, port, onetime_pwd = self.authenticate(endpoint, base_dir)
+        self.verbose(f"Connecting to UFTPD {host}:{port}")
+        with pyuftp.uftp.open(host, port, onetime_pwd) as uftp:
+            st = uftp.stat(file_name)
+            if st['st_mode']&stat.S_IFDIR:
+                uftp.rmdir(file_name)
             else:
-                sharing = "disabled"
-            print(f"  Sharing support:  {sharing}")
-            print(f"  Server status:    {server.get('status', 'N/A')}")
-
-class Auth(Base):
+                uftp.rm(file_name)
 
+class Checksum(pyuftp.base.Base):
+    
     def add_command_args(self):
-        self.parser.prog = "pyuftp auth"
+        self.parser.prog = "pyuftp checksum"
         self.parser.description = self.get_synopsis()
-        self.parser.add_argument("authURL", help="Auth URL")
-
+        self.parser.add_argument("remoteURL", help="Remote UFTP URL")
+        self.parser.add_argument("-a", "--algorithm", help="Hash algorithm to use (MD5, SHA-1, SHA-256, SHA-512")
     def get_synopsis(self):
-        return """Authenticate only, returning UFTP address and one-time password"""
+        return """Checksum a remote file"""
 
     def run(self, args):
         super().run(args)
-        endpoint, base_dir, _ = self.parse_url(self.args.authURL)
+        endpoint, base_dir, file_name = self.parse_url(self.args.remoteURL)
         if endpoint is None:
             raise ValueError(f"Does not seem to be a valid URL: {self.args.authURL}")
+        if file_name is None:
+            file_name = "."
         host, port, onetime_pwd = self.authenticate(endpoint, base_dir)
-        print(f"Connect to {host}:{port} password: {onetime_pwd}")
-        return host, port, onetime_pwd
-
-class CopyBase(Base):
+        self.verbose(f"Connecting to UFTPD {host}:{port}")
+        _hash = ""
+        with pyuftp.uftp.open(host, port, onetime_pwd) as uftp:
+            for (entry, _) in crawl_remote(uftp, base_dir, file_name):
+                entry = os.path.relpath(entry, base_dir)
+                _hash, _f = uftp.checksum(entry, self.args.algorithm)
+                print(_hash, _f)
+            return _hash
 
-    def add_base_args(self):
-        Base.add_base_args(self)
-        self.parser.add_argument("-B", "--bytes", help="Byte range: range_spec", required=False)
+class Find(pyuftp.base.Base):
+    
+    def add_command_args(self):
+        self.parser.prog = "pyuftp find"
+        self.parser.description = self.get_synopsis()
+        self.parser.add_argument("remoteURL", help="Remote UFTP URL")
+        self.parser.add_argument("-r", "--recurse", required=False, action="store_true",
+                                 help="Recurse into subdirectories, if applicable")
+        self.parser.add_argument("-F", "--files-only", required=False, action="store_true",
+                                 help="Only list files, not directories")
+        self.parser.add_argument("-p", "--pattern", required=False, type=str, default="*",
+                                 help="Only list entries matching this pattern")
+        
+    def get_synopsis(self):
+        return """List all files in a remote directory"""
 
     def run(self, args):
         super().run(args)
-        self.init_range()
+        endpoint, base_dir, file_name = self.parse_url(self.args.remoteURL)
+        if endpoint is None:
+            raise ValueError(f"Does not seem to be a valid URL: {self.args.authURL}")
+        host, port, onetime_pwd = self.authenticate(endpoint, base_dir)
+        self.verbose(f"Connecting to UFTPD {host}:{port}")
+        with pyuftp.uftp.open(host, port, onetime_pwd) as uftp:
+            base = "."
+            pattern = self.args.pattern
+            if len(file_name)>0:
+                if uftp.is_dir(file_name):
+                    base = file_name
+                    uftp.cwd(base)
+                else:
+                    pattern = file_name
+            if base_dir=="/":
+                # to clean-up the output since normpath does not collapse two leading '/'
+                base_dir = ""
+            for (entry, _) in crawl_remote(uftp, base, pattern,
+                                           all=self.args.recurse,
+                                           files_only=self.args.files_only):
+                print(os.path.normpath(base_dir+"/"+entry))
+
+
+_factors = {"k":1024, "m":1024*1024, "g":1024*1024*1024}
+
+def parse_value_with_units(value):
+    multiplier = value[-1].lower()
+    _factor = 1
+    if not multiplier in "0123456789":
+        _factor = _factors.get(multiplier)
+        if not _factor:
+            raise ValueError(f"Cannot parse '{value}'")
+        value = value[:-1]
+    return _factor * int(value)
+
+def is_wildcard(path):
+    return "*" in path or "?" in path
+
+def crawl_remote(uftp, base_dir, file_pattern="*", recurse=False, all=False, files_only=True, _level=0):
+    """ returns tuples (name, size) """
+    if not files_only and _level==0:
+        # return top-level dir because Unix 'find' does it
+        bd = uftp.stat(".")
+        yield base_dir, bd["st_size"]
+    for x in uftp.listdir("."):
+        if not x.is_dir or not files_only:
+            if not fnmatch.fnmatch(x.path, file_pattern):
+                continue
+            else:
+                yield base_dir+"/"+x.path, x.size
+        if x.is_dir and (all or (recurse and fnmatch.fnmatch(x.path, file_pattern))):
+            try:
+                uftp.cwd(x.path)
+            except OSError:
+                continue
+            for y, size in crawl_remote(uftp, base_dir+"/"+x.path, file_pattern, recurse, all, _level+1):
+                yield y, size
+            uftp.cdup()
+    
+def crawl_local(base_dir, file_pattern="*", recurse=False, all=False):
+    for x in os.listdir(base_dir):
+        if not os.path.isdir(base_dir+"/"+x):
+            if not fnmatch.fnmatch(x, file_pattern):
+                continue
+            else:
+                yield base_dir+"/"+x
+        if all or (recurse and fnmatch.fnmatch(x, file_pattern)):
+            for y in crawl_local(base_dir+"/"+x, file_pattern, recurse, all):
+                yield y
 
-    def init_range(self):
-        self.start_byte = 0
-        self.end_byte = -1
-        self.have_range = False
-        self.range_read_write = False
-        if self.args.bytes:
-            self.have_range = True
-            tok = self.args.bytes.split("-")
-            if len(tok[0])>0:
-                self.start_byte = pyuftp.utils.parse_value_with_units(tok[0])
-                self.end_byte = sys.maxsize
-            if len(tok[1])>0:
-                self.end_byte = pyuftp.utils.parse_value_with_units(tok[1])
-            self.range_read_write = len(tok)>2 and tok[2]=="p"
-            self.verbose(f"Range {self.start_byte}-{self.end_byte} rw={self.range_read_write}")
-
-    def _get_range(self, default_length=-1):
-        offset = 0
-        length = default_length
-        if self.have_range:
-            offset = self.start_byte
-            length = self.end_byte - self.start_byte + 1
-        return offset, length
+class GzipWriter(object):
+    
+    def __init__(self, target):
+        self.target = target
+        self.compressor = zlib.compressobj(wbits=31)
+        self._closed = False
+
+    def write(self, data):
+        compressed = self.compressor.compress(data)
+        self.target.write(compressed)
+        return len(data)
 
-    def log_usage(self, send, source, target, size, duration):
-        if not self.is_verbose:
+    def flush(self, finish = False):
+        if self._closed:
             return
-        if send:
-            operation = "Sent"
+        if finish:
+            compressed = self.compressor.flush()
         else:
-            operation = "Received"
-        rate = 0.001*float(size)/(float(duration)+1)
-        if rate<1000:
-            unit = "kB/sec"
-            rate = int(rate)
+            compressed = self.compressor.flush(zlib.Z_SYNC_FLUSH)
+        self.target.write(compressed)
+        self.target.flush()
+
+    def close(self):
+        if self._closed:
+            return
+        self.flush(finish=True)
+        self.target.close()
+        self._closed = True
+    
+class GzipReader(object):
+    
+    def __init__(self, source):
+        self.source = source
+        self.decompressor = zlib.decompressobj(wbits=31)
+        self.stored = b""
+
+    def read(self, length):
+        buf = bytearray(self.stored)
+        have = len(buf)
+        finish = False
+        while have<length and not finish:
+            data = self.source.read(length-have)
+            if len(data)==0:
+                finish = True
+                decompressed = self.decompressor.flush()
+            else:
+                decompressed = self.decompressor.decompress(data)
+            buf+=decompressed
+            have = len(buf)
+        if have>length:
+            result = buf[0:length]
+            self.stored = buf[length:]
         else:
-            unit = "MB/sec"
-            rate = int(rate / 1000)
-        print(f"USAGE [{threading.current_thread().name}] [{operation}] {source}-->{target} [{size} bytes] [{rate} {unit}]")
+            result = buf
+            self.stored = b""
+        return result
+    
+    def close(self):
+        self.source.close()
```

### Comparing `pyuftp-0.0.6/pyuftp/client.py` & `pyuftp-1.0.2/pyuftp/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 """ Main client class """
 
 import pyuftp.base, pyuftp.cp, pyuftp.share, pyuftp.utils, pyuftp._version
 
 import platform, sys
 
 _commands = {
-            "authenticate": pyuftp.base.Auth(),
-            "checksum": pyuftp.utils.Checksum(),
-            "cp": pyuftp.cp.Copy(),
-            "find": pyuftp.utils.Find(),
-            "info": pyuftp.base.Info(),
-            "ls": pyuftp.utils.Ls(),
-            "mkdir": pyuftp.utils.Mkdir(),
-            "rcp": pyuftp.cp.RemoteCopy(),
-            "rm": pyuftp.utils.Rm(),
-            "share": pyuftp.share.Share(),
+            "authenticate": pyuftp.base.Auth,
+            "checksum": pyuftp.utils.Checksum,
+            "cp": pyuftp.cp.Copy,
+            "find": pyuftp.utils.Find,
+            "info": pyuftp.base.Info,
+            "issue-token": pyuftp.base.IssueToken,
+            "ls": pyuftp.utils.Ls,
+            "mkdir": pyuftp.utils.Mkdir,
+            "rcp": pyuftp.cp.RemoteCopy,
+            "rm": pyuftp.utils.Rm,
+            "share": pyuftp.share.Share,
         }
 
+def get_command(name):
+    return _commands.get(name)()
+
 def show_version():
     print("PyUFTP commandline client for UFTP (UNICORE FTP) "
           "%s, https://www.unicore.eu" % pyuftp._version.get_versions().get('version', "n/a"))
     print("Python %s" % sys.version)
     print("OS: %s" % platform.platform())
 
 
 def help():
     s = """PyUFTP commandline client for UFTP (UNICORE FTP) %s, https://www.unicore.eu
 Usage: pyuftp <command> [OPTIONS] <args>
 The following commands are available:""" % pyuftp._version.get_versions().get('version', "n/a")
     print(s)
     for cmd in _commands:
-        print (f" {cmd:20} - {_commands[cmd].get_synopsis()}")
+        print (f" {cmd:20} - {get_command(cmd).get_synopsis()}")
     print("Enter 'pyuftp <command> -h' for help on a particular command.")
 
 def run(args):
     _help = ["help", "-h", "--help"]
     if len(args)<1 or args[0] in _help:
         help()
         return
@@ -43,15 +47,15 @@
         show_version()
         return
 
     command = None
     cmd = args[0]
     for k in _commands:
         if k.startswith(cmd):
-            command = _commands[k]
+            command = get_command(k)
             break
     if command is None:
         raise ValueError(f"No such command: {cmd}")
     command.run(args[1:])
 
 def main():
     """
```

### Comparing `pyuftp-0.0.6/pyuftp/cp.py` & `pyuftp-1.0.2/pyuftp/cp.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,45 +1,54 @@
 """ Copy command class and helpers """
 
 import pyuftp.base, pyuftp.uftp, pyuftp.utils
-import os.path, pathlib, sys
-import threading
-import concurrent.futures
+import os, os.path, pathlib, sys, threading
+from concurrent.futures import ThreadPoolExecutor
     
 class Copy(pyuftp.base.CopyBase):
     
     def add_command_args(self):
         self.parser.prog = "pyuftp cp"
         self.parser.description = self.get_synopsis()
         self.parser.add_argument("source", nargs="+", help="Source(s)")
         self.parser.add_argument("target", help="Target")
         self.parser.add_argument("-r", "--recurse", required=False, action="store_true",
-                                 help="recurse into subdirectories, if applicable")
+                                 help="Recurse into subdirectories, if applicable")
         self.parser.add_argument("-a", "--archive", action="store_true", required=False,
                                  help="Tell server to interpret data as tar/zip stream and unpack it")
-        self.parser.add_argument("-n", "--number-of-threads", required=False, type=int, default=1,
-                                 help="Maximum number of parallel UFTP sessions to use")
+        self.parser.add_argument("-t", "--threads", required=False, type=int, default=1,
+                                 help="Maximum number of client threads / parallel UFTP sessions to use")
         self.parser.add_argument("-R", "--resume", required=False, action="store_true",
                                  help="Check existing target file(s) and try to resume")
-
+        self.parser.add_argument("-D", "--show-performance", required=False, action="store_true",
+                                 help="Show detailed transfer rates during the transfer")
+    
     def get_synopsis(self):
         return """Copy file(s)"""
 
     def run(self, args):
         super().run(args)
-        self.init_range()
         self.archive_mode = self.args.archive
-        self.number_of_threads = self.args.number_of_threads
-        self.verbose(f"Number of threads = {self.number_of_threads}")
+        if self.archive_mode:
+            self.verbose("Archive mode = True")
         self.resume = self.args.resume and not self.args.target=="-"
-        self.verbose(f"Resume mode = {self.resume}")
+        if self.resume:
+            self.verbose("Resume mode = True")
+        self.show_performance = self.args.show_performance
+        if self.show_performance:
+            self.verbose("Performance display = True")
+            self.performance_display = pyuftp.uftp.PerformanceDisplay(self.number_of_threads)
+        else:
+            self.performance_display = None
+        self.number_of_threads = self.args.threads
         if self.number_of_threads>1:
+            self.verbose(f"Number of threads = {self.number_of_threads}")
             self.thread_storage = threading.local()
-            self.executor = concurrent.futures.ThreadPoolExecutor(max_workers=self.number_of_threads,
-                                                                  thread_name_prefix="Thread")
+            self.executor = ThreadPoolExecutor(max_workers=self.number_of_threads,
+                                                thread_name_prefix="Thread")
         endpoint, _, _ = self.parse_url(self.args.target)
         for s in self.args.source:
             self.verbose(f"Copy {s} --> {self.args.target}")
             if not endpoint:
                 self.do_download(s, self.args.target)
             else:
                 self.do_upload(s, self.args.target)
@@ -63,17 +72,20 @@
         endpoint, base_dir, file_name  = self.parse_url(remote)
         if (file_name is None or len(file_name)==0) and not self.args.recurse:
             print(f"pyuftp cp: --recurse not specified, omitting directory '{remote}'")
             return
         host, port, onetime_pwd = self.authenticate(endpoint, base_dir)
         self.verbose(f"Connecting to UFTPD {host}:{port}")
         with pyuftp.uftp.open(host, port, onetime_pwd) as uftp:
+            uftp.key = self.key
+            uftp.algo = self.algo
+            uftp.number_of_streams = self.number_of_streams
+            uftp.compress = self.compress
             for (item, remote_size) in pyuftp.utils.crawl_remote(uftp, ".", file_name, recurse=self.args.recurse):
-                offset, length = self._get_range()
-                rw = self.range_read_write
+                offset, length, rw = self._get_range()
                 if os.path.isdir(local):
                     target = os.path.normpath(local+"/"+item)
                     local_dir = os.path.dirname(target)
                     if len(local_dir)>0 and not os.path.isdir(local_dir):
                         os.makedirs(local_dir, mode=0o755, exist_ok=True)
                 else:
                     target = local
@@ -83,35 +95,48 @@
                         if size==remote_size:
                             self.verbose(f"'{target}': skipping.")
                             continue
                         else:
                             self.verbose(f"'{target}': resuming at {size}.")
                             offset = size
                             length = remote_size - offset
+                else:
+                    exists, size = self.check_download_exists(target)
+                    if exists and not rw:
+                        try:
+                            with open(target, "r+b") as fl:
+                                fl.truncate(0)
+                                self.verbose(f"'{target}': truncating.")
+                        except OSError:
+                            pass
                 args = [endpoint, base_dir, item, offset, length, target, rw]
                 if self.number_of_threads==1:
+                    uftp.performance_display = self.performance_display
                     Worker(self, uftp=uftp).download(*args)
                 else:
-                    self.executor.submit(Worker(self, self.thread_storage).download, *args)
+                    self.executor.submit(Worker(self, self.thread_storage, None, self.performance_display).download, *args)
 
     def do_upload(self, local, remote):
         """ upload local source (which can specify wildcards) to a remote location """
         endpoint, base_dir, remote_file_name  = self.parse_url(remote)
         host, port, onetime_pwd = self.authenticate(endpoint, base_dir)
         self.verbose(f"Connecting to UFTPD {host}:{port}")
         with pyuftp.uftp.open(host, port, onetime_pwd) as uftp:
+            uftp.key = self.key
+            uftp.algo = self.algo
+            uftp.number_of_streams = self.number_of_streams
+            uftp.compress = self.compress
             if self.archive_mode:
                 uftp.set_archive_mode()
             if "-"==local:
-                offset, length = self._get_range()
+                offset, length, rw = self._get_range()
                 remote_offset = offset if self.range_read_write else 0
-                writer = uftp.get_write_socket(remote_file_name, offset, length).makefile("wb")
-                total, duration = uftp.copy_data(sys.stdin.buffer, writer, length)
-                self.log_usage(True, "stdin", remote_file_name, total, duration)
-                writer.close()
+                with uftp.get_writer(remote_file_name, remote_offset, length, rw) as writer:
+                    total, duration = uftp.copy_data(sys.stdin.buffer, writer, length)
+                    self.log_usage(True, "stdin", remote_file_name, total, duration)
                 uftp.finish_transfer()
             else:
                 local_base_dir = os.path.dirname(local)
                 if local_base_dir == "":
                     local_base_dir = "."
                 file_pattern = os.path.basename(local)
                 remote_is_directory = True
@@ -124,79 +149,86 @@
                     if remote_is_directory:
                         target = os.path.normpath(remote_file_name+"/"+rel_path)
                     else:
                         target = remote_file_name
                     if target.startswith("/"):
                         target = target[1:]
                     local_size = os.stat(item).st_size
-                    offset, length = self._get_range(local_size)
-                    rw = self.range_read_write
+                    offset, length, rw = self._get_range(local_size)
                     if self.resume:
                         exists, remote_size = self.check_upload_exists(uftp, target)
                         if exists:
                             if local_size==remote_size:
                                 self.verbose(f"'{target}': skipping.")
                                 continue
                             else:
                                 self.verbose(f"'{target}': resuming at {remote_size}.")
                                 offset = remote_size
                                 length = local_size - offset
                     args = [endpoint, base_dir, item, target, offset, length, rw]
                     if self.number_of_threads==1:
+                        uftp.performance_display = self.performance_display
                         Worker(self, uftp=uftp).upload(*args)
                     else:
-                        f = self.executor.submit(Worker(self, self.thread_storage).upload, *args)
+                        f = self.executor.submit(Worker(self, self.thread_storage, None, self.performance_display).upload, *args)
 
 class Worker():
-    """ performs uploads/downloads, suitable for running in a pool thread """
-    def __init__(self, base_command, thread_local=None, uftp=None):
+    """ performs uploads/downloads, suselfitable for running in a pool thread """
+    def __init__(self, base_command: Copy, thread_local=None, uftp: pyuftp.uftp.UFTP=None, performance_display=None):
         self.base = base_command
         self.thread_storage = thread_local
         self.uftp = uftp
+        self.performance_display = performance_display
 
     def setup(self, endpoint, base_dir):
         if self.thread_storage is not None:
             self.uftp = getattr(self.thread_storage, "uftp", None)
         if self.uftp is not None:
             return
         host, port, onetime_pwd = self.base.authenticate(endpoint, base_dir)
         self.base.verbose(f"[{threading.current_thread().name}] Connecting to UFTPD {host}:{port}")
-        self.uftp = pyuftp.uftp.UFTP()
+        self.uftp = pyuftp.uftp.UFTP(self.base.number_of_streams, self.base.key, self.base.algo, self.base.compress)
         self.uftp.open_session(host, port, onetime_pwd)
         if self.thread_storage is not None:
             self.thread_storage.uftp = self.uftp
+        self.uftp.performance_display = self.performance_display
 
     def download(self, endpoint, base_dir, item, offset, length, target, write_range=False):
         self.setup(endpoint, base_dir)
         source = os.path.basename(item)
-        reader = self.uftp.get_read_socket(source, offset, length).makefile("rb")
-        if "-"==target:
-            total, duration = self.uftp.copy_data(reader, sys.stdout.buffer, length)
-            target="stdout"
-        else:
-            pathlib.Path(target).touch()
-            with open(target, "r+b") as f:
-                if offset>0 and write_range:
-                    f.seek(offset)
-                total, duration = self.uftp.copy_data(reader, f, length)
+        with self.uftp.get_reader(source, offset, length) as (reader, _):
+            if "-"==target:
+                total, duration = self.uftp.copy_data(reader, sys.stdout.buffer, length)
+                target="stdout"
+            else:
+                pathlib.Path(target).touch()
+                with open(target, "r+b") as f:
+                    if offset>0 and write_range:
+                        f.seek(offset)
+                    elif not write_range:
+                        try:
+                            f.truncate(0)
+                        except OSError:
+                            # can happen if it is not a regular file, e.g. /dev/null
+                            pass
+                    total, duration = self.uftp.copy_data(reader, f, length)
         self.base.log_usage(False, item, target, total, duration)
         self.uftp.finish_transfer()
         return "OK"
 
     def upload(self, endpoint, base_dir, item, target, offset, length, write_range=False):
         self.setup(endpoint, base_dir)
         remote_offset = offset if write_range else 0
-        writer = self.uftp.get_write_socket(target, remote_offset, length).makefile("wb")
-        with open(item, "rb") as f:
-            if offset>0:
-                f.seek(offset)
-            total, duration = self.uftp.copy_data(f, writer, length)
-        self.base.log_usage(True, item, target, total, duration)
-        writer.close()
+        with self.uftp.get_writer(target, remote_offset, length, write_range) as writer:
+            with open(item, "rb") as f:
+                if offset>0:
+                    f.seek(offset)
+                total, duration = self.uftp.copy_data(f, writer, length)
         self.uftp.finish_transfer()
+        self.base.log_usage(True, item, target, total, duration)
         return "OK"
 
 class RemoteCopy(pyuftp.base.CopyBase):
 
     def add_command_args(self):
         self.parser.prog = "pyuftp rcp"
         self.parser.description = self.get_synopsis()
@@ -225,15 +257,14 @@
                 s_endpoint, s_base_dir, s_filename = self.parse_url(s)
                 s_host, s_port, s_password = self.authenticate(s_endpoint, s_base_dir)
                 s_server = f"{s_host}:{s_port}"
             else:
                 s_server = self.args.server
                 s_password = self.args.one_time_password
                 s_filename = s
-            offset, length = self._get_range()
+            offset, length, rw = self._get_range()
             t_endpoint, t_base_dir, t_filename  = self.parse_url(self.args.target)
             t_host, t_port, t_password = self.authenticate(t_endpoint, t_base_dir)
             with pyuftp.uftp.open(t_host, t_port, t_password) as uftp:
-                if offset>0 or length>-1:
-                    uftp._send_range(offset, length)
+                uftp.set_remote_write_range(offset, length, rw)
                 reply = uftp.receive_file(t_filename, s_filename, s_server, s_password)
-                self.verbose(reply)
+                self.verbose(reply)
```

### Comparing `pyuftp-0.0.6/pyuftp/share.py` & `pyuftp-1.0.2/pyuftp/share.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,25 +7,25 @@
 
     def add_command_args(self):
         self.parser.prog = "pyuftp share"
         self.parser.description = self.get_synopsis()
         self.parser.add_argument("-s", "--server", default=os.getenv("UFTP_SHARE_URL"),
                                  help="URL to the share service e.g. <https://host:port/SITE/rest/share/NAME")
         self.parser.add_argument("-a", "--access",
-                                 help="allow access for the specified user")
+                                 help="Allow access for the specified user")
         self.parser.add_argument("-l", "--list", action="store_true",
-                            help="list shares")
+                            help="List shares")
         self.parser.add_argument("-w", "--write", action="store_true",
-                            help="allow write access to the shared path")
+                            help="Allow write access to the shared path")
         self.parser.add_argument("-d", "--delete", action="store_true",
-                            help="delete access to the shared path")
+                            help="Delete access to the shared path")
         self.parser.add_argument("-1", "--one-time", action="store_true",
-                            help="allow only one access to a share (one-time share)")
+                            help="Allow only one access to a share (one-time share)")
         self.parser.add_argument("-L", "--lifetime", type=int, default=0,
-                            help="limit lifetime of share (in seconds)")
+                            help="Limit lifetime of share (in seconds)")
         self.parser.add_argument("path", help="shared path", nargs="?", default=None)
 
     def get_synopsis(self):
         return """Create, update and delete shares"""
 
     def run(self, args):
         super().run(args)
@@ -61,13 +61,13 @@
         _path = self.args.path
         _onetime = self.args.one_time
         _lifetime = self.args.lifetime
         req = {"path": _path, "user": _target, "access": _access}
         if _onetime:
             req['onetime']="true"
         if _lifetime>0:
-            req['lifetime']=str(lifetime)
+            req['lifetime']=str(_lifetime)
         location = pyuftp.authenticate.post_json(self.server, self.credential, req, as_json=False)
         if not _delete:
             _info = pyuftp.authenticate.get_json(location, self.credential)
             self.verbose(json.dumps(_info, indent=2))
             print("Shared to %s" % _info['share']['http'])
```

### Comparing `pyuftp-0.0.6/versioneer.py` & `pyuftp-1.0.2/versioneer.py`

 * *Files identical despite different names*

