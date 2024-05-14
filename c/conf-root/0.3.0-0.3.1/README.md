# Comparing `tmp/conf_root-0.3.0.tar.gz` & `tmp/conf_root-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conf_root-0.3.0.tar", last modified: Mon May 13 13:00:36 2024, max compression
+gzip compressed data, was "conf_root-0.3.1.tar", last modified: Tue May 14 13:16:29 2024, max compression
```

## Comparing `conf_root-0.3.0.tar` & `conf_root-0.3.1.tar`

### file list

```diff
@@ -1,28 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:00:36.587498 conf_root-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-13 13:00:32.000000 conf_root-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-05-13 13:00:36.587498 conf_root-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4724 2024-05-13 13:00:32.000000 conf_root-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:00:36.583497 conf_root-0.3.0/conf_root/
--rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-05-13 13:00:32.000000 conf_root-0.3.0/conf_root/ConfRoot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-05-13 13:00:32.000000 conf_root-0.3.0/conf_root/Configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-13 13:00:32.000000 conf_root-0.3.0/conf_root/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:00:36.583497 conf_root-0.3.0/conf_root/agents/
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-13 13:00:32.000000 conf_root-0.3.0/conf_root/agents/BasicAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-13 13:00:32.000000 conf_root-0.3.0/conf_root/agents/JsonAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-13 13:00:32.000000 conf_root-0.3.0/conf_root/agents/RuamelYamlAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-13 13:00:32.000000 conf_root-0.3.0/conf_root/agents/YamlAgent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:00:36.587498 conf_root-0.3.0/conf_root.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-05-13 13:00:36.000000 conf_root-0.3.0/conf_root.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-13 13:00:36.000000 conf_root-0.3.0/conf_root.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 13:00:36.000000 conf_root-0.3.0/conf_root.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 13:00:36.000000 conf_root-0.3.0/conf_root.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-13 13:00:36.000000 conf_root-0.3.0/conf_root.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 13:00:36.587498 conf_root-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-13 13:00:32.000000 conf_root-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:00:36.587498 conf_root-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-13 13:00:32.000000 conf_root-0.3.0/tests/test_argparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-13 13:00:32.000000 conf_root-0.3.0/tests/test_json_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-13 13:00:32.000000 conf_root-0.3.0/tests/test_nested_dataclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-05-13 13:00:32.000000 conf_root-0.3.0/tests/test_normal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-05-13 13:00:32.000000 conf_root-0.3.0/tests/test_ruamel_yaml_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-05-13 13:00:32.000000 conf_root-0.3.0/tests/test_yaml_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:16:29.922479 conf_root-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-14 13:16:23.000000 conf_root-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-05-14 13:16:29.922479 conf_root-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-05-14 13:16:23.000000 conf_root-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:16:29.918479 conf_root-0.3.1/conf_root/
+-rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-05-14 13:16:23.000000 conf_root-0.3.1/conf_root/ConfRoot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-05-14 13:16:23.000000 conf_root-0.3.1/conf_root/Configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-14 13:16:23.000000 conf_root-0.3.1/conf_root/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:16:29.918479 conf_root-0.3.1/conf_root/agents/
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-14 13:16:23.000000 conf_root-0.3.1/conf_root/agents/BasicAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-14 13:16:23.000000 conf_root-0.3.1/conf_root/agents/JsonAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-14 13:16:23.000000 conf_root-0.3.1/conf_root/agents/SingleFileYamlAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-14 13:16:23.000000 conf_root-0.3.1/conf_root/agents/YamlAgent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:16:29.922479 conf_root-0.3.1/conf_root.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-05-14 13:16:29.000000 conf_root-0.3.1/conf_root.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-14 13:16:29.000000 conf_root-0.3.1/conf_root.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 13:16:29.000000 conf_root-0.3.1/conf_root.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 13:16:29.000000 conf_root-0.3.1/conf_root.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 13:16:29.000000 conf_root-0.3.1/conf_root.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 13:16:29.922479 conf_root-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-14 13:16:23.000000 conf_root-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:16:29.922479 conf_root-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-14 13:16:23.000000 conf_root-0.3.1/tests/test_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-05-14 13:16:23.000000 conf_root-0.3.1/tests/test_multi_file_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-14 13:16:23.000000 conf_root-0.3.1/tests/test_nested_dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-14 13:16:23.000000 conf_root-0.3.1/tests/test_single_file_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-14 13:16:23.000000 conf_root-0.3.1/tests/test_wrap.py
```

### Comparing `conf_root-0.3.0/LICENSE` & `conf_root-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `conf_root-0.3.0/PKG-INFO` & `conf_root-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conf_root
-Version: 0.3.0
+Version: 0.3.1
 Summary: 基于dataclass的符合逻辑的配置取用方式。
 Home-page: https://github.com/ciaranchen/conf_root
 Author: ciaranchen
 Author-email: ciaranchen@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -50,20 +50,20 @@
 app_config.load()
 ```
 
 > note: dataclass 中的字段需指定类型。如果不指定类型，将被视为类变量而不会被解析为dataclass中的字段。这个库在dataclass的基础上进行解析，将无法直接处理类变量。
 
 ### 参数解释
 
-#### `ConfRoot(path = None, agent: Optional[Type[BasicAgent]] = YamlAgent)`
+#### `ConfRoot(path = None, agent_class: Optional[Type[BasicAgent]] = YamlAgent)`
 
 - path 为基本路径。当它为None时，将会设置为当前文件路径。
-- agent 为配置存储的形式。当前支持JsonAgent/YamlAgent/RuamelAgent。默认为YamlAgent。
+- agent_class 为配置存储的形式。当前支持JsonAgent/YamlAgent/SingleFileYamlAgent。默认为YamlAgent。
     - 对于存储到多个文件的agent（JsonAgent、YamlAgent），path是配置存储的文件夹路径。
-    - 对于存储到单个文件的agent（RuamelAgent），path是配置存储的文件路径。
+    - 对于存储到单个文件的agent（SingleFileYamlAgent），path是配置存储的文件路径。
     - 如果指定为None，可以不产生配置文件存储；同时也不会为类添加save与load方法。
     - 可以继承BasicAgent进行拓展以适配更多类型的序列化方式。
 
 #### `ConfRoot.wrap`
 
 可以使用不同方式调用。详见上方示例。
 
@@ -116,27 +116,27 @@
 嵌套时可以只指定agent=None来避免产生存储的文件。
 
 ```python
 from conf_root import ConfRoot, JsonAgent
 from dataclasses import dataclass, field
 
 
-@ConfRoot(agent=None).wrap
+@ConfRoot(agent_class=None).wrap
 @dataclass
 class DataBaseUserConfig:
-    database_user: str = 'admin'
-    database_password: str = 'default_password'
+  database_user: str = 'admin'
+  database_password: str = 'default_password'
 
 
-@ConfRoot(agent=JsonAgent).wrap
+@ConfRoot(agent_class=JsonAgent).wrap
 # 可通过agent_class指定配置文件格式
 # 此时默认配置文件名为 `config.json`
 @dataclass
 class AppConfig:
-    database_host: str = 'localhost'
-    database_port: int = 5432
-    # 可嵌套dataclass定义
-    user_config: DataBaseUserConfig = field(default_factory=DataBaseUserConfig)
+  database_host: str = 'localhost'
+  database_port: int = 5432
+  # 可嵌套dataclass定义
+  user_config: DataBaseUserConfig = field(default_factory=DataBaseUserConfig)
 
 
 app_config = AppConfig()
 ```
```

### Comparing `conf_root-0.3.0/README.md` & `conf_root-0.3.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -35,20 +35,20 @@
 app_config.load()
 ```
 
 > note: dataclass 中的字段需指定类型。如果不指定类型，将被视为类变量而不会被解析为dataclass中的字段。这个库在dataclass的基础上进行解析，将无法直接处理类变量。
 
 ### 参数解释
 
-#### `ConfRoot(path = None, agent: Optional[Type[BasicAgent]] = YamlAgent)`
+#### `ConfRoot(path = None, agent_class: Optional[Type[BasicAgent]] = YamlAgent)`
 
 - path 为基本路径。当它为None时，将会设置为当前文件路径。
-- agent 为配置存储的形式。当前支持JsonAgent/YamlAgent/RuamelAgent。默认为YamlAgent。
+- agent_class 为配置存储的形式。当前支持JsonAgent/YamlAgent/SingleFileYamlAgent。默认为YamlAgent。
     - 对于存储到多个文件的agent（JsonAgent、YamlAgent），path是配置存储的文件夹路径。
-    - 对于存储到单个文件的agent（RuamelAgent），path是配置存储的文件路径。
+    - 对于存储到单个文件的agent（SingleFileYamlAgent），path是配置存储的文件路径。
     - 如果指定为None，可以不产生配置文件存储；同时也不会为类添加save与load方法。
     - 可以继承BasicAgent进行拓展以适配更多类型的序列化方式。
 
 #### `ConfRoot.wrap`
 
 可以使用不同方式调用。详见上方示例。
 
@@ -101,27 +101,27 @@
 嵌套时可以只指定agent=None来避免产生存储的文件。
 
 ```python
 from conf_root import ConfRoot, JsonAgent
 from dataclasses import dataclass, field
 
 
-@ConfRoot(agent=None).wrap
+@ConfRoot(agent_class=None).wrap
 @dataclass
 class DataBaseUserConfig:
-    database_user: str = 'admin'
-    database_password: str = 'default_password'
+  database_user: str = 'admin'
+  database_password: str = 'default_password'
 
 
-@ConfRoot(agent=JsonAgent).wrap
+@ConfRoot(agent_class=JsonAgent).wrap
 # 可通过agent_class指定配置文件格式
 # 此时默认配置文件名为 `config.json`
 @dataclass
 class AppConfig:
-    database_host: str = 'localhost'
-    database_port: int = 5432
-    # 可嵌套dataclass定义
-    user_config: DataBaseUserConfig = field(default_factory=DataBaseUserConfig)
+  database_host: str = 'localhost'
+  database_port: int = 5432
+  # 可嵌套dataclass定义
+  user_config: DataBaseUserConfig = field(default_factory=DataBaseUserConfig)
 
 
 app_config = AppConfig()
 ```
```

### Comparing `conf_root-0.3.0/conf_root/ConfRoot.py` & `conf_root-0.3.1/conf_root/ConfRoot.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,19 +5,20 @@
 
 from conf_root.Configuration import Configuration
 from conf_root.agents.BasicAgent import BasicAgent
 from conf_root.agents.YamlAgent import YamlAgent
 
 
 class ConfRoot:
-    def __init__(self, path: str = None, agent: Optional[Type[BasicAgent]] = YamlAgent):
+    def __init__(self, path: str = None, agent_class: Optional[Type[BasicAgent]] = YamlAgent):
         self.path = Path(path) if path is not None else Path()
-        self.agent_class = agent
-        self.persist = (agent is not None)
-        self.agent_obj = self.agent_class(self.path)
+        self.agent_class = agent_class
+        self.persist = (agent_class is not None)
+        if self.persist:
+            self.agent = self.agent_class(self.path)
 
     def wrap(self, *args, **kwargs):
         def decorator(cls, name: Optional[str] = None):
             if not is_dataclass(cls):
                 raise TypeError(f"Target class must be a dataclass, got {cls}")
             if name is None:
                 name = cls.__qualname__.replace('<locals>.', '')
@@ -29,18 +30,18 @@
             origin_init = cls.__init__
 
             def decorated_init(_self, *args, **kwargs):
                 origin_init(_self, *args, **kwargs)
                 self.post_init(_self, configuration)
 
             def save(_self):
-                return _self._agent.save(configuration, _self)
+                return self.agent.save(configuration, _self)
 
             def load(_self):
-                data = _self._agent.load(configuration)
+                data = self.agent.load(configuration)
                 configuration.data2obj(_self, data)
 
             decorated_init.__name__ = '__init__'
             cls.__init__ = decorated_init
             if self.persist:
                 cls.save = save
                 cls.load = load
@@ -56,22 +57,21 @@
             return lambda cls: decorator(cls, args[0])
         # 无args, 只有kwargs的情况下，直接给出decorator
         # @wrap() or @wrap(name='config')
         return lambda cls: decorator(cls, **kwargs)
 
     def post_init(self, instance, configuration):
         if self.persist:
-            instance._agent = self.agent_obj
-            if instance._agent.exist(configuration):
+            if self.agent.exist(configuration):
                 # 如果已存在，读取和实例化
-                data = instance._agent.load(configuration)
+                data = self.agent.load(configuration)
                 configuration.data2obj(instance, data)
             else:
                 # 若文件不存在，根据默认值创建
-                instance._agent.create(configuration)
+                self.agent.create(configuration)
 
     def from_argparse(self, parser: argparse.ArgumentParser, cls_name: str = 'argparse'):
         def get_default(action):
             if isinstance(action, argparse._StoreConstAction):
                 return action.const
             if action.default:
                 return action.default
@@ -110,9 +110,9 @@
                 default = get_default(action)
                 _type = get_type(action)
                 field = (name, _type, default)
             fields.append(field)
 
         fields = sorted(fields, key=lambda x: x[2] == MISSING, reverse=True)
 
-        cls = make_dataclass(cls_name.replace(f'.{self.agent_obj.default_extension}', ''), fields)
+        cls = make_dataclass(cls_name.replace(f'.{self.agent.default_extension}', ''), fields)
         return self.wrap(cls_name)(cls)
```

### Comparing `conf_root-0.3.0/conf_root/Configuration.py` & `conf_root-0.3.1/conf_root/Configuration.py`

 * *Files identical despite different names*

### Comparing `conf_root-0.3.0/conf_root/agents/BasicAgent.py` & `conf_root-0.3.1/conf_root/agents/BasicAgent.py`

 * *Files identical despite different names*

### Comparing `conf_root-0.3.0/conf_root/agents/JsonAgent.py` & `conf_root-0.3.1/conf_root/agents/JsonAgent.py`

 * *Files identical despite different names*

### Comparing `conf_root-0.3.0/conf_root/agents/RuamelYamlAgent.py` & `conf_root-0.3.1/conf_root/agents/SingleFileYamlAgent.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from ruamel.yaml import YAML
 
 from conf_root.Configuration import Configuration
 from conf_root.agents.BasicAgent import BasicAgent
 
 
-class RuamelYamlAgent(BasicAgent):
+class SingleFileYamlAgent(BasicAgent):
     """
     Similar with yaml agent, but save in single file.
     """
     default_extension: str = 'yml'
 
     def __init__(self, location):
         parent_directory = Path(location).parent
@@ -38,15 +38,16 @@
 
     def _load(self):
         with open(self.location, 'r') as f:
             return self.yaml.load(f)
 
     def load(self, configuration: Configuration) -> None:
         super().load(configuration)
-        return self._load()
+        res = self._load()
+        return res[configuration.name]
 
     def save(self, configuration: Configuration, obj: object) -> None:
         super().save(configuration, obj)
         total_data = self._load()
 
         data = configuration.obj2data(obj)
         total_data[configuration.name] = data
```

### Comparing `conf_root-0.3.0/conf_root/agents/YamlAgent.py` & `conf_root-0.3.1/conf_root/agents/YamlAgent.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
             with open(location, "w") as file:
                 self.yaml.dump(default_dict, file)
 
     def load(self, configuration) -> Dict[str, Any]:
         super().load(configuration)
         location = self.get_configuration_location(configuration)
         with open(location, encoding='utf-8') as file:
-            data = self.yaml.safe_load(file)
+            data = self.yaml.load(file)
         # 将dict展开为对象。
         return data
 
     def save(self, configuration, obj):
         super().save(configuration, obj)
         location = self.get_configuration_location(configuration)
         data_dict = configuration.obj2data(obj)
```

### Comparing `conf_root-0.3.0/conf_root.egg-info/PKG-INFO` & `conf_root-0.3.1/conf_root.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conf_root
-Version: 0.3.0
+Version: 0.3.1
 Summary: 基于dataclass的符合逻辑的配置取用方式。
 Home-page: https://github.com/ciaranchen/conf_root
 Author: ciaranchen
 Author-email: ciaranchen@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -50,20 +50,20 @@
 app_config.load()
 ```
 
 > note: dataclass 中的字段需指定类型。如果不指定类型，将被视为类变量而不会被解析为dataclass中的字段。这个库在dataclass的基础上进行解析，将无法直接处理类变量。
 
 ### 参数解释
 
-#### `ConfRoot(path = None, agent: Optional[Type[BasicAgent]] = YamlAgent)`
+#### `ConfRoot(path = None, agent_class: Optional[Type[BasicAgent]] = YamlAgent)`
 
 - path 为基本路径。当它为None时，将会设置为当前文件路径。
-- agent 为配置存储的形式。当前支持JsonAgent/YamlAgent/RuamelAgent。默认为YamlAgent。
+- agent_class 为配置存储的形式。当前支持JsonAgent/YamlAgent/SingleFileYamlAgent。默认为YamlAgent。
     - 对于存储到多个文件的agent（JsonAgent、YamlAgent），path是配置存储的文件夹路径。
-    - 对于存储到单个文件的agent（RuamelAgent），path是配置存储的文件路径。
+    - 对于存储到单个文件的agent（SingleFileYamlAgent），path是配置存储的文件路径。
     - 如果指定为None，可以不产生配置文件存储；同时也不会为类添加save与load方法。
     - 可以继承BasicAgent进行拓展以适配更多类型的序列化方式。
 
 #### `ConfRoot.wrap`
 
 可以使用不同方式调用。详见上方示例。
 
@@ -116,27 +116,27 @@
 嵌套时可以只指定agent=None来避免产生存储的文件。
 
 ```python
 from conf_root import ConfRoot, JsonAgent
 from dataclasses import dataclass, field
 
 
-@ConfRoot(agent=None).wrap
+@ConfRoot(agent_class=None).wrap
 @dataclass
 class DataBaseUserConfig:
-    database_user: str = 'admin'
-    database_password: str = 'default_password'
+  database_user: str = 'admin'
+  database_password: str = 'default_password'
 
 
-@ConfRoot(agent=JsonAgent).wrap
+@ConfRoot(agent_class=JsonAgent).wrap
 # 可通过agent_class指定配置文件格式
 # 此时默认配置文件名为 `config.json`
 @dataclass
 class AppConfig:
-    database_host: str = 'localhost'
-    database_port: int = 5432
-    # 可嵌套dataclass定义
-    user_config: DataBaseUserConfig = field(default_factory=DataBaseUserConfig)
+  database_host: str = 'localhost'
+  database_port: int = 5432
+  # 可嵌套dataclass定义
+  user_config: DataBaseUserConfig = field(default_factory=DataBaseUserConfig)
 
 
 app_config = AppConfig()
 ```
```

### Comparing `conf_root-0.3.0/setup.py` & `conf_root-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="conf_root",  # 包名
-    version="0.3.0",  # 版本号
+    version="0.3.1",  # 版本号
     install_requires=[
         "ruamel.yaml"
     ],
     author="ciaranchen",
     author_email="ciaranchen@qq.com",
     description="基于dataclass的符合逻辑的配置取用方式。",
     long_description=long_description,
```

### Comparing `conf_root-0.3.0/tests/test_argparse.py` & `conf_root-0.3.1/tests/test_argparse.py`

 * *Files identical despite different names*

### Comparing `conf_root-0.3.0/tests/test_json_agent.py` & `conf_root-0.3.1/tests/test_multi_file_agent.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 import os
 import unittest
 from dataclasses import dataclass
 
-from conf_root import ConfRoot, JsonAgent
+from conf_root import ConfRoot, YamlAgent, JsonAgent
 
 
-class TestJsonConfig(unittest.TestCase):
+class TestYamlAgent(unittest.TestCase):
     def __init__(self, methodName="runTest"):
         super().__init__(methodName)
-        self.location = 'settings.json'
+        self.agent = YamlAgent
+        self.location = 'settings.' + self.agent.default_extension
+        self.test_load_content = "database_host: 127.0.0.1\ndatabase_port: 5432"
 
     def tearDown(self):
         # 这个方法将在每个测试方法结束后运行
         # 使用os.remove删除在测试中创建的文件
         try:
             os.remove(self.location)
         except FileNotFoundError:
             pass  # 如果文件不存在，忽略错误（也可以根据需求抛出异常）
 
     def test_create(self):
-        @ConfRoot(agent=JsonAgent).wrap(self.location)
+        @ConfRoot(agent_class=self.agent).wrap(self.location)
         @dataclass
         class AppConfig:
             not_default: str
             database_host: str = 'localhost'
             database_port: int = 5432
 
         app_config = AppConfig('admin')
@@ -38,32 +40,32 @@
             content = file.read()
         self.assertTrue('localhost' in content)
         self.assertTrue('5432' in content)
         # admin 因为非默认配置，不在配置文件中。
         self.assertFalse('admin' in content)
 
     def test_load(self):
-        @ConfRoot(agent=JsonAgent).wrap(self.location)
+        content = self.test_load_content
+        # 将处理后的内容写回文件（可以先备份原文件）
+        with open(self.location, 'w') as file:
+            file.write(content)
+
+        @ConfRoot(agent_class=self.agent).wrap(self.location)
         @dataclass
         class AppConfig:
             not_default: str
             database_host: str = 'localhost'
             database_port: int = 5432
 
-        content = """{"database_host": "127.0.0.1", "database_port": 5432}"""
-        # 将处理后的内容写回文件（可以先备份原文件）
-        with open(self.location, 'w') as file:
-            file.write(content)
-
         app_config = AppConfig('admin')
         self.assertEqual(app_config.database_host, '127.0.0.1')
         self.assertEqual(app_config.database_port, 5432)
 
     def test_save(self):
-        @ConfRoot(agent=JsonAgent).wrap(self.location)
+        @ConfRoot(agent_class=self.agent).wrap(self.location)
         @dataclass
         class AppConfig:
             not_default: str
             database_host: str = 'localhost'
             database_port: int = 5432
 
         app_config = AppConfig('admin')
@@ -75,7 +77,15 @@
         # 打开文件，读取内容
         self.assertTrue(os.path.exists(self.location))
         with open(self.location, 'r') as file:
             content = file.read()
         self.assertTrue('192.168.1.1' in content)
         self.assertTrue('3309' in content)
         self.assertTrue('admin' in content)
+
+
+class TestJsonConfig(TestYamlAgent):
+    def __init__(self, methodName="runTest"):
+        super().__init__(methodName)
+        self.agent = JsonAgent
+        self.location = 'settings.' + self.agent.default_extension
+        self.test_load_content = """{"database_host": "127.0.0.1", "database_port": 5432}"""
```

### Comparing `conf_root-0.3.0/tests/test_nested_dataclass.py` & `conf_root-0.3.1/tests/test_nested_dataclass.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import os
 import unittest
 from dataclasses import dataclass, field as dataclass_field
 
 from conf_root import ConfRoot
 
 
-@ConfRoot(agent=None).wrap()
+@ConfRoot(agent_class=None).wrap()
 @dataclass
 class NestedConfig:
     config1: str = 'nest_config1'
     config2: str = 'nest_config2'
 
 
 @dataclass
 class AppConfig:
     nc_defined: NestedConfig
     nc_default: NestedConfig = dataclass_field(default_factory=NestedConfig)
 
 
-class TestConfig(unittest.TestCase):
+class TestNestedDataclass(unittest.TestCase):
     def __init__(self, methodName="runTest"):
         super().__init__(methodName)
         self.location = 'nested_config.yml'
 
     def tearDown(self):
         # 这个方法将在每个测试方法结束后运行
         # 使用os.remove删除在测试中创建的文件
```

### Comparing `conf_root-0.3.0/tests/test_normal.py` & `conf_root-0.3.1/tests/test_wrap.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,15 +45,15 @@
             content = file.read()
         self.assertTrue('42' in content)
         self.replace_text(self.yaml_location, '42', '43')
         app_config2 = AppConfig()
         self.assertEqual(app_config2.something, 43)
 
     def test_default_json_configuration(self):
-        @ConfRoot(agent=JsonAgent).wrap('config')
+        @ConfRoot(agent_class=JsonAgent).wrap('config')
         @dataclass
         class AppConfig:
             something: int = 42
 
         app_config = AppConfig()
         self.assertTrue(os.path.exists(self.json_location))
         with open(self.json_location, 'r') as file:
```

### Comparing `conf_root-0.3.0/tests/test_ruamel_yaml_agent.py` & `conf_root-0.3.1/tests/test_single_file_agent.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import unittest
 
 import os
 import unittest
 from dataclasses import dataclass
 
 from conf_root import ConfRoot
-from conf_root.agents.RuamelYamlAgent import RuamelYamlAgent
+from conf_root.agents.SingleFileYamlAgent import SingleFileYamlAgent
 
 
-class TestRuamelYamlAgent(unittest.TestCase):
+class TestSingleFileYamlAgent(unittest.TestCase):
     location = 'settings.yml'
 
     def __init__(self, methodName="runTest"):
         super().__init__(methodName)
-        self.conf_root = ConfRoot(self.location, agent=RuamelYamlAgent)
+        self.conf_root = ConfRoot(self.location, agent_class=SingleFileYamlAgent)
 
     @classmethod
     def tearDownClass(cls):
         super().tearDownClass()
         # 使用os.remove删除在测试中创建的文件
         try:
             os.remove(cls.location)
```

