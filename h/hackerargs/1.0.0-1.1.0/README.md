# Comparing `tmp/hackerargs-1.0.0.tar.gz` & `tmp/hackerargs-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hackerargs-1.0.0.tar", last modified: Mon May 13 18:58:17 2024, max compression
+gzip compressed data, was "hackerargs-1.1.0.tar", last modified: Tue May 14 20:01:12 2024, max compression
```

## Comparing `hackerargs-1.0.0.tar` & `hackerargs-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)        0 2024-05-13 18:58:17.262904 hackerargs-1.0.0/
--rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)     1055 2024-05-11 21:31:25.000000 hackerargs-1.0.0/LICENSE
--rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)     7804 2024-05-13 18:58:17.251710 hackerargs-1.0.0/PKG-INFO
--rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)     7476 2024-05-13 18:47:12.000000 hackerargs-1.0.0/README.md
-drwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)        0 2024-05-13 18:58:16.887506 hackerargs-1.0.0/hackerargs/
--rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)       55 2024-05-12 02:54:31.000000 hackerargs-1.0.0/hackerargs/__init__.py
--rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)      380 2024-05-12 19:36:14.000000 hackerargs-1.0.0/hackerargs/argparse_access.py
--rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)     8924 2024-05-12 21:11:53.000000 hackerargs-1.0.0/hackerargs/args.py
--rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)     1185 2024-05-12 00:25:18.000000 hackerargs-1.0.0/hackerargs/strict_bool_yaml.py
-drwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)        0 2024-05-13 18:58:17.226528 hackerargs-1.0.0/hackerargs.egg-info/
--rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)     7804 2024-05-13 18:58:16.000000 hackerargs-1.0.0/hackerargs.egg-info/PKG-INFO
--rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)      373 2024-05-13 18:58:16.000000 hackerargs-1.0.0/hackerargs.egg-info/SOURCES.txt
--rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)        1 2024-05-13 18:58:16.000000 hackerargs-1.0.0/hackerargs.egg-info/dependency_links.txt
--rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)        7 2024-05-13 18:58:16.000000 hackerargs-1.0.0/hackerargs.egg-info/requires.txt
--rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)       11 2024-05-13 18:58:16.000000 hackerargs-1.0.0/hackerargs.egg-info/top_level.txt
--rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)      394 2024-05-13 18:58:00.000000 hackerargs-1.0.0/pyproject.toml
--rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)       38 2024-05-13 18:58:17.267944 hackerargs-1.0.0/setup.cfg
-drwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)        0 2024-05-13 18:58:17.172559 hackerargs-1.0.0/tests/
--rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)      492 2024-05-12 21:02:44.000000 hackerargs-1.0.0/tests/test_access.py
--rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)      776 2024-05-12 21:02:22.000000 hackerargs-1.0.0/tests/test_positional.py
--rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)      913 2024-05-12 21:02:25.000000 hackerargs-1.0.0/tests/test_priority.py
+drwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)        0 2024-05-14 20:01:12.846654 hackerargs-1.1.0/
+-rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)     1055 2024-05-11 21:31:25.000000 hackerargs-1.1.0/LICENSE
+-rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)     4533 2024-05-14 20:01:12.840648 hackerargs-1.1.0/PKG-INFO
+-rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)     4205 2024-05-14 19:53:25.000000 hackerargs-1.1.0/README.md
+drwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)        0 2024-05-14 20:01:12.700977 hackerargs-1.1.0/hackerargs/
+-rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)       55 2024-05-12 02:54:31.000000 hackerargs-1.1.0/hackerargs/__init__.py
+-rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)      380 2024-05-12 19:36:14.000000 hackerargs-1.1.0/hackerargs/argparse_access.py
+-rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)     9253 2024-05-14 19:08:39.000000 hackerargs-1.1.0/hackerargs/args.py
+-rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)     1185 2024-05-12 00:25:18.000000 hackerargs-1.1.0/hackerargs/strict_bool_yaml.py
+drwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)        0 2024-05-14 20:01:12.833223 hackerargs-1.1.0/hackerargs.egg-info/
+-rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)     4533 2024-05-14 20:01:12.000000 hackerargs-1.1.0/hackerargs.egg-info/PKG-INFO
+-rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)      399 2024-05-14 20:01:12.000000 hackerargs-1.1.0/hackerargs.egg-info/SOURCES.txt
+-rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)        1 2024-05-14 20:01:12.000000 hackerargs-1.1.0/hackerargs.egg-info/dependency_links.txt
+-rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)        7 2024-05-14 20:01:12.000000 hackerargs-1.1.0/hackerargs.egg-info/requires.txt
+-rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)       11 2024-05-14 20:01:12.000000 hackerargs-1.1.0/hackerargs.egg-info/top_level.txt
+-rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)      394 2024-05-14 19:59:34.000000 hackerargs-1.1.0/pyproject.toml
+-rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)       38 2024-05-14 20:01:12.847644 hackerargs-1.1.0/setup.cfg
+drwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)        0 2024-05-14 20:01:12.817928 hackerargs-1.1.0/tests/
+-rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)      414 2024-05-14 19:08:39.000000 hackerargs-1.1.0/tests/test_access.py
+-rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)      934 2024-05-14 19:08:39.000000 hackerargs-1.1.0/tests/test_argv_string.py
+-rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)      776 2024-05-12 21:02:22.000000 hackerargs-1.1.0/tests/test_positional.py
+-rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)      913 2024-05-12 21:02:25.000000 hackerargs-1.1.0/tests/test_priority.py
```

### Comparing `hackerargs-1.0.0/LICENSE` & `hackerargs-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hackerargs-1.0.0/hackerargs/args.py` & `hackerargs-1.1.0/hackerargs/args.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,232 +1,245 @@
+from __future__ import annotations
 import sys
 import os
 from pathlib import Path
 import argparse
 import yaml
-from typing import Any, Optional, Union
+from typing import Any, Optional
 import logging
+from collections.abc import MutableMapping
 
 from .strict_bool_yaml import StrictBoolSafeLoader
 from . import argparse_access
 
 logger = logging.getLogger('hackerargs')
 
 
-def yaml_load(stream) -> Union[dict[str, Any], Any]:
+def yaml_load(stream) -> dict[str, Any] | Any:
     """ Parse stream using StrictBoolSafeLoader.
         If stream is yaml-formatted string or file, then returns parsed
         dict[str -> Any] where values have inferred python types.
         If stream is string, returns it cast to inferred python type.
 
         Uses PyYAML parser, which largely supports YAML v1.1
         https://yaml.org/spec/1.1/
         other than *not* parsing yes/no/on/off as booleans.
     """
     return yaml.load(stream, Loader = StrictBoolSafeLoader)
 
 
-class WriteOnceDict:
-    def __init__(self):
-        self._privatedict = dict()
-
-    def __contains__(self, key: str) -> bool:
-        return bool(key in self._privatedict)
-
-    def __repr__(self) -> str:
-        return str(self._privatedict)
+def get_yaml(inputs: list[str | argparse.ArgumentParser]) -> str | None:
+    def is_yaml(x: str | argparse.ArgumentParser) -> bool:
+        yaml_exts = ['.yaml', '.yml']
+        return type(x) == str and any(x.endswith(ye) for ye in yaml_exts)
+    yaml_files = [inp for inp in inputs if is_yaml(inp)]
+    if len(yaml_files) > 1:
+        raise ValueError('Must provide zero or one yaml files.')
+    return yaml_files[0] if len(yaml_files) != 0 else None
     
-    def __getitem__(self, key: str) -> Any:
-        return self._privatedict[key]
     
-    def __getattr__(self, key: str) -> Any:
-        return self._privatedict[key]
+def get_argparser(
+    inputs: list[str | argparse.ArgumentParser]
+) -> argparse.ArgumentParser | None:
+    is_argparser = lambda x: type(x) == argparse.ArgumentParser
+    parsers = [inp for inp in inputs if is_argparser(inp)]
+    if len(parsers) > 1:
+        raise ValueError('Must provide zero or one ArgumentParsers.')
+    return parsers[0] if len(parsers) != 0 else None
+
 
-    def __setattr__(self, key: str, value: Any) -> None:
-        if '_privatedict' in dir(self) and key in self._privatedict:
-            raise KeyError((
-                'Attempting to set class variable with same name '
-                'as key in WriteOnceDict.'
+def get_priority_yaml(parse_args_yaml: str | None, argv: list[str]) -> str | None:
+    """ Prioritize between yaml input to `parse_args` method,
+        and --config yaml in argv, returning a single yaml file for loading.
+        Returns None if neither yaml is found.
+    """
+    # get possible yaml from --config cli arg
+    if '--config' in argv:
+        cli_yaml = argv[argv.index('--config') + 1]
+    else:
+        cli_yaml = None
+
+    if parse_args_yaml and not cli_yaml:
+        return parse_args_yaml
+    elif not parse_args_yaml and cli_yaml:
+        return cli_yaml
+    elif parse_args_yaml and cli_yaml:
+        if parse_args_yaml != cli_yaml:
+            logger.warning((
+                f'Called parse_args with {parse_args_yaml}, '
+                f'but using {cli_yaml} instead, from --config CLI option'
             ))
-        super().__setattr__(key, value)
-        return
+        return cli_yaml
+    return None
+
+
+def check_duplicate_argv_keys(argv: list[str]) -> None:
+    is_key = lambda x: x.startswith('-') or x.startswith('--')
+    keys = [k for k in argv if is_key(k)]
+    if len(set(keys)) < len(keys):
+        raise ValueError(f'Found duplicate keys in {keys=}')
+    return
+
+
+def get_user_no_spec_keys( 
+    parser_dict: dict, 
+    parser: argparse.ArgumentParser, 
+    argv: list[str]
+) -> list[str]:
+    """ parser_dict: result from ArgumentParser.parse_known_args()
+        Returns list of keys in parser_dict that the user did not specify,
+        and are not positional arguments: argparser default values were
+        used for these.
+    """
+    no_user_spec = lambda k: f'--{k}' not in argv and f'-{k}' not in argv
+    positional_args = argparse_access.get_positional_keys(parser)
+    return [key for key in parser_dict.keys()
+            if no_user_spec(key) and key not in positional_args]
+
+
+class WriteOnceDict(MutableMapping, dict):
+    __getitem__ = dict.__getitem__
+    __iter__ = dict.__iter__
+    __len__ = dict.__len__
+
+    def __init__(self):
+        """ dict where each key can be written to only once,
+            and entries cannot be deleted.
+
+            Subclasses MutableMapping and dict, so it supports standard dict
+            methods like: keys(), get(), items(), setdefault(), values().
+        """
+        pass
+
+    def __getattr__(self, key: str) -> Any:
+        return self[key]
 
     def __setitem__(self, key: str, value: Any) -> None:
-        if key in self._privatedict:
-            raise KeyError('Write-once only dict')
-        self._privatedict[key] = value
+        if key in self:
+            raise KeyError(f'{key} has already been set.')
+        dict.__setitem__(self, key, value)
         return
 
     def __delitem__(self, key: str) -> None:
-        raise KeyError('Cannot delete items in write-once only dict')
-
-    def get(self, key: str) -> Any:
-        return self._privatedict[key]
+        raise KeyError('Cannot delete from WriteOnceDict.')
 
     def setdefault(self, key: str, default_value: Any) -> Any:
-        """ If key is not in args, set args[key] = default_value.
-            Then return args[key].
-            Ensures that values are never overwritten.
+        """ If key does not exist, store {key: default_value}.
+            Returns value of key. Ensures that values are never overwritten.
         """
-        if key not in self._privatedict:
-            self._privatedict[key] = default_value
-        return self._privatedict[key]
+        if key not in self:
+            self[key] = default_value
+        return self[key]
     
-    def keys(self):
-        return self._privatedict.keys()
-
-    def items(self):
-        return self._privatedict.items()
-
-    def parse_args(self, *inps: list[str]) -> None:
-        """ Parse args from sys.argv, and optional inputs
-            config_yaml, ArgumentParser.
-            When --conflig cli arg is set, prioritizes that yaml file.
+    def parse_args(
+        self,
+        *inputs: list[str | argparse.ArgumentParser],
+        argv: Optional[list[str]] = None,
+    ) -> None:
+        """ Parse CLI args using argparse.ArgumentParser and load YAML config.
+            If argv is given, use that instead of sys.argv.
 
+            Initialization priority
+            -----------------------
+            1. (Highest priority) argparse, user-specified values
+            2. Unknown CLI args specified by user in --{key} {val} format
+            3. YAML file. YAML provided by --config {yaml} CLI option takes
+                priority over yaml_file provided as argument to parse_args.
+            4. (Lowest) argparse default values for options not specified by user
+            
             Usage
             -----
-            parse_args()
-                If --config {yaml_file} is set, loads that yaml first.
-                Then, parses CLI args in `--{key} {val}` format,
-                updating hackerargs.
-
-            parse_args(ArgumentParser)
-                If --config {yaml_file} is set, loads that yaml first.
-                Calls ArgumentParser.parse_args(), and uses output to
-                update hackerargs. Then parses unknown CLI args in
-                `--{key} {val}` format, updating hackerargs.
-            
-            parse_args(yaml_file)
-                If no --config CLI option is set, loads from yaml_file first.
-                Otherwise, uses --config yaml instead, and raises a warning.
-                Then, parses CLI args in `--{key} {val}` format,
-                updating hackerargs.
-            
-            parse_args(yaml_file, ArgumentParser) or 
-            parse_args(ArgumentParser, yaml_file)
-                If no --config CLI option is set, loads from yaml_file first.
-                Otherwise, uses --config yaml instead, and raises a warning.
-                Calls ArgumentParser.parse_args(), and uses output to
-                update hackerargs. Then parses unknown CLI args in
-                `--{key} {val}` format, updating hackerargs.
+            - parse_args()
+            - parse_args(argparse.ArgumentParser)
+            - parse_args(yaml_file)
+            - parse_args(yaml_file, ArgumentParser) or 
+              parse_args(ArgumentParser, yaml_file)
+            argv_string is a named optional parameter:
+            - parse_args(argv = ['--string', 'text', '--float', '3.14'])
+            - ...
+            - parse_args(ArgumentParser, yaml_file,
+                argv = ['--string', 'text', '--float', '3.14'])
         """
-        if len(self._privatedict) != 0:
-            raise ValueError((
-                'Expected empty hackerargs. Do not set anything in hackerargs '
-                'before calling `parse_args`.'
-            ))
+        logger.debug('f{inputs=}')
+        if len(self) != 0:
+            raise ValueError('hackerargs must be empty to call `parse_args`.')
+
+        maybe_yaml = get_yaml(inputs)
+        maybe_parser = get_argparser(inputs)
+        if argv is None:
+            argv = sys.argv[1:]
+        logger.debug(f'Found {argv=}')
+        check_duplicate_argv_keys(argv)
 
-        def is_yaml(x: Any) -> bool:
-            return type(x) == str and (x.endswith('.yaml') or x.endswith('.yml'))
-        yaml_files = [inp for inp in inps if is_yaml(inp)]
-        if len(yaml_files) > 1:
-            raise ValueError('Must provide zero or one yaml files.')
-        maybe_yaml = yaml_files[0] if len(yaml_files) != 0 else None
-        
-        parsers = [inp for inp in inps if type(inp) == argparse.ArgumentParser]
-        if len(parsers) > 1:
-            raise ValueError('Must provide zero or one ArgumentParsers.')
-        maybe_parser = parsers[0] if len(parsers) != 0 else None
-
-        # find possible yaml file from --config cli arg
-        argv = sys.argv
-        if '--config' in argv:
-            cli_yaml = argv[argv.index('--config') + 1]
+        # form argparser
+        if maybe_parser is None:
+            parser = argparse.ArgumentParser(allow_abbrev = False)
         else:
-            cli_yaml = None
+            parser = maybe_parser
 
-        # init from yaml
-        if maybe_yaml and not cli_yaml:
-            self.__init_from_yaml(maybe_yaml)
-        elif not maybe_yaml and cli_yaml:
-            self.__init_from_yaml(cli_yaml)
-        elif maybe_yaml and cli_yaml:
-            if maybe_yaml != cli_yaml:
-                logger.warning((
-                    f'Called parse_args with {maybe_yaml}, '
-                    f'but using {cli_yaml} instead, from --config CLI option'
-                ))
-            self.__init_from_yaml(cli_yaml)
+        parser_namespace, unknown = parser.parse_known_args(argv)
+        parser_dict = vars(parser_namespace)
+        logger.debug(f'Found parser known dict {parser_dict}')
+
+        no_spec_keys = get_user_no_spec_keys(parser_dict, parser, argv)
+        spec_keys = [k for k in parser_dict.keys() if k not in no_spec_keys]
+
+        logger.info((
+            'hackerargs: (Priority 1 -- highest) '
+            'Updating with ArgumentParser args specified by user'
+        ))
+        for key in spec_keys:
+            value = parser_dict[key]
+            # if type != str, value has type from argparse already
+            self[key] = yaml_load(value) if type(value) == str else value
+
+        logger.info((
+            'hackerargs: (Priority 2) '
+            'Updating with unknown CLI args specified by user'
+        ))
+        self.__update_with_unknown_cli_args(unknown)
 
-        self.__parse_cli_args(maybe_parser)
+        logger.info((
+            'hackerargs: (Priority 3) '
+            'Updating with YAML config'
+        ))
+        yaml_fn = get_priority_yaml(maybe_yaml, argv)
+        if yaml_fn is not None:
+            self.__load_yaml_setdefault(yaml_fn)
+
+        logger.info((
+            'hackerargs: (Priority 4) '
+            'Updating with argparser default values, not specified by user'
+        ))
+        for key in no_spec_keys:
+            value = parser_dict[key]
+            # if type != str, value has type from argparse already
+            self.setdefault(key, yaml_load(value) if type(value) == str else value)
         return
 
-    def __init_from_yaml(self, yaml_fn: str) -> None:
-        logger.info(f'Loading hackerargs from {yaml_fn} ...')
+    def __load_yaml_setdefault(self, yaml_fn: str) -> None:
+        logger.info(f'Loading args from {yaml_fn} ...')
         with open(yaml_fn) as f:
-            args = yaml_load(f)
-        self._privatedict = args
-        return
-
-    def __parse_cli_args(
-        self, 
-        parser: Optional[argparse.ArgumentParser] = None
-    ) -> None:
-        """ Parse command-line arguments, updating hackerargs.
-            If ArgumentParser is given, use it to parse sys.argv first.
-            Unknown args must follow `--{key} {val}` format, and values
-            have types inferred by yaml loader.
-        """
-        if parser is None:
-            parser = argparse.ArgumentParser(allow_abbrev = False)
-
-        logger.info('Updating arguments with command-line options ...')
-        args_namespace, unknown = parser.parse_known_args()
-        args_dict = vars(args_namespace)
-
-        positional_args = argparse_access.get_positional_keys(parser)
-
-        # Update with parsed args
-        argv = sys.argv
-        no_spec = lambda k: f'--{k}' not in argv and f'-{k}' not in argv
-        logger.debug(f'argparse found {args_dict.items()=}')
-        for key, val in args_dict.items():
-            if (no_spec(key)
-                and key in self._privatedict
-                and key not in positional_args
-            ):
-                # k, v parsed by argparser, but not specified by user as
-                # optional arg, and not as positional arg,
-                # means default value must have been used
-                logger.info((
-                    f'argparse attempting to use default for {key=} '
-                    f'(not specified by user), but {key=} is in hackerargs '
-                    'already. No update made: yaml file takes priority.'
-                ))
-                continue
-
-            if type(val) == str:
-                self._privatedict[key] = yaml_load(val)
-            else:
-                # val type parsed with argparse
-                self._privatedict[key] = val
-
-        self.__update_with_unknown_cli_args(unknown)
+            yaml_args = yaml_load(f)
+        for key, value in yaml_args.items():
+            self.setdefault(key, value)
         return
 
     def __update_with_unknown_cli_args(self, unknown: list[str]) -> None:
         """ Update with unknown CLI args, of form `--{key} {val}. """
         logger.debug(f'Found {unknown=}')
         if len(unknown) % 2 != 0:
-            raise ValueError('Require even number of unknown arguments')
-        seen_keys = set()
-        for i in range(len(unknown) // 2):
-            key = unknown[i * 2]
-            val = unknown[i * 2 + 1]
-
-            if key[:2] != '--':
-                raise ValueError(
-                    f'Keys must start with --, but {key=} does not'
-                )
-            if key in seen_keys:
-                raise ValueError(f'Duplicate found: {key=}')
-            seen_keys.add(key)
-
-            trimmed_key = key[2:]
-            self._privatedict[trimmed_key] = yaml_load(val)
+            raise ValueError((
+                'Require even number of unknown arguments, but found '
+                f'{unknown=}'
+            ))
+        for key, val in zip(unknown[0::2], unknown[1::2]):
+            if not key.startswith('--'):
+                raise ValueError(f'Unknown CLI {key=} must starts with --')
+            self[key[2:]] = yaml_load(val)
         return
 
     def save_to_yaml(self, out_yaml_file: str) -> None:
         """ Saves args into yaml file.
             Create parent folders recursively if needed.
         """
         Path(os.path.dirname(out_yaml_file)).mkdir(
```

### Comparing `hackerargs-1.0.0/hackerargs/strict_bool_yaml.py` & `hackerargs-1.1.0/hackerargs/strict_bool_yaml.py`

 * *Files identical despite different names*

### Comparing `hackerargs-1.0.0/tests/test_positional.py` & `hackerargs-1.1.0/tests/test_positional.py`

 * *Files identical despite different names*

### Comparing `hackerargs-1.0.0/tests/test_priority.py` & `hackerargs-1.1.0/tests/test_priority.py`

 * *Files identical despite different names*

