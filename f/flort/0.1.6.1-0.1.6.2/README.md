# Comparing `tmp/flort-0.1.6.1.tar.gz` & `tmp/flort-0.1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flort-0.1.6.1.tar", last modified: Thu May  9 20:39:34 2024, max compression
+gzip compressed data, was "flort-0.1.6.2.tar", last modified: Tue May 14 17:39:12 2024, max compression
```

## Comparing `flort-0.1.6.1.tar` & `flort-0.1.6.2.tar`

### file list

```diff
@@ -1,16 +1,20 @@
-drwxr-xr-x   0 nd        (1000) nd        (1000)        0 2024-05-09 20:39:34.435208 flort-0.1.6.1/
--rw-r--r--   0 nd        (1000) nd        (1000)     1500 2024-04-04 14:04:22.000000 flort-0.1.6.1/LICENSE
--rw-r--r--   0 nd        (1000) nd        (1000)     1718 2024-05-09 20:39:34.435208 flort-0.1.6.1/PKG-INFO
--rw-r--r--   0 nd        (1000) nd        (1000)     1264 2024-04-04 14:43:55.000000 flort-0.1.6.1/README.md
-drwxr-xr-x   0 nd        (1000) nd        (1000)        0 2024-05-09 20:39:34.434208 flort-0.1.6.1/flort/
--rw-r--r--   0 nd        (1000) nd        (1000)        0 2024-04-04 12:51:02.000000 flort-0.1.6.1/flort/__init__.py
--rw-r--r--   0 nd        (1000) nd        (1000)       60 2024-04-04 12:51:31.000000 flort-0.1.6.1/flort/__main__.py
--rw-r--r--   0 nd        (1000) nd        (1000)     4280 2024-05-09 20:39:07.000000 flort-0.1.6.1/flort/cli.py
-drwxr-xr-x   0 nd        (1000) nd        (1000)        0 2024-05-09 20:39:34.434208 flort-0.1.6.1/flort.egg-info/
--rw-r--r--   0 nd        (1000) nd        (1000)     1718 2024-05-09 20:39:34.000000 flort-0.1.6.1/flort.egg-info/PKG-INFO
--rw-r--r--   0 nd        (1000) nd        (1000)      223 2024-05-09 20:39:34.000000 flort-0.1.6.1/flort.egg-info/SOURCES.txt
--rw-r--r--   0 nd        (1000) nd        (1000)        1 2024-05-09 20:39:34.000000 flort-0.1.6.1/flort.egg-info/dependency_links.txt
--rw-r--r--   0 nd        (1000) nd        (1000)       46 2024-05-09 20:39:34.000000 flort-0.1.6.1/flort.egg-info/entry_points.txt
--rw-r--r--   0 nd        (1000) nd        (1000)        6 2024-05-09 20:39:34.000000 flort-0.1.6.1/flort.egg-info/top_level.txt
--rw-r--r--   0 nd        (1000) nd        (1000)       38 2024-05-09 20:39:34.435208 flort-0.1.6.1/setup.cfg
--rw-r--r--   0 nd        (1000) nd        (1000)      780 2024-05-09 20:39:31.000000 flort-0.1.6.1/setup.py
+drwxr-xr-x   0 nd        (1000) nd        (1000)        0 2024-05-14 17:39:12.550633 flort-0.1.6.2/
+-rw-r--r--   0 nd        (1000) nd        (1000)     1500 2024-04-04 14:04:22.000000 flort-0.1.6.2/LICENSE
+-rw-r--r--   0 nd        (1000) nd        (1000)     1743 2024-05-14 17:39:12.550633 flort-0.1.6.2/PKG-INFO
+-rw-r--r--   0 nd        (1000) nd        (1000)     1264 2024-04-04 14:43:55.000000 flort-0.1.6.2/README.md
+drwxr-xr-x   0 nd        (1000) nd        (1000)        0 2024-05-14 17:39:12.549633 flort-0.1.6.2/flort/
+-rw-r--r--   0 nd        (1000) nd        (1000)        0 2024-04-04 12:51:02.000000 flort-0.1.6.2/flort/__init__.py
+-rw-r--r--   0 nd        (1000) nd        (1000)       61 2024-05-14 17:13:43.000000 flort-0.1.6.2/flort/__main__.py
+-rw-r--r--   0 nd        (1000) nd        (1000)     4988 2024-05-14 17:38:03.000000 flort-0.1.6.2/flort/cli.py
+drwxr-xr-x   0 nd        (1000) nd        (1000)        0 2024-05-14 17:39:12.550633 flort-0.1.6.2/flort.egg-info/
+-rw-r--r--   0 nd        (1000) nd        (1000)     1743 2024-05-14 17:39:12.000000 flort-0.1.6.2/flort.egg-info/PKG-INFO
+-rw-r--r--   0 nd        (1000) nd        (1000)      287 2024-05-14 17:39:12.000000 flort-0.1.6.2/flort.egg-info/SOURCES.txt
+-rw-r--r--   0 nd        (1000) nd        (1000)        1 2024-05-14 17:39:12.000000 flort-0.1.6.2/flort.egg-info/dependency_links.txt
+-rw-r--r--   0 nd        (1000) nd        (1000)       46 2024-05-14 17:39:12.000000 flort-0.1.6.2/flort.egg-info/entry_points.txt
+-rw-r--r--   0 nd        (1000) nd        (1000)        9 2024-05-14 17:39:12.000000 flort-0.1.6.2/flort.egg-info/requires.txt
+-rw-r--r--   0 nd        (1000) nd        (1000)       12 2024-05-14 17:39:12.000000 flort-0.1.6.2/flort.egg-info/top_level.txt
+-rw-r--r--   0 nd        (1000) nd        (1000)       38 2024-05-14 17:39:12.550633 flort-0.1.6.2/setup.cfg
+-rw-r--r--   0 nd        (1000) nd        (1000)      803 2024-05-14 17:39:10.000000 flort-0.1.6.2/setup.py
+drwxr-xr-x   0 nd        (1000) nd        (1000)        0 2024-05-14 17:39:12.550633 flort-0.1.6.2/tests/
+-rw-r--r--   0 nd        (1000) nd        (1000)        0 2024-05-14 17:20:58.000000 flort-0.1.6.2/tests/__init__.py
+-rw-r--r--   0 nd        (1000) nd        (1000)     2028 2024-05-14 17:36:24.000000 flort-0.1.6.2/tests/test_cli.py
```

### Comparing `flort-0.1.6.1/LICENSE` & `flort-0.1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flort-0.1.6.1/PKG-INFO` & `flort-0.1.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: flort
-Version: 0.1.6.1
-Summary: A utilty to flatten your source code directory into a single file for LLM usage
+Version: 0.1.6.2
+Summary: A utility to flatten your source code directory into a single file for LLM usage
 Home-page: https://github.com/chris17453/flort
 Author: Chris Watkins
 Author-email: chris@watkinslabs.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: argparse
 
 # flort
 
 flort is a command-line tool for generating a single file with the contents of your code directories.. for use in LLMs.
 
 ## Installation
```

### Comparing `flort-0.1.6.1/README.md` & `flort-0.1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `flort-0.1.6.1/flort/cli.py` & `flort-0.1.6.2/flort/cli.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,108 +1,113 @@
 import os
 import argparse
 from pathlib import Path
+import logging
 
+# Configure logging
+logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
 
 def clean_content(file_path):
     """Cleans up the content of a file by removing unnecessary whitespace."""
     with open(file_path, 'r') as file:
         lines = file.readlines()
         cleaned_lines = [line.strip() for line in lines if line.strip()]
         return '\n'.join(cleaned_lines)
 
-def generate_tree(directory):
-    """Generates a tree structure of the given directory, ignoring .git folders."""
+def generate_tree(directories, extensions=None):
+    """Generates a tree structure for multiple directories."""
     tree_structure = ''
-    for root, dirs, files in os.walk(directory):
-        if '.git' in dirs:
-            dirs.remove('.git')  # Ignore .git folder
-        level = root.replace(directory, '').count(os.sep)
-        indent = '|   ' * level + '|-- '
-        tree_structure += f"{indent}{os.path.basename(root)}/\n"
-        sub_indent = '|   ' * (level + 1) + '|-- '
-        for file in files:
-            tree_structure += f"{sub_indent}{file}\n"
+    for directory in directories:
+        directory = str(directory)  # Convert directory to string
+        for root, dirs, files in os.walk(directory):
+            if extensions:
+                dirs[:] = [d for d in dirs if any(Path(root) / d / f for f in os.listdir(Path(root) / d) if Path(f).suffix in extensions)]
+                included_files = [f for f in files if Path(f).suffix in extensions]
+            else:
+                included_files = files
+            
+            level = root.replace(directory, '').count(os.sep)
+            indent = '|   ' * level + '|-- '
+            sub_indent = '|   ' * (level + 1) + '|-- '
+
+            if included_files or dirs:
+                tree_structure += f"{indent}{os.path.basename(root)}/\n"
+                for file in included_files:
+                    tree_structure += f"{sub_indent}{file}\n"
     return tree_structure
 
-
-def list_files(directory, compress=False, extensions=None):
-    """Lists files in the given directory with optional compression."""
-    directory_path = Path(directory)
-    if not directory_path.is_dir():
-        print(f"The path {directory} is not a valid directory.")
-        return
-    
-    print(f"Processing directory: {directory_path}")
+def list_files(directories, compress=False, extensions=None):
+    """Lists files in multiple directories."""
+    try:
+        files_info = []
+        num_files = 0
+        for directory in directories:
+            directory_path = Path(directory)
+            if not directory_path.is_dir():
+                logging.error(f"The path {directory} is not a valid directory.")
+                continue
+
+            #logging.info(f"Processing directory: {directory_path}")
+
+            for file_path in directory_path.rglob('*'):
+                if file_path.is_file() and '.git' not in file_path.parts:
+                    if extensions is None or file_path.suffix.lower() in extensions:
+                        num_files += 1
+                        file_info = [f"Path: {file_path}", f"File: {file_path.name}", "-------"]
+
+                        try:
+                            if compress:
+                                compressed_content = clean_content(file_path)
+                                file_info.append(compressed_content)
+                            else:
+                                with open(file_path, 'r') as f:
+                                    file_info.append(f.read())
+                        except Exception as e:
+                            logging.error(f"Error reading file {file_path}: {e}")
+                        
+                        files_info.append('\n'.join(file_info))
+
+        logging.info(f"Number of eligible files processed: {num_files}")
+        return '\n'.join(files_info)
+    except Exception as e:
+        logging.error(f"Error processing directories: {e}")
+        return ""
     
-    files_info = ""
-    num_files = 0
-    for file_path in directory_path.rglob('*'):
-        if file_path.is_file() and '.git' not in file_path.parts:
-            if extensions is None or file_path.suffix.lower() in extensions:
-                num_files += 1
-                file_info = f"Path: {file_path}\n"
-                file_info += f"File: {file_path.name}\n"
-                file_info += "-------\n"
-
-                if compress:
-                    compressed_content = clean_content(file_path)
-                    file_info += compressed_content
-                else:
-                    with open(file_path, 'r') as f:
-                        file_data = f.read()
-                        file_info += file_data
-                    
-                files_info += file_info
-    
-    print(f"Number of eligible files processed: {num_files}")
-    return files_info
-
-def write_file(file_path,data):
+def write_file(file_path, data):
     """Writes data to the specified file."""
     with open(file_path, 'w') as file:
         file.write(data)
-    print("Output written to file.")
+    logging.info(f"Output written to file: {file_path}")
+
+def print_configuration(directories, extensions):
+    """Prints the directories and extensions being processed."""
+    logging.info(f"Directories being processed: {', '.join(directories)}")
+    logging.info(f"File extensions being processed: {', '.join(extensions)}")
+
 def main():
     """Main function to parse arguments and execute operations."""
-    parser = argparse.ArgumentParser(description="%(prog): List and optionally compress files in a directory.")
-    parser.add_argument('directory', metavar='DIRECTORY', type=str, help='Directory to list files from.')
+    parser = argparse.ArgumentParser(description="flort: List and optionally compress files in directories.", prog='flort')
+    parser.add_argument('directories', metavar='DIRECTORY', type=str, nargs='+', help='Directories to list files from.')
     parser.add_argument('--compress', default=False, action='store_true', help='Compress the listed files by removing whitespace.')
     parser.add_argument('--output', type=str, default="stdio", help='Output file path. Defaults to stdout if not specified.')
-    parser.add_argument('--php', action='store_true', help='Include PHP files.')
-    parser.add_argument('--js', action='store_true', help='Include JavaScript files.')
-    parser.add_argument('--py', action='store_true', help='Include Python files.')
-    parser.add_argument('--c', action='store_true', help='Include C files.')
-    parser.add_argument('--cpp', action='store_true', help='Include C++ files.')    
-    parser.add_argument('--sh', action='store_true', help='Include sh files.')    
-    parser.add_argument('--no-tree', action='store_true', help='Dont print the tree at the beginning.')    
-    args = parser.parse_args()
-    
-    extensions = []
-    output = []
-    if args.php:
-        extensions.append('.php')
-    if args.js:
-        extensions.append('.js')
-    if args.py:
-        extensions.append('.py')
-    if args.c:
-        extensions.append('.c')
-        extensions.append('.h')
-    if args.cpp:
-        extensions.append('.cpp')
-        extensions.append('.h')
-    if args.sh:
-        extensions.append('.sh')
-    if args.no_tree != True:
-        output.append(generate_tree(args.directory))
-    
-    output.append(list_files(args.directory, compress=args.compress, extensions=extensions))
+    parser.add_argument('--no-tree', action='store_true', help='Do not print the tree at the beginning.')
+    args, unknown_args = parser.parse_known_args()
+
+    # Treat unknown args as extensions that start with '--'
+    extensions = [f".{ext.lstrip('-')}" for ext in unknown_args if ext.startswith('--')]
+
+    # Print configuration
+    print_configuration(args.directories, extensions)
 
-    if args.output != "stdio":    
-        write_file(args.output, "\n".join(output))
+    output_content = []
+    if not args.no_tree:
+        output_content.append(generate_tree(args.directories, extensions=extensions))
+
+    output_content.append(list_files(args.directories, compress=args.compress, extensions=extensions))
+
+    if args.output != "stdio":
+        write_file(args.output, "\n".join(output_content))
     else:
-        print("\n".join(output))
+        print("\n".join(output_content))
 
 if __name__ == "__main__":
     main()
-
```

### Comparing `flort-0.1.6.1/flort.egg-info/PKG-INFO` & `flort-0.1.6.2/flort.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: flort
-Version: 0.1.6.1
-Summary: A utilty to flatten your source code directory into a single file for LLM usage
+Version: 0.1.6.2
+Summary: A utility to flatten your source code directory into a single file for LLM usage
 Home-page: https://github.com/chris17453/flort
 Author: Chris Watkins
 Author-email: chris@watkinslabs.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: argparse
 
 # flort
 
 flort is a command-line tool for generating a single file with the contents of your code directories.. for use in LLMs.
 
 ## Installation
```

### Comparing `flort-0.1.6.1/setup.py` & `flort-0.1.6.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from setuptools import setup, find_packages
 
 setup(
     name='flort',
-    version='0.1.6.1',
+    version='0.1.6.2',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'flort = flort.__main__:main'
         ]
     },
     install_requires=[
-        # Add any dependencies here
+        'argparse',
+        # Add other dependencies here
     ],
     author='Chris Watkins',
     author_email='chris@watkinslabs.com',
-    description='A utilty to flatten your source code directory into a single file for LLM usage',
+    description='A utility to flatten your source code directory into a single file for LLM usage',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/chris17453/flort',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: BSD License',
         'Operating System :: OS Independent',
```

