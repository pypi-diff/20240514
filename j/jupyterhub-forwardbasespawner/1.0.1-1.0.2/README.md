# Comparing `tmp/jupyterhub_forwardbasespawner-1.0.1.tar.gz` & `tmp/jupyterhub_forwardbasespawner-1.0.2.tar.gz`

## Comparing `jupyterhub_forwardbasespawner-1.0.1.tar` & `jupyterhub_forwardbasespawner-1.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.1/.gitlab-ci.yml
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.1/.readthedocs.yaml
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.1/CHANGELOG.md
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.1/release_notes.md
--rw-r--r--   0        0        0   120884 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.1/docs/Doxyfile
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.1/docs/Makefile
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.1/docs/apiendpoints.md
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.1/docs/changelog.md
--rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.1/docs/conf.py
--rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.1/docs/index.md
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.1/docs/make.bat
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.1/docs/requirements.txt
--rw-r--r--   0        0        0    17685 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.1/docs/_static/rest-api.yml
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.1/docs/spawners/forwardbasespawner.md
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.1/forwardbasespawner/__init__.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.1/forwardbasespawner/_version.py
--rw-r--r--   0        0        0     5806 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.1/forwardbasespawner/api_events.py
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.1/forwardbasespawner/api_list_servers.py
--rw-r--r--   0        0        0     3741 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.1/forwardbasespawner/api_setup_tunnel.py
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.1/forwardbasespawner/api_sshnode_restarted.py
--rw-r--r--   0        0        0    64098 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.1/forwardbasespawner/forward.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.1/forwardbasespawner/utils.py
--rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.1/.gitignore
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.1/LICENSE
--rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.1/README.md
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     4603 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.2/.gitlab-ci.yml
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.2/.readthedocs.yaml
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.2/CHANGELOG.md
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.2/release_notes.md
+-rw-r--r--   0        0        0   120884 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.2/docs/Doxyfile
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.2/docs/Makefile
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.2/docs/apiendpoints.md
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.2/docs/changelog.md
+-rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.2/docs/conf.py
+-rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.2/docs/index.md
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.2/docs/make.bat
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.2/docs/requirements.txt
+-rw-r--r--   0        0        0    17685 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.2/docs/_static/rest-api.yml
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.2/docs/spawners/forwardbasespawner.md
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.2/forwardbasespawner/__init__.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.2/forwardbasespawner/_version.py
+-rw-r--r--   0        0        0     5806 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.2/forwardbasespawner/api_events.py
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.2/forwardbasespawner/api_list_servers.py
+-rw-r--r--   0        0        0     3741 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.2/forwardbasespawner/api_setup_tunnel.py
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.2/forwardbasespawner/api_sshnode_restarted.py
+-rw-r--r--   0        0        0    64124 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.2/forwardbasespawner/forward.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.2/forwardbasespawner/utils.py
+-rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.2/LICENSE
+-rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.2/README.md
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4603 2020-02-02 00:00:00.000000 jupyterhub_forwardbasespawner-1.0.2/PKG-INFO
```

### Comparing `jupyterhub_forwardbasespawner-1.0.1/.gitlab-ci.yml` & `jupyterhub_forwardbasespawner-1.0.2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `jupyterhub_forwardbasespawner-1.0.1/docs/Doxyfile` & `jupyterhub_forwardbasespawner-1.0.2/docs/Doxyfile`

 * *Files identical despite different names*

### Comparing `jupyterhub_forwardbasespawner-1.0.1/docs/Makefile` & `jupyterhub_forwardbasespawner-1.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jupyterhub_forwardbasespawner-1.0.1/docs/apiendpoints.md` & `jupyterhub_forwardbasespawner-1.0.2/docs/apiendpoints.md`

 * *Files identical despite different names*

### Comparing `jupyterhub_forwardbasespawner-1.0.1/docs/conf.py` & `jupyterhub_forwardbasespawner-1.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jupyterhub_forwardbasespawner-1.0.1/docs/index.md` & `jupyterhub_forwardbasespawner-1.0.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `jupyterhub_forwardbasespawner-1.0.1/docs/make.bat` & `jupyterhub_forwardbasespawner-1.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jupyterhub_forwardbasespawner-1.0.1/docs/_static/rest-api.yml` & `jupyterhub_forwardbasespawner-1.0.2/docs/_static/rest-api.yml`

 * *Files identical despite different names*

### Comparing `jupyterhub_forwardbasespawner-1.0.1/docs/spawners/forwardbasespawner.md` & `jupyterhub_forwardbasespawner-1.0.2/docs/spawners/forwardbasespawner.md`

 * *Files identical despite different names*

### Comparing `jupyterhub_forwardbasespawner-1.0.1/forwardbasespawner/api_events.py` & `jupyterhub_forwardbasespawner-1.0.2/forwardbasespawner/api_events.py`

 * *Files identical despite different names*

### Comparing `jupyterhub_forwardbasespawner-1.0.1/forwardbasespawner/api_list_servers.py` & `jupyterhub_forwardbasespawner-1.0.2/forwardbasespawner/api_list_servers.py`

 * *Files identical despite different names*

### Comparing `jupyterhub_forwardbasespawner-1.0.1/forwardbasespawner/api_setup_tunnel.py` & `jupyterhub_forwardbasespawner-1.0.2/forwardbasespawner/api_setup_tunnel.py`

 * *Files identical despite different names*

### Comparing `jupyterhub_forwardbasespawner-1.0.1/forwardbasespawner/api_sshnode_restarted.py` & `jupyterhub_forwardbasespawner-1.0.2/forwardbasespawner/api_sshnode_restarted.py`

 * *Files identical despite different names*

### Comparing `jupyterhub_forwardbasespawner-1.0.1/forwardbasespawner/forward.py` & `jupyterhub_forwardbasespawner-1.0.2/forwardbasespawner/forward.py`

 * *Files 0% similar despite different names*

```diff
@@ -1419,15 +1419,15 @@
                     name=self.svc_name, namespace=self.namespace
                 )
                 v1.create_namespaced_service(
                     body=service_manifest, namespace=self.namespace
                 )
             else:
                 raise e
-        return self.svc_name, self.port
+        return f"{self.svc_name}.{self.namespace}.svc", self.port
 
     async def ssh_default_svc_remove(self):
         """Remove Kubernetes Service
         Used parameters: self.svc_name and self.namespace
 
         Returns:
           None
```

### Comparing `jupyterhub_forwardbasespawner-1.0.1/.gitignore` & `jupyterhub_forwardbasespawner-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterhub_forwardbasespawner-1.0.1/LICENSE` & `jupyterhub_forwardbasespawner-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterhub_forwardbasespawner-1.0.1/README.md` & `jupyterhub_forwardbasespawner-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `jupyterhub_forwardbasespawner-1.0.1/pyproject.toml` & `jupyterhub_forwardbasespawner-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 profile = "black"
 
 [tool.tbump]
 # Uncomment this if your project is hosted on GitHub:
 github_url = "https://github.com/kreuzert/jupyterhub-forwardbasespawner"
 
 [tool.tbump.version]
-current = "1.0.1"
+current = "1.0.2"
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
   (?P<pre>((a|b|rc)\d+)|)
```

### Comparing `jupyterhub_forwardbasespawner-1.0.1/PKG-INFO` & `jupyterhub_forwardbasespawner-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jupyterhub-forwardbasespawner
-Version: 1.0.1
+Version: 1.0.2
 Summary: JupyterHub BaseSpawner class. Enables remote single-user server.
 Author-email: Tim Kreuzer <t.kreuzer@fz-juelich.de>, Alice Grosch <a.grosch@fz-juelich.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Forschungszentrum Juelich GmbH
         
         Redistribution and use in source and binary forms, with or without
```

