# Comparing `tmp/tinygui-1.0.0.tar.gz` & `tmp/tinygui-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinygui-1.0.0.tar", last modified: Thu Mar 14 06:37:43 2024, max compression
+gzip compressed data, was "tinygui-1.0.1.tar", last modified: Tue May 14 11:03:55 2024, max compression
```

## Comparing `tinygui-1.0.0.tar` & `tinygui-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-03-14 06:37:43.850327 tinygui-1.0.0/
--rw-rw-rw-   0        0        0     1093 2024-01-17 07:33:18.000000 tinygui-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      503 2024-03-14 06:37:43.848331 tinygui-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      612 2024-03-14 06:30:58.000000 tinygui-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-14 06:37:43.850368 tinygui-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-14 06:37:43.814422 tinygui-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2024-03-14 06:37:43.822410 tinygui-1.0.0/src/tinygui/
--rw-rw-rw-   0        0        0       21 2024-03-14 06:29:18.000000 tinygui-1.0.0/src/tinygui/__init__.py
--rw-rw-rw-   0        0        0     1269 2024-03-14 06:30:58.000000 tinygui-1.0.0/src/tinygui/tinygui.py
-drwxrwxrwx   0        0        0        0 2024-03-14 06:37:43.847334 tinygui-1.0.0/src/tinygui.egg-info/
--rw-rw-rw-   0        0        0      503 2024-03-14 06:37:43.000000 tinygui-1.0.0/src/tinygui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2024-03-14 06:37:43.000000 tinygui-1.0.0/src/tinygui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-14 06:37:43.000000 tinygui-1.0.0/src/tinygui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-03-14 06:37:43.000000 tinygui-1.0.0/src/tinygui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 11:03:55.046754 tinygui-1.0.1/
+-rw-rw-rw-   0        0        0     1093 2024-05-13 06:57:48.000000 tinygui-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      511 2024-05-14 11:03:55.044742 tinygui-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      620 2024-05-14 10:36:13.000000 tinygui-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-14 11:03:55.046754 tinygui-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-14 11:03:55.027590 tinygui-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-14 11:03:55.033692 tinygui-1.0.1/src/tinygui/
+-rw-rw-rw-   0        0        0       21 2024-04-29 06:18:34.000000 tinygui-1.0.1/src/tinygui/__init__.py
+-rw-rw-rw-   0        0        0     1809 2024-05-09 03:08:39.000000 tinygui-1.0.1/src/tinygui/tinygui.py
+drwxrwxrwx   0        0        0        0 2024-05-14 11:03:55.043223 tinygui-1.0.1/src/tinygui.egg-info/
+-rw-rw-rw-   0        0        0      511 2024-05-14 11:03:55.000000 tinygui-1.0.1/src/tinygui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2024-05-14 11:03:55.000000 tinygui-1.0.1/src/tinygui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 11:03:55.000000 tinygui-1.0.1/src/tinygui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-14 11:03:55.000000 tinygui-1.0.1/src/tinygui.egg-info/top_level.txt
```

### Comparing `tinygui-1.0.0/LICENSE` & `tinygui-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tinygui-1.0.0/pyproject.toml` & `tinygui-1.0.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "tinygui"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name = "xiaoheli", email = "1173324325@qq.com" },
 ]
 dependencies = []
-description = "A small example package"
+description = "A small example package for gui"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `tinygui-1.0.0/src/tinygui/tinygui.py` & `tinygui-1.0.1/src/tinygui/tinygui.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import tkinter as tk
+import pygame
 from tkinter.ttk import *
 from tkinter import*
 pwd = ''
 root = ''
 def tk_init(txt=''):
     global pwd,root
     pwd = ''
@@ -43,8 +44,22 @@
     except:
         pass
     return str(pwd)
 
 def get_value():
     return str(pwd)
 
+# pygame窗口显示文本方法
+def draw_text(screen, text, pos, mark=0):
+    # 设置文本框的外观
+    text_box_rect = pygame.Rect(pos, (100, 40))
+    text_layer = pygame.Surface(pos, pygame.SRCALPHA)
+    text_layer.fill((255, 255, 255, 0))
+    screen.blit(text_layer, pos)
+    font = pygame.font.Font(None, 55)
+    text_surface = font.render(text, True, (0, 0, 0))
+    text_rect = text_surface.get_rect(center=text_box_rect.center)
+    screen.blit(text_surface, text_rect)
+    pygame.display.update()
+
+
```

