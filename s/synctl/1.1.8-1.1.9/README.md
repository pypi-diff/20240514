# Comparing `tmp/synctl-1.1.8.tar.gz` & `tmp/synctl-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synctl-1.1.8.tar", last modified: Wed Apr 17 05:53:04 2024, max compression
+gzip compressed data, was "synctl-1.1.9.tar", last modified: Mon Apr 29 06:47:23 2024, max compression
```

## Comparing `synctl-1.1.8.tar` & `synctl-1.1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 swethalohith   (501) staff       (20)        0 2024-04-17 05:53:04.891816 synctl-1.1.8/
--rw-r--r--   0 swethalohith   (501) staff       (20)     1064 2023-11-24 04:36:16.000000 synctl-1.1.8/LICENSE
--rw-r--r--   0 swethalohith   (501) staff       (20)     1640 2024-04-17 05:53:04.891662 synctl-1.1.8/PKG-INFO
--rw-r--r--   0 swethalohith   (501) staff       (20)    35137 2024-04-17 05:15:05.000000 synctl-1.1.8/README.md
--rw-r--r--   0 swethalohith   (501) staff       (20)       81 2023-11-29 08:33:08.000000 synctl-1.1.8/pyproject.toml
--rw-r--r--   0 swethalohith   (501) staff       (20)       38 2024-04-17 05:53:04.891866 synctl-1.1.8/setup.cfg
--rw-r--r--   0 swethalohith   (501) staff       (20)     2143 2023-11-29 08:33:08.000000 synctl-1.1.8/setup.py
-drwxr-xr-x   0 swethalohith   (501) staff       (20)        0 2024-04-17 05:53:04.889192 synctl-1.1.8/synctl/
--rw-r--r--   0 swethalohith   (501) staff       (20)        0 2023-11-29 08:33:08.000000 synctl-1.1.8/synctl/__init__.py
--rw-r--r--   0 swethalohith   (501) staff       (20)       22 2024-04-17 05:18:14.000000 synctl-1.1.8/synctl/__version__.py
--rwxr-xr-x   0 swethalohith   (501) staff       (20)   228546 2024-04-17 05:15:05.000000 synctl-1.1.8/synctl/cli.py
-drwxr-xr-x   0 swethalohith   (501) staff       (20)        0 2024-04-17 05:53:04.891023 synctl-1.1.8/synctl.egg-info/
--rw-r--r--   0 swethalohith   (501) staff       (20)     1640 2024-04-17 05:53:04.000000 synctl-1.1.8/synctl.egg-info/PKG-INFO
--rw-r--r--   0 swethalohith   (501) staff       (20)      328 2024-04-17 05:53:04.000000 synctl-1.1.8/synctl.egg-info/SOURCES.txt
--rw-r--r--   0 swethalohith   (501) staff       (20)        1 2024-04-17 05:53:04.000000 synctl-1.1.8/synctl.egg-info/dependency_links.txt
--rw-r--r--   0 swethalohith   (501) staff       (20)       43 2024-04-17 05:53:04.000000 synctl-1.1.8/synctl.egg-info/entry_points.txt
--rw-r--r--   0 swethalohith   (501) staff       (20)        1 2023-11-24 05:57:32.000000 synctl-1.1.8/synctl.egg-info/not-zip-safe
--rw-r--r--   0 swethalohith   (501) staff       (20)       17 2024-04-17 05:53:04.000000 synctl-1.1.8/synctl.egg-info/requires.txt
--rw-r--r--   0 swethalohith   (501) staff       (20)        7 2024-04-17 05:53:04.000000 synctl-1.1.8/synctl.egg-info/top_level.txt
-drwxr-xr-x   0 swethalohith   (501) staff       (20)        0 2024-04-17 05:53:04.891183 synctl-1.1.8/tests/
--rw-r--r--   0 swethalohith   (501) staff       (20)    21585 2023-12-18 04:49:58.000000 synctl-1.1.8/tests/test_synctl.py
+drwxr-xr-x   0 swethalohith   (501) staff       (20)        0 2024-04-29 06:47:23.309816 synctl-1.1.9/
+-rw-r--r--   0 swethalohith   (501) staff       (20)     1064 2023-11-24 04:36:16.000000 synctl-1.1.9/LICENSE
+-rw-r--r--   0 swethalohith   (501) staff       (20)     1640 2024-04-29 06:47:23.309650 synctl-1.1.9/PKG-INFO
+-rw-r--r--   0 swethalohith   (501) staff       (20)    35443 2024-04-29 06:38:54.000000 synctl-1.1.9/README.md
+-rw-r--r--   0 swethalohith   (501) staff       (20)       81 2023-11-29 08:33:08.000000 synctl-1.1.9/pyproject.toml
+-rw-r--r--   0 swethalohith   (501) staff       (20)       38 2024-04-29 06:47:23.309883 synctl-1.1.9/setup.cfg
+-rw-r--r--   0 swethalohith   (501) staff       (20)     2143 2023-11-29 08:33:08.000000 synctl-1.1.9/setup.py
+drwxr-xr-x   0 swethalohith   (501) staff       (20)        0 2024-04-29 06:47:23.307147 synctl-1.1.9/synctl/
+-rw-r--r--   0 swethalohith   (501) staff       (20)        0 2023-11-29 08:33:08.000000 synctl-1.1.9/synctl/__init__.py
+-rw-r--r--   0 swethalohith   (501) staff       (20)       22 2024-04-29 06:43:29.000000 synctl-1.1.9/synctl/__version__.py
+-rwxr-xr-x   0 swethalohith   (501) staff       (20)   237287 2024-04-29 06:38:49.000000 synctl-1.1.9/synctl/cli.py
+drwxr-xr-x   0 swethalohith   (501) staff       (20)        0 2024-04-29 06:47:23.308973 synctl-1.1.9/synctl.egg-info/
+-rw-r--r--   0 swethalohith   (501) staff       (20)     1640 2024-04-29 06:47:23.000000 synctl-1.1.9/synctl.egg-info/PKG-INFO
+-rw-r--r--   0 swethalohith   (501) staff       (20)      328 2024-04-29 06:47:23.000000 synctl-1.1.9/synctl.egg-info/SOURCES.txt
+-rw-r--r--   0 swethalohith   (501) staff       (20)        1 2024-04-29 06:47:23.000000 synctl-1.1.9/synctl.egg-info/dependency_links.txt
+-rw-r--r--   0 swethalohith   (501) staff       (20)       43 2024-04-29 06:47:23.000000 synctl-1.1.9/synctl.egg-info/entry_points.txt
+-rw-r--r--   0 swethalohith   (501) staff       (20)        1 2023-11-24 05:57:32.000000 synctl-1.1.9/synctl.egg-info/not-zip-safe
+-rw-r--r--   0 swethalohith   (501) staff       (20)       17 2024-04-29 06:47:23.000000 synctl-1.1.9/synctl.egg-info/requires.txt
+-rw-r--r--   0 swethalohith   (501) staff       (20)        7 2024-04-29 06:47:23.000000 synctl-1.1.9/synctl.egg-info/top_level.txt
+drwxr-xr-x   0 swethalohith   (501) staff       (20)        0 2024-04-29 06:47:23.309130 synctl-1.1.9/tests/
+-rw-r--r--   0 swethalohith   (501) staff       (20)    21585 2023-12-18 04:49:58.000000 synctl-1.1.9/tests/test_synctl.py
```

### Comparing `synctl-1.1.8/LICENSE` & `synctl-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `synctl-1.1.8/PKG-INFO` & `synctl-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synctl
-Version: 1.1.8
+Version: 1.1.9
 Summary: Instana Synthetic CLI
 Home-page: https://github.com/instana/synthetic-synctl
 Author: Rong Zhu Shang, Swetha Lohith
 Author-email: shangrz@cn.ibm.com, Swetha.Lohith@ibm.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/instana/synthetic-synctl/issues
 Project-URL: Source, https://github.com/instana/synthetic-synctl
```

### Comparing `synctl-1.1.8/README.md` & `synctl-1.1.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Synthetic Command Line Tool(synctl) is used to manage synthetic tests, locations and credentials.
 
 # Table of Contents
 - [Features](#features)
 - [Installation](#installation)
 - [Upgrade](#upgrade)
 - [Size the PoP hardware configuration](#size-the-pop-hardware-configuration)
+- [Estimate the cost of Instana-hosted PoP](#estimate-the-cost-of-instana-hosted-pop)
 - [Configure an Instana Backend](#configure-an-instana-backend)
     - [Use a configuration file](#use-a-configuration-file-recommended)
     - [Use command options](#use-command-options)
     - [Use environment variables](#use-environment-variables)
 - [Manage configuration files](#manage-configuration-files)
     - [synctl config Syntax](#synctl-config-syntax)
     - [synctl config Options](#synctl-config-options)
@@ -99,15 +100,26 @@
 ```
 
 # Size the PoP hardware configuration
 synctl can be used to estimate the size of the PoP hardware configuration.
 
 ### synctl pop-sizing Syntax
 ```
-synctl get pop-size
+# synctl get pop-size
+
+# synctl get size
+```
+# Estimate the cost of Instana-hosted PoP
+synctl can be used to estimate the cost of Instana-hosted synthetic PoP.
+
+### synctl cost estimation Syntax
+```
+# synctl get pop-cost
+
+# synctl get cost
 ```
 # Configure an Instana Backend
 `synctl` support three types of configurations:
 - Use configurations file, the default config file is under `~/.synthetic/config.json`.
 - Use `--host` and `--token` options to specify the host and token.
 - Set environment variables before run synctl command, `SYN_SERVER_HOSTNAME`, `SYN_API_TOKEN` are used to store host and token.
```

### Comparing `synctl-1.1.8/setup.py` & `synctl-1.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `synctl-1.1.8/synctl/cli.py` & `synctl-1.1.9/synctl/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 SYN_LO = "lo"  # short for location
 SYN_APPLICATION = "application"
 SYN_APP = "app"  # short for application
 SYN_CRED = "cred"  # short for credentials
 SYN_ALERT = "alert"  # short for smart alerts
 SYN_RESULT = "result"
 POP_SIZE = "pop-size"
+POP_COST = "pop-cost"
 
 POSITION_PARAMS = "commands"
 OPTIONS_PARAMS = "options"
 
 NOT_APPLICABLE = "N/A"
 
 NORMAL_CODE, ERROR_CODE = (0, 1)
@@ -96,22 +97,22 @@
     print(f"synctl version: {VERSION}")
 
 
 def general_helper() -> None:
     m = """Usage: synctl [--verify-tls] <command> [options]
 
 Options:
-  -h, --help            show this help message and exit
-  --version, -v         show version
-  --verify-tls          verify tls certificate
+    -h, --help          show this help message and exit
+    --version, -v       show version
+    --verify-tls        verify tls certificate
 
 Commands:
     config              manage configuration file
     create              create a Synthetic test, credential and smart alert
-    get                 get Synthetic tests, locations, credentials, smart alert and pop-size
+    get                 get Synthetic tests, locations, credentials, smart alert, pop-size and pop-cost
     patch               patch a Synthetic test
     update              update a Synthetic test and smart alert
     delete              delete Synthetic tests, locations credentials and smart alert
 
 Use "synctl <command> -h/--help" for more information about a command.
     """
     print(m)
@@ -173,15 +174,15 @@
 # create a credential
 synctl create cred --key MY_PASS --value password123
 
 # create a smart alert
 synctl create alert --name "Smart-alert" --alert-channel "$ALERT_CHANNEL" --test "$SYNTHETIC_TEST" --violation-count 2
 """
 
-GET_USAGE = """synctl get {location,lo,test,application,app,cred,alert, pop-size} [id] [options]
+GET_USAGE = """synctl get {location,lo,test,application,app,cred,alert, pop-size, pop-cost} [id] [options]
 
 examples:
 # display all tests
 synctl get test
 
 # display all locations
 synctl get location
@@ -193,15 +194,18 @@
 # display all credentials
 synctl get cred
 
 # Display all alert
 synctl get alert
 
 # Estimate the size of the PoP hardware configuration
-synctl get pop-size"""
+synctl get pop-size
+
+# Estimate the cost of Instana-hosted Pop
+synctl get pop-cost"""
 
 PATCH_USAGE = """synctl patch test id [options]
 
 examples:
 # set active to false
 synctl patch test <syn-id> --active false
 
@@ -227,19 +231,19 @@
     --timeout 1m \\
     --frequency 5 \\
     --app-id "$APP_ID" \\
     --custom-property "key1=value1,key2=value2"
 
 # update alert with multiple options
 synctl update alert <alert-id> --name "Smart-alert" \\
-       --alert-channel "$ALERT_CHANNEL1" "$ALERT_CHANNEL2" "$ALERT_CHANNEL3" ... \\
-       --test "$SYNTHETIC_TEST1" "$SYNTHETIC_TEST2" "$SYNTHETIC_TEST3" ... \\
-       --violation-count 2 \\
-       --severity warning 
-       
+    --alert-channel "$ALERT_CHANNEL1" "$ALERT_CHANNEL2" "$ALERT_CHANNEL3" ... \\
+    --test "$SYNTHETIC_TEST1" "$SYNTHETIC_TEST2" "$SYNTHETIC_TEST3" ... \\
+    --violation-count 2 \\
+    --severity warning
+
 # enable/disable a smart alert
 synctl update alert <alert-id> --enable
 synctl update alert <alert-id> --disable
 """
 
 DELETE_USAGE = """synctl delete {location,lo,test,cred,alert} [id...] [options]
 
@@ -377,135 +381,255 @@
             "testCount": 5,
             "frequency": 5,
             "cpuLimit": 4000,
             "memLimit": 3000,
             "imageSize": 1500,
         }
 
+        self.factors = {
+            "browserTest": 1,
+            "APIScript": 0.042,
+            "APISimple": 0.025
+        }
+
     def ask_question(self,question, options=None):
         answer = input(question)
         if options:
             while answer not in options:
                 print("Invalid input")
                 answer = input(question)
         return answer
 
+    def get_api_simple_test(self):
+        api_simple_test = {}
+        api_simple_test["testCount"] = int(self.ask_question("How many API Simple tests do you want to create? (0 if no) "))
+        if api_simple_test["testCount"] > 0:
+            while True:
+                api_simple_test["frequency"] = int(self.ask_question("What is the test frequency for your API Simple tests? (1-120) "))
+                if api_simple_test["frequency"] > 0 and api_simple_test["frequency"] <= 120:
+                    break
+                else:
+                    print("frequency is not valid, it should be in [1,120]")
+        return api_simple_test
+
+    def get_api_script_test(self):
+        api_script_test = {}
+        api_script_test["testCount"] = int(self.ask_question("How many API Script tests do you want to create? (0 if no) "))
+        if api_script_test["testCount"] > 0:
+            while True:
+                api_script_test["frequency"] = int(self.ask_question("What is the test frequency for your API Script tests? (1-120) "))
+                if api_script_test["frequency"] > 0 and api_script_test["frequency"] <= 120:
+                    break
+                else:
+                    print("frequency is not valid, it should be in [1,120]")
+        return api_script_test
+
+    def get_browser_script_test(self):
+        browser_script_test = {}
+        browser_script_test["testCount"] = int(self.ask_question("How many Browser tests (Webpage Action, Webpage Script and BrowserScript) do you want to create? (0 if no) "))
+        if browser_script_test["testCount"] > 0:
+            while True:
+                browser_script_test["frequency"] = int(self.ask_question("What is the test frequency for Browser tests? (1-120) "))
+                if browser_script_test["frequency"] > 0 and browser_script_test["frequency"] <= 120:
+                    break
+                else:
+                    print("frequency is not valid, it should be in [1,120]")
+        return browser_script_test
+
     def size_estimate(self, user_tests, default_frequency, user_frequency, default_tests):
         pod_estimate = int(user_tests * default_frequency) / int(user_frequency * default_tests)
         return math.ceil(pod_estimate)
 
+    def test_exec_estimate(self, tests, frequency, loc):
+        #The total test executions per month(30 days)
+        return int(tests * ((30 * 24 * 60) / frequency) * loc)
+
     def pop_size_estimate(self):
+        pop_estimate_size = {}
         print("Please answer below questions for estimating the self-hosted PoP hardware size:\n")
         try:
             while True:
-                api_simple = int(self.ask_question("How many API Simple tests do you want to create? (0 if no) "))
-                if api_simple > 0:
-                    while True:
-                        api_simple_frequency = int(self.ask_question("What is the test frequency for your API Simple tests? (1-120)  "))
-                        if api_simple_frequency > 0 and api_simple_frequency <= 120:
-                            http_pod_count = int(self.size_estimate(api_simple, self.http["frequency"], api_simple_frequency, self.http["testCount"]))
-                            break
-                        else:
-                            print("frequency is not valid, it should be in [1,120]")
-                    break
-                elif api_simple == 0:
-                    http_pod_count = 0
+                pop_estimate_size["api_simple"] = self.get_api_simple_test()
+                if pop_estimate_size["api_simple"]["testCount"] == 0:
+                    pop_estimate_size["http_pod_count"] = 0
                     break
-                else:
+                elif pop_estimate_size["api_simple"]["testCount"] < 0:
                     print("Invalid input")
+                else:
+                    pop_estimate_size["http_pod_count"] = int(self.size_estimate(pop_estimate_size["api_simple"]["testCount"], self.http["frequency"], pop_estimate_size["api_simple"]["frequency"], self.http["testCount"]))
+                    break
 
             while True:
-                api_script = int(self.ask_question("How many API Script tests do you want to create? (0 if no) "))
-                if api_script > 0:
-                    while True:
-                        api_script_frequency = int(self.ask_question("What is the test frequency for your API Script tests? (1-120) "))
-                        if api_script_frequency > 0 and api_script_frequency <= 120:
-                            javascript_pod_count = int(self.size_estimate(api_script, self.javascript["frequency"], api_script_frequency, self.javascript["testCount"]))
-                            break
-                        else:
-                            print("frequency is not valid, it should be in [1,120]")
+                pop_estimate_size["api_script"] = self.get_api_script_test()
+                if pop_estimate_size["api_script"]["testCount"] == 0:
+                    pop_estimate_size["javascript_pod_count"] = 0
                     break
-                elif api_script == 0:
-                    javascript_pod_count = 0
-                    break
-                else:
+                elif pop_estimate_size["api_script"]["testCount"] < 0:
                     print("Invalid input")
+                else:
+                    pop_estimate_size["javascript_pod_count"] = int(self.size_estimate(pop_estimate_size["api_script"]["testCount"], self.javascript["frequency"], pop_estimate_size["api_script"]["frequency"], self.javascript["testCount"]))
+                    break
 
             while True:
-                browser_script = int(self.ask_question("How many Browser tests (Webpage Action, Webpage Script and BrowserScript) do you want to create? (0 if no) "))
-                if browser_script > 0:
-                    while True:
-                        browser_script_frequency = int(self.ask_question("What is the test frequency for Browser tests? (1-120) "))
-                        if browser_script_frequency > 0 and browser_script_frequency <= 120:
-                            browserscript_pod_count = int(self.size_estimate(browser_script, self.browserscript["frequency"], browser_script_frequency, self.browserscript["testCount"]))
-                            break
-                        else:
-                            print("frequency is not valid, it should be in [1,120]")
-                    break
-                elif browser_script == 0:
-                    browserscript_pod_count = 0
+                pop_estimate_size["browser_script"] = self.get_browser_script_test()
+                if pop_estimate_size["browser_script"]["testCount"] == 0:
+                    pop_estimate_size["browserscript_pod_count"] = 0
                     break
-                else:
+                elif pop_estimate_size["browser_script"]["testCount"] < 0:
                     print("Invalid input")
+                else:
+                    pop_estimate_size["browserscript_pod_count"] = int(self.size_estimate(pop_estimate_size["browser_script"]["testCount"], self.browserscript["frequency"], pop_estimate_size["browser_script"]["frequency"], self.browserscript["testCount"]))
+                    break
 
-            agent = self.ask_question("Do you want to install the Instana-agent to monitor your PoP? (Y/N) ", options=["Y", "N", "y", "n"])
+            pop_estimate_size["agent"] = self.ask_question("Do you want to install the Instana-agent to monitor your PoP? (Y/N) ", options=["Y", "N", "y", "n"])
             while True:
-                if agent in ["y", "Y"]:
-                    worker_nodes = int(self.ask_question("How many worker nodes in your kubernetes cluster?  "))
-                    k8ssensor_pod_count = 3
-                    if worker_nodes <= 0:
+                if pop_estimate_size["agent"] in ["y", "Y"]:
+                    pop_estimate_size["worker_nodes"] = int(self.ask_question("How many worker nodes in your kubernetes cluster? "))
+                    if pop_estimate_size["worker_nodes"] <= 0:
                         print("Number of worker nodes must be greater than 0.")
-                    elif worker_nodes > 0:
+                    else:
+                        pop_estimate_size["k8ssensor_pod_count"] = 3 if pop_estimate_size["worker_nodes"] >= 3 else 1
                         break
                 else:
-                    worker_nodes = 0
-                    k8ssensor_pod_count = 0
+                    pop_estimate_size["worker_nodes"] = 0
+                    pop_estimate_size["k8ssensor_pod_count"] = 0
                     break
 
-            if api_simple == 0 and api_script == 0 and browser_script == 0:
-                controller_pod_count = 0
-                redis_pod_count = 0
-            else:
-                controller_pod_count = 1
-                redis_pod_count = 1
-
-            cpu = self.controller["cpuLimit"] * controller_pod_count + self.redis["cpuLimit"] * redis_pod_count + http_pod_count * self.http["cpuLimit"] + \
-                  javascript_pod_count * self.javascript["cpuLimit"] + browserscript_pod_count * self.browserscript["cpuLimit"] + \
-                  worker_nodes * self.agent["cpuLimit"] + self.k8ssensor["cpuLimit"] * k8ssensor_pod_count
-
-            memory = http_pod_count * self.http["memLimit"] + javascript_pod_count * self.javascript["memLimit"] + \
-                     browserscript_pod_count * self.browserscript["memLimit"] + worker_nodes * self.agent["memLimit"] +  \
-                     self.k8ssensor["memLimit"] * k8ssensor_pod_count +  self.controller["memLimit"] * controller_pod_count + \
-                     self.redis["memLimit"] * redis_pod_count
-
-            disk_size = http_pod_count * self.http["imageSize"] + javascript_pod_count * self.javascript["imageSize"] + \
-                        browserscript_pod_count * self.browserscript["imageSize"] + controller_pod_count * self.controller["imageSize"] + \
-                        redis_pod_count * self.redis["imageSize"] + worker_nodes * self.agent["imageSize"] + \
-                        k8ssensor_pod_count * self.k8ssensor["imageSize"]
-
-            max_label_length = max(len(str(api_simple)), len(str(api_script)), len(str(browser_script)), len(str(agent)))
-            print("\nYour requirement is:")
-            print(f"   API    Simple: {api_simple:<{max_label_length}}        Frequency: {api_simple_frequency}min" if api_simple > 0 else f"   API    Simple: {api_simple:<{max_label_length}}")
-            print(f"   API    Script: {api_script:<{max_label_length}}        Frequency: {api_script_frequency}min" if api_script > 0 else f"   API    Script: {api_script:<{max_label_length}}")
-            print(f"   Browser  Test: {browser_script:<{max_label_length}}        Frequency: {browser_script_frequency}min" if browser_script > 0 else f"   Browser  Test: {browser_script:<{max_label_length}}")
-            print(f"   Install Agent: {agent:<{max_label_length}}        Worker Nodes: {worker_nodes}" if agent == "Y" else f"   Install Agent: {agent:<{max_label_length}}")
-
-            print("\nThe estimated sizing is:")
-            print(f"   CPU:     {cpu}m")
-            print(f"   Memory:  {memory}Mi")
-            print(f"   Disk:    {disk_size/1000}GB")
-
-            print("\nThe recommended engine pods:")
-            print(f"   http           playback engines: {http_pod_count} \n"
-                  f"   javascript     playback engines: {javascript_pod_count} \n"
-                  f"   browserscript  playback engines: {browserscript_pod_count} ")
+            if pop_estimate_size["api_simple"]["testCount"] == 0 and pop_estimate_size["api_script"]["testCount"] == 0 and pop_estimate_size["browser_script"]["testCount"] == 0:
+                pop_estimate_size["controller_pod_count"] = 0
+                pop_estimate_size["redis_pod_count"] = 0
+            else:
+                pop_estimate_size["controller_pod_count"] = 1
+                pop_estimate_size["redis_pod_count"] = 1
+
+            pop_estimate_size["cpu"] = self.controller["cpuLimit"] * pop_estimate_size["controller_pod_count"] + self.redis["cpuLimit"] * pop_estimate_size["redis_pod_count"] + pop_estimate_size["http_pod_count"] * self.http["cpuLimit"] + \
+                  pop_estimate_size["javascript_pod_count"] * self.javascript["cpuLimit"] + pop_estimate_size["browserscript_pod_count"] * self.browserscript["cpuLimit"] + \
+                  pop_estimate_size["worker_nodes"] * self.agent["cpuLimit"] + self.k8ssensor["cpuLimit"] * pop_estimate_size["k8ssensor_pod_count"]
+
+            pop_estimate_size["memory"] = pop_estimate_size["http_pod_count"] * self.http["memLimit"] + pop_estimate_size["javascript_pod_count"] * self.javascript["memLimit"] + \
+                     pop_estimate_size["browserscript_pod_count"] * self.browserscript["memLimit"] + pop_estimate_size["worker_nodes"] * self.agent["memLimit"] +  \
+                     self.k8ssensor["memLimit"] * pop_estimate_size["k8ssensor_pod_count"] +  self.controller["memLimit"] * pop_estimate_size["controller_pod_count"] + \
+                     self.redis["memLimit"] * pop_estimate_size["redis_pod_count"]
+
+            pop_estimate_size["disk_size"] = pop_estimate_size["http_pod_count"] * self.http["imageSize"] + pop_estimate_size["javascript_pod_count"] * self.javascript["imageSize"] + \
+                        pop_estimate_size["browserscript_pod_count"] * self.browserscript["imageSize"] + pop_estimate_size["controller_pod_count"] * self.controller["imageSize"] + \
+                        pop_estimate_size["redis_pod_count"] * self.redis["imageSize"] + pop_estimate_size["worker_nodes"] * self.agent["imageSize"] + \
+                        pop_estimate_size["k8ssensor_pod_count"] * self.k8ssensor["imageSize"]
+
+            return pop_estimate_size
+        except ValueError as e:
+            self.exit_synctl(ERROR_CODE, f"Exception: {e}")
+
+    def pop_cost_estimate(self):
+        cost_estimate = {}
+
+        print("List price for 1 unit(part number) is $12/month and 1 part number entitles 1000 Resource Units (RU) per month.")
+        print("The relationship between RU and test executions are:\n"
+        "   ● 1 API Simple test executed = 0.025 RU \n"
+        "   ● 1 API Script test executed = 0.042 RU \n"
+        "   ● 1 Browser    test executed = 1 RU")
+        print("The minimum quantity per month is 30 part numbers, priced at $360.")
+
+        print("\nPlease answer below questions for estimating the cost of Synthetic tests running on Instana hosted PoPs.\n")
+        try:
+            while True:
+                cost_estimate["locations"] = int(self.ask_question("How many managed locations will be used? "))
+                if cost_estimate["locations"] > 0:
+                    while True:
+                        cost_estimate["api_simple"] = self.get_api_simple_test()
+                        if cost_estimate["api_simple"]["testCount"] == 0:
+                            cost_estimate["api_simple_test_exec"] = 0
+                            cost_estimate["api_simple_res"] = 0
+                            break
+                        elif cost_estimate["api_simple"]["testCount"] < 0:
+                            print("Invalid input")
+                        else:
+                            cost_estimate["api_simple_test_exec"] = self.test_exec_estimate(cost_estimate["api_simple"]["testCount"], cost_estimate["api_simple"]["frequency"], cost_estimate["locations"])
+                            # resource units per month
+                            cost_estimate["api_simple_res"] = cost_estimate["api_simple_test_exec"] * self.factors["APISimple"]
+                            break
+
+                    while True:
+                        cost_estimate["api_script"] = self.get_api_script_test()
+                        if cost_estimate["api_script"]["testCount"] == 0:
+                            cost_estimate["api_script_test_exec"] = 0
+                            cost_estimate["api_script_res"] = 0
+                            break
+                        elif cost_estimate["api_script"]["testCount"] < 0:
+                            print("Invalid input")
+                        else:
+                            cost_estimate["api_script_test_exec"] = self.test_exec_estimate(cost_estimate["api_script"]["testCount"], cost_estimate["api_script"]["frequency"], cost_estimate["locations"])
+                            cost_estimate["api_script_res"] = cost_estimate["api_script_test_exec"] * self.factors["APIScript"]
+                            break
+
+                    while True:
+                        cost_estimate["browser_script"] = self.get_browser_script_test()
+                        if cost_estimate["browser_script"]["testCount"] == 0:
+                            cost_estimate["browserscript_test_exec"] = 0
+                            cost_estimate["browserscript_res"] = 0
+                            break
+                        elif cost_estimate["browser_script"]["testCount"] < 0:
+                            print("Invalid input")
+                        else:
+                            cost_estimate["browserscript_test_exec"] = self.test_exec_estimate(cost_estimate["browser_script"]["testCount"], cost_estimate["browser_script"]["frequency"], cost_estimate["locations"])
+                            cost_estimate["browserscript_res"] = cost_estimate["browserscript_test_exec"] * self.factors["browserTest"]
+                            break
+
+                    # Total resource units per month
+                    cost_estimate["total_resource"] = cost_estimate["api_simple_res"] + cost_estimate["api_script_res"] + cost_estimate["browserscript_res"]
 
+                    # Total parts per month
+                    cost_estimate["total_parts"] = round(cost_estimate["total_resource"]/1000, 0)
+
+                    # Total estimated cost per month
+                    # List price for 1 unit = $12
+                    cost_estimate["total_cost"] = cost_estimate["total_parts"] * 12
+
+                    if cost_estimate["total_cost"] < 360:
+                        cost_estimate["total_resource"] = 29920.32
+                        cost_estimate["total_parts"] = 30.0
+                        cost_estimate["total_cost"] = 360.0
+
+                    return cost_estimate
+                else:
+                    print("number of locations cannot be less than 1")
         except ValueError as e:
-            print(f"Exception: {e}")
+            self.exit_synctl(ERROR_CODE,f"Exception: {e}")
+
+    def print_estimated_pop_size(self):
 
+        pop_estimate_size = self.pop_size_estimate()
+        max_label_length = max(len(str(pop_estimate_size["api_simple"]["testCount"])), len(str(pop_estimate_size["api_script"]["testCount"])), len(str(pop_estimate_size["browser_script"]["testCount"])), len(str(pop_estimate_size["agent"])))
+        print("\nYour requirement is:")
+        print(f'   API    Simple: {pop_estimate_size["api_simple"]["testCount"]:<{max_label_length},}           Frequency: {pop_estimate_size["api_simple"]["frequency"]}min' if pop_estimate_size["api_simple"]["testCount"] > 0 else f'   API    Simple: {pop_estimate_size["api_simple"]["testCount"]:<{max_label_length}}')
+        print(f'   API    Script: {pop_estimate_size["api_script"]["testCount"]:<{max_label_length},}           Frequency: {pop_estimate_size["api_script"]["frequency"]}min' if pop_estimate_size["api_script"]["testCount"] > 0 else f'   API    Script: {pop_estimate_size["api_script"]["testCount"]:<{max_label_length}}')
+        print(f'   Browser  Test: {pop_estimate_size["browser_script"]["testCount"]:<{max_label_length},}           Frequency: {pop_estimate_size["browser_script"]["frequency"]}min' if pop_estimate_size["browser_script"]["testCount"] > 0 else f'   Browser  Test: {pop_estimate_size["browser_script"]["testCount"]:<{max_label_length}}')
+        agent_yes = "Yes" if pop_estimate_size["agent"] in ["y", "Y"] else "No"
+        print(f'   Install Agent: {agent_yes:<{max_label_length}}        Worker Nodes: {pop_estimate_size["worker_nodes"]}' if pop_estimate_size["agent"].upper() == "Y" else f'   Install Agent: {agent_yes:<{max_label_length}}')
+
+        print("\nThe estimated sizing is:")
+        print(f'   CPU:     {pop_estimate_size["cpu"]:,}m')
+        print(f'   Memory:  {pop_estimate_size["memory"]:,}Mi')
+        print(f'   Disk:    {pop_estimate_size["disk_size"]/1000:,}GB')
+
+        print("\nThe recommended engine pods:")
+        print(f'   http           playback engines: {pop_estimate_size["http_pod_count"]} \n'
+              f'   javascript     playback engines: {pop_estimate_size["javascript_pod_count"]} \n'
+              f'   browserscript  playback engines: {pop_estimate_size["browserscript_pod_count"]}')
+
+    def print_estimated_cost(self):
+
+        cost_estimate = self.pop_cost_estimate()
+        print(f'\nThe total executions per month:\n    API   Simple executions: {cost_estimate["api_simple_test_exec"]:,}')
+        print(f'    API   Script executions: {cost_estimate["api_script_test_exec"]:,}')
+        print(f'    Browser Test executions: {cost_estimate["browserscript_test_exec"]:,}\n')
+
+        print(f'The total cost estimated:\n    Cost per month is: ${cost_estimate["total_cost"]:,}')
+        print(f'    Number of part numbers per month is: {cost_estimate["total_parts"]:,}')
+        print(f'    Resource Units per month is: {cost_estimate["total_resource"]:,}')
 
 class ConfigurationFile(Base):
     def __init__(self) -> None:
         Base.__init__(self)
 
         HOME_PATH = self.get_home_path()
         self.CONFIG_FOLDER = HOME_PATH + "/.synthetic/"
@@ -4054,15 +4178,15 @@
 
         self.parser_create = sub_parsers.add_parser(
             'create', help='create a Synthetic test, credential or alert', add_help=True, usage=CREATE_USAGE)
         self.parser_create._positionals.title = POSITION_PARAMS
         self.parser_create._optionals.title = OPTIONS_PARAMS
 
         self.parser_get = sub_parsers.add_parser(
-            'get', help='get Synthetic test, location, credential, alert or pop-size', usage=GET_USAGE)
+            'get', help='get Synthetic test, location, credential, alert, pop-size or pop-cost', usage=GET_USAGE)
         self.parser_get._positionals.title = POSITION_PARAMS
         self.parser_get._optionals.title = OPTIONS_PARAMS
 
         self.parser_patch = sub_parsers.add_parser(
             'patch', help='patch a Synthetic test', usage=PATCH_USAGE)
         self.parser_patch._positionals.title = POSITION_PARAMS
         self.parser_patch._optionals.title = OPTIONS_PARAMS
@@ -4210,15 +4334,15 @@
             '--host', type=str, metavar="<host>", help='set hostname')
         self.parser_create.add_argument(
             '--token', type=str, metavar="<token>", help='set token')
 
 
     def get_command_options(self):
         self.parser_get.add_argument(
-            'op_type', choices=['location', 'lo', 'test', 'application', 'app', 'cred', 'alert', 'alert-channel', 'result', 'pop-size'],
+            'op_type', choices=['location', 'lo', 'test', 'application', 'app', 'cred', 'alert', 'alert-channel', 'result', 'pop-size', 'size', 'pop-cost', 'cost'],
             help="command list")
         # parser_get.add_argument('type_id', type=str,
         #                         required=False, help='test id or location id')
         self.parser_get.add_argument(
             '--type', '-t', type=int, choices=[0, 1, 2, 3, 4], metavar='<int>', help='Synthetic type, 0 HTTPAction, 1 HTTPScript, 2 BrowserScript, 3 WebpageScript, 4 WebpageAction')
         self.parser_get.add_argument(
             'id', type=str, nargs="?", help='Synthetic test id')
@@ -4677,16 +4801,18 @@
                     if get_args.har is None:
                         a_result_details = syn_instance.retrieve_test_result_details(get_args.id, get_args.test)
                     else:
                         a_result_details = syn_instance.retrieve_test_result_details(get_args.id, get_args.test, get_args.har)
                     syn_instance.print_result_details(a_result_details, test_result["items"])
             else:
                 print('testid is required')
-        elif get_args.op_type == POP_SIZE:
-            pop_estimate.pop_size_estimate()
+        elif get_args.op_type == POP_SIZE or get_args.op_type == 'size':
+            pop_estimate.print_estimated_pop_size()
+        elif get_args.op_type == POP_COST or get_args.op_type == 'cost':
+            pop_estimate.print_estimated_cost()
     elif COMMAND_CREATE == get_args.sub_command:
         if get_args.syn_type == SYN_CRED:
             cred_payload = CredentialConfiguration()
             if get_args.key is not None:
                 cred_payload.set_credential_name(get_args.key)
             if get_args.value is not None:
                 cred_payload.set_credential_value(get_args.value)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `synctl-1.1.8/synctl.egg-info/PKG-INFO` & `synctl-1.1.9/synctl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synctl
-Version: 1.1.8
+Version: 1.1.9
 Summary: Instana Synthetic CLI
 Home-page: https://github.com/instana/synthetic-synctl
 Author: Rong Zhu Shang, Swetha Lohith
 Author-email: shangrz@cn.ibm.com, Swetha.Lohith@ibm.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/instana/synthetic-synctl/issues
 Project-URL: Source, https://github.com/instana/synthetic-synctl
```

### Comparing `synctl-1.1.8/tests/test_synctl.py` & `synctl-1.1.9/tests/test_synctl.py`

 * *Files identical despite different names*

