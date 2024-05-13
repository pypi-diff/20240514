# Comparing `tmp/sarathi-0.0.3.tar.gz` & `tmp/sarathi-0.0.4a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sarathi-0.0.3.tar", last modified: Sun May 12 07:37:38 2024, max compression
+gzip compressed data, was "sarathi-0.0.4a0.tar", last modified: Mon May 13 23:44:17 2024, max compression
```

## Comparing `sarathi-0.0.3.tar` & `sarathi-0.0.4a0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxrwxrwx   0     1000     1000        0 2024-05-12 07:37:38.284242 sarathi-0.0.3/
--rwxrwxrwx   0     1000     1000     1072 2024-03-29 02:09:03.000000 sarathi-0.0.3/LICENSE
--rwxrwxrwx   0     1000     1000     2395 2024-05-12 07:37:38.284242 sarathi-0.0.3/PKG-INFO
--rwxrwxrwx   0     1000     1000     1747 2024-05-12 06:33:49.000000 sarathi-0.0.3/README.md
--rwxrwxrwx   0     1000     1000       38 2024-05-12 07:37:38.284242 sarathi-0.0.3/setup.cfg
--rwxrwxrwx   0     1000     1000     1170 2024-05-12 07:36:33.000000 sarathi-0.0.3/setup.py
-drwxrwxrwx   0     1000     1000        0 2024-05-12 07:37:37.990730 sarathi-0.0.3/src/
-drwxrwxrwx   0     1000     1000        0 2024-05-12 07:37:38.028687 sarathi-0.0.3/src/sarathi/
--rwxrwxrwx   0     1000     1000        0 2024-05-12 03:13:37.000000 sarathi-0.0.3/src/sarathi/__init__.py
-drwxrwxrwx   0     1000     1000        0 2024-05-12 07:37:38.172540 sarathi-0.0.3/src/sarathi/cli/
--rwxrwxrwx   0     1000     1000        0 2024-05-12 03:13:37.000000 sarathi-0.0.3/src/sarathi/cli/__init__.py
--rwxrwxrwx   0     1000     1000     1477 2024-05-12 06:11:13.000000 sarathi-0.0.3/src/sarathi/cli/cli_handler.py
--rwxrwxrwx   0     1000     1000     1711 2024-05-12 06:26:08.000000 sarathi-0.0.3/src/sarathi/cli/gendocstrings.py
--rwxrwxrwx   0     1000     1000      883 2024-05-12 06:11:13.000000 sarathi-0.0.3/src/sarathi/cli/qahelper.py
--rwxrwxrwx   0     1000     1000     2137 2024-05-12 06:11:13.000000 sarathi-0.0.3/src/sarathi/cli/sgit.py
-drwxrwxrwx   0     1000     1000        0 2024-05-12 07:37:38.199410 sarathi-0.0.3/src/sarathi/code/
--rwxrwxrwx   0     1000     1000        0 2024-05-12 03:13:37.000000 sarathi-0.0.3/src/sarathi/code/__init__.py
--rwxrwxrwx   0     1000     1000     4715 2024-05-12 06:11:13.000000 sarathi-0.0.3/src/sarathi/code/codetasks.py
-drwxrwxrwx   0     1000     1000        0 2024-05-12 07:37:38.244124 sarathi-0.0.3/src/sarathi/llm/
--rwxrwxrwx   0     1000     1000        0 2024-05-12 03:13:37.000000 sarathi-0.0.3/src/sarathi/llm/__init__.py
--rwxrwxrwx   0     1000     1000     1516 2024-05-12 03:13:37.000000 sarathi-0.0.3/src/sarathi/llm/call_llm.py
--rwxrwxrwx   0     1000     1000     2683 2024-05-12 03:13:37.000000 sarathi-0.0.3/src/sarathi/llm/prompts.py
-drwxrwxrwx   0     1000     1000        0 2024-05-12 07:37:38.274325 sarathi-0.0.3/src/sarathi/utils/
--rwxrwxrwx   0     1000     1000      507 2024-05-12 03:13:38.000000 sarathi-0.0.3/src/sarathi/utils/formatters.py
--rwxrwxrwx   0     1000     1000     2220 2024-05-12 03:13:38.000000 sarathi-0.0.3/src/sarathi/utils/io.py
-drwxrwxrwx   0     1000     1000        0 2024-05-12 07:37:38.099558 sarathi-0.0.3/src/sarathi.egg-info/
--rwxrwxrwx   0     1000     1000     2395 2024-05-12 07:37:37.000000 sarathi-0.0.3/src/sarathi.egg-info/PKG-INFO
--rwxrwxrwx   0     1000     1000      604 2024-05-12 07:37:37.000000 sarathi-0.0.3/src/sarathi.egg-info/SOURCES.txt
--rwxrwxrwx   0     1000     1000        1 2024-05-12 07:37:37.000000 sarathi-0.0.3/src/sarathi.egg-info/dependency_links.txt
--rwxrwxrwx   0     1000     1000       57 2024-05-12 07:37:37.000000 sarathi-0.0.3/src/sarathi.egg-info/entry_points.txt
--rwxrwxrwx   0     1000     1000       47 2024-05-12 07:37:37.000000 sarathi-0.0.3/src/sarathi.egg-info/requires.txt
--rwxrwxrwx   0     1000     1000        8 2024-05-12 07:37:37.000000 sarathi-0.0.3/src/sarathi.egg-info/top_level.txt
+drwxrwxrwx   0     1000     1000        0 2024-05-13 23:44:17.980162 sarathi-0.0.4a0/
+-rwxrwxrwx   0     1000     1000     1072 2024-03-29 02:09:03.000000 sarathi-0.0.4a0/LICENSE
+-rwxrwxrwx   0     1000     1000     2283 2024-05-13 23:44:17.928030 sarathi-0.0.4a0/PKG-INFO
+-rwxrwxrwx   0     1000     1000     1633 2024-05-13 23:42:07.000000 sarathi-0.0.4a0/README.md
+-rwxrwxrwx   0     1000     1000       38 2024-05-13 23:44:17.980162 sarathi-0.0.4a0/setup.cfg
+-rwxrwxrwx   0     1000     1000     1171 2024-05-13 23:37:44.000000 sarathi-0.0.4a0/setup.py
+drwxrwxrwx   0     1000     1000        0 2024-05-13 23:44:17.311336 sarathi-0.0.4a0/src/
+drwxrwxrwx   0     1000     1000        0 2024-05-13 23:44:17.416645 sarathi-0.0.4a0/src/sarathi/
+-rwxrwxrwx   0     1000     1000        0 2024-05-12 03:13:37.000000 sarathi-0.0.4a0/src/sarathi/__init__.py
+-rwxrwxrwx   0     1000     1000      216 2024-05-12 07:56:43.000000 sarathi-0.0.4a0/src/sarathi/ab.py
+drwxrwxrwx   0     1000     1000        0 2024-05-13 23:44:17.727115 sarathi-0.0.4a0/src/sarathi/cli/
+-rwxrwxrwx   0     1000     1000        0 2024-05-12 03:13:37.000000 sarathi-0.0.4a0/src/sarathi/cli/__init__.py
+-rwxrwxrwx   0     1000     1000     1477 2024-05-12 06:11:13.000000 sarathi-0.0.4a0/src/sarathi/cli/cli_handler.py
+-rwxrwxrwx   0     1000     1000     1711 2024-05-12 06:26:08.000000 sarathi-0.0.4a0/src/sarathi/cli/gendocstrings.py
+-rwxrwxrwx   0     1000     1000      883 2024-05-12 06:11:13.000000 sarathi-0.0.4a0/src/sarathi/cli/qahelper.py
+-rwxrwxrwx   0     1000     1000     2137 2024-05-12 06:11:13.000000 sarathi-0.0.4a0/src/sarathi/cli/sgit.py
+drwxrwxrwx   0     1000     1000        0 2024-05-13 23:44:17.816929 sarathi-0.0.4a0/src/sarathi/code/
+-rwxrwxrwx   0     1000     1000        0 2024-05-12 03:13:37.000000 sarathi-0.0.4a0/src/sarathi/code/__init__.py
+-rwxrwxrwx   0     1000     1000     4715 2024-05-12 06:11:13.000000 sarathi-0.0.4a0/src/sarathi/code/codetasks.py
+drwxrwxrwx   0     1000     1000        0 2024-05-13 23:44:17.878566 sarathi-0.0.4a0/src/sarathi/llm/
+-rwxrwxrwx   0     1000     1000        0 2024-05-12 03:13:37.000000 sarathi-0.0.4a0/src/sarathi/llm/__init__.py
+-rwxrwxrwx   0     1000     1000     1516 2024-05-12 03:13:37.000000 sarathi-0.0.4a0/src/sarathi/llm/call_llm.py
+-rwxrwxrwx   0     1000     1000     2683 2024-05-12 03:13:37.000000 sarathi-0.0.4a0/src/sarathi/llm/prompts.py
+drwxrwxrwx   0     1000     1000        0 2024-05-13 23:44:17.919798 sarathi-0.0.4a0/src/sarathi/utils/
+-rwxrwxrwx   0     1000     1000      507 2024-05-12 03:13:38.000000 sarathi-0.0.4a0/src/sarathi/utils/formatters.py
+-rwxrwxrwx   0     1000     1000     2220 2024-05-12 03:13:38.000000 sarathi-0.0.4a0/src/sarathi/utils/io.py
+drwxrwxrwx   0     1000     1000        0 2024-05-13 23:44:17.548917 sarathi-0.0.4a0/src/sarathi.egg-info/
+-rwxrwxrwx   0     1000     1000     2283 2024-05-13 23:44:16.000000 sarathi-0.0.4a0/src/sarathi.egg-info/PKG-INFO
+-rwxrwxrwx   0     1000     1000      622 2024-05-13 23:44:16.000000 sarathi-0.0.4a0/src/sarathi.egg-info/SOURCES.txt
+-rwxrwxrwx   0     1000     1000        1 2024-05-13 23:44:16.000000 sarathi-0.0.4a0/src/sarathi.egg-info/dependency_links.txt
+-rwxrwxrwx   0     1000     1000       57 2024-05-13 23:44:16.000000 sarathi-0.0.4a0/src/sarathi.egg-info/entry_points.txt
+-rwxrwxrwx   0     1000     1000       47 2024-05-13 23:44:16.000000 sarathi-0.0.4a0/src/sarathi.egg-info/requires.txt
+-rwxrwxrwx   0     1000     1000        8 2024-05-13 23:44:16.000000 sarathi-0.0.4a0/src/sarathi.egg-info/top_level.txt
```

### Comparing `sarathi-0.0.3/LICENSE` & `sarathi-0.0.4a0/LICENSE`

 * *Files identical despite different names*

### Comparing `sarathi-0.0.3/PKG-INFO` & `sarathi-0.0.4a0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarathi
-Version: 0.0.3
+Version: 0.0.4a0
 Summary: A CLI coding assistant
 Home-page: https://github.com/abhishek9sharma/sarathi
 Author: Abhishek Sharma
 License: MIT
 Project-URL: Bug Reports, https://github.com/abhishek9sharma/sarathi/issues
 Project-URL: Source, https://github.com/abhishek9sharma/sarathi
 Keywords: cli coding assistant
@@ -18,38 +18,37 @@
 License-File: LICENSE
 
 # sarathi
 A CLI coding assistant
 
 
 ## Installation
-You can install the package from the GitHub repository using pip. Make sure you have Python and pip installed on your system.
+You can install the package using below command. Make sure you have Python and pip installed on your system.
     
         - pip install sarathi
-        - pip install https://github.com/abhishek9sharma/sarathi.git
-
+ 
 ## Setting OpenAI API Key
 To use certain features of this package, you need to set up your OpenAI API key. If you don't have one, you can sign up for an account on the [OpenAI website](https://openai.com/product). Once you have your API key, you can set it in your environment variables. Here's how you can do it:
 
 ### For Linux/macOS:
 
     - export OPENAI_API_KEY=YOUR_API_KEY
 
 
 ## Usage
 
 #### Generating Git Commit Messages
 Sarathi provides a convenient command `sarathi git autocommit` to generate commit messages for Git commits. 
 - Stage the files you want to commit
-- Run `sarathi git autocommit`. This command will automatically analyze your staged changes (using git add .), generate a commit message, and if you confirm will commit your changes to the repository with the generate message
+- Run `sarathi git autocommit`. This command will automatically analyze your staged changes, generate a commit message via OPEN AI, show the generated message to you, and if you confirm, will commit your changes to the repository with the generated message.
 
 #### Generating docstring messages
-You can generate docstrings for your python code using the below commands.
+You can generate docstrings for your python code using commands such as below
 
-- Run `sarathi docstrgen -f /scratchpad/ghmount/sarathi/src/sarathi/utils/formatters.py`. This command analyze the methods in the file passed and generates docstrings for functions if they do not exist.
-- Run `sarathi docstrgen -d /scratchpad/ghmount/sarathi/src/sarathi/`. This command analyzes the methods in all files presend in the directory specified and generates docstrings for functions if they do not exist.
+- Run `sarathi docstrgen -f src/sarathi/code/codetasks.py`. This command analyzes the methods in the file provided in the argument, and generates docstrings for functions.
+- Run `sarathi docstrgen -d src/sarathi/`. This command analyzes the methods in all files present in the directory provided in the argument,  and generates docstrings for function.
 
 
 ## Helpul references
     - https://dev.to/taikedz/ive-parked-my-side-projects-3o62
     - https://github.com/lightningorb/autocommit
```

### Comparing `sarathi-0.0.3/README.md` & `sarathi-0.0.4a0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 # sarathi
 A CLI coding assistant
 
 
 ## Installation
-You can install the package from the GitHub repository using pip. Make sure you have Python and pip installed on your system.
+You can install the package using below command. Make sure you have Python and pip installed on your system.
     
         - pip install sarathi
-        - pip install https://github.com/abhishek9sharma/sarathi.git
-
+ 
 ## Setting OpenAI API Key
 To use certain features of this package, you need to set up your OpenAI API key. If you don't have one, you can sign up for an account on the [OpenAI website](https://openai.com/product). Once you have your API key, you can set it in your environment variables. Here's how you can do it:
 
 ### For Linux/macOS:
 
     - export OPENAI_API_KEY=YOUR_API_KEY
 
 
 ## Usage
 
 #### Generating Git Commit Messages
 Sarathi provides a convenient command `sarathi git autocommit` to generate commit messages for Git commits. 
 - Stage the files you want to commit
-- Run `sarathi git autocommit`. This command will automatically analyze your staged changes (using git add .), generate a commit message, and if you confirm will commit your changes to the repository with the generate message
+- Run `sarathi git autocommit`. This command will automatically analyze your staged changes, generate a commit message via OPEN AI, show the generated message to you, and if you confirm, will commit your changes to the repository with the generated message.
 
 #### Generating docstring messages
-You can generate docstrings for your python code using the below commands.
+You can generate docstrings for your python code using commands such as below
 
-- Run `sarathi docstrgen -f /scratchpad/ghmount/sarathi/src/sarathi/utils/formatters.py`. This command analyze the methods in the file passed and generates docstrings for functions if they do not exist.
-- Run `sarathi docstrgen -d /scratchpad/ghmount/sarathi/src/sarathi/`. This command analyzes the methods in all files presend in the directory specified and generates docstrings for functions if they do not exist.
+- Run `sarathi docstrgen -f src/sarathi/code/codetasks.py`. This command analyzes the methods in the file provided in the argument, and generates docstrings for functions.
+- Run `sarathi docstrgen -d src/sarathi/`. This command analyzes the methods in all files present in the directory provided in the argument,  and generates docstrings for function.
 
 
 ## Helpul references
     - https://dev.to/taikedz/ive-parked-my-side-projects-3o62
     - https://github.com/lightningorb/autocommit
```

### Comparing `sarathi-0.0.3/setup.py` & `sarathi-0.0.4a0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_namespace_packages, find_packages, setup
 
 setup(
     name="sarathi",
-    version="0.0.3",
+    version="0.0.4a",
     description="A CLI coding assistant",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/abhishek9sharma/sarathi",
     author="Abhishek Sharma",
     license="MIT",
     classifiers=[
```

### Comparing `sarathi-0.0.3/src/sarathi/cli/cli_handler.py` & `sarathi-0.0.4a0/src/sarathi/cli/cli_handler.py`

 * *Files identical despite different names*

### Comparing `sarathi-0.0.3/src/sarathi/cli/gendocstrings.py` & `sarathi-0.0.4a0/src/sarathi/cli/gendocstrings.py`

 * *Files identical despite different names*

### Comparing `sarathi-0.0.3/src/sarathi/cli/qahelper.py` & `sarathi-0.0.4a0/src/sarathi/cli/qahelper.py`

 * *Files identical despite different names*

### Comparing `sarathi-0.0.3/src/sarathi/cli/sgit.py` & `sarathi-0.0.4a0/src/sarathi/cli/sgit.py`

 * *Files identical despite different names*

### Comparing `sarathi-0.0.3/src/sarathi/code/codetasks.py` & `sarathi-0.0.4a0/src/sarathi/code/codetasks.py`

 * *Files identical despite different names*

### Comparing `sarathi-0.0.3/src/sarathi/llm/call_llm.py` & `sarathi-0.0.4a0/src/sarathi/llm/call_llm.py`

 * *Files identical despite different names*

### Comparing `sarathi-0.0.3/src/sarathi/llm/prompts.py` & `sarathi-0.0.4a0/src/sarathi/llm/prompts.py`

 * *Files identical despite different names*

### Comparing `sarathi-0.0.3/src/sarathi/utils/io.py` & `sarathi-0.0.4a0/src/sarathi/utils/io.py`

 * *Files identical despite different names*

### Comparing `sarathi-0.0.3/src/sarathi.egg-info/PKG-INFO` & `sarathi-0.0.4a0/src/sarathi.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarathi
-Version: 0.0.3
+Version: 0.0.4a0
 Summary: A CLI coding assistant
 Home-page: https://github.com/abhishek9sharma/sarathi
 Author: Abhishek Sharma
 License: MIT
 Project-URL: Bug Reports, https://github.com/abhishek9sharma/sarathi/issues
 Project-URL: Source, https://github.com/abhishek9sharma/sarathi
 Keywords: cli coding assistant
@@ -18,38 +18,37 @@
 License-File: LICENSE
 
 # sarathi
 A CLI coding assistant
 
 
 ## Installation
-You can install the package from the GitHub repository using pip. Make sure you have Python and pip installed on your system.
+You can install the package using below command. Make sure you have Python and pip installed on your system.
     
         - pip install sarathi
-        - pip install https://github.com/abhishek9sharma/sarathi.git
-
+ 
 ## Setting OpenAI API Key
 To use certain features of this package, you need to set up your OpenAI API key. If you don't have one, you can sign up for an account on the [OpenAI website](https://openai.com/product). Once you have your API key, you can set it in your environment variables. Here's how you can do it:
 
 ### For Linux/macOS:
 
     - export OPENAI_API_KEY=YOUR_API_KEY
 
 
 ## Usage
 
 #### Generating Git Commit Messages
 Sarathi provides a convenient command `sarathi git autocommit` to generate commit messages for Git commits. 
 - Stage the files you want to commit
-- Run `sarathi git autocommit`. This command will automatically analyze your staged changes (using git add .), generate a commit message, and if you confirm will commit your changes to the repository with the generate message
+- Run `sarathi git autocommit`. This command will automatically analyze your staged changes, generate a commit message via OPEN AI, show the generated message to you, and if you confirm, will commit your changes to the repository with the generated message.
 
 #### Generating docstring messages
-You can generate docstrings for your python code using the below commands.
+You can generate docstrings for your python code using commands such as below
 
-- Run `sarathi docstrgen -f /scratchpad/ghmount/sarathi/src/sarathi/utils/formatters.py`. This command analyze the methods in the file passed and generates docstrings for functions if they do not exist.
-- Run `sarathi docstrgen -d /scratchpad/ghmount/sarathi/src/sarathi/`. This command analyzes the methods in all files presend in the directory specified and generates docstrings for functions if they do not exist.
+- Run `sarathi docstrgen -f src/sarathi/code/codetasks.py`. This command analyzes the methods in the file provided in the argument, and generates docstrings for functions.
+- Run `sarathi docstrgen -d src/sarathi/`. This command analyzes the methods in all files present in the directory provided in the argument,  and generates docstrings for function.
 
 
 ## Helpul references
     - https://dev.to/taikedz/ive-parked-my-side-projects-3o62
     - https://github.com/lightningorb/autocommit
```

### Comparing `sarathi-0.0.3/src/sarathi.egg-info/SOURCES.txt` & `sarathi-0.0.4a0/src/sarathi.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 setup.py
 src/sarathi/__init__.py
+src/sarathi/ab.py
 src/sarathi.egg-info/PKG-INFO
 src/sarathi.egg-info/SOURCES.txt
 src/sarathi.egg-info/dependency_links.txt
 src/sarathi.egg-info/entry_points.txt
 src/sarathi.egg-info/requires.txt
 src/sarathi.egg-info/top_level.txt
 src/sarathi/cli/__init__.py
```

