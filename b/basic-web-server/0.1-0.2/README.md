# Comparing `tmp/basic_web_server-0.1.tar.gz` & `tmp/basic_web_server-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basic_web_server-0.1.tar", last modified: Tue May 14 00:40:39 2024, max compression
+gzip compressed data, was "basic_web_server-0.2.tar", last modified: Tue May 14 01:39:15 2024, max compression
```

## Comparing `basic_web_server-0.1.tar` & `basic_web_server-0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 00:40:39.841579 basic_web_server-0.1/
--rw-rw-rw-   0        0        0      228 2024-05-14 00:40:39.839581 basic_web_server-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      856 2024-05-13 23:51:18.000000 basic_web_server-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-14 00:40:39.838579 basic_web_server-0.1/basic_web_server.egg-info/
--rw-rw-rw-   0        0        0      228 2024-05-14 00:40:39.000000 basic_web_server-0.1/basic_web_server.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2024-05-14 00:40:39.000000 basic_web_server-0.1/basic_web_server.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 00:40:39.000000 basic_web_server-0.1/basic_web_server.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-14 00:40:39.000000 basic_web_server-0.1/basic_web_server.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4736 2024-05-13 23:19:59.000000 basic_web_server-0.1/basic_webserver.py
--rw-rw-rw-   0        0        0       42 2024-05-14 00:40:39.842582 basic_web_server-0.1/setup.cfg
--rw-rw-rw-   0        0        0      365 2024-05-14 00:40:31.000000 basic_web_server-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 01:39:15.752792 basic_web_server-0.2/
+-rw-rw-rw-   0        0        0      228 2024-05-14 01:39:15.739240 basic_web_server-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      856 2024-05-13 23:51:18.000000 basic_web_server-0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 01:39:15.737237 basic_web_server-0.2/basic_web_server.egg-info/
+-rw-rw-rw-   0        0        0      228 2024-05-14 01:39:15.000000 basic_web_server-0.2/basic_web_server.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2024-05-14 01:39:15.000000 basic_web_server-0.2/basic_web_server.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 01:39:15.000000 basic_web_server-0.2/basic_web_server.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-14 01:39:15.000000 basic_web_server-0.2/basic_web_server.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4855 2024-05-14 01:39:10.000000 basic_web_server-0.2/basic_webserver.py
+-rw-rw-rw-   0        0        0       42 2024-05-14 01:39:15.753788 basic_web_server-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      365 2024-05-14 01:38:52.000000 basic_web_server-0.2/setup.py
```

### Comparing `basic_web_server-0.1/README.md` & `basic_web_server-0.2/README.md`

 * *Files identical despite different names*

### Comparing `basic_web_server-0.1/basic_webserver.py` & `basic_web_server-0.2/basic_webserver.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,20 +72,23 @@
         for line in lines[1:]:
             if b':' in line:
                 header, value = line.decode('utf-8').split(': ', 1)
                 headers[header] = value
             else:
                 pass
 
+        client_ip = headers.get('X-Forwarded-For', '').split(',')[0].strip() or client_address[0]
+
         body = None
 
         if lines[-1]:
             body = lines[-1].decode('utf-8')
 
-        return Request(method, path, headers, body, client_address)
+        return Request(method, path, headers, body, (client_ip, client_address[1]))
+
 
     def find_handler(self, request_path):
         handler = self.router.get_route(request_path)
         if handler is None:
             return self.default_handler, {}
         return handler, {}
```

