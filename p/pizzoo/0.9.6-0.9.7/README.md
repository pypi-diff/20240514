# Comparing `tmp/pizzoo-0.9.6.tar.gz` & `tmp/pizzoo-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pizzoo-0.9.6.tar", last modified: Mon May 13 14:22:16 2024, max compression
+gzip compressed data, was "pizzoo-0.9.7.tar", last modified: Mon May 13 16:42:23 2024, max compression
```

## Comparing `pizzoo-0.9.6.tar` & `pizzoo-0.9.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 14:22:16.043040 pizzoo-0.9.6/
--rw-rw-rw-   0        0        0       13 2024-05-13 14:21:35.000000 pizzoo-0.9.6/MANIFEST.in
--rw-rw-rw-   0        0        0     7155 2024-05-13 14:22:16.043040 pizzoo-0.9.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-13 14:22:16.039040 pizzoo-0.9.6/pizzoo/
--rw-rw-rw-   0        0        0    43264 2024-04-19 15:34:13.000000 pizzoo-0.9.6/pizzoo/MatrixLight6.bdf
--rw-rw-rw-   0        0        0    21798 2024-05-04 08:50:51.000000 pizzoo-0.9.6/pizzoo/__init__.py
--rw-rw-rw-   0        0        0     1444 2024-04-19 15:38:24.000000 pizzoo-0.9.6/pizzoo/_constants.py
--rw-rw-rw-   0        0        0    17046 2024-05-03 00:00:18.000000 pizzoo-0.9.6/pizzoo/_renderers.py
--rw-rw-rw-   0        0        0      705 2024-04-28 16:47:36.000000 pizzoo-0.9.6/pizzoo/_utils.py
--rw-rw-rw-   0        0        0    21871 2024-05-10 19:21:17.000000 pizzoo-0.9.6/pizzoo/game.py
-drwxrwxrwx   0        0        0        0 2024-05-13 14:22:16.042040 pizzoo-0.9.6/pizzoo.egg-info/
--rw-rw-rw-   0        0        0     7155 2024-05-13 14:22:16.000000 pizzoo-0.9.6/pizzoo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      286 2024-05-13 14:22:16.000000 pizzoo-0.9.6/pizzoo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 14:22:16.000000 pizzoo-0.9.6/pizzoo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-05-13 14:22:16.000000 pizzoo-0.9.6/pizzoo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-13 14:22:16.000000 pizzoo-0.9.6/pizzoo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 14:22:16.043040 pizzoo-0.9.6/setup.cfg
--rw-rw-rw-   0        0        0     1206 2024-05-13 14:22:12.000000 pizzoo-0.9.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 16:42:23.336680 pizzoo-0.9.7/
+-rw-rw-rw-   0        0        0       13 2024-05-13 14:21:35.000000 pizzoo-0.9.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     7178 2024-05-13 16:42:23.335681 pizzoo-0.9.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-13 16:42:23.331678 pizzoo-0.9.7/pizzoo/
+-rw-rw-rw-   0        0        0    21793 2024-05-13 16:40:42.000000 pizzoo-0.9.7/pizzoo/__init__.py
+-rw-rw-rw-   0        0        0     1444 2024-04-19 15:38:24.000000 pizzoo-0.9.7/pizzoo/_constants.py
+-rw-rw-rw-   0        0        0    17046 2024-05-03 00:00:18.000000 pizzoo-0.9.7/pizzoo/_renderers.py
+-rw-rw-rw-   0        0        0      705 2024-04-28 16:47:36.000000 pizzoo-0.9.7/pizzoo/_utils.py
+-rw-rw-rw-   0        0        0    94332 2024-05-13 16:40:11.000000 pizzoo-0.9.7/pizzoo/default.bdf
+-rw-rw-rw-   0        0        0    21871 2024-05-10 19:21:17.000000 pizzoo-0.9.7/pizzoo/game.py
+drwxrwxrwx   0        0        0        0 2024-05-13 16:42:23.334680 pizzoo-0.9.7/pizzoo.egg-info/
+-rw-rw-rw-   0        0        0     7178 2024-05-13 16:42:23.000000 pizzoo-0.9.7/pizzoo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      281 2024-05-13 16:42:23.000000 pizzoo-0.9.7/pizzoo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 16:42:23.000000 pizzoo-0.9.7/pizzoo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-05-13 16:42:23.000000 pizzoo-0.9.7/pizzoo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-13 16:42:23.000000 pizzoo-0.9.7/pizzoo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 16:42:23.336680 pizzoo-0.9.7/setup.cfg
+-rw-rw-rw-   0        0        0     1206 2024-05-13 16:41:13.000000 pizzoo-0.9.7/setup.py
```

### Comparing `pizzoo-0.9.6/PKG-INFO` & `pizzoo-0.9.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pizzoo
-Version: 0.9.6
+Version: 0.9.7
 Summary: Pizzoo is a easy-to-use library for rendering on pixel matrix screens like the Pixoo64, featuring easy new device integration, animation tools, and XML template rendering support.
 Home-page: https://github.com/pabletos/pizzoo#readme
 Author: Pablo Huet
 License: MIT
 Keywords: pixoo,pixoo64,divoom,screen,pixel,matrix,render,buffer,LED matrix,LED,raspberry,raspberry pi
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Multimedia :: Graphics
@@ -33,17 +33,17 @@
 		<img src="https://img.shields.io/badge/-docs-red?logo=readthedocs&logoColor=white">
 	</a>
 	<a
 	href='https://pypi.org/project/pizzoo/'
 	target='_blank'
 	rel="noreferrer"
 	>
-	<img src="https://img.shields.io/badge/version-0.9.0-blue?logo=pypi&logoColor=%23ffffff"/>
+	<img src="https://img.shields.io/pypi/v/pizzoo?logo=pypi&label=version&logoColor=%23ffffff"/>
 	</a>
-	<img src="https://img.shields.io/badge/status-beta-yellow"/>
+	<img src="https://img.shields.io/pypi/dm/pizzoo?logo=pypi&logoColor=%23ffffff"/>
 </p>
 
 Pizzoo is a robust Python library designed for developers who want to unlock the full potential of matrix LED displays, particularly the Pixoo64, a 64x64 pixel LED display, and extend its functionalities to various other devices. Whether you're looking to create dynamic animations, develop interactive games, or integrate unique display functionalities, Pizzoo provides you with the tools and flexibility to innovate and express your creative ideas.
 
 ## Features
 
 * **Full Animation Creation and Control**:
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: pizzoo Version: 0.9.6 Summary: Pizzoo is a easy-to-
+Metadata-Version: 2.1 Name: pizzoo Version: 0.9.7 Summary: Pizzoo is a easy-to-
 use library for rendering on pixel matrix screens like the Pixoo64, featuring
 easy new device integration, animation tools, and XML template rendering
 support. Home-page: https://github.com/pabletos/pizzoo#readme Author: Pablo
 Huet License: MIT Keywords:
 pixoo,pixoo64,divoom,screen,pixel,matrix,render,buffer,LED
 matrix,LED,raspberry,raspberry pi Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Multimedia :: Graphics Classifier: License :: OSI Approved
 :: MIT License Description-Content-Type: text/markdown Requires-Dist:
 requests~=2.31.0 Requires-Dist: Pillow~=10.0.0 Requires-Dist: bdfparser~=2.2.0
                                  [Pizzoo logo]
 _[_B_u_y_ _M_e_ _a_ _C_o_f_f_e_e_ _a_t_ _k_o_-_f_i_._c_o_m_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_d_o_c_s_-
-_r_e_d_?_l_o_g_o_=_r_e_a_d_t_h_e_d_o_c_s_&_l_o_g_o_C_o_l_o_r_=_w_h_i_t_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_v_e_r_s_i_o_n_-
-_0_._9_._0_-_b_l_u_e_?_l_o_g_o_=_p_y_p_i_&_l_o_g_o_C_o_l_o_r_=_%_2_3_f_f_f_f_f_f_][https://img.shields.io/badge/status-
-beta-yellow]
+_r_e_d_?_l_o_g_o_=_r_e_a_d_t_h_e_d_o_c_s_&_l_o_g_o_C_o_l_o_r_=_w_h_i_t_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/
+_p_i_z_z_o_o_?_l_o_g_o_=_p_y_p_i_&_l_a_b_e_l_=_v_e_r_s_i_o_n_&_l_o_g_o_C_o_l_o_r_=_%_2_3_f_f_f_f_f_f_][https://img.shields.io/
+pypi/dm/pizzoo?logo=pypi&logoColor=%23ffffff]
 Pizzoo is a robust Python library designed for developers who want to unlock
 the full potential of matrix LED displays, particularly the Pixoo64, a 64x64
 pixel LED display, and extend its functionalities to various other devices.
 Whether you're looking to create dynamic animations, develop interactive games,
 or integrate unique display functionalities, Pizzoo provides you with the tools
 and flexibility to innovate and express your creative ideas. ## Features *
 **Full Animation Creation and Control**: With frame-by-frame programatic
```

### Comparing `pizzoo-0.9.6/pizzoo/__init__.py` & `pizzoo-0.9.7/pizzoo/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 		'''
 		self.renderer = renderer(address=address, pizzoo=self, debug=debug, **renderer_params)
 		self.__compute_device_specs()
 		self.__debug = debug
 		# Initialize buffer
 		self.add_frame()
 		# get current dir of this file:
-		self.load_font('default', join(self.__current_dir, 'MatrixLight6.bdf'), False)
+		self.load_font('default', join(self.__current_dir, 'default.bdf'), False)
 
 	def __compute_device_specs(self):
 		self.size = self.renderer.get_size()
 		self.pixel_count = self.size * self.size
 		self.__max_frames = self.renderer.get_max_frames()
 		
 	def load_font(self, font_name, path, soft=True):
```

### Comparing `pizzoo-0.9.6/pizzoo/_constants.py` & `pizzoo-0.9.7/pizzoo/_constants.py`

 * *Files identical despite different names*

### Comparing `pizzoo-0.9.6/pizzoo/_renderers.py` & `pizzoo-0.9.7/pizzoo/_renderers.py`

 * *Files identical despite different names*

### Comparing `pizzoo-0.9.6/pizzoo/_utils.py` & `pizzoo-0.9.7/pizzoo/_utils.py`

 * *Files identical despite different names*

### Comparing `pizzoo-0.9.6/pizzoo/game.py` & `pizzoo-0.9.7/pizzoo/game.py`

 * *Files identical despite different names*

### Comparing `pizzoo-0.9.6/pizzoo.egg-info/PKG-INFO` & `pizzoo-0.9.7/pizzoo.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pizzoo
-Version: 0.9.6
+Version: 0.9.7
 Summary: Pizzoo is a easy-to-use library for rendering on pixel matrix screens like the Pixoo64, featuring easy new device integration, animation tools, and XML template rendering support.
 Home-page: https://github.com/pabletos/pizzoo#readme
 Author: Pablo Huet
 License: MIT
 Keywords: pixoo,pixoo64,divoom,screen,pixel,matrix,render,buffer,LED matrix,LED,raspberry,raspberry pi
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Multimedia :: Graphics
@@ -33,17 +33,17 @@
 		<img src="https://img.shields.io/badge/-docs-red?logo=readthedocs&logoColor=white">
 	</a>
 	<a
 	href='https://pypi.org/project/pizzoo/'
 	target='_blank'
 	rel="noreferrer"
 	>
-	<img src="https://img.shields.io/badge/version-0.9.0-blue?logo=pypi&logoColor=%23ffffff"/>
+	<img src="https://img.shields.io/pypi/v/pizzoo?logo=pypi&label=version&logoColor=%23ffffff"/>
 	</a>
-	<img src="https://img.shields.io/badge/status-beta-yellow"/>
+	<img src="https://img.shields.io/pypi/dm/pizzoo?logo=pypi&logoColor=%23ffffff"/>
 </p>
 
 Pizzoo is a robust Python library designed for developers who want to unlock the full potential of matrix LED displays, particularly the Pixoo64, a 64x64 pixel LED display, and extend its functionalities to various other devices. Whether you're looking to create dynamic animations, develop interactive games, or integrate unique display functionalities, Pizzoo provides you with the tools and flexibility to innovate and express your creative ideas.
 
 ## Features
 
 * **Full Animation Creation and Control**:
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: pizzoo Version: 0.9.6 Summary: Pizzoo is a easy-to-
+Metadata-Version: 2.1 Name: pizzoo Version: 0.9.7 Summary: Pizzoo is a easy-to-
 use library for rendering on pixel matrix screens like the Pixoo64, featuring
 easy new device integration, animation tools, and XML template rendering
 support. Home-page: https://github.com/pabletos/pizzoo#readme Author: Pablo
 Huet License: MIT Keywords:
 pixoo,pixoo64,divoom,screen,pixel,matrix,render,buffer,LED
 matrix,LED,raspberry,raspberry pi Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Multimedia :: Graphics Classifier: License :: OSI Approved
 :: MIT License Description-Content-Type: text/markdown Requires-Dist:
 requests~=2.31.0 Requires-Dist: Pillow~=10.0.0 Requires-Dist: bdfparser~=2.2.0
                                  [Pizzoo logo]
 _[_B_u_y_ _M_e_ _a_ _C_o_f_f_e_e_ _a_t_ _k_o_-_f_i_._c_o_m_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_d_o_c_s_-
-_r_e_d_?_l_o_g_o_=_r_e_a_d_t_h_e_d_o_c_s_&_l_o_g_o_C_o_l_o_r_=_w_h_i_t_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_v_e_r_s_i_o_n_-
-_0_._9_._0_-_b_l_u_e_?_l_o_g_o_=_p_y_p_i_&_l_o_g_o_C_o_l_o_r_=_%_2_3_f_f_f_f_f_f_][https://img.shields.io/badge/status-
-beta-yellow]
+_r_e_d_?_l_o_g_o_=_r_e_a_d_t_h_e_d_o_c_s_&_l_o_g_o_C_o_l_o_r_=_w_h_i_t_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/
+_p_i_z_z_o_o_?_l_o_g_o_=_p_y_p_i_&_l_a_b_e_l_=_v_e_r_s_i_o_n_&_l_o_g_o_C_o_l_o_r_=_%_2_3_f_f_f_f_f_f_][https://img.shields.io/
+pypi/dm/pizzoo?logo=pypi&logoColor=%23ffffff]
 Pizzoo is a robust Python library designed for developers who want to unlock
 the full potential of matrix LED displays, particularly the Pixoo64, a 64x64
 pixel LED display, and extend its functionalities to various other devices.
 Whether you're looking to create dynamic animations, develop interactive games,
 or integrate unique display functionalities, Pizzoo provides you with the tools
 and flexibility to innovate and express your creative ideas. ## Features *
 **Full Animation Creation and Control**: With frame-by-frame programatic
```

### Comparing `pizzoo-0.9.6/setup.py` & `pizzoo-0.9.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 long_description = open('%s\\README.md' % 'C:\\Users\\Usuario\\Documents\\Projects\\pizzoo', encoding='utf-8').read()
 
 # https://packaging.python.org/en/latest/guides/distributing-packages-using-setuptools/
 setup(
     name="pizzoo",
-    version="0.9.6",
+    version="0.9.7",
     author="Pablo Huet",
     description="Pizzoo is a easy-to-use library for rendering on pixel matrix screens like the Pixoo64, featuring easy new device integration, animation tools, and XML template rendering support.",
     long_description=long_description,
 	long_description_content_type='text/markdown',
 	license="MIT",
     keywords="pixoo, pixoo64, divoom, screen, pixel, matrix, render, buffer, LED matrix, LED, raspberry, raspberry pi",
     url="https://github.com/pabletos/pizzoo#readme",
```

