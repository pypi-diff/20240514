# Comparing `tmp/xnLinkFinder-6.0.tar.gz` & `tmp/xnlinkfinder-6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xnLinkFinder-6.0.tar", last modified: Mon Apr  1 19:54:25 2024, max compression
+gzip compressed data, was "xnlinkfinder-6.1.tar", last modified: Tue May 14 12:09:53 2024, max compression
```

## Comparing `xnLinkFinder-6.0.tar` & `xnlinkfinder-6.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-04-01 19:54:25.145756 xnLinkFinder-6.0/
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)     1068 2024-03-08 20:41:39.000000 xnLinkFinder-6.0/LICENSE
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)    45567 2024-04-01 19:54:25.135725 xnLinkFinder-6.0/PKG-INFO
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)    44932 2024-04-01 19:35:18.000000 xnLinkFinder-6.0/README.md
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)       38 2024-04-01 19:54:25.145756 xnLinkFinder-6.0/setup.cfg
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)     2374 2024-04-01 19:36:06.000000 xnLinkFinder-6.0/setup.py
-drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-04-01 19:54:24.742086 xnLinkFinder-6.0/xnLinkFinder/
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)       17 2024-04-01 19:35:42.000000 xnLinkFinder-6.0/xnLinkFinder/__init__.py
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)   188628 2024-04-01 19:42:18.000000 xnLinkFinder-6.0/xnLinkFinder/xnLinkFinder.py
-drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-04-01 19:54:25.123421 xnLinkFinder-6.0/xnLinkFinder.egg-info/
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)    45567 2024-04-01 19:54:24.000000 xnLinkFinder-6.0/xnLinkFinder.egg-info/PKG-INFO
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)      298 2024-04-01 19:54:24.000000 xnLinkFinder-6.0/xnLinkFinder.egg-info/SOURCES.txt
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)        1 2024-04-01 19:54:24.000000 xnLinkFinder-6.0/xnLinkFinder.egg-info/dependency_links.txt
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)       64 2024-04-01 19:54:24.000000 xnLinkFinder-6.0/xnLinkFinder.egg-info/entry_points.txt
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)       89 2024-04-01 19:54:24.000000 xnLinkFinder-6.0/xnLinkFinder.egg-info/requires.txt
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)       13 2024-04-01 19:54:24.000000 xnLinkFinder-6.0/xnLinkFinder.egg-info/top_level.txt
+drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-05-14 12:09:53.440029 xnlinkfinder-6.1/
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)     1068 2024-05-02 21:06:21.000000 xnlinkfinder-6.1/LICENSE
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)    46211 2024-05-14 12:09:53.414963 xnlinkfinder-6.1/PKG-INFO
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)    45600 2024-05-14 12:06:49.000000 xnlinkfinder-6.1/README.md
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)       38 2024-05-14 12:09:53.443409 xnlinkfinder-6.1/setup.cfg
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)     2365 2024-05-02 21:06:21.000000 xnlinkfinder-6.1/setup.py
+drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-05-14 12:09:53.040545 xnlinkfinder-6.1/xnLinkFinder/
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)       17 2024-05-05 21:42:06.000000 xnlinkfinder-6.1/xnLinkFinder/__init__.py
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)   189784 2024-05-14 12:08:59.000000 xnlinkfinder-6.1/xnLinkFinder/xnLinkFinder.py
+drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-05-14 12:09:53.384744 xnlinkfinder-6.1/xnLinkFinder.egg-info/
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)    46211 2024-05-14 12:09:52.000000 xnlinkfinder-6.1/xnLinkFinder.egg-info/PKG-INFO
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)      298 2024-05-14 12:09:52.000000 xnlinkfinder-6.1/xnLinkFinder.egg-info/SOURCES.txt
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)        1 2024-05-14 12:09:52.000000 xnlinkfinder-6.1/xnLinkFinder.egg-info/dependency_links.txt
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)       64 2024-05-14 12:09:52.000000 xnlinkfinder-6.1/xnLinkFinder.egg-info/entry_points.txt
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)       80 2024-05-14 12:09:52.000000 xnlinkfinder-6.1/xnLinkFinder.egg-info/requires.txt
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)       13 2024-05-14 12:09:52.000000 xnlinkfinder-6.1/xnLinkFinder.egg-info/top_level.txt
```

### Comparing `xnLinkFinder-6.0/LICENSE` & `xnlinkfinder-6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xnLinkFinder-6.0/PKG-INFO` & `xnlinkfinder-6.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,10 @@
-Metadata-Version: 2.1
-Name: xnLinkFinder
-Version: 6.0
-Summary: A python script to find endpoints from a URL, a file of URLs, a directory of files, a Burp XML file or a ZAP ASCII message file. It also gets potential parameters and a target specific wordlist.
-Home-page: https://github.com/xnl-h4ck3r/xnlLinkFinder
-Author: @xnl-h4ck3r
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: argparse
-Requires-Dist: requests
-Requires-Dist: psutil
-Requires-Dist: pyyaml
-Requires-Dist: termcolor
-Requires-Dist: urlparse3
-Requires-Dist: beautifulsoup4
-Requires-Dist: lxml
-Requires-Dist: html5lib
-Requires-Dist: urllib3
-
 <center><img src="https://github.com/xnl-h4ck3r/xnLinkFinder/blob/main/xnLinkFinder/images/title.png"></center>
 
-## About - v6.0
+## About - v6.1
 
 This is a tool used to discover endpoints (and potential parameters) for a given target. It can find them by:
 
 - crawling a target (pass a domain/URL)
 - crawling multiple targets (pass a file of domains/URLs)
 - searching files in a given directory (pass a directory name)
 - get them from a **Burp** project (pass location of a Burp XML file)
@@ -86,14 +67,15 @@
 | -x          | --exclude                  | Additional Link exclusions (to the list in `config.yml`) in a comma separated list, e.g. `careers,forum`                                                                                                                                                                                                                                                                                                                                                                                           |
 | -orig       | --origin                   | Whether you want the origin of the link to be in the output. Displayed as `LINK-URL [ORIGIN-URL]` in the output (default: false)                                                                                                                                                                                                                                                                                                                                                                   |
 | -prefixed   |                            | Whether you want to see which links were prefixed in the output. Displays `(PREFIXED)` after link and origin in the output (default: false)                                                                                                                                                                                                                                                                                                                                                        |
 | -xrel       | --exclude-relative-links   | By default, if any links in the results start with `./` or `../`, they will be included. If this argument is used, these relative links will not be added.                                                                                                                                                                                                                                                                                                                                         |
 | -t          | --timeout †                | How many seconds to wait for the server to send data before giving up (default: 10 seconds)                                                                                                                                                                                                                                                                                                                                                                                                        |
 | -inc        | --include                  | Include input (`-i`) links in the output (default: false)                                                                                                                                                                                                                                                                                                                                                                                                                                          |
 | -u          | --user-agent †             | What User Agents to get links for, e.g. `-u desktop mobile`. Possible values are `desktop`, `mobile`, `set-top-boxes` and `game-console`. Also there are `mobile-apple`, `mobile-android` and `mobile-windows` that are subsets of `mobile` but can be used separately.                                                                                                                                                                                                                            |
+| -uc         | --user-agent-custom †      | A custom User Agent string to use for all requests. This will override the `-u`/`--user-agent` argument. This can be used when a program requires a specific User Agent header to identify you for example.                                                                                                                                                                                                                                                                                        |
 | -insecure   | †                          | Whether TLS certificate checks should be disabled when making requests (delfault: false)                                                                                                                                                                                                                                                                                                                                                                                                           |
 | -s429       | †                          | Stop when > 95 percent of responses return 429 Too Many Requests (default: false)                                                                                                                                                                                                                                                                                                                                                                                                                  |
 | -s403       | †                          | Stop when > 95 percent of responses return 403 Forbidden (default: false)                                                                                                                                                                                                                                                                                                                                                                                                                          |
 | -sTO        | †                          | Stop when > 95 percent of requests time out (default: false)                                                                                                                                                                                                                                                                                                                                                                                                                                       |
 | -sCE        | †                          | Stop when > 95 percent of requests have connection errors (default: false)                                                                                                                                                                                                                                                                                                                                                                                                                         |
 | -m          | --memory-threshold         | The memory threshold percentage. If the machines memory goes above the threshold, the program will be stopped and ended gracefully before running out of memory (default: 95)                                                                                                                                                                                                                                                                                                                      |
 | -mfs        | --max-file-size †          | The maximum file size (in bytes) of a file to be checked if -i is a directory. If the file size is over, it will be ignored (default: 500 MB). Setting to 0 means no files will be ignored, regardless of size.                                                                                                                                                                                                                                                                                    |
@@ -273,15 +255,15 @@
 - Pass cookies (`-c`), headers (`-H`) and regex (`-ra`) values within single quotes, e.g. `-ra '/api/v[0-9]\.[0-9]\*'`
 - Set the `-o` option to give a specific output file name for Links, rather than the default of `output.txt`. If you plan on running a large depth of searches, start with 2 with option `-v` to check what is being returned. Then you can increase the Depth, and the new output will be appended to the existing file, unless you pass `-ow`.
 - Set the `-op` option to give a specific output file name for Potential Parameters, rather than the default of `parameters.txt`. Any output will be appended to the existing file, unless you pass `-ow`.
 - If using a high Depth (`-d`) be wary of some sites using dynamic links so will it will just keep finding new ones. If no new links are being found, then xnlLinkFinder will stop searching. Providing the Stop flags (`s429`, `s403`, `sTO`, `sCE`) should also be considered.
 - If you are finding a large number of links, especially if the Depth (`-d` value) is high, and have limited resources, the program will stop when it reaches the memory Threshold (`-m`) value and end gracefully with data intact before getting killed.
 - If you decide to cancel xnLinkFinder (using `Ctrl-C`) in the middle of running, be patient and any gathered data will be saved before ending gracefully.
 - Using the `-orig` option will show the URL where the link was found. This can mean you have duplicate links in the output if the same link was found on multiple sources, but it will suffixed with the origin URL in square brackets.
-- When making requests, xnLinkFinder will use a random User-Agent from the current group, which defaults to `desktop`. If you have a target that could have different links for different user agent groups, the specify `-u desktop mobile` for example (separate with a space). The `mobile` user agent option is an combination of `mobile-apple`, `mobile-android` and `mobile-windows`.
+- When making requests, xnLinkFinder will use a random User-Agent from the current group, which defaults to `desktop` (unless the `-uc`/`--user-agent-custom` argument is used). If you have a target that could have different links for different user agent groups, then specify `-u desktop mobile` for example (separate with a space). The `mobile` user agent option is an combination of `mobile-apple`, `mobile-android` and `mobile-windows`. Possible values are `desktop`, `mobile`, `set-top-boxes` and `game-console`.
 - When `-i` has been set to a directory, the contents of the files in the root of that directory will be searched for links. Files in sub-directories are not searched. Any files that are over the size set by `-mfs` (default: 500 MB) will be skipped.
 - When using the `-replay-proxy` option, sometimes requests can take longer. If you start seeing more `Request Timeout` errors (you'll see errors if you use `-v` or `-vv` options) then consider using `-t` to raise the timeout limit.
 - If you know a target will only have ASCII characters in links and parameters then consider passing `-ascii-only`. This can eliminate a number of false positives that can sometimes get returned from binary data.
 - If you pass a [waymore](https://github.com/xnl-h4ck3r/waymore) results directory, it is worth passing the `-d`/`--depth` argument to search any extra links found from URL requests and also the `-u`/`--user-agent` if you think there could be different content found, e.g. `-u desktop mobile`.
 - Always pass the `-owl`/`--output-wordlist` filename to save the target specific wordlist. This list can be very useful when fuzzing a target.
 - The words for the target specific wordlist are taken from the following sources (any of 3 characters or more), but are also determined by the other wordlist arguments (see Usage section above):
   - All responses with certain conditions:
```

### Comparing `xnLinkFinder-6.0/README.md` & `xnlinkfinder-6.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,28 @@
+Metadata-Version: 2.1
+Name: xnLinkFinder
+Version: 6.1
+Summary: A python script to find endpoints from a URL, a file of URLs, a directory of files, a Burp XML file or a ZAP ASCII message file. It also gets potential parameters and a target specific wordlist.
+Home-page: https://github.com/xnl-h4ck3r/xnlLinkFinder
+Author: @xnl-h4ck3r
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: psutil
+Requires-Dist: pyyaml
+Requires-Dist: termcolor
+Requires-Dist: urlparse3
+Requires-Dist: beautifulsoup4
+Requires-Dist: lxml
+Requires-Dist: html5lib
+Requires-Dist: urllib3
+
 <center><img src="https://github.com/xnl-h4ck3r/xnLinkFinder/blob/main/xnLinkFinder/images/title.png"></center>
 
-## About - v6.0
+## About - v6.1
 
 This is a tool used to discover endpoints (and potential parameters) for a given target. It can find them by:
 
 - crawling a target (pass a domain/URL)
 - crawling multiple targets (pass a file of domains/URLs)
 - searching files in a given directory (pass a directory name)
 - get them from a **Burp** project (pass location of a Burp XML file)
@@ -67,14 +85,15 @@
 | -x          | --exclude                  | Additional Link exclusions (to the list in `config.yml`) in a comma separated list, e.g. `careers,forum`                                                                                                                                                                                                                                                                                                                                                                                           |
 | -orig       | --origin                   | Whether you want the origin of the link to be in the output. Displayed as `LINK-URL [ORIGIN-URL]` in the output (default: false)                                                                                                                                                                                                                                                                                                                                                                   |
 | -prefixed   |                            | Whether you want to see which links were prefixed in the output. Displays `(PREFIXED)` after link and origin in the output (default: false)                                                                                                                                                                                                                                                                                                                                                        |
 | -xrel       | --exclude-relative-links   | By default, if any links in the results start with `./` or `../`, they will be included. If this argument is used, these relative links will not be added.                                                                                                                                                                                                                                                                                                                                         |
 | -t          | --timeout †                | How many seconds to wait for the server to send data before giving up (default: 10 seconds)                                                                                                                                                                                                                                                                                                                                                                                                        |
 | -inc        | --include                  | Include input (`-i`) links in the output (default: false)                                                                                                                                                                                                                                                                                                                                                                                                                                          |
 | -u          | --user-agent †             | What User Agents to get links for, e.g. `-u desktop mobile`. Possible values are `desktop`, `mobile`, `set-top-boxes` and `game-console`. Also there are `mobile-apple`, `mobile-android` and `mobile-windows` that are subsets of `mobile` but can be used separately.                                                                                                                                                                                                                            |
+| -uc         | --user-agent-custom †      | A custom User Agent string to use for all requests. This will override the `-u`/`--user-agent` argument. This can be used when a program requires a specific User Agent header to identify you for example.                                                                                                                                                                                                                                                                                        |
 | -insecure   | †                          | Whether TLS certificate checks should be disabled when making requests (delfault: false)                                                                                                                                                                                                                                                                                                                                                                                                           |
 | -s429       | †                          | Stop when > 95 percent of responses return 429 Too Many Requests (default: false)                                                                                                                                                                                                                                                                                                                                                                                                                  |
 | -s403       | †                          | Stop when > 95 percent of responses return 403 Forbidden (default: false)                                                                                                                                                                                                                                                                                                                                                                                                                          |
 | -sTO        | †                          | Stop when > 95 percent of requests time out (default: false)                                                                                                                                                                                                                                                                                                                                                                                                                                       |
 | -sCE        | †                          | Stop when > 95 percent of requests have connection errors (default: false)                                                                                                                                                                                                                                                                                                                                                                                                                         |
 | -m          | --memory-threshold         | The memory threshold percentage. If the machines memory goes above the threshold, the program will be stopped and ended gracefully before running out of memory (default: 95)                                                                                                                                                                                                                                                                                                                      |
 | -mfs        | --max-file-size †          | The maximum file size (in bytes) of a file to be checked if -i is a directory. If the file size is over, it will be ignored (default: 500 MB). Setting to 0 means no files will be ignored, regardless of size.                                                                                                                                                                                                                                                                                    |
@@ -254,15 +273,15 @@
 - Pass cookies (`-c`), headers (`-H`) and regex (`-ra`) values within single quotes, e.g. `-ra '/api/v[0-9]\.[0-9]\*'`
 - Set the `-o` option to give a specific output file name for Links, rather than the default of `output.txt`. If you plan on running a large depth of searches, start with 2 with option `-v` to check what is being returned. Then you can increase the Depth, and the new output will be appended to the existing file, unless you pass `-ow`.
 - Set the `-op` option to give a specific output file name for Potential Parameters, rather than the default of `parameters.txt`. Any output will be appended to the existing file, unless you pass `-ow`.
 - If using a high Depth (`-d`) be wary of some sites using dynamic links so will it will just keep finding new ones. If no new links are being found, then xnlLinkFinder will stop searching. Providing the Stop flags (`s429`, `s403`, `sTO`, `sCE`) should also be considered.
 - If you are finding a large number of links, especially if the Depth (`-d` value) is high, and have limited resources, the program will stop when it reaches the memory Threshold (`-m`) value and end gracefully with data intact before getting killed.
 - If you decide to cancel xnLinkFinder (using `Ctrl-C`) in the middle of running, be patient and any gathered data will be saved before ending gracefully.
 - Using the `-orig` option will show the URL where the link was found. This can mean you have duplicate links in the output if the same link was found on multiple sources, but it will suffixed with the origin URL in square brackets.
-- When making requests, xnLinkFinder will use a random User-Agent from the current group, which defaults to `desktop`. If you have a target that could have different links for different user agent groups, the specify `-u desktop mobile` for example (separate with a space). The `mobile` user agent option is an combination of `mobile-apple`, `mobile-android` and `mobile-windows`.
+- When making requests, xnLinkFinder will use a random User-Agent from the current group, which defaults to `desktop` (unless the `-uc`/`--user-agent-custom` argument is used). If you have a target that could have different links for different user agent groups, then specify `-u desktop mobile` for example (separate with a space). The `mobile` user agent option is an combination of `mobile-apple`, `mobile-android` and `mobile-windows`. Possible values are `desktop`, `mobile`, `set-top-boxes` and `game-console`.
 - When `-i` has been set to a directory, the contents of the files in the root of that directory will be searched for links. Files in sub-directories are not searched. Any files that are over the size set by `-mfs` (default: 500 MB) will be skipped.
 - When using the `-replay-proxy` option, sometimes requests can take longer. If you start seeing more `Request Timeout` errors (you'll see errors if you use `-v` or `-vv` options) then consider using `-t` to raise the timeout limit.
 - If you know a target will only have ASCII characters in links and parameters then consider passing `-ascii-only`. This can eliminate a number of false positives that can sometimes get returned from binary data.
 - If you pass a [waymore](https://github.com/xnl-h4ck3r/waymore) results directory, it is worth passing the `-d`/`--depth` argument to search any extra links found from URL requests and also the `-u`/`--user-agent` if you think there could be different content found, e.g. `-u desktop mobile`.
 - Always pass the `-owl`/`--output-wordlist` filename to save the target specific wordlist. This list can be very useful when fuzzing a target.
 - The words for the target specific wordlist are taken from the following sources (any of 3 characters or more), but are also determined by the other wordlist arguments (see Usage section above):
   - All responses with certain conditions:
```

### Comparing `xnLinkFinder-6.0/setup.py` & `xnlinkfinder-6.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,19 +30,19 @@
     version=__import__('xnLinkFinder').__version__,
     description="A python script to find endpoints from a URL, a file of URLs, a directory of files, a Burp XML file or a ZAP ASCII message file. It also gets potential parameters and a target specific wordlist.",
     long_description=open("README.md").read(),
     long_description_content_type='text/markdown',
     author="@xnl-h4ck3r",
     url="https://github.com/xnl-h4ck3r/xnlLinkFinder",
     py_modules=["xnLinkFinder"],
-    install_requires=["argparse","requests","psutil","pyyaml","termcolor","urlparse3","beautifulsoup4","lxml","html5lib","urllib3"],
+    install_requires=["requests","psutil","pyyaml","termcolor","urlparse3","beautifulsoup4","lxml","html5lib","urllib3"],
     entry_points={
         'console_scripts': [
             'xnLinkFinder = xnLinkFinder.xnLinkFinder:main',
         ],
     },
 )
 
 if configNew:
     print('\n\033[33mIMPORTANT: The file '+target_directory+'/config.yml already exists.\nCreating config.yml.NEW but leaving existing config.\nIf you need the new file, then remove the current one and rename config.yml.NEW to config.yml\n\033[0m')
 else:
-    print('\n\033[92mThe file '+target_directory+'/config.yml has been created.\n\033[0m')
+    print('\n\033[92mThe file '+target_directory+'/config.yml has been created.\n\033[0m')
```

### Comparing `xnLinkFinder-6.0/xnLinkFinder/xnLinkFinder.py` & `xnlinkfinder-6.1/xnLinkFinder/xnLinkFinder.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,15 @@
 
 # A comma separated list of Link exclusions used when the exclusions from config.yml cannot be found
 # Links are NOT output if they contain these strings. This just applies to the links found in endpoints, not the origin link in which it was found
 DEFAULT_LINK_EXCLUSIONS = ".css,.jpg,.jpeg,.png,.svg,.img,.gif,.mp4,.flv,.ogv,.webm,.webp,.mov,.mp3,.m4a,.m4p,.scss,.tif,.tiff,.ttf,.otf,.woff,.woff2,.bmp,.ico,.eot,.htc,.rtf,.swf,.image,w3.org,doubleclick.net,youtube.com,.vue,jquery,bootstrap,font,jsdelivr.net,vimeo.com,pinterest.com,facebook,linkedin,twitter,instagram,google,mozilla.org,jibe.com,schema.org,schemas.microsoft.com,wordpress.org,w.org,wix.com,parastorage.com,whatwg.org,polyfill,typekit.net,schemas.openxmlformats.org,openweathermap.org,openoffice.org,reactjs.org,angularjs.org,java.com,purl.org,/image,/img,/css,/wp-json,/wp-content,/wp-includes,/theme,/audio,/captcha,/font,node_modules,.wav,.gltf,.pict,.svgz,.eps,.midi,.mid,.avif,xmlns.com,rdfs.org,ogp.me,newrelic.com,optimizely.com"
 
 # A comma separated list of Content-Type exclusions used when the exclusions from config.yml cannot be found
 # These content types will NOT be checked
-DEFAULT_CONTENTTYPE_EXCLUSIONS = "text/css,image/jpeg,image/jpg,image/png,image/svg+xml,image/gif,image/tiff,image/webp,image/bmp,image/x-icon,image/vnd.microsoft.icon,font/ttf,font/woff,font/woff2,font/x-woff2,font/x-woff,font/otf,audio/mpeg,audio/wav,audio/webm,audio/aac,audio/ogg,audio/wav,audio/webm,video/mp4,video/mpeg,video/webm,video/ogg,video/mp2t,video/webm,video/x-msvideo,application/font-woff,application/font-woff2,application/vnd.android.package-archive,binary/octet-stream,application/octet-stream,application/pdf,application/x-font-ttf,application/x-font-otf,application/x-font-woff,application/vnd.ms-fontobject,image/avif,application/zip,application/x-zip-compressed,application/x-msdownload,application/x-apple-diskimage,application/x-rpm,application/vnd.debian.binary-package,application/x-font-truetype,font/opentype,image/pjpeg,application/x-troff-man,application/font-otf,application/x-ms-application,application/x-msdownload"
+DEFAULT_CONTENTTYPE_EXCLUSIONS = "text/css,image/jpeg,image/jpg,image/png,image/svg+xml,image/gif,image/tiff,image/webp,image/bmp,image/x-icon,image/vnd.microsoft.icon,font/ttf,font/woff,font/woff2,font/x-woff2,font/x-woff,font/otf,audio/mpeg,audio/wav,audio/webm,audio/aac,audio/ogg,audio/wav,audio/webm,video/mp4,video/mpeg,video/webm,video/ogg,video/mp2t,video/webm,video/x-msvideo,application/font-woff,application/font-woff2,application/vnd.android.package-archive,binary/octet-stream,application/octet-stream,application/pdf,application/x-font-ttf,application/x-font-otf,application/x-font-woff,application/vnd.ms-fontobject,image/avif,application/zip,application/x-zip-compressed,application/x-msdownload,application/x-apple-diskimage,application/x-rpm,application/vnd.debian.binary-package,application/x-font-truetype,font/opentype,image/pjpeg,application/x-troff-man,application/font-otf,application/x-ms-application,application/x-msdownload,image/jp2,video/x-m4v"
 
 # A comma separated list of file extension exclusions used when the file ext exclusions from config.yml cannot be found
 # In Directory mode, files with these extensions will NOT be checked
 DEFAULT_FILEEXT_EXCLUSIONS = ".zip,.dmg,.rpm,.deb,.gz,.tar,.jpg,.jpeg,.png,.svg,.img,.gif,.mp4,.flv,.ogv,.webm,.webp,.mov,.mp3,.m4a,.m4p,.scss,.tif,.tiff,.ttf,.otf,.woff,.woff2,.bmp,.ico,.eot,.htc,.rtf,.swf,.image,.wav,.gltf,.pict,.svgz,.eps,.midi,.mid,.pdf"
 
 # A list of files used in the Link Finding Regex when the exclusions from config.yml cannot be found.
 # These are used in the 5th capturing group that aren't obvious links, but could be files
@@ -934,16 +934,20 @@
     return makeRequest
 
 
 def processUrl(url):
 
     global burpFile, zapFile, caidoFile, totalRequests, skippedRequests, failedRequests, userAgent, requestHeaders, tooManyRequests, tooManyForbidden, tooManyTimeouts, tooManyConnectionErrors, stopProgram, waymoreMode, stopProgram, failedPrefixLinks, currentDepth
     
+    # If a custom user agent string was passed then use that in the header, else
     # Choose a random user agent string to use from the current group
-    userAgent = random.choice(userAgents[currentUAGroup])
+    if args.user_agent_custom != "":
+        userAgent = args.user_agent_custom
+    else:
+        userAgent = random.choice(userAgents[currentUAGroup])
     requestHeaders["User-Agent"] = userAgent
 
     try: 
         # If waymore Mode then the url maybe from index.txt get the source URL from the line
         if waymoreMode and args.input.endswith("index.txt") :
             values = url.split(",")
             archiveUrl = values[1]
@@ -1866,15 +1870,15 @@
                 oldList = linksFound.copy()
                 p = mp.Pool(args.processes)
                 p.map(processUrl, oldList)
                 p.close()
                 p.join()
 
                 # If -spkf wasn't passed and there are any failed prefixed links, remove them from linksFound
-                if not args.scope_prefix_keep_failed:
+                if not args.scope_prefix_keep_failed and failedPrefixLinks is not None:
                     for fail in failedPrefixLinks:
                         try:
                             linksFound.remove(fail)
                         except:
                             pass
 
                 # Get the current number of Links found this time
@@ -2127,21 +2131,27 @@
                 colored("-t: " + str(args.timeout), "magenta")
                 + colored(" The number of seconds to wait for a response.", "white")
             )
             write(
                 colored("-inc: " + str(args.include), "magenta")
                 + colored(" Include input (-i) links in the output.", "white")
             )
-            write(
-                colored("-u: " + str(args.user_agent), "magenta")
-                + colored(
-                    " What User Agents to use for requests. If more than one specified then all requests will be made per User Agent group.",
-                    "white",
+            if args.user_agent_custom != "":
+                write(
+                    colored("-uc: " + str(args.user_agent_custom), "magenta")
+                    + colored(" The custom User Agent used for all requests", "white")
+                )
+            else:
+                write(
+                    colored("-u: " + str(args.user_agent), "magenta")
+                    + colored(
+                        " What User Agents to use for requests. If more than one specified then all requests will be made per User Agent group.",
+                        "white",
+                    )
                 )
-            )
 
             if args.cookies != "":
                 write(
                     colored("-c: " + args.cookies, "magenta")
                     + colored(" Cookies passed with requests.", "white")
                 )
 
@@ -3020,15 +3030,15 @@
 
             # If it's a directory
             if dirPassed:
                 processDirectory()
 
             else:
                 # Show the current User Agent group
-                if len(args.user_agent) > 1:
+                if len(args.user_agent) > 1 and args.user_agent_custom == "":
                     write(
                         colored("\nUser-Agent Group: ", "cyan")
                         + colored(args.user_agent[currentUAGroup], "white")
                     )
 
                 if urlPassed:
                     # It's not a standard file, so assume it's just a single URL
@@ -3162,29 +3172,33 @@
         if vverbose():
             writerr(colored("ERROR processInput 1: " + str(e), "red"))
 
 
 # Set user agents to process
 def setUserAgents():
     global userAgents
-    for ua in args.user_agent:
-        if ua == "desktop":
-            userAgents.append(UA_DESKTOP)
-        elif ua == "mobile":
-            userAgents.append(UA_MOBILE)
-        elif ua == "mobile-apple":
-            userAgents.append(UA_MOBILE_APPLE)
-        elif ua == "mobile-android":
-            userAgents.append(UA_MOBILE_ANDROID)
-        elif ua == "mobile-windows":
-            userAgents.append(UA_MOBILE_WINDOWS)
-        elif ua == "set-top-boxes":
-            userAgents.append(UA_SETTOPBOXES)
-        elif ua == "game-console":
-            userAgents.append(UA_GAMECONSOLE)
+    # If a custom user agent was passed then only use that, else check which groups were specified
+    if args.user_agent_custom != "":
+        userAgents.append([args.user_agent_custom])
+    else:
+        for ua in args.user_agent:
+            if ua == "desktop":
+                userAgents.append(UA_DESKTOP)
+            elif ua == "mobile":
+                userAgents.append(UA_MOBILE)
+            elif ua == "mobile-apple":
+                userAgents.append(UA_MOBILE_APPLE)
+            elif ua == "mobile-android":
+                userAgents.append(UA_MOBILE_ANDROID)
+            elif ua == "mobile-windows":
+                userAgents.append(UA_MOBILE_WINDOWS)
+            elif ua == "set-top-boxes":
+                userAgents.append(UA_SETTOPBOXES)
+            elif ua == "game-console":
+                userAgents.append(UA_GAMECONSOLE)
     if userAgents == []:
         userAgents = [UA_DESKTOP]
 
 
 # Set the headers to be used for all requests
 def setHeaders():
 
@@ -3818,14 +3832,21 @@
             "set-top-boxes",
             "game-console",
         ],
         default=["desktop"],
         metavar="",
     )
     parser.add_argument(
+        "-uc",
+        "--user-agent-custom",
+        action="store",
+        help="A custom User Agent string to use for all requests. This will override the -u/--user-agent argument. This can be used when a program requires a specific User Agent header to identify you for example.",
+        default="",
+    )
+    parser.add_argument(
         "-insecure",
         action="store_true",
         help="Whether TLS certificate checks should be made disabled making requests (default: false)",
     )
     parser.add_argument(
         "-s429",
         action="store_true",
```

### Comparing `xnLinkFinder-6.0/xnLinkFinder.egg-info/PKG-INFO` & `xnlinkfinder-6.1/xnLinkFinder.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: xnLinkFinder
-Version: 6.0
+Version: 6.1
 Summary: A python script to find endpoints from a URL, a file of URLs, a directory of files, a Burp XML file or a ZAP ASCII message file. It also gets potential parameters and a target specific wordlist.
 Home-page: https://github.com/xnl-h4ck3r/xnlLinkFinder
 Author: @xnl-h4ck3r
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: argparse
 Requires-Dist: requests
 Requires-Dist: psutil
 Requires-Dist: pyyaml
 Requires-Dist: termcolor
 Requires-Dist: urlparse3
 Requires-Dist: beautifulsoup4
 Requires-Dist: lxml
 Requires-Dist: html5lib
 Requires-Dist: urllib3
 
 <center><img src="https://github.com/xnl-h4ck3r/xnLinkFinder/blob/main/xnLinkFinder/images/title.png"></center>
 
-## About - v6.0
+## About - v6.1
 
 This is a tool used to discover endpoints (and potential parameters) for a given target. It can find them by:
 
 - crawling a target (pass a domain/URL)
 - crawling multiple targets (pass a file of domains/URLs)
 - searching files in a given directory (pass a directory name)
 - get them from a **Burp** project (pass location of a Burp XML file)
@@ -86,14 +85,15 @@
 | -x          | --exclude                  | Additional Link exclusions (to the list in `config.yml`) in a comma separated list, e.g. `careers,forum`                                                                                                                                                                                                                                                                                                                                                                                           |
 | -orig       | --origin                   | Whether you want the origin of the link to be in the output. Displayed as `LINK-URL [ORIGIN-URL]` in the output (default: false)                                                                                                                                                                                                                                                                                                                                                                   |
 | -prefixed   |                            | Whether you want to see which links were prefixed in the output. Displays `(PREFIXED)` after link and origin in the output (default: false)                                                                                                                                                                                                                                                                                                                                                        |
 | -xrel       | --exclude-relative-links   | By default, if any links in the results start with `./` or `../`, they will be included. If this argument is used, these relative links will not be added.                                                                                                                                                                                                                                                                                                                                         |
 | -t          | --timeout †                | How many seconds to wait for the server to send data before giving up (default: 10 seconds)                                                                                                                                                                                                                                                                                                                                                                                                        |
 | -inc        | --include                  | Include input (`-i`) links in the output (default: false)                                                                                                                                                                                                                                                                                                                                                                                                                                          |
 | -u          | --user-agent †             | What User Agents to get links for, e.g. `-u desktop mobile`. Possible values are `desktop`, `mobile`, `set-top-boxes` and `game-console`. Also there are `mobile-apple`, `mobile-android` and `mobile-windows` that are subsets of `mobile` but can be used separately.                                                                                                                                                                                                                            |
+| -uc         | --user-agent-custom †      | A custom User Agent string to use for all requests. This will override the `-u`/`--user-agent` argument. This can be used when a program requires a specific User Agent header to identify you for example.                                                                                                                                                                                                                                                                                        |
 | -insecure   | †                          | Whether TLS certificate checks should be disabled when making requests (delfault: false)                                                                                                                                                                                                                                                                                                                                                                                                           |
 | -s429       | †                          | Stop when > 95 percent of responses return 429 Too Many Requests (default: false)                                                                                                                                                                                                                                                                                                                                                                                                                  |
 | -s403       | †                          | Stop when > 95 percent of responses return 403 Forbidden (default: false)                                                                                                                                                                                                                                                                                                                                                                                                                          |
 | -sTO        | †                          | Stop when > 95 percent of requests time out (default: false)                                                                                                                                                                                                                                                                                                                                                                                                                                       |
 | -sCE        | †                          | Stop when > 95 percent of requests have connection errors (default: false)                                                                                                                                                                                                                                                                                                                                                                                                                         |
 | -m          | --memory-threshold         | The memory threshold percentage. If the machines memory goes above the threshold, the program will be stopped and ended gracefully before running out of memory (default: 95)                                                                                                                                                                                                                                                                                                                      |
 | -mfs        | --max-file-size †          | The maximum file size (in bytes) of a file to be checked if -i is a directory. If the file size is over, it will be ignored (default: 500 MB). Setting to 0 means no files will be ignored, regardless of size.                                                                                                                                                                                                                                                                                    |
@@ -273,15 +273,15 @@
 - Pass cookies (`-c`), headers (`-H`) and regex (`-ra`) values within single quotes, e.g. `-ra '/api/v[0-9]\.[0-9]\*'`
 - Set the `-o` option to give a specific output file name for Links, rather than the default of `output.txt`. If you plan on running a large depth of searches, start with 2 with option `-v` to check what is being returned. Then you can increase the Depth, and the new output will be appended to the existing file, unless you pass `-ow`.
 - Set the `-op` option to give a specific output file name for Potential Parameters, rather than the default of `parameters.txt`. Any output will be appended to the existing file, unless you pass `-ow`.
 - If using a high Depth (`-d`) be wary of some sites using dynamic links so will it will just keep finding new ones. If no new links are being found, then xnlLinkFinder will stop searching. Providing the Stop flags (`s429`, `s403`, `sTO`, `sCE`) should also be considered.
 - If you are finding a large number of links, especially if the Depth (`-d` value) is high, and have limited resources, the program will stop when it reaches the memory Threshold (`-m`) value and end gracefully with data intact before getting killed.
 - If you decide to cancel xnLinkFinder (using `Ctrl-C`) in the middle of running, be patient and any gathered data will be saved before ending gracefully.
 - Using the `-orig` option will show the URL where the link was found. This can mean you have duplicate links in the output if the same link was found on multiple sources, but it will suffixed with the origin URL in square brackets.
-- When making requests, xnLinkFinder will use a random User-Agent from the current group, which defaults to `desktop`. If you have a target that could have different links for different user agent groups, the specify `-u desktop mobile` for example (separate with a space). The `mobile` user agent option is an combination of `mobile-apple`, `mobile-android` and `mobile-windows`.
+- When making requests, xnLinkFinder will use a random User-Agent from the current group, which defaults to `desktop` (unless the `-uc`/`--user-agent-custom` argument is used). If you have a target that could have different links for different user agent groups, then specify `-u desktop mobile` for example (separate with a space). The `mobile` user agent option is an combination of `mobile-apple`, `mobile-android` and `mobile-windows`. Possible values are `desktop`, `mobile`, `set-top-boxes` and `game-console`.
 - When `-i` has been set to a directory, the contents of the files in the root of that directory will be searched for links. Files in sub-directories are not searched. Any files that are over the size set by `-mfs` (default: 500 MB) will be skipped.
 - When using the `-replay-proxy` option, sometimes requests can take longer. If you start seeing more `Request Timeout` errors (you'll see errors if you use `-v` or `-vv` options) then consider using `-t` to raise the timeout limit.
 - If you know a target will only have ASCII characters in links and parameters then consider passing `-ascii-only`. This can eliminate a number of false positives that can sometimes get returned from binary data.
 - If you pass a [waymore](https://github.com/xnl-h4ck3r/waymore) results directory, it is worth passing the `-d`/`--depth` argument to search any extra links found from URL requests and also the `-u`/`--user-agent` if you think there could be different content found, e.g. `-u desktop mobile`.
 - Always pass the `-owl`/`--output-wordlist` filename to save the target specific wordlist. This list can be very useful when fuzzing a target.
 - The words for the target specific wordlist are taken from the following sources (any of 3 characters or more), but are also determined by the other wordlist arguments (see Usage section above):
   - All responses with certain conditions:
```

