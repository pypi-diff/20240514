# Comparing `tmp/tempit-0.1.4.tar.gz` & `tmp/tempit-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tempit-0.1.4.tar", last modified: Mon May 13 08:54:15 2024, max compression
+gzip compressed data, was "tempit-0.1.5.tar", last modified: Mon May 13 16:41:37 2024, max compression
```

## Comparing `tempit-0.1.4.tar` & `tempit-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 08:54:15.596791 tempit-0.1.4/
--rw-rw-rw-   0        0        0     1068 2024-05-10 08:37:29.000000 tempit-0.1.4/LICENSE.txt
--rw-rw-rw-   0        0        0     5000 2024-05-13 08:54:15.595785 tempit-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     4341 2024-05-13 07:52:51.000000 tempit-0.1.4/README.md
--rw-rw-rw-   0        0        0       42 2024-05-13 08:54:15.597785 tempit-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      878 2024-05-13 07:54:34.000000 tempit-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-13 08:54:15.571436 tempit-0.1.4/tempit/
--rw-rw-rw-   0        0        0       50 2024-05-09 20:06:13.000000 tempit-0.1.4/tempit/__init__.py
--rw-rw-rw-   0        0        0     9656 2024-05-13 06:36:00.000000 tempit-0.1.4/tempit/core.py
--rw-rw-rw-   0        0        0     5498 2024-05-10 06:26:45.000000 tempit-0.1.4/tempit/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-13 08:54:15.592773 tempit-0.1.4/tempit.egg-info/
--rw-rw-rw-   0        0        0     5000 2024-05-13 08:54:15.000000 tempit-0.1.4/tempit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2024-05-13 08:54:15.000000 tempit-0.1.4/tempit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 08:54:15.000000 tempit-0.1.4/tempit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-13 08:54:15.000000 tempit-0.1.4/tempit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-13 08:54:15.000000 tempit-0.1.4/tempit.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-13 08:54:15.591153 tempit-0.1.4/tests/
--rw-rw-rw-   0        0        0    12577 2024-05-13 08:25:53.000000 tempit-0.1.4/tests/test_tempit.py
+drwxrwxrwx   0        0        0        0 2024-05-13 16:41:37.622376 tempit-0.1.5/
+-rw-rw-rw-   0        0        0     1068 2024-05-10 08:37:29.000000 tempit-0.1.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     7236 2024-05-13 16:41:37.621372 tempit-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     6577 2024-05-13 16:35:58.000000 tempit-0.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-13 16:41:37.622376 tempit-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      878 2024-05-13 14:57:01.000000 tempit-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 16:41:37.602375 tempit-0.1.5/tempit/
+-rw-rw-rw-   0        0        0       50 2024-05-09 20:06:13.000000 tempit-0.1.5/tempit/__init__.py
+-rw-rw-rw-   0        0        0    11238 2024-05-13 16:16:07.000000 tempit-0.1.5/tempit/core.py
+-rw-rw-rw-   0        0        0     5498 2024-05-10 06:26:45.000000 tempit-0.1.5/tempit/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-13 16:41:37.618377 tempit-0.1.5/tempit.egg-info/
+-rw-rw-rw-   0        0        0     7236 2024-05-13 16:41:37.000000 tempit-0.1.5/tempit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2024-05-13 16:41:37.000000 tempit-0.1.5/tempit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 16:41:37.000000 tempit-0.1.5/tempit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-13 16:41:37.000000 tempit-0.1.5/tempit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-13 16:41:37.000000 tempit-0.1.5/tempit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 16:41:37.616373 tempit-0.1.5/tests/
+-rw-rw-rw-   0        0        0    12928 2024-05-13 16:32:13.000000 tempit-0.1.5/tests/test_tempit.py
```

### Comparing `tempit-0.1.4/LICENSE.txt` & `tempit-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tempit-0.1.4/PKG-INFO` & `tempit-0.1.5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tempit
-Version: 0.1.4
+Version: 0.1.5
 Summary: A dead simple time decorator
 Home-page: https://github.com/mcrespoae/tempit
 Author: mcrespoae
 Author-email: info@mariocrespo.es
 Keywords: tempit,time,decorator,performance,concurrency,parallel,benchmark
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
@@ -83,50 +83,85 @@
 
 More examples can be found in the [examples.py](examples/examples.py) script.
 
 ## Features
 
 - Simplified usage.
 - Accurate measurement of function execution time.
-- Support for `classmethod` and `staticmethods`.
+- Support for functions, methods, `classmethod`, `staticmethods` and classes.
 - Parallel execution mode for performance measurement.
 - Human-readable time formatting.
 - Optional verbose mode for detailed information.
+- Optional recursion checker.
 
 ## Parameters
 
 Using the decorator @tempit without any parameters executes the function once and displays the execution time. However, you can enhance the experience using the following arguments:
 
 - `run_times` (int, optional): Specifies the number of function executions. Defaults to 1.
 - `concurrency_mode` (bool, optional): Determines the concurrency mode for the function execution. It uses [joblib](https://pypi.org/project/joblib/) for parallel computing. The  default execution backend is "loky" but if the function is being triggered other than the main thread or main process, the backend will be changed to multithreading to aovid pickle errors. If, for any other reason, fails, the program will try to execute the func run_times non concurrently in the main process. Defaults to True.
 - `verbose` (bool, optional): Controls whether detailed information is printed after execution. Defaults to False.
+- `check_for_recursion` (bool, optional): Checks for recursion in the decorated function. Please, read the [Recursive functions](#recursive-functions) for detailed information. Defaults to False.
 
-## Note with recursive functions
+## Recursive functions
 
-This package doesn't work well with recursive functions. The specific reason and limitation are that using recursive functions with this package may result in very verbose output, making it difficult to read, especially for larger values.
+Measuring the time of recursive functions using decorators can be tricky due to potential verbosity in output. Using recursive functions with this package may result in very verbose output (one per each recursive call plus the original one), making it difficult to read.
 
-To avoid this issue, you can encapsulate the recursive function within another function and call it without printing messages. Here's an example:
+There are two potential solutions for this issue, [use the recursion detector](#using-the-check_for_recursion-parameter) or [encapsulating the recursive function](#encapsulating-the-recursive-function).
+
+### Using the `check_for_recursion` parameter
+
+If you're aware that your function utilizes recursion, you can use the `check_for_recursion` parameter.
+
+Activating this option has some overhead in performance but it enables users to decorate recursive functions with a clean output.
+
+```python
+@tempit(run_times=3, concurrent_execution=True, verbose=False, check_for_recursion=True)
+def recursive_func(n):
+    if n == 0:
+        return 0
+    else:
+        return n + recursive_func(n - 1)
+
+
+# Using the check_for_recursion parameter for the tempit decorator recursive function
+result = recursive_func(3)
+```
+
+### Encapsulating the recursive function
+
+Another option is to encapsulate the recursive function within another function then, decorate and call the parent function. Here's an example:
 
 ```python
 @tempit
 def encapsulated_recursive_function(n):
     """A non-verbose wrapper for the recursive function."""
     def recursive_func(n):
         if n == 0:
             return 0
         else:
             return n + recursive_func(n - 1)
 
     return recursive_func(n)
 
-# Using the encapsulated recursive function
+# Encapsulating the recursive function
 result = encapsulated_recursive_function(3)
 ```
 
-This approach makes the output cleaner and easier to read, especially when dealing with recursive functions with many calls.
+This approach enhances readability without incurring any performance penalties. However, its main drawback is that users must modify their code to measure this type of function.
+
+## Limitations
+
+While this package generally delivers excellent performance and reliability, it's essential to be aware of certain scenarios where using the `tempit` decorator could lead to unexpected behavior or crashes:
+
+- If a class is decorated with tempit, and subsequently, a new process is spawned after creating an instance of the class, calling a method within the newly created process may result in a `PicklingError`.
+
+This limitation arises due to how Python's pickling mechanism handles decorated classes and processes. When a decorated class instance is pickled for use in a separate process, inconsistencies in object references can occur, leading to pickling failures.
+
+To mitigate this issue, consider redesigning your application logic to avoid decorating classes that are used within processes spawned later in the program's execution. Alternatively, explore alternative serialization approaches or use dill or other serialization libraries that offer more robust handling of complex object hierarchies.
 
 ## Contributing
 
 Contributions are welcome! Please follow these guidelines when contributing:
 
 1. Fork the repository.
 2. Use `make install` to install all depedencies.
```

### Comparing `tempit-0.1.4/README.md` & `tempit-0.1.5/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -65,50 +65,85 @@
 
 More examples can be found in the [examples.py](examples/examples.py) script.
 
 ## Features
 
 - Simplified usage.
 - Accurate measurement of function execution time.
-- Support for `classmethod` and `staticmethods`.
+- Support for functions, methods, `classmethod`, `staticmethods` and classes.
 - Parallel execution mode for performance measurement.
 - Human-readable time formatting.
 - Optional verbose mode for detailed information.
+- Optional recursion checker.
 
 ## Parameters
 
 Using the decorator @tempit without any parameters executes the function once and displays the execution time. However, you can enhance the experience using the following arguments:
 
 - `run_times` (int, optional): Specifies the number of function executions. Defaults to 1.
 - `concurrency_mode` (bool, optional): Determines the concurrency mode for the function execution. It uses [joblib](https://pypi.org/project/joblib/) for parallel computing. The  default execution backend is "loky" but if the function is being triggered other than the main thread or main process, the backend will be changed to multithreading to aovid pickle errors. If, for any other reason, fails, the program will try to execute the func run_times non concurrently in the main process. Defaults to True.
 - `verbose` (bool, optional): Controls whether detailed information is printed after execution. Defaults to False.
+- `check_for_recursion` (bool, optional): Checks for recursion in the decorated function. Please, read the [Recursive functions](#recursive-functions) for detailed information. Defaults to False.
 
-## Note with recursive functions
+## Recursive functions
 
-This package doesn't work well with recursive functions. The specific reason and limitation are that using recursive functions with this package may result in very verbose output, making it difficult to read, especially for larger values.
+Measuring the time of recursive functions using decorators can be tricky due to potential verbosity in output. Using recursive functions with this package may result in very verbose output (one per each recursive call plus the original one), making it difficult to read.
 
-To avoid this issue, you can encapsulate the recursive function within another function and call it without printing messages. Here's an example:
+There are two potential solutions for this issue, [use the recursion detector](#using-the-check_for_recursion-parameter) or [encapsulating the recursive function](#encapsulating-the-recursive-function).
+
+### Using the `check_for_recursion` parameter
+
+If you're aware that your function utilizes recursion, you can use the `check_for_recursion` parameter.
+
+Activating this option has some overhead in performance but it enables users to decorate recursive functions with a clean output.
+
+```python
+@tempit(run_times=3, concurrent_execution=True, verbose=False, check_for_recursion=True)
+def recursive_func(n):
+    if n == 0:
+        return 0
+    else:
+        return n + recursive_func(n - 1)
+
+
+# Using the check_for_recursion parameter for the tempit decorator recursive function
+result = recursive_func(3)
+```
+
+### Encapsulating the recursive function
+
+Another option is to encapsulate the recursive function within another function then, decorate and call the parent function. Here's an example:
 
 ```python
 @tempit
 def encapsulated_recursive_function(n):
     """A non-verbose wrapper for the recursive function."""
     def recursive_func(n):
         if n == 0:
             return 0
         else:
             return n + recursive_func(n - 1)
 
     return recursive_func(n)
 
-# Using the encapsulated recursive function
+# Encapsulating the recursive function
 result = encapsulated_recursive_function(3)
 ```
 
-This approach makes the output cleaner and easier to read, especially when dealing with recursive functions with many calls.
+This approach enhances readability without incurring any performance penalties. However, its main drawback is that users must modify their code to measure this type of function.
+
+## Limitations
+
+While this package generally delivers excellent performance and reliability, it's essential to be aware of certain scenarios where using the `tempit` decorator could lead to unexpected behavior or crashes:
+
+- If a class is decorated with tempit, and subsequently, a new process is spawned after creating an instance of the class, calling a method within the newly created process may result in a `PicklingError`.
+
+This limitation arises due to how Python's pickling mechanism handles decorated classes and processes. When a decorated class instance is pickled for use in a separate process, inconsistencies in object references can occur, leading to pickling failures.
+
+To mitigate this issue, consider redesigning your application logic to avoid decorating classes that are used within processes spawned later in the program's execution. Alternatively, explore alternative serialization approaches or use dill or other serialization libraries that offer more robust handling of complex object hierarchies.
 
 ## Contributing
 
 Contributions are welcome! Please follow these guidelines when contributing:
 
 1. Fork the repository.
 2. Use `make install` to install all depedencies.
```

### Comparing `tempit-0.1.4/setup.py` & `tempit-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-VERSION = "0.1.4"
+VERSION = "0.1.5"
 setup(
     name="tempit",
     version=VERSION,
     author="mcrespoae",
     author_email="info@mariocrespo.es",
     packages=["tempit"],
     description="A dead simple time decorator",
```

### Comparing `tempit-0.1.4/tempit/core.py` & `tempit-0.1.5/tempit/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 import time
 from functools import partial, wraps
 from typing import Any, Callable, Dict, List, Tuple
 
 from .utils import print_tempit_values
 
 
-def tempit(*args: Any, run_times: int = 1, concurrent_execution: bool = True, verbose: bool = False) -> Callable:
+def tempit(
+    *args: Any,
+    run_times: int = 1,
+    concurrent_execution: bool = True,
+    verbose: bool = False,
+    check_for_recursion: bool = False,
+) -> Callable:
     """
     Decorator function that measures the execution time of a given function. It can be called like @tempit or using arguments @tempit(...)
 
     Args:
         args: contains the function to be decorated if no arguments are provided when calling the decorator
         run_times (int, optional): The number of times the function should be executed. Defaults to 1.
         concurrent_execution (bool, optional): This parameter will allow for the concurrent execution of the function using joblib.
@@ -40,38 +46,75 @@
             # function body
 
         # The decorated function can be used as usual
         result = my_function(arg1_value, arg2_value)
     """
 
     def decorator(
-        func: Callable, run_times: int = 1, concurrent_execution: bool = True, verbose: bool = False
+        func: Callable,
+        run_times: int = 1,
+        concurrent_execution: bool = True,
+        verbose: bool = False,
+        check_for_recursion: bool = False,
     ) -> Callable:
         @wraps(func)
         def tempit_wrapper(*args: Tuple, **kwargs: Dict) -> Any:
+            is_recursive, run_times_final, concurrent_execution_final = check_is_recursive_func(check_for_recursion, func, run_times, concurrent_execution)
             callable_func, args, args_to_print = extract_callable_and_args_if_method(func, *args)
             result, total_times, real_time = function_execution(
                 callable_func,
-                run_times,
-                concurrent_execution,
+                run_times_final,
+                concurrent_execution_final,
                 *args,
                 **kwargs,
             )
-
-            print_tempit_values(run_times, verbose, callable_func, total_times, real_time, *args_to_print, **kwargs)
-
+            if not is_recursive:
+                print_tempit_values(run_times, verbose, callable_func, total_times, real_time, *args_to_print, **kwargs)
             return result
 
         return tempit_wrapper
 
     if args:  # If arguments are not provided, return a decorator
-        return decorator(*args, run_times=run_times, concurrent_execution=concurrent_execution, verbose=verbose)
+        return decorator(
+            *args,
+            run_times=run_times,
+            concurrent_execution=concurrent_execution,
+            verbose=verbose,
+            check_for_recursion=check_for_recursion,
+        )
 
     else:  # Otherwise, return a partial function
-        return partial(decorator, run_times=run_times, concurrent_execution=concurrent_execution, verbose=verbose)
+        return partial(
+            decorator,
+            run_times=run_times,
+            concurrent_execution=concurrent_execution,
+            verbose=verbose,
+            check_for_recursion=check_for_recursion,
+        )
+
+
+def check_is_recursive_func(check_for_recursion: bool, func: Callable, run_times: int, concurrent_execution: bool) -> Tuple[bool, int, bool]:
+    """
+    Checks if the function is being called recursively.
+    Returns:
+        Tuple[bool, int, bool]: A tuple containing True if the function is being called recursively, False otherwise.
+        The second element is the number of times the function has been called, and the third element is a boolean indicating if the function has crashed.
+    """
+
+    if check_for_recursion:
+        import sys
+        from inspect import getframeinfo
+        func_name = func.__name__
+        func_filename = ""
+        if hasattr(func, '__code__'):
+            func_filename = func.__code__.co_filename
+        frame = getframeinfo(sys._getframe(2), context=0)
+        if frame.function == func_name and func_filename == frame.filename:
+            return True, 1, False
+    return False, run_times, concurrent_execution
 
 
 def extract_callable_and_args_if_method(func, *args) -> Tuple[Callable, Tuple, Tuple]:
     """
     Extracts the callable function and arguments from a given function, if it is a method.
     Args:
         func (Callable): The function to extract the callable from.
@@ -80,15 +123,14 @@
         Tuple[Callable, Tuple, Tuple]: A tuple containing the extracted callable function, the modified arguments,
         and the arguments to be printed.
     Raises:
         None
     """
     callable_func = func
     args_to_print = args
-
     is_method = hasattr(args[0], func.__name__) if args else False
     if is_method:
         args_to_print = args[1:]
         if isinstance(func, classmethod):
             args = (args[0].__class__,) + args[1:]  # type: ignore
             callable_func = func.__func__
         elif isinstance(func, staticmethod):
@@ -144,16 +186,17 @@
     total_times: List[float] = []
     for _ in range(run_times):
         start_time: float = time.perf_counter()
         try:
             result: Any = func(*args, **kwargs)
         except Exception as e:
             print(e)
-        end_time: float = time.perf_counter()
-        total_times.append(end_time - start_time)
+        finally:
+            end_time: float = time.perf_counter()
+            total_times.append(end_time - start_time)
     return result, total_times
 
 
 def tempit_with_concurrency(func: Callable, run_times: int, *args: Tuple, **kwargs: Dict) -> Tuple[Any, List[float]]:
     """
     Executes a given function concurrently a specified number of times using joblib.
```

### Comparing `tempit-0.1.4/tempit/utils.py` & `tempit-0.1.5/tempit/utils.py`

 * *Files identical despite different names*

### Comparing `tempit-0.1.4/tempit.egg-info/PKG-INFO` & `tempit-0.1.5/tempit.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tempit
-Version: 0.1.4
+Version: 0.1.5
 Summary: A dead simple time decorator
 Home-page: https://github.com/mcrespoae/tempit
 Author: mcrespoae
 Author-email: info@mariocrespo.es
 Keywords: tempit,time,decorator,performance,concurrency,parallel,benchmark
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
@@ -83,50 +83,85 @@
 
 More examples can be found in the [examples.py](examples/examples.py) script.
 
 ## Features
 
 - Simplified usage.
 - Accurate measurement of function execution time.
-- Support for `classmethod` and `staticmethods`.
+- Support for functions, methods, `classmethod`, `staticmethods` and classes.
 - Parallel execution mode for performance measurement.
 - Human-readable time formatting.
 - Optional verbose mode for detailed information.
+- Optional recursion checker.
 
 ## Parameters
 
 Using the decorator @tempit without any parameters executes the function once and displays the execution time. However, you can enhance the experience using the following arguments:
 
 - `run_times` (int, optional): Specifies the number of function executions. Defaults to 1.
 - `concurrency_mode` (bool, optional): Determines the concurrency mode for the function execution. It uses [joblib](https://pypi.org/project/joblib/) for parallel computing. The  default execution backend is "loky" but if the function is being triggered other than the main thread or main process, the backend will be changed to multithreading to aovid pickle errors. If, for any other reason, fails, the program will try to execute the func run_times non concurrently in the main process. Defaults to True.
 - `verbose` (bool, optional): Controls whether detailed information is printed after execution. Defaults to False.
+- `check_for_recursion` (bool, optional): Checks for recursion in the decorated function. Please, read the [Recursive functions](#recursive-functions) for detailed information. Defaults to False.
 
-## Note with recursive functions
+## Recursive functions
 
-This package doesn't work well with recursive functions. The specific reason and limitation are that using recursive functions with this package may result in very verbose output, making it difficult to read, especially for larger values.
+Measuring the time of recursive functions using decorators can be tricky due to potential verbosity in output. Using recursive functions with this package may result in very verbose output (one per each recursive call plus the original one), making it difficult to read.
 
-To avoid this issue, you can encapsulate the recursive function within another function and call it without printing messages. Here's an example:
+There are two potential solutions for this issue, [use the recursion detector](#using-the-check_for_recursion-parameter) or [encapsulating the recursive function](#encapsulating-the-recursive-function).
+
+### Using the `check_for_recursion` parameter
+
+If you're aware that your function utilizes recursion, you can use the `check_for_recursion` parameter.
+
+Activating this option has some overhead in performance but it enables users to decorate recursive functions with a clean output.
+
+```python
+@tempit(run_times=3, concurrent_execution=True, verbose=False, check_for_recursion=True)
+def recursive_func(n):
+    if n == 0:
+        return 0
+    else:
+        return n + recursive_func(n - 1)
+
+
+# Using the check_for_recursion parameter for the tempit decorator recursive function
+result = recursive_func(3)
+```
+
+### Encapsulating the recursive function
+
+Another option is to encapsulate the recursive function within another function then, decorate and call the parent function. Here's an example:
 
 ```python
 @tempit
 def encapsulated_recursive_function(n):
     """A non-verbose wrapper for the recursive function."""
     def recursive_func(n):
         if n == 0:
             return 0
         else:
             return n + recursive_func(n - 1)
 
     return recursive_func(n)
 
-# Using the encapsulated recursive function
+# Encapsulating the recursive function
 result = encapsulated_recursive_function(3)
 ```
 
-This approach makes the output cleaner and easier to read, especially when dealing with recursive functions with many calls.
+This approach enhances readability without incurring any performance penalties. However, its main drawback is that users must modify their code to measure this type of function.
+
+## Limitations
+
+While this package generally delivers excellent performance and reliability, it's essential to be aware of certain scenarios where using the `tempit` decorator could lead to unexpected behavior or crashes:
+
+- If a class is decorated with tempit, and subsequently, a new process is spawned after creating an instance of the class, calling a method within the newly created process may result in a `PicklingError`.
+
+This limitation arises due to how Python's pickling mechanism handles decorated classes and processes. When a decorated class instance is pickled for use in a separate process, inconsistencies in object references can occur, leading to pickling failures.
+
+To mitigate this issue, consider redesigning your application logic to avoid decorating classes that are used within processes spawned later in the program's execution. Alternatively, explore alternative serialization approaches or use dill or other serialization libraries that offer more robust handling of complex object hierarchies.
 
 ## Contributing
 
 Contributions are welcome! Please follow these guidelines when contributing:
 
 1. Fork the repository.
 2. Use `make install` to install all depedencies.
```

### Comparing `tempit-0.1.4/tests/test_tempit.py` & `tempit-0.1.5/tests/test_tempit.py`

 * *Files 1% similar despite different names*

```diff
@@ -281,14 +281,24 @@
     def test_run_from_other_process(self):
         with ProcessPoolExecutor(max_workers=1) as executor:
             future = executor.submit(my_process_function, 1, b=2)
             result = future.result()
 
         self.assertEqual(result, 3)
 
+    def test_recursive(self):
+        @tempit(run_times=2, concurrent_execution=True, verbose=True, check_for_recursion=True)
+        def my_function(n: int = 10):
+            if n < 2:
+                return n
+            return my_function(n - 2) + my_function(n - 1)
+
+        result = my_function(7)
+        self.assertEqual(result, 13)
+
     @unittest.skipUnless(not IN_GITHUB_ACTIONS, "Skip if running in GitHub Actions: too expensive.")
     def test_tempit_long_running_function(self):
         @tempit(run_times=4, concurrent_execution=True)
         def my_concurrent_function(a=2_000_000, n=16):
             for _ in range(a):
                 pass  #
             return fib(n=n)
```

