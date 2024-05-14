# Comparing `tmp/xdot-1.3.tar.gz` & `tmp/xdot-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xdot-1.3.tar", last modified: Sat Sep  9 16:09:06 2023, max compression
+gzip compressed data, was "xdot-1.4.tar", last modified: Tue May 14 09:49:14 2024, max compression
```

## Comparing `xdot-1.3.tar` & `xdot-1.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-09 16:09:06.643827 xdot-1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2023-09-09 16:09:06.639826 xdot-1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5496 2023-09-09 16:08:42.000000 xdot-1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-09 16:09:06.643827 xdot-1.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1811 2023-09-09 16:08:42.000000 xdot-1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-09 16:09:06.639826 xdot-1.3/xdot/
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2023-09-09 16:08:42.000000 xdot-1.3/xdot/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3262 2023-09-09 16:08:42.000000 xdot-1.3/xdot/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-09 16:09:06.639826 xdot-1.3/xdot/dot/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-09-09 16:08:42.000000 xdot-1.3/xdot/dot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4416 2023-09-09 16:08:42.000000 xdot-1.3/xdot/dot/lexer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6308 2023-09-09 16:08:42.000000 xdot-1.3/xdot/dot/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2996 2023-09-09 16:08:42.000000 xdot-1.3/xdot/dot/scanner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-09 16:09:06.639826 xdot-1.3/xdot/ui/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2023-09-09 16:08:42.000000 xdot-1.3/xdot/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13759 2023-09-09 16:08:42.000000 xdot-1.3/xdot/ui/_xdotparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5816 2023-09-09 16:08:42.000000 xdot-1.3/xdot/ui/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3589 2023-09-09 16:08:42.000000 xdot-1.3/xdot/ui/animation.py
--rw-r--r--   0 runner    (1001) docker     (127)    34503 2023-09-09 16:08:42.000000 xdot-1.3/xdot/ui/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)    23214 2023-09-09 16:08:42.000000 xdot-1.3/xdot/ui/elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2023-09-09 16:08:42.000000 xdot-1.3/xdot/ui/pen.py
--rw-r--r--   0 runner    (1001) docker     (127)    30024 2023-09-09 16:08:42.000000 xdot-1.3/xdot/ui/window.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-09 16:09:06.639826 xdot-1.3/xdot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2023-09-09 16:09:06.000000 xdot-1.3/xdot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      454 2023-09-09 16:09:06.000000 xdot-1.3/xdot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-09 16:09:06.000000 xdot-1.3/xdot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-09-09 16:09:06.000000 xdot-1.3/xdot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-09-09 16:09:06.000000 xdot-1.3/xdot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-09-09 16:09:06.000000 xdot-1.3/xdot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:49:14.262294 xdot-1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-14 09:49:14.262294 xdot-1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-05-14 09:48:56.000000 xdot-1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 09:49:14.262294 xdot-1.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1833 2024-05-14 09:48:56.000000 xdot-1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:49:14.258294 xdot-1.4/xdot/
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-14 09:48:56.000000 xdot-1.4/xdot/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3375 2024-05-14 09:48:56.000000 xdot-1.4/xdot/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:49:14.258294 xdot-1.4/xdot/dot/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-14 09:48:56.000000 xdot-1.4/xdot/dot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-05-14 09:48:56.000000 xdot-1.4/xdot/dot/lexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-05-14 09:48:56.000000 xdot-1.4/xdot/dot/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-05-14 09:48:56.000000 xdot-1.4/xdot/dot/scanner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:49:14.262294 xdot-1.4/xdot/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-14 09:48:56.000000 xdot-1.4/xdot/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13744 2024-05-14 09:48:56.000000 xdot-1.4/xdot/ui/_xdotparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5816 2024-05-14 09:48:56.000000 xdot-1.4/xdot/ui/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-05-14 09:48:56.000000 xdot-1.4/xdot/ui/animation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34503 2024-05-14 09:48:56.000000 xdot-1.4/xdot/ui/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23468 2024-05-14 09:48:56.000000 xdot-1.4/xdot/ui/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-14 09:48:56.000000 xdot-1.4/xdot/ui/pen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30366 2024-05-14 09:48:56.000000 xdot-1.4/xdot/ui/window.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:49:14.258294 xdot-1.4/xdot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-14 09:49:14.000000 xdot-1.4/xdot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-14 09:49:14.000000 xdot-1.4/xdot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 09:49:14.000000 xdot-1.4/xdot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-14 09:49:14.000000 xdot-1.4/xdot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-14 09:49:14.000000 xdot-1.4/xdot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-14 09:49:14.000000 xdot-1.4/xdot.egg-info/top_level.txt
```

### Comparing `xdot-1.3/PKG-INFO` & `xdot-1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: xdot
-Version: 1.3
+Version: 1.4
 Summary: Interactive viewer for Graphviz dot files
 Home-page: https://github.com/jrfonseca/xdot.py
 Author: Jose Fonseca
 Author-email: jose.r.fonseca@gmail.com
 License: LGPL
 Description: 
                 xdot.py is an interactive viewer for graphs written in Graphviz's dot
```

### Comparing `xdot-1.3/README.md` & `xdot-1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -110,14 +110,16 @@
       Q                         quit
       P                         print
       T                         toggle toolbar
       W                         zoom to fit
       Escape                    halt animation
       Ctrl-drag                 zoom in/out
       Shift-drag                zooms an area
+      Click (on edge)           focus edge's source node
+      Ctrl-click (on edge)      focus edge's *destination* node
 
 If `-` is given as input file then _xdot.py_ will read the dot graph from the standard input.
 
 Embedding
 ---------
 
 See included `sample.py` script for an example of how to embedded _xdot.py_ into another application.
```

### Comparing `xdot-1.3/setup.py` & `xdot-1.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # - https://docs.python.org/3/distutils/packageindex.html
 #
 
 from setuptools import setup
 
 setup(
     name='xdot',
-    version='1.3',
+    version='1.4',
     author='Jose Fonseca',
     author_email='jose.r.fonseca@gmail.com',
     url='https://github.com/jrfonseca/xdot.py',
     description="Interactive viewer for Graphviz dot files",
     long_description="""
         xdot.py is an interactive viewer for graphs written in Graphviz's dot
         language.
@@ -52,10 +52,11 @@
         'Programming Language :: Python :: 3 :: Only',
 
         'Topic :: Multimedia :: Graphics :: Viewers',
     ],
 
     install_requires=[
         'PyGObject',
-        'numpy'
+        'numpy',
+        'packaging',
     ],
 )
```

### Comparing `xdot-1.3/xdot/__init__.py` & `xdot-1.4/xdot/__init__.py`

 * *Files identical despite different names*

### Comparing `xdot-1.3/xdot/__main__.py` & `xdot-1.4/xdot/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,16 @@
   F                         find
   Q                         quit
   P                         print
   T                         toggle show/hide toolbar
   Escape                    halt animation
   Ctrl-drag                 zoom in/out
   Shift-drag                zooms an area
+  Click (on edge)           focus edge's source node
+  Ctrl-click (on edge)      focus edge's *destination* node
 '''
     )
     parser.add_argument(
         'inputfile', metavar='file', nargs='?',
         help='input file to be viewed')
     parser.add_argument(
         '-f', '--filter', choices=['dot', 'neato', 'twopi', 'circo', 'fdp'],
```

### Comparing `xdot-1.3/xdot/dot/lexer.py` & `xdot-1.4/xdot/dot/lexer.py`

 * *Files identical despite different names*

### Comparing `xdot-1.3/xdot/dot/parser.py` & `xdot-1.4/xdot/dot/parser.py`

 * *Files identical despite different names*

### Comparing `xdot-1.3/xdot/dot/scanner.py` & `xdot-1.4/xdot/dot/scanner.py`

 * *Files identical despite different names*

### Comparing `xdot-1.3/xdot/ui/_xdotparser.py` & `xdot-1.4/xdot/ui/_xdotparser.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 
 import colorsys
 import re
 import sys
 
-from distutils.version import LooseVersion
+from packaging.version import Version
 
 from ..dot.lexer import DotLexer
 from ..dot.parser import DotParser
 
 from ..ui.colors import lookup_color
 from ..ui.pen import Pen
 from ..ui import elements
@@ -260,15 +260,15 @@
     def __init__(self, xdotcode, graphviz_version=None):
         lexer = DotLexer(buf=xdotcode)
         DotParser.__init__(self, lexer)
 
         # https://github.com/jrfonseca/xdot.py/issues/92
         self.broken_backslashes = False
         if graphviz_version is not None and \
-                LooseVersion(graphviz_version) < LooseVersion("2.46.0"):
+                Version(graphviz_version) < Version("2.46.0"):
             self.broken_backslashes = True
 
         self.nodes = []
         self.edges = []
         self.shapes = []
         self.node_by_name = {}
         self.top_graph = True
```

### Comparing `xdot-1.3/xdot/ui/actions.py` & `xdot-1.4/xdot/ui/actions.py`

 * *Files identical despite different names*

### Comparing `xdot-1.3/xdot/ui/animation.py` & `xdot-1.4/xdot/ui/animation.py`

 * *Files identical despite different names*

### Comparing `xdot-1.3/xdot/ui/colors.py` & `xdot-1.4/xdot/ui/colors.py`

 * *Files identical despite different names*

### Comparing `xdot-1.3/xdot/ui/elements.py` & `xdot-1.4/xdot/ui/elements.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,24 +97,28 @@
     def get_text(self):
         return None
 
 
 class TextShape(Shape):
 
     LEFT, CENTER, RIGHT = -1, 0, 1
-    DEFAULT_FONTNAME = Gtk.Settings.get_default().get_property("gtk-font-name")
 
     def __init__(self, pen, x, y, j, w, t):
         Shape.__init__(self)
         self.pen = pen.copy()
         self.x = x
         self.y = y
         self.j = j  # Centering
         self.w = w  # width
         self.t = t  # text
+        default_settings = Gtk.Settings.get_default()
+        if default_settings:
+            self.default_fontname = default_settings.get_property("gtk-font-name")
+        else:
+            self.default_fontname = self.pen.fontname
 
     def _font_available(self, fontname, pango_context):
         available_fonts = [family.get_name() for family in pango_context.list_families()]
         return fontname in available_fonts
 
     def _draw(self, cr, highlight, bounding):
 
@@ -165,18 +169,18 @@
             layout.set_attributes(attrs)
 
             if self._font_available(self.pen.fontname, pango_context=context):
                 font.set_family(self.pen.fontname)
             else:
                 msg = "Font family {fontname!r} is not available, using {default!r}".format(
                     fontname=self.pen.fontname,
-                    default=self.DEFAULT_FONTNAME
+                    default=self.default_fontname
                 )
                 warnings.warn(msg)
-                font.set_family(self.DEFAULT_FONTNAME)
+                font.set_family(self.default_fontname)
 
             font.set_absolute_size(self.pen.fontsize*Pango.SCALE)
             layout.set_font_description(font)
 
             # set text
             layout.set_text(text, -1)
 
@@ -623,27 +627,28 @@
     def is_inside(self, x, y):
         if self.is_inside_begin(x, y):
             return True
         if self.is_inside_end(x, y):
             return True
         return False
 
-    def get_jump(self, x, y):
+    def get_jump(self, x, y, to_dst = False):
         for shape in self.shapes:
             x1, y1, x2, y2 = shape.bounding
             if (x1 - self.RADIUS) <= x and x <= (x2 + self.RADIUS) and (y1 - self.RADIUS) <= y and y <= (y2 + self.RADIUS):
                 break
 
         else:
             return None
 
         for shape in self.shapes:
             distance = shape.get_smallest_distance(x, y)
             if distance is not None and distance <= self.RADIUS:
-                return Jump(self, self.src.x, self.src.y)
+                jmp_dest = self.dst if to_dst else self.src
+                return Jump(self, jmp_dest.x, jmp_dest.y)
 
         return None
 
     def __repr__(self):
         return "<Edge %s -> %s>" % (self.src, self.dst)
 
 
@@ -726,17 +731,17 @@
     def get_url(self, x, y):
         for node in self.nodes:
             url = node.get_url(x, y)
             if url is not None:
                 return url
         return None
 
-    def get_jump(self, x, y):
+    def get_jump(self, x, y, to_dst = False):
         for edge in self.edges:
-            jump = edge.get_jump(x, y)
+            jump = edge.get_jump(x, y, to_dst)
             if jump is not None:
                 return jump
         for node in self.nodes:
             jump = node.get_jump(x, y)
             if jump is not None:
                 return jump
         return None
```

### Comparing `xdot-1.3/xdot/ui/pen.py` & `xdot-1.4/xdot/ui/pen.py`

 * *Files identical despite different names*

### Comparing `xdot-1.3/xdot/ui/window.py` & `xdot-1.4/xdot/ui/window.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,14 +78,15 @@
                         Gdk.EventMask.SMOOTH_SCROLL_MASK)
         self.connect("motion-notify-event", self.on_area_motion_notify)
         self.connect("scroll-event", self.on_area_scroll_event)
         self.connect("size-allocate", self.on_area_size_allocate)
 
         self.connect('key-press-event', self.on_key_press_event)
         self.last_mtime = None
+        self.mtime_changed = False
 
         GLib.timeout_add(1000, self.update)
 
         self.x, self.y = 0.0, 0.0
         self.zoom_ratio = 1.0
         self.zoom_to_fit_on_resize = False
         self.animation = animation.NoAnimation(self)
@@ -146,21 +147,22 @@
     def set_dotcode(self, dotcode, filename=None, center=True):
         self.openfilename = None
         if self._set_dotcode(dotcode, filename, center=center):
             if filename is None:
                 self.last_mtime = None
             else:
                 self.last_mtime = os.stat(filename).st_mtime
+            self.mtime_changed = False
             self.openfilename = filename
             return True
 
     def set_xdotcode(self, xdotcode, center=True):
         assert isinstance(xdotcode, bytes)
 
-        if self.graphviz_version is None:
+        if self.graphviz_version is None and self.filter is not None:
             stdout = subprocess.check_output([self.filter, '-V'], stderr=subprocess.STDOUT)
             stdout = stdout.rstrip()
             mo = re.match(br'^.* - .* version (?P<version>.*) \(.*\)$', stdout)
             assert mo
             self.graphviz_version = mo.group('version').decode('ascii')
 
         parser = XDotParser(xdotcode, graphviz_version=self.graphviz_version)
@@ -182,14 +184,17 @@
         if self.openfilename is not None:
             try:
                 current_mtime = os.stat(self.openfilename).st_mtime
             except OSError:
                 return True
             if current_mtime != self.last_mtime:
                 self.last_mtime = current_mtime
+                self.mtime_changed = True
+            elif self.mtime_changed:
+                self.mtime_changed = False
                 self.reload()
         return True
 
     def _draw_graph(self, cr, rect):
         w, h = float(rect.width), float(rect.height)
         cx, cy = 0.5 * w, 0.5 * h
         x, y, ratio = self.x, self.y, self.zoom_ratio
@@ -434,15 +439,16 @@
                 return True
 
             if event.button == 1:
                 url = self.get_url(x, y)
                 if url is not None:
                     self.emit('clicked', url.url, event)
                 else:
-                    jump = self.get_jump(x, y)
+                    ctrl_held = event.state & Gdk.ModifierType.CONTROL_MASK
+                    jump = self.get_jump(x, y, to_dst=ctrl_held)
                     if jump is not None:
                         self.animate_to(jump.x, jump.y)
 
                 return True
 
         if event.button == 1 or event.button == 2:
             return True
@@ -519,17 +525,17 @@
         x, y = self.window2graph(x, y)
         return self.graph.get_element(x, y)
 
     def get_url(self, x, y):
         x, y = self.window2graph(x, y)
         return self.graph.get_url(x, y)
 
-    def get_jump(self, x, y):
+    def get_jump(self, x, y, to_dst = False):
         x, y = self.window2graph(x, y)
-        return self.graph.get_jump(x, y)
+        return self.graph.get_jump(x, y, to_dst)
 
 
 class FindMenuToolAction(Gtk.Action):
     __gtype_name__ = "FindMenuToolAction"
 
     def do_create_tool_item(self):
         return Gtk.ToolItem()
```

### Comparing `xdot-1.3/xdot.egg-info/PKG-INFO` & `xdot-1.4/xdot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: xdot
-Version: 1.3
+Version: 1.4
 Summary: Interactive viewer for Graphviz dot files
 Home-page: https://github.com/jrfonseca/xdot.py
 Author: Jose Fonseca
 Author-email: jose.r.fonseca@gmail.com
 License: LGPL
 Description: 
                 xdot.py is an interactive viewer for graphs written in Graphviz's dot
```

