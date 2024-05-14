# Comparing `tmp/atksh_utils-0.8.7.tar.gz` & `tmp/atksh_utils-0.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atksh_utils-0.8.7.tar", last modified: Sat Apr 27 00:27:48 2024, max compression
+gzip compressed data, was "atksh_utils-0.8.8.tar", last modified: Tue May 14 08:04:01 2024, max compression
```

## Comparing `atksh_utils-0.8.7.tar` & `atksh_utils-0.8.8.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:27:48.842633 atksh_utils-0.8.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:27:48.834633 atksh_utils-0.8.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:27:48.838633 atksh_utils-0.8.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-27 00:27:41.000000 atksh_utils-0.8.7/.github/workflows/publish_to_pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-04-27 00:27:41.000000 atksh_utils-0.8.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-27 00:27:41.000000 atksh_utils-0.8.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-27 00:27:41.000000 atksh_utils-0.8.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7969 2024-04-27 00:27:48.842633 atksh_utils-0.8.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-04-27 00:27:41.000000 atksh_utils-0.8.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-27 00:27:41.000000 atksh_utils-0.8.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-27 00:27:48.842633 atksh_utils-0.8.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:27:48.834633 atksh_utils-0.8.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:27:48.838633 atksh_utils-0.8.7/src/atksh_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 00:27:41.000000 atksh_utils-0.8.7/src/atksh_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:27:48.842633 atksh_utils-0.8.7/src/atksh_utils/basic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 00:27:41.000000 atksh_utils-0.8.7/src/atksh_utils/basic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-27 00:27:41.000000 atksh_utils-0.8.7/src/atksh_utils/basic/functools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:27:48.842633 atksh_utils-0.8.7/src/atksh_utils/nlp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 00:27:41.000000 atksh_utils-0.8.7/src/atksh_utils/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-04-27 00:27:41.000000 atksh_utils-0.8.7/src/atksh_utils/nlp/str_kernel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:27:48.842633 atksh_utils-0.8.7/src/atksh_utils/openai/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-27 00:27:41.000000 atksh_utils-0.8.7/src/atksh_utils/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25789 2024-04-27 00:27:41.000000 atksh_utils-0.8.7/src/atksh_utils/openai/api.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6457 2024-04-27 00:27:41.000000 atksh_utils-0.8.7/src/atksh_utils/openai/askgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     6710 2024-04-27 00:27:41.000000 atksh_utils-0.8.7/src/atksh_utils/openai/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 00:27:41.000000 atksh_utils-0.8.7/src/atksh_utils/openai/history.py
--rw-r--r--   0 runner    (1001) docker     (127)     8388 2024-04-27 00:27:41.000000 atksh_utils-0.8.7/src/atksh_utils/openai/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-27 00:27:41.000000 atksh_utils-0.8.7/src/atksh_utils/openai/token.py
--rw-r--r--   0 runner    (1001) docker     (127)    21570 2024-04-27 00:27:41.000000 atksh_utils-0.8.7/src/atksh_utils/openai/tool.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-27 00:27:48.000000 atksh_utils-0.8.7/src/atksh_utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:27:48.842633 atksh_utils-0.8.7/src/atksh_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7969 2024-04-27 00:27:48.000000 atksh_utils-0.8.7/src/atksh_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-27 00:27:48.000000 atksh_utils-0.8.7/src/atksh_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 00:27:48.000000 atksh_utils-0.8.7/src/atksh_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-27 00:27:48.000000 atksh_utils-0.8.7/src/atksh_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-27 00:27:48.000000 atksh_utils-0.8.7/src/atksh_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-27 00:27:48.000000 atksh_utils-0.8.7/src/atksh_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:27:48.842633 atksh_utils-0.8.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 00:27:41.000000 atksh_utils-0.8.7/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:01.877420 atksh_utils-0.8.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:01.869420 atksh_utils-0.8.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:01.869420 atksh_utils-0.8.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-14 08:03:49.000000 atksh_utils-0.8.8/.github/workflows/publish_to_pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-14 08:03:49.000000 atksh_utils-0.8.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-14 08:03:49.000000 atksh_utils-0.8.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-14 08:03:49.000000 atksh_utils-0.8.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7945 2024-05-14 08:04:01.877420 atksh_utils-0.8.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5770 2024-05-14 08:03:49.000000 atksh_utils-0.8.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-14 08:03:49.000000 atksh_utils-0.8.8/demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-14 08:03:49.000000 atksh_utils-0.8.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-14 08:04:01.877420 atksh_utils-0.8.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:01.869420 atksh_utils-0.8.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:01.873420 atksh_utils-0.8.8/src/atksh_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:03:49.000000 atksh_utils-0.8.8/src/atksh_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:01.873420 atksh_utils-0.8.8/src/atksh_utils/basic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:03:49.000000 atksh_utils-0.8.8/src/atksh_utils/basic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-14 08:03:49.000000 atksh_utils-0.8.8/src/atksh_utils/basic/functools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:01.873420 atksh_utils-0.8.8/src/atksh_utils/nlp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:03:49.000000 atksh_utils-0.8.8/src/atksh_utils/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-05-14 08:03:49.000000 atksh_utils-0.8.8/src/atksh_utils/nlp/str_kernel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:01.873420 atksh_utils-0.8.8/src/atksh_utils/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-14 08:03:49.000000 atksh_utils-0.8.8/src/atksh_utils/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25784 2024-05-14 08:03:49.000000 atksh_utils-0.8.8/src/atksh_utils/openai/api.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6304 2024-05-14 08:03:49.000000 atksh_utils-0.8.8/src/atksh_utils/openai/askgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6710 2024-05-14 08:03:49.000000 atksh_utils-0.8.8/src/atksh_utils/openai/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:03:49.000000 atksh_utils-0.8.8/src/atksh_utils/openai/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8388 2024-05-14 08:03:49.000000 atksh_utils-0.8.8/src/atksh_utils/openai/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-14 08:03:49.000000 atksh_utils-0.8.8/src/atksh_utils/openai/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21489 2024-05-14 08:03:49.000000 atksh_utils-0.8.8/src/atksh_utils/openai/tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-14 08:04:01.000000 atksh_utils-0.8.8/src/atksh_utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:01.877420 atksh_utils-0.8.8/src/atksh_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7945 2024-05-14 08:04:01.000000 atksh_utils-0.8.8/src/atksh_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-14 08:04:01.000000 atksh_utils-0.8.8/src/atksh_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 08:04:01.000000 atksh_utils-0.8.8/src/atksh_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-14 08:04:01.000000 atksh_utils-0.8.8/src/atksh_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-14 08:04:01.000000 atksh_utils-0.8.8/src/atksh_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 08:04:01.000000 atksh_utils-0.8.8/src/atksh_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:04:01.873420 atksh_utils-0.8.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:03:49.000000 atksh_utils-0.8.8/tests/__init__.py
```

### Comparing `atksh_utils-0.8.7/.github/workflows/publish_to_pypi.yaml` & `atksh_utils-0.8.8/.github/workflows/publish_to_pypi.yaml`

 * *Files identical despite different names*

### Comparing `atksh_utils-0.8.7/.gitignore` & `atksh_utils-0.8.8/.gitignore`

 * *Files identical despite different names*

### Comparing `atksh_utils-0.8.7/LICENSE` & `atksh_utils-0.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `atksh_utils-0.8.7/PKG-INFO` & `atksh_utils-0.8.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atksh-utils
-Version: 0.8.7
+Version: 0.8.8
 Summary: atksh's utils
 Home-page: https://github.com/atksh/atksh_utils
 Author: atksh
 License: MIT License
         
         Copyright (c) 2023 atksh
         
@@ -25,27 +25,27 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: openai~=1.23.6
+Requires-Dist: openai~=1.29.0
 Requires-Dist: beautifulsoup4<5.0.0,>=4.11.1
 Requires-Dist: requests<3.0.0,>=2.0.0
 Requires-Dist: duckduckgo_search~=4.1.1
 Requires-Dist: dill<0.4.0,>=0.3.7
 Requires-Dist: numba<0.59.0,>=0.56.4
 Requires-Dist: pylatexenc==2.10
 Requires-Dist: scipy<2.0.0,>=1.9.0
 Requires-Dist: sympy<2.0.0,>=1.9.0
 Requires-Dist: soundfile<0.13.0,>=0.12.1
 Requires-Dist: sounddevice<0.5.0,>=0.4.6
 Requires-Dist: pypdf~=3.17.2
-Requires-Dist: tiktoken~=0.5.2
+Requires-Dist: tiktoken~=0.7.0
 Requires-Dist: backoff<3.0.0,>=2.2.1
 Provides-Extra: dev
 Requires-Dist: black~=23.0.0; extra == "dev"
 Requires-Dist: pytest~=7.2.2; extra == "dev"
 Requires-Dist: isort~=5.12.0; extra == "dev"
 Requires-Dist: pre-commit~=3.2.2; extra == "dev"
 
@@ -151,15 +151,15 @@
 python -m pip install -e '.[dev]'
 pre-commit install
 ```
 
 ## OpenAI
 
 ```python
-ai = OpenAI(key, "gpt-3.5-turbo-1106")
+ai = OpenAI(key, "gpt-4o")
 
 print(ai("Just answer the value of (5243 + 642) x (5314 - 4231) // 100"))
 # The value of the expression (5243 + 642) x (5314 - 4231) // 100 is 7112.
 
 
 def mul(a: int, b: int) -> int:
     """This is a multiplication function.
@@ -217,12 +217,12 @@
 ai.set_function(sub)
 ai.set_function(div)
 
 print(ai("Just answer the value of (5243 + 642) x (5314 - 4231) // 100")[1])
 # The value of (5243 + 642) x (5314 - 4231) // 100 is 63734.
 
 
-ai = OpenAI(key, "gpt-3.5-turbo-1106")
+ai = OpenAI(key, "gpt-4o")
 ai.set_browser_functions()
 print(ai("How the weather in Tokyo?")[1])
 # The current weather in Tokyo varies depending on the source. According to AccuWeather, it is partly sunny with a temperature of 89°F. BBC Weather predicts thundery showers tonight with a low temperature of 22°C. Timeanddate.com reports an overcast sky with a temperature of 82°F. The Weather Network and The Weather Channel provide forecasts for the next 7 and 13 days respectively. Weather Underground also offers weather conditions for Tokyo and other cities.
 ```
```

### Comparing `atksh_utils-0.8.7/README.md` & `atksh_utils-0.8.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 python -m pip install -e '.[dev]'
 pre-commit install
 ```
 
 ## OpenAI
 
 ```python
-ai = OpenAI(key, "gpt-3.5-turbo-1106")
+ai = OpenAI(key, "gpt-4o")
 
 print(ai("Just answer the value of (5243 + 642) x (5314 - 4231) // 100"))
 # The value of the expression (5243 + 642) x (5314 - 4231) // 100 is 7112.
 
 
 def mul(a: int, b: int) -> int:
     """This is a multiplication function.
@@ -166,12 +166,12 @@
 ai.set_function(sub)
 ai.set_function(div)
 
 print(ai("Just answer the value of (5243 + 642) x (5314 - 4231) // 100")[1])
 # The value of (5243 + 642) x (5314 - 4231) // 100 is 63734.
 
 
-ai = OpenAI(key, "gpt-3.5-turbo-1106")
+ai = OpenAI(key, "gpt-4o")
 ai.set_browser_functions()
 print(ai("How the weather in Tokyo?")[1])
 # The current weather in Tokyo varies depending on the source. According to AccuWeather, it is partly sunny with a temperature of 89°F. BBC Weather predicts thundery showers tonight with a low temperature of 22°C. Timeanddate.com reports an overcast sky with a temperature of 82°F. The Weather Network and The Weather Channel provide forecasts for the next 7 and 13 days respectively. Weather Underground also offers weather conditions for Tokyo and other cities.
 ```
```

### Comparing `atksh_utils-0.8.7/pyproject.toml` & `atksh_utils-0.8.8/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools>=62.6", "setuptools_scm[toml]>=6.2", "wheel"]
 
 [project]
 dependencies = [
-  "openai~=1.23.6",
+  "openai~=1.29.0",
   "beautifulsoup4>=4.11.1,<5.0.0",
   "requests>=2.0.0,<3.0.0",
   "duckduckgo_search~=4.1.1",
   "dill>=0.3.7,<0.4.0",
   "numba>=0.56.4,<0.59.0",
   "pylatexenc==2.10",
   "scipy>=1.9.0,<2.0.0",
   "sympy>=1.9.0,<2.0.0",
   "soundfile>=0.12.1,<0.13.0",
   "sounddevice>=0.4.6,<0.5.0",
   "pypdf~=3.17.2",
-  "tiktoken~=0.5.2",
+  "tiktoken~=0.7.0",
   "backoff>=2.2.1,<3.0.0",
 ]
 description = "atksh's utils"
 dynamic = ["version"]
 license = {file = "LICENSE"}
 name = "atksh-utils"
 readme = "README.md"
```

### Comparing `atksh_utils-0.8.7/src/atksh_utils/basic/functools.py` & `atksh_utils-0.8.8/src/atksh_utils/basic/functools.py`

 * *Files identical despite different names*

### Comparing `atksh_utils-0.8.7/src/atksh_utils/nlp/str_kernel.py` & `atksh_utils-0.8.8/src/atksh_utils/nlp/str_kernel.py`

 * *Files identical despite different names*

### Comparing `atksh_utils-0.8.7/src/atksh_utils/openai/api.py` & `atksh_utils-0.8.8/src/atksh_utils/openai/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         self.model_name = model_name
         self.temperature = temperature
         self.top_p = top_p
         self._functions: list[FunctionWrapper] = []
         self.max_num_messages = max_num_messages
         if max_num_input_tokens > 0:
             self.max_num_input_tokens = max_num_input_tokens
-        elif "gpt-4-0125-preview" in self.model_name or "gpt-4-turbo" in self.model_name:
+        elif "gpt-4-0125-preview" in self.model_name or "gpt-4o" in self.model_name:
             self.max_num_input_tokens = 120000
         elif "gpt-4-32k-0613" in self.model_name:
             self.max_num_input_tokens = 28000
         else:
             self.max_num_input_tokens = 15000
         self.is_child = is_child
```

### Comparing `atksh_utils-0.8.7/src/atksh_utils/openai/askgpt.py` & `atksh_utils-0.8.8/src/atksh_utils/openai/askgpt.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,35 +81,34 @@
     token = chunk.choices[0].delta.content
     if token:
         tokens.append(token)
         if token.endswith("\n"):
             print_tokens()
 
 
-def setup_ai(use_gpt4) -> OpenAI:
+def setup_ai() -> OpenAI:
     key = os.getenv("OPENAI_API_KEY")
-    ai = OpenAI(key, "gpt-4-turbo" if use_gpt4 else "gpt-3.5-turbo")
+    ai = OpenAI(key, "gpt-4o")
     ai.set_browser_functions()
     ai.set_python_functions()
     ai.set_bash_function()
     ai.set_utility_functions()
     return ai
 
 
 def ask():
     os.environ["ASKGPT_VERBOSE"] = "0"
     parser = argparse.ArgumentParser()
     parser.add_argument("--verbose", action="store_true", help="Verbose mode.")
     parser.add_argument("--enable-speech", action="store_true", help="Enable speech.")
-    parser.add_argument("--disable-gpt4", action="store_true", help="Disable GPT-4.")
     args = parser.parse_args()
     verbose = args.verbose
     if verbose:
         os.environ["ASKGPT_VERBOSE"] = "1"
-    ai = setup_ai(not args.disable_gpt4)
+    ai = setup_ai()
     not_called = True
     user_prompt = None
     try:
         while True:
             empty_input_count = 0
             lines = []
             lines.append(
```

### Comparing `atksh_utils-0.8.7/src/atksh_utils/openai/functional.py` & `atksh_utils-0.8.8/src/atksh_utils/openai/functional.py`

 * *Files identical despite different names*

### Comparing `atksh_utils-0.8.7/src/atksh_utils/openai/prompt.py` & `atksh_utils-0.8.8/src/atksh_utils/openai/prompt.py`

 * *Files identical despite different names*

### Comparing `atksh_utils-0.8.7/src/atksh_utils/openai/token.py` & `atksh_utils-0.8.8/src/atksh_utils/openai/token.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import tiktoken
 
-ENC = tiktoken.get_encoding("cl100k_base")
+ENC = tiktoken.get_encoding("o200k_base")
 
 
 def count_token(text: str) -> int:
     ids = ENC.encode(text)
     return len(ids)
```

### Comparing `atksh_utils-0.8.7/src/atksh_utils/openai/tool.py` & `atksh_utils-0.8.8/src/atksh_utils/openai/tool.py`

 * *Files 0% similar despite different names*

```diff
@@ -251,19 +251,15 @@
         return f"Error: {error}.\nPlease try again or try another text."
 
     return translate
 
 
 def get_browser_functions(ai: "OpenAI"):
     visit_page_model_name = ai.model_name
-    visit_page_max_context_length = (
-        100000
-        if "gpt-4-preview" in visit_page_model_name or "gpt-4-turbo" in visit_page_model_name
-        else 10000
-    )
+    visit_page_max_context_length = 100000 if "gpt-4o" in visit_page_model_name else 10000
     visit_page_max_context_length -= count_token(VISIT_PAGE_SUMMARIZE_PROMPT)
 
     def _search_summarize(query_text: str, results: str) -> str:
         """Summarizes the query text and results."""
         search_result_child = ai.make_child(ai.model_name, temperature=0.2, top_p=0.8)
         search_result_child.set_system_prompt(SEARCH_RESULT_SUMMARIZE_PROMPT)
         error = "Unknown error."
```

### Comparing `atksh_utils-0.8.7/src/atksh_utils.egg-info/PKG-INFO` & `atksh_utils-0.8.8/src/atksh_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atksh-utils
-Version: 0.8.7
+Version: 0.8.8
 Summary: atksh's utils
 Home-page: https://github.com/atksh/atksh_utils
 Author: atksh
 License: MIT License
         
         Copyright (c) 2023 atksh
         
@@ -25,27 +25,27 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: openai~=1.23.6
+Requires-Dist: openai~=1.29.0
 Requires-Dist: beautifulsoup4<5.0.0,>=4.11.1
 Requires-Dist: requests<3.0.0,>=2.0.0
 Requires-Dist: duckduckgo_search~=4.1.1
 Requires-Dist: dill<0.4.0,>=0.3.7
 Requires-Dist: numba<0.59.0,>=0.56.4
 Requires-Dist: pylatexenc==2.10
 Requires-Dist: scipy<2.0.0,>=1.9.0
 Requires-Dist: sympy<2.0.0,>=1.9.0
 Requires-Dist: soundfile<0.13.0,>=0.12.1
 Requires-Dist: sounddevice<0.5.0,>=0.4.6
 Requires-Dist: pypdf~=3.17.2
-Requires-Dist: tiktoken~=0.5.2
+Requires-Dist: tiktoken~=0.7.0
 Requires-Dist: backoff<3.0.0,>=2.2.1
 Provides-Extra: dev
 Requires-Dist: black~=23.0.0; extra == "dev"
 Requires-Dist: pytest~=7.2.2; extra == "dev"
 Requires-Dist: isort~=5.12.0; extra == "dev"
 Requires-Dist: pre-commit~=3.2.2; extra == "dev"
 
@@ -151,15 +151,15 @@
 python -m pip install -e '.[dev]'
 pre-commit install
 ```
 
 ## OpenAI
 
 ```python
-ai = OpenAI(key, "gpt-3.5-turbo-1106")
+ai = OpenAI(key, "gpt-4o")
 
 print(ai("Just answer the value of (5243 + 642) x (5314 - 4231) // 100"))
 # The value of the expression (5243 + 642) x (5314 - 4231) // 100 is 7112.
 
 
 def mul(a: int, b: int) -> int:
     """This is a multiplication function.
@@ -217,12 +217,12 @@
 ai.set_function(sub)
 ai.set_function(div)
 
 print(ai("Just answer the value of (5243 + 642) x (5314 - 4231) // 100")[1])
 # The value of (5243 + 642) x (5314 - 4231) // 100 is 63734.
 
 
-ai = OpenAI(key, "gpt-3.5-turbo-1106")
+ai = OpenAI(key, "gpt-4o")
 ai.set_browser_functions()
 print(ai("How the weather in Tokyo?")[1])
 # The current weather in Tokyo varies depending on the source. According to AccuWeather, it is partly sunny with a temperature of 89°F. BBC Weather predicts thundery showers tonight with a low temperature of 22°C. Timeanddate.com reports an overcast sky with a temperature of 82°F. The Weather Network and The Weather Channel provide forecasts for the next 7 and 13 days respectively. Weather Underground also offers weather conditions for Tokyo and other cities.
 ```
```

### Comparing `atksh_utils-0.8.7/src/atksh_utils.egg-info/SOURCES.txt` & `atksh_utils-0.8.8/src/atksh_utils.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 .gitignore
 .pre-commit-config.yaml
 LICENSE
 README.md
+demo.py
 pyproject.toml
 setup.cfg
 .github/workflows/publish_to_pypi.yaml
 src/atksh_utils/__init__.py
 src/atksh_utils/version.py
 src/atksh_utils.egg-info/PKG-INFO
 src/atksh_utils.egg-info/SOURCES.txt
```

