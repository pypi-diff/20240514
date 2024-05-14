# Comparing `tmp/mpd_now_playable-1.1.0.tar.gz` & `tmp/mpd_now_playable-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpd_now_playable-1.1.0.tar", last modified: Tue May 14 03:48:19 2024, max compression
+gzip compressed data, was "mpd_now_playable-1.1.1.tar", last modified: Tue May 14 04:08:22 2024, max compression
```

## Comparing `mpd_now_playable-1.1.0.tar` & `mpd_now_playable-1.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     3230 2024-03-07 04:52:56.592214 mpd_now_playable-1.1.0/README.md
--rw-r--r--   0        0        0     1914 2024-05-14 03:48:19.943338 mpd_now_playable-1.1.0/pyproject.toml
--rw-r--r--   0        0        0       87 2024-03-07 04:52:35.897735 mpd_now_playable-1.1.0/src/corefoundationasyncio/__init__.py
--rw-r--r--   0        0        0     7343 2024-03-07 04:52:35.897945 mpd_now_playable-1.1.0/src/corefoundationasyncio/eventloop.py
--rw-r--r--   0        0        0        0 2024-03-07 04:52:35.898117 mpd_now_playable-1.1.0/src/mpd_now_playable/__init__.py
--rw-r--r--   0        0        0      483 2024-03-07 04:52:35.898278 mpd_now_playable-1.1.0/src/mpd_now_playable/async_tools.py
--rw-r--r--   0        0        0     1405 2024-05-14 03:07:09.976223 mpd_now_playable-1.1.0/src/mpd_now_playable/cache.py
--rw-r--r--   0        0        0      869 2024-05-09 02:51:47.711237 mpd_now_playable-1.1.0/src/mpd_now_playable/cli.py
--rw-r--r--   0        0        0        0 2024-03-07 04:52:35.898623 mpd_now_playable-1.1.0/src/mpd_now_playable/cocoa/__init__.py
--rw-r--r--   0        0        0     6961 2024-05-14 03:11:01.951769 mpd_now_playable-1.1.0/src/mpd_now_playable/cocoa/now_playing.py
--rw-r--r--   0        0        0     1657 2024-05-13 05:11:01.883611 mpd_now_playable-1.1.0/src/mpd_now_playable/cocoa/persistent_id.py
--rw-r--r--   0        0        0        0 2024-03-07 04:52:35.899242 mpd_now_playable-1.1.0/src/mpd_now_playable/mpd/__init__.py
--rw-r--r--   0        0        0     1698 2024-05-14 03:07:23.846226 mpd_now_playable-1.1.0/src/mpd_now_playable/mpd/artwork_cache.py
--rw-r--r--   0        0        0     4155 2024-05-13 05:09:56.754721 mpd_now_playable-1.1.0/src/mpd_now_playable/mpd/listener.py
--rw-r--r--   0        0        0    27419 2024-03-07 04:52:35.899776 mpd_now_playable-1.1.0/src/mpd_now_playable/mpd/logo.svg
--rw-r--r--   0        0        0     2536 2024-03-07 04:52:35.900036 mpd_now_playable-1.1.0/src/mpd_now_playable/mpd/types.py
--rw-r--r--   0        0        0      433 2024-03-07 04:52:35.900181 mpd_now_playable-1.1.0/src/mpd_now_playable/player.py
--rw-r--r--   0        0        0        0 2024-03-07 04:52:35.900247 mpd_now_playable-1.1.0/src/mpd_now_playable/py.typed
--rw-r--r--   0        0        0      735 2024-05-13 05:09:17.349547 mpd_now_playable-1.1.0/src/mpd_now_playable/song.py
--rw-r--r--   0        0        0      234 2024-03-07 04:52:35.900786 mpd_now_playable-1.1.0/src/mpd_now_playable/type_tools.py
--rw-r--r--   0        0        0     4352 1970-01-01 00:00:00.000000 mpd_now_playable-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     4223 2024-05-14 04:04:04.537115 mpd_now_playable-1.1.1/README.md
+-rw-r--r--   0        0        0     1914 2024-05-14 04:08:22.717033 mpd_now_playable-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0       87 2024-03-07 04:52:35.897735 mpd_now_playable-1.1.1/src/corefoundationasyncio/__init__.py
+-rw-r--r--   0        0        0     7343 2024-03-07 04:52:35.897945 mpd_now_playable-1.1.1/src/corefoundationasyncio/eventloop.py
+-rw-r--r--   0        0        0        0 2024-03-07 04:52:35.898117 mpd_now_playable-1.1.1/src/mpd_now_playable/__init__.py
+-rw-r--r--   0        0        0      483 2024-03-07 04:52:35.898278 mpd_now_playable-1.1.1/src/mpd_now_playable/async_tools.py
+-rw-r--r--   0        0        0     1384 2024-05-14 04:06:47.011108 mpd_now_playable-1.1.1/src/mpd_now_playable/cache.py
+-rw-r--r--   0        0        0      869 2024-05-09 02:51:47.711237 mpd_now_playable-1.1.1/src/mpd_now_playable/cli.py
+-rw-r--r--   0        0        0        0 2024-03-07 04:52:35.898623 mpd_now_playable-1.1.1/src/mpd_now_playable/cocoa/__init__.py
+-rw-r--r--   0        0        0     6961 2024-05-14 03:11:01.951769 mpd_now_playable-1.1.1/src/mpd_now_playable/cocoa/now_playing.py
+-rw-r--r--   0        0        0     1657 2024-05-13 05:11:01.883611 mpd_now_playable-1.1.1/src/mpd_now_playable/cocoa/persistent_id.py
+-rw-r--r--   0        0        0        0 2024-03-07 04:52:35.899242 mpd_now_playable-1.1.1/src/mpd_now_playable/mpd/__init__.py
+-rw-r--r--   0        0        0     1698 2024-05-14 03:07:23.846226 mpd_now_playable-1.1.1/src/mpd_now_playable/mpd/artwork_cache.py
+-rw-r--r--   0        0        0     4155 2024-05-13 05:09:56.754721 mpd_now_playable-1.1.1/src/mpd_now_playable/mpd/listener.py
+-rw-r--r--   0        0        0    27419 2024-03-07 04:52:35.899776 mpd_now_playable-1.1.1/src/mpd_now_playable/mpd/logo.svg
+-rw-r--r--   0        0        0     2536 2024-03-07 04:52:35.900036 mpd_now_playable-1.1.1/src/mpd_now_playable/mpd/types.py
+-rw-r--r--   0        0        0      433 2024-03-07 04:52:35.900181 mpd_now_playable-1.1.1/src/mpd_now_playable/player.py
+-rw-r--r--   0        0        0        0 2024-03-07 04:52:35.900247 mpd_now_playable-1.1.1/src/mpd_now_playable/py.typed
+-rw-r--r--   0        0        0      735 2024-05-13 05:09:17.349547 mpd_now_playable-1.1.1/src/mpd_now_playable/song.py
+-rw-r--r--   0        0        0      234 2024-03-07 04:52:35.900786 mpd_now_playable-1.1.1/src/mpd_now_playable/type_tools.py
+-rw-r--r--   0        0        0     5345 1970-01-01 00:00:00.000000 mpd_now_playable-1.1.1/PKG-INFO
```

### Comparing `mpd_now_playable-1.1.0/README.md` & `mpd_now_playable-1.1.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -4,38 +4,49 @@
 This enables your keyboard's standard media keys to control MPD, as well as more esoteric music control methods like the buttons on your Bluetooth headphones.
 
 ## Installation
 
 The recommended way to install mpd-now-playable and its dependencies is with [pipx](https://pypa.github.io/pipx/):
 ```shell
 pipx install mpd-now-playable
+# or, if you'd like to use a separate cache service, one of these:
+pipx install mpd-now-playable[redis,msgpack]
+pipx install mpd-now-playable[memcached,msgpack]
 ```
 
 Once pipx is done, the `mpd-now-playable` script should be available on your `$PATH` and ready to use.
 
 Most likely, you'll want mpd-now-playable to stay running in the background as a launchd service. [Here's the service plist I use](https://git.00dani.me/00dani/mpd-now-playable/src/branch/main/me.00dani.mpd-now-playable.plist), but it's hardcoded to my `$HOME` so you'll want to customise it.
 
 ## Configuration
 
 You may not need any configuration! If you've got a relatively normal MPD setup on your local machine, mpd-now-playable ought to just work out of the box, as it uses sensible defaults. If you need to control a remote MPD server, or your MPD clients use a password, though, you'll need configuration for that use case.
 
-Currently, mpd-now-playable can only be configured through environment variables. Command-line arguments are intentionally not supported, since your MPD password is among the supported settings and command-line arguments are not a secure way to pass secrets such as passwords into commands. Reading configuration from a file is secure, so mpd-now-playable may support a config file in future.
+Currently, mpd-now-playable can only be configured through environment variables. Command-line arguments are intentionally not supported, since your MPD password is among the supported settings and command-line arguments are not a secure way to pass secrets such as passwords into commands. Reading configuration from a file is secure, provided the file itself is kept secure, so mpd-now-playable may support a config file in future.
 
 The following environment variables are read. The `MPD_HOST` and `MPD_PORT` variables are supported in the same way `mpc` uses them, but you can alternatively provide your password as a separate `MPD_PASSWORD` variable if you wish.
 
 - `MPD_HOST` - defaults to `localhost`, which should be fine for most users. If you want to control a remote MPD server, though, you can.
 - `MPD_PORT` - defaults to 6600, which will almost always be the correct port to use.
 - `MPD_PASSWORD` - has no default. Set this only if your MPD server expects a password. You can also provide a password by setting `MPD_HOST=password@host`, if you want to be consistent with how `mpc` works.
 
+Additionally, mpd-now-playable caches your album artwork, by default simply in memory. It may be configured to use an external cache, and currently supports Redis and Memcached for this purpose. To use one of these, set the environment variable `MPD_NOW_PLAYABLE_CACHE` to an appropriate URL for your cache service:
+
+- For Redis, use something like `redis://localhost:6379/0`.
+- For Memcached, use something like `memcached://localhost:11211`.
+
+You may provide a `namespace` query parameter to prefix cache keys if you wish, as well as a `password` query parameter if your service requires a password to access. As with your other environment variables, keep your cache password secure.
+
 One simple secure way to set your environment variables is with a small wrapper script like this:
 ```shell
 #!/bin/sh
 export MPD_HOSTNAME=my.cool.mpd.host
 export MPD_PORT=6700
 export MPD_PASSWORD=swordfish
+export MPD_NOW_PLAYABLE_CACHE='redis://localhost:6379/0?namespace=mpd-now-playable&password=fishsword'
 exec mpd-now-playable
 ```
 Make sure this wrapper script is only readable by you, with something like `chmod 700`!
 
 ## Limitations
 
 mpd-now-playable is currently *very* specific to MacOS. I did my best to keep the generic MPD and extremely Apple parts separate, but it definitely won't work with MPRIS2 or the Windows system media feature.
```

### Comparing `mpd_now_playable-1.1.0/pyproject.toml` & `mpd_now_playable-1.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 classifiers = [
     "Environment :: No Input/Output (Daemon)",
     "License :: OSI Approved :: MIT License",
     "Operating System :: MacOS :: MacOS X",
     "Programming Language :: Python :: 3.12",
     "Topic :: Multimedia :: Sound/Audio :: Players",
 ]
-version = "1.1.0"
+version = "1.1.1"
 
 [project.license]
 text = "MIT"
 
 [project.optional-dependencies]
 redis = [
     "aiocache[redis]",
```

### Comparing `mpd_now_playable-1.1.0/src/corefoundationasyncio/eventloop.py` & `mpd_now_playable-1.1.1/src/corefoundationasyncio/eventloop.py`

 * *Files identical despite different names*

### Comparing `mpd_now_playable-1.1.0/src/mpd_now_playable/cache.py` & `mpd_now_playable-1.1.1/src/mpd_now_playable/cache.py`

 * *Files 9% similar despite different names*

```diff
@@ -43,13 +43,12 @@
 
 	if parsed_url.port:
 		kwargs["port"] = parsed_url.port
 
 	if parsed_url.password:
 		kwargs["password"] = parsed_url.password
 
-	namespace = ":".join(s for s in [kwargs.get("namespace"), namespace] if s)
-	del kwargs["namespace"]
+	namespace = ":".join(s for s in [kwargs.pop("namespace", ""), namespace] if s)
 
 	serializer = OrmsgpackSerializer if HAS_ORMSGPACK else PickleSerializer
 
 	return Cache(backend, serializer=serializer(), namespace=namespace, **kwargs)
```

### Comparing `mpd_now_playable-1.1.0/src/mpd_now_playable/cli.py` & `mpd_now_playable-1.1.1/src/mpd_now_playable/cli.py`

 * *Files identical despite different names*

### Comparing `mpd_now_playable-1.1.0/src/mpd_now_playable/cocoa/now_playing.py` & `mpd_now_playable-1.1.1/src/mpd_now_playable/cocoa/now_playing.py`

 * *Files identical despite different names*

### Comparing `mpd_now_playable-1.1.0/src/mpd_now_playable/cocoa/persistent_id.py` & `mpd_now_playable-1.1.1/src/mpd_now_playable/cocoa/persistent_id.py`

 * *Files identical despite different names*

### Comparing `mpd_now_playable-1.1.0/src/mpd_now_playable/mpd/artwork_cache.py` & `mpd_now_playable-1.1.1/src/mpd_now_playable/mpd/artwork_cache.py`

 * *Files identical despite different names*

### Comparing `mpd_now_playable-1.1.0/src/mpd_now_playable/mpd/listener.py` & `mpd_now_playable-1.1.1/src/mpd_now_playable/mpd/listener.py`

 * *Files identical despite different names*

### Comparing `mpd_now_playable-1.1.0/src/mpd_now_playable/mpd/logo.svg` & `mpd_now_playable-1.1.1/src/mpd_now_playable/mpd/logo.svg`

 * *Files identical despite different names*

### Comparing `mpd_now_playable-1.1.0/src/mpd_now_playable/mpd/types.py` & `mpd_now_playable-1.1.1/src/mpd_now_playable/mpd/types.py`

 * *Files identical despite different names*

### Comparing `mpd_now_playable-1.1.0/src/mpd_now_playable/song.py` & `mpd_now_playable-1.1.1/src/mpd_now_playable/song.py`

 * *Files identical despite different names*

### Comparing `mpd_now_playable-1.1.0/PKG-INFO` & `mpd_now_playable-1.1.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpd-now-playable
-Version: 1.1.0
+Version: 1.1.1
 Summary: Expose your MPD server as a 'now playable' app on MacOS
 Author-Email: Danielle McLean <dani@00dani.me>
 License: MIT
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3.12
@@ -32,38 +32,49 @@
 This enables your keyboard's standard media keys to control MPD, as well as more esoteric music control methods like the buttons on your Bluetooth headphones.
 
 ## Installation
 
 The recommended way to install mpd-now-playable and its dependencies is with [pipx](https://pypa.github.io/pipx/):
 ```shell
 pipx install mpd-now-playable
+# or, if you'd like to use a separate cache service, one of these:
+pipx install mpd-now-playable[redis,msgpack]
+pipx install mpd-now-playable[memcached,msgpack]
 ```
 
 Once pipx is done, the `mpd-now-playable` script should be available on your `$PATH` and ready to use.
 
 Most likely, you'll want mpd-now-playable to stay running in the background as a launchd service. [Here's the service plist I use](https://git.00dani.me/00dani/mpd-now-playable/src/branch/main/me.00dani.mpd-now-playable.plist), but it's hardcoded to my `$HOME` so you'll want to customise it.
 
 ## Configuration
 
 You may not need any configuration! If you've got a relatively normal MPD setup on your local machine, mpd-now-playable ought to just work out of the box, as it uses sensible defaults. If you need to control a remote MPD server, or your MPD clients use a password, though, you'll need configuration for that use case.
 
-Currently, mpd-now-playable can only be configured through environment variables. Command-line arguments are intentionally not supported, since your MPD password is among the supported settings and command-line arguments are not a secure way to pass secrets such as passwords into commands. Reading configuration from a file is secure, so mpd-now-playable may support a config file in future.
+Currently, mpd-now-playable can only be configured through environment variables. Command-line arguments are intentionally not supported, since your MPD password is among the supported settings and command-line arguments are not a secure way to pass secrets such as passwords into commands. Reading configuration from a file is secure, provided the file itself is kept secure, so mpd-now-playable may support a config file in future.
 
 The following environment variables are read. The `MPD_HOST` and `MPD_PORT` variables are supported in the same way `mpc` uses them, but you can alternatively provide your password as a separate `MPD_PASSWORD` variable if you wish.
 
 - `MPD_HOST` - defaults to `localhost`, which should be fine for most users. If you want to control a remote MPD server, though, you can.
 - `MPD_PORT` - defaults to 6600, which will almost always be the correct port to use.
 - `MPD_PASSWORD` - has no default. Set this only if your MPD server expects a password. You can also provide a password by setting `MPD_HOST=password@host`, if you want to be consistent with how `mpc` works.
 
+Additionally, mpd-now-playable caches your album artwork, by default simply in memory. It may be configured to use an external cache, and currently supports Redis and Memcached for this purpose. To use one of these, set the environment variable `MPD_NOW_PLAYABLE_CACHE` to an appropriate URL for your cache service:
+
+- For Redis, use something like `redis://localhost:6379/0`.
+- For Memcached, use something like `memcached://localhost:11211`.
+
+You may provide a `namespace` query parameter to prefix cache keys if you wish, as well as a `password` query parameter if your service requires a password to access. As with your other environment variables, keep your cache password secure.
+
 One simple secure way to set your environment variables is with a small wrapper script like this:
 ```shell
 #!/bin/sh
 export MPD_HOSTNAME=my.cool.mpd.host
 export MPD_PORT=6700
 export MPD_PASSWORD=swordfish
+export MPD_NOW_PLAYABLE_CACHE='redis://localhost:6379/0?namespace=mpd-now-playable&password=fishsword'
 exec mpd-now-playable
 ```
 Make sure this wrapper script is only readable by you, with something like `chmod 700`!
 
 ## Limitations
 
 mpd-now-playable is currently *very* specific to MacOS. I did my best to keep the generic MPD and extremely Apple parts separate, but it definitely won't work with MPRIS2 or the Windows system media feature.
```

