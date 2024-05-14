# Comparing `tmp/confcls-0.1.4.tar.gz` & `tmp/confcls-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "confcls-0.1.4.tar", max compression
+gzip compressed data, was "confcls-0.1.5.tar", max compression
```

## Comparing `confcls-0.1.4.tar` & `confcls-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1480 2024-05-14 14:52:17.715267 confcls-0.1.4/LICENSE
--rw-r--r--   0        0        0     5227 2024-05-14 17:46:42.396362 confcls-0.1.4/README.md
--rw-r--r--   0        0        0      187 2024-05-14 09:51:31.518086 confcls-0.1.4/confcls/__init__.py
--rw-r--r--   0        0        0     2352 2024-05-14 08:53:55.090298 confcls-0.1.4/confcls/configurable.py
--rw-r--r--   0        0        0      494 2024-05-14 14:44:48.827305 confcls-0.1.4/confcls/object.py
--rw-r--r--   0        0        0      907 2024-05-14 17:46:13.092277 confcls-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     6027 2024-05-14 17:46:42.789944 confcls-0.1.4/setup.py
--rw-r--r--   0        0        0     5979 2024-05-14 17:46:42.790188 confcls-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1480 2024-05-14 14:52:17.715267 confcls-0.1.5/LICENSE
+-rw-r--r--   0        0        0     5227 2024-05-14 17:49:33.616837 confcls-0.1.5/README.md
+-rw-r--r--   0        0        0      187 2024-05-14 09:51:31.518086 confcls-0.1.5/confcls/__init__.py
+-rw-r--r--   0        0        0     2352 2024-05-14 08:53:55.090298 confcls-0.1.5/confcls/configurable.py
+-rw-r--r--   0        0        0      494 2024-05-14 14:44:48.827305 confcls-0.1.5/confcls/object.py
+-rw-r--r--   0        0        0      874 2024-05-14 17:49:06.880765 confcls-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     6027 2024-05-14 17:49:34.000216 confcls-0.1.5/setup.py
+-rw-r--r--   0        0        0     5900 2024-05-14 17:49:34.000456 confcls-0.1.5/PKG-INFO
```

### Comparing `confcls-0.1.4/LICENSE` & `confcls-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `confcls-0.1.4/README.md` & `confcls-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `confcls-0.1.4/confcls/configurable.py` & `confcls-0.1.5/confcls/configurable.py`

 * *Files identical despite different names*

### Comparing `confcls-0.1.4/pyproject.toml` & `confcls-0.1.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 [tool.poetry]
 name = "confcls"
-version = "0.1.4"
+version = "0.1.5"
 description = "Class instance configurator"
 authors = [
     "Václav Krpec <vencik@razdva.cz>",
 ]
 packages = [
     { include = "confcls" },
 ]
 readme = "README.md"
-license = "BSD 3-clause license"
 keywords = ["config", "configuration"]
 classifiers = [
     "License :: OSI Approved :: BSD License",
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3.9",
 ]
```

### Comparing `confcls-0.1.4/setup.py` & `confcls-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 extras_require = \
 {'all': ['smart-open>=7.0.4,<8.0.0']}
 
 setup_kwargs = {
     'name': 'confcls',
-    'version': '0.1.4',
+    'version': '0.1.5',
     'description': 'Class instance configurator',
     'long_description': '# Class Instance Configurator\n\nA simple configuration library allowing instantiation of classes from config. files.\n\nConfiguration files are in JSON format and simply specify the type of the created object\nand keyword arguments for its construction.\nThe library also supports free-form config. objects for which respective dataclass-like\ntypes are automatically created from a meta-class (so that the programmer doesn’t even\nhave to declare them).\n\nSupport for remote config. is provided by (optional) use of `smart-open`.\n\n## Examples\n\n### Instantiation of a class from config. file\n\nAssuming you have the following general class:\n\n**my\\_module.py**\n\n    from confcls import Configurable\n\n    class MyClass(Configurable):\n        def __init__(self, arg1: str, arg2: int, arg3: list[str], arg4: dict[str, float]):\n            self.foo = arg1\n            self.bar = arg2\n            self.baz = [arg4[name] for name in arg3 if name in arg4]\n\nYou can now store its instance configuration in a JSON file:\n\n**my\\_obj.json**\n\n    {\n        "__type__" : "my_module.MyClass",\n        "arg1" : "Hello world!",\n        "arg2" : 123,\n        "arg3" : ["abc", "ghi"],\n        "arg4" : {\n            "abc" : 0.123,\n            "def" : 0.987\n        }\n    }\n\nAnd instantiate the configured instance, thus:\n\n    from my_module import MyClass\n\n    my_obj = MyClass.from_file("my_obj.json")\n\n(You may also call `confcls.Configurable.from_file` directly if you don’t wish\nto specify and/or import the type.)\n\nThe instantiation does support nesting; your constructor arguments may indeed be other\nclass instances:\n\n**my\\_obj.json**\n\n    {\n        "__type__" : "my_module.Class1",\n        "foo" : 123,\n        "bar" : {\n            "__type__" : "my_module.Class2",\n            "arg1" : 345,\n            "arg2" : "whatever"\n        },\n        "baz" : {\n            "__type__" : "my_module.Class3",\n            "arg" : {\n                "__type__" : "my_module.Class2",\n                "arg1" : 567,\n                "arg2" : "something else"\n            }\n        }\n    }\n\nThe above configuration instantiates the same object as the following code:\n\n    my_obj = Class1(\n        foo=123,\n        bar=Class2(arg1=345, arg2="whatever"),\n        baz=Class3(arg=Class2(arg1=567, arg2="something else)),\n    )\n\n### Dataclass config\n\nYou may want to create a (nested) dataclass configuration.\nThe principle is exactly the same as above; you simply define your configuration\ndata classes and instantiate them from configuration:\n\n**my\\_config.py**\n\n    from dataclasses import dataclass\n    from confcls import Configurable\n\n    @dataclass\n    class Configuration(Configurable):\n        number: int\n        fpnum: float = 0.0  # number with default\n        item1: Item1\n        opt_item2: Item2 = None  # optional instance\n\n    @dataclass\n    class Item1:  # note that nested dataclasses don\'t even need to be Configurable\n        foo: int\n        bar: float = 1.0\n\n    @dataclass Item2:\n        baz: str\n\nNow, your configuration may look like this:\n\n    {\n        "__type__" : "my_config.Configuration",\n        "number" : 123,\n        "item1" : {\n            "__type__" : "my_config.Item1",\n            "foo" : 345,\n            "bar" : 0.5\n        }\n    }\n\n### Automatic dataclass-like instances\n\nIf you’re very lazy, you don’t even have to declare your config. dataclasses.\nJust let `confcls` create the types for you, on demand:\n\n**my\\_config.json**\n\n    {\n        "__type__" : "confcls.Configuration",\n        "myarg1" : "whatever you like",\n        "myarg2" : {\n            "__type__" : "confcls.Object",\n            "absolutely" : "anything",\n            "really" : 123\n        }\n    }\n\n`confcls.Object` is a free-form class which can be instantiated with any keyword\narguments (and the instance contains them as members).\nSo now, you can access your configuration e.g. like this:\n\n    from confcls import Configuration  # Configurable extension of confcls.Object\n\n    config = Configuration.from_file("my_config.json")\n    assert config.myarg2.absolutely == "anything"\n\nNote that this sort of configuration doesn’t support defaults as there’s nowhere\nto define them (if you want defaults, just declare your (data)classes with them).\nAlso note that you may combine the declared/free-form approaches (if it makes sense).\n\nFinally, observe that the `Configurable.from_file` member function has `auto_obj`\nparameter (with `False` default).\nSetting that parameter to `True` allows you to omit the `type` specification\nin your configuration.\nIn that case, the library will automatically treat all JSON objects in the config.\nfile as if the `confcls.Object` type was specified.\n\n## Development\n\nTo develop `confcls`, you shall need make, pyenv and poetry installed.\nThen, setup and initialise your development environment:\n\n    $ make setup\n    $ make init\n\nTo run mypy type checks, unit tests, and the linter use the `mypy`, `test` and `lint`\nmake targets, respectively.\nAlternatively, use the `check` target to do all that.\n\n    $ make check\n\nThe Python package is built by the `build` target.\nThe package may be published using the `publish` target.\n\n    $ make build\n    $ make publish\n\n## Author\n\nVáclav Krpec &lt;<vencik@razdva.cz>&gt;\n',
     'author': 'Václav Krpec',
     'author_email': 'vencik@razdva.cz',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `confcls-0.1.4/PKG-INFO` & `confcls-0.1.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: confcls
-Version: 0.1.4
+Version: 0.1.5
 Summary: Class instance configurator
-License: BSD 3-clause license
 Keywords: config,configuration
 Author: Václav Krpec
 Author-email: vencik@razdva.cz
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
-Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: all
 Requires-Dist: smart-open (>=7.0.4,<8.0.0); extra == "all"
 Project-URL: Homepage, https://github.com/vencik/confcls
 Project-URL: Repository, https://github.com/vencik/confcls
 Description-Content-Type: text/markdown
```

