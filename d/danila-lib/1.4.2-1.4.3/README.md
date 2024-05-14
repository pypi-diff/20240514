# Comparing `tmp/danila-lib-1.4.2.tar.gz` & `tmp/danila-lib-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danila-lib-1.4.2.tar", last modified: Tue May 14 11:35:10 2024, max compression
+gzip compressed data, was "danila-lib-1.4.3.tar", last modified: Tue May 14 11:45:43 2024, max compression
```

## Comparing `danila-lib-1.4.2.tar` & `danila-lib-1.4.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 11:35:10.881436 danila-lib-1.4.2/
--rw-rw-rw-   0        0        0     9615 2024-05-14 11:35:10.881436 danila-lib-1.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     5060 2024-04-22 21:01:41.000000 danila-lib-1.4.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-14 11:35:10.803124 danila-lib-1.4.2/danila/
--rw-rw-rw-   0        0        0        0 2024-04-15 11:55:56.000000 danila-lib-1.4.2/danila/__init__.py
--rw-rw-rw-   0        0        0     1896 2024-05-14 11:10:44.000000 danila-lib-1.4.2/danila/danila.py
--rw-rw-rw-   0        0        0     9741 2024-05-06 15:01:57.000000 danila-lib-1.4.2/danila/danila_v1.py
--rw-rw-rw-   0        0        0    10159 2024-05-07 07:31:38.000000 danila-lib-1.4.2/danila/danila_v2.py
--rw-rw-rw-   0        0        0    10591 2024-05-14 11:34:55.000000 danila-lib-1.4.2/danila/danila_v3.py
-drwxrwxrwx   0        0        0        0 2024-05-14 11:35:10.818745 danila-lib-1.4.2/danila_lib.egg-info/
--rw-rw-rw-   0        0        0     9615 2024-05-14 11:35:10.000000 danila-lib-1.4.2/danila_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      920 2024-05-14 11:35:10.000000 danila-lib-1.4.2/danila_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 11:35:10.000000 danila-lib-1.4.2/danila_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1879 2024-05-14 11:35:10.000000 danila-lib-1.4.2/danila_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-14 11:35:10.000000 danila-lib-1.4.2/danila_lib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-14 11:35:10.818745 danila-lib-1.4.2/data/
--rw-rw-rw-   0        0        0        0 2024-04-15 12:01:57.000000 danila-lib-1.4.2/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 11:35:10.834364 danila-lib-1.4.2/data/neuro/
--rw-rw-rw-   0        0        0     5722 2024-04-22 21:09:12.000000 danila-lib-1.4.2/data/neuro/Letters_recognize.py
--rw-rw-rw-   0        0        0     2754 2024-04-22 10:33:16.000000 danila-lib-1.4.2/data/neuro/Rama_classify_class.py
--rw-rw-rw-   0        0        0     2121 2024-04-22 11:59:10.000000 danila-lib-1.4.2/data/neuro/Rama_detect_class.py
--rw-rw-rw-   0        0        0     2570 2024-05-14 11:34:55.000000 danila-lib-1.4.2/data/neuro/Rama_prod_classify_class.py
--rw-rw-rw-   0        0        0     3159 2024-04-22 19:35:07.000000 danila-lib-1.4.2/data/neuro/Text_detect_class.py
--rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.4.2/data/neuro/__init__.py
--rw-rw-rw-   0        0        0     6373 2024-05-06 15:05:03.000000 danila-lib-1.4.2/data/neuro/letters_in_image.py
--rw-rw-rw-   0        0        0      830 2024-05-14 11:12:36.000000 danila-lib-1.4.2/data/neuro/models.py
--rw-rw-rw-   0        0        0     2975 2024-05-14 11:04:15.000000 danila-lib-1.4.2/data/neuro/objs_in_image.py
--rw-rw-rw-   0        0        0     4337 2024-05-07 07:39:22.000000 danila-lib-1.4.2/data/neuro/text_recognize_yolo.py
-drwxrwxrwx   0        0        0        0 2024-05-14 11:35:10.881436 danila-lib-1.4.2/data/result/
--rw-rw-rw-   0        0        0       89 2023-11-28 06:30:22.000000 danila-lib-1.4.2/data/result/Class_im.py
--rw-rw-rw-   0        0        0      108 2023-12-12 16:53:34.000000 danila-lib-1.4.2/data/result/Class_text.py
--rw-rw-rw-   0        0        0     2811 2024-04-22 19:35:07.000000 danila-lib-1.4.2/data/result/Image_text_areas.py
--rw-rw-rw-   0        0        0      311 2024-04-22 18:52:56.000000 danila-lib-1.4.2/data/result/Label_area.py
--rw-rw-rw-   0        0        0      105 2024-05-14 11:34:55.000000 danila-lib-1.4.2/data/result/Rama_prod.py
--rw-rw-rw-   0        0        0     3233 2024-04-22 18:17:45.000000 danila-lib-1.4.2/data/result/Rect.py
--rw-rw-rw-   0        0        0      539 2024-04-22 18:52:56.000000 danila-lib-1.4.2/data/result/Text_area.py
--rw-rw-rw-   0        0        0      716 2024-04-22 10:33:16.000000 danila-lib-1.4.2/data/result/Yolo_label_rect.py
--rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.4.2/data/result/__init__.py
--rw-rw-rw-   0        0        0      126 2024-05-14 11:04:15.000000 danila-lib-1.4.2/data/result/prod_classify_result.py
--rw-rw-rw-   0        0        0      122 2024-05-06 08:55:07.000000 danila-lib-1.4.2/data/result/word_compare_result.py
--rw-rw-rw-   0        0        0       42 2024-05-14 11:35:10.881436 danila-lib-1.4.2/setup.cfg
--rw-rw-rw-   0        0        0      983 2024-05-14 11:35:07.000000 danila-lib-1.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 11:45:43.029764 danila-lib-1.4.3/
+-rw-rw-rw-   0        0        0     9615 2024-05-14 11:45:43.029764 danila-lib-1.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5060 2024-04-22 21:01:41.000000 danila-lib-1.4.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 11:45:43.014145 danila-lib-1.4.3/danila/
+-rw-rw-rw-   0        0        0        0 2024-04-15 11:55:56.000000 danila-lib-1.4.3/danila/__init__.py
+-rw-rw-rw-   0        0        0     1896 2024-05-14 11:10:44.000000 danila-lib-1.4.3/danila/danila.py
+-rw-rw-rw-   0        0        0     9741 2024-05-06 15:01:57.000000 danila-lib-1.4.3/danila/danila_v1.py
+-rw-rw-rw-   0        0        0    10159 2024-05-07 07:31:38.000000 danila-lib-1.4.3/danila/danila_v2.py
+-rw-rw-rw-   0        0        0    10591 2024-05-14 11:34:55.000000 danila-lib-1.4.3/danila/danila_v3.py
+drwxrwxrwx   0        0        0        0 2024-05-14 11:45:43.014145 danila-lib-1.4.3/danila_lib.egg-info/
+-rw-rw-rw-   0        0        0     9615 2024-05-14 11:45:42.000000 danila-lib-1.4.3/danila_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      920 2024-05-14 11:45:42.000000 danila-lib-1.4.3/danila_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 11:45:42.000000 danila-lib-1.4.3/danila_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1879 2024-05-14 11:45:42.000000 danila-lib-1.4.3/danila_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-14 11:45:42.000000 danila-lib-1.4.3/danila_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 11:45:43.014145 danila-lib-1.4.3/data/
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:01:57.000000 danila-lib-1.4.3/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 11:45:43.029764 danila-lib-1.4.3/data/neuro/
+-rw-rw-rw-   0        0        0     5722 2024-04-22 21:09:12.000000 danila-lib-1.4.3/data/neuro/Letters_recognize.py
+-rw-rw-rw-   0        0        0     2754 2024-04-22 10:33:16.000000 danila-lib-1.4.3/data/neuro/Rama_classify_class.py
+-rw-rw-rw-   0        0        0     2121 2024-04-22 11:59:10.000000 danila-lib-1.4.3/data/neuro/Rama_detect_class.py
+-rw-rw-rw-   0        0        0     2595 2024-05-14 11:45:22.000000 danila-lib-1.4.3/data/neuro/Rama_prod_classify_class.py
+-rw-rw-rw-   0        0        0     3159 2024-04-22 19:35:07.000000 danila-lib-1.4.3/data/neuro/Text_detect_class.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.4.3/data/neuro/__init__.py
+-rw-rw-rw-   0        0        0     6373 2024-05-06 15:05:03.000000 danila-lib-1.4.3/data/neuro/letters_in_image.py
+-rw-rw-rw-   0        0        0      830 2024-05-14 11:12:36.000000 danila-lib-1.4.3/data/neuro/models.py
+-rw-rw-rw-   0        0        0     2975 2024-05-14 11:04:15.000000 danila-lib-1.4.3/data/neuro/objs_in_image.py
+-rw-rw-rw-   0        0        0     4337 2024-05-07 07:39:22.000000 danila-lib-1.4.3/data/neuro/text_recognize_yolo.py
+drwxrwxrwx   0        0        0        0 2024-05-14 11:45:43.029764 danila-lib-1.4.3/data/result/
+-rw-rw-rw-   0        0        0       89 2023-11-28 06:30:22.000000 danila-lib-1.4.3/data/result/Class_im.py
+-rw-rw-rw-   0        0        0      108 2023-12-12 16:53:34.000000 danila-lib-1.4.3/data/result/Class_text.py
+-rw-rw-rw-   0        0        0     2811 2024-04-22 19:35:07.000000 danila-lib-1.4.3/data/result/Image_text_areas.py
+-rw-rw-rw-   0        0        0      311 2024-04-22 18:52:56.000000 danila-lib-1.4.3/data/result/Label_area.py
+-rw-rw-rw-   0        0        0      105 2024-05-14 11:34:55.000000 danila-lib-1.4.3/data/result/Rama_prod.py
+-rw-rw-rw-   0        0        0     3233 2024-04-22 18:17:45.000000 danila-lib-1.4.3/data/result/Rect.py
+-rw-rw-rw-   0        0        0      539 2024-04-22 18:52:56.000000 danila-lib-1.4.3/data/result/Text_area.py
+-rw-rw-rw-   0        0        0      716 2024-04-22 10:33:16.000000 danila-lib-1.4.3/data/result/Yolo_label_rect.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.4.3/data/result/__init__.py
+-rw-rw-rw-   0        0        0      126 2024-05-14 11:04:15.000000 danila-lib-1.4.3/data/result/prod_classify_result.py
+-rw-rw-rw-   0        0        0      122 2024-05-06 08:55:07.000000 danila-lib-1.4.3/data/result/word_compare_result.py
+-rw-rw-rw-   0        0        0       42 2024-05-14 11:45:43.029764 danila-lib-1.4.3/setup.cfg
+-rw-rw-rw-   0        0        0      983 2024-05-14 11:45:40.000000 danila-lib-1.4.3/setup.py
```

### Comparing `danila-lib-1.4.2/PKG-INFO` & `danila-lib-1.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danila-lib
-Version: 1.4.2
+Version: 1.4.3
 Summary: This is the module for detecting and classifying text on rama pictures
 Home-page: https://github.com/Arseniy-Zhuck/danila_lib
 Author: arseniy_zhuck
 Author-email: arseniyzhuck@mail.ru
 Project-URL: GitHub, https://github.com/Arseniy-Zhuck/danila_lib
 Keywords: rama detect machine-learning computer-vision
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `danila-lib-1.4.2/README.md` & `danila-lib-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.2/danila/danila.py` & `danila-lib-1.4.3/danila/danila.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.2/danila/danila_v1.py` & `danila-lib-1.4.3/danila/danila_v1.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.2/danila/danila_v2.py` & `danila-lib-1.4.3/danila/danila_v2.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.2/danila/danila_v3.py` & `danila-lib-1.4.3/danila/danila_v3.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.2/danila_lib.egg-info/PKG-INFO` & `danila-lib-1.4.3/danila_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danila-lib
-Version: 1.4.2
+Version: 1.4.3
 Summary: This is the module for detecting and classifying text on rama pictures
 Home-page: https://github.com/Arseniy-Zhuck/danila_lib
 Author: arseniy_zhuck
 Author-email: arseniyzhuck@mail.ru
 Project-URL: GitHub, https://github.com/Arseniy-Zhuck/danila_lib
 Keywords: rama detect machine-learning computer-vision
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `danila-lib-1.4.2/danila_lib.egg-info/SOURCES.txt` & `danila-lib-1.4.3/danila_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.2/danila_lib.egg-info/requires.txt` & `danila-lib-1.4.3/danila_lib.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.2/data/neuro/Letters_recognize.py` & `danila-lib-1.4.3/data/neuro/Letters_recognize.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.2/data/neuro/Rama_classify_class.py` & `danila-lib-1.4.3/data/neuro/Rama_classify_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.2/data/neuro/Rama_detect_class.py` & `danila-lib-1.4.3/data/neuro/Rama_detect_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.2/data/neuro/Rama_prod_classify_class.py` & `danila-lib-1.4.3/data/neuro/Rama_prod_classify_class.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,14 +43,15 @@
         cv2.imwrite('img.jpg', img)
         results = self.model(['img.jpg'], size = 256)
         json_res = results.pandas().xyxy[0].to_json(orient="records")
         res2 = json.loads(json_res)
         img_objs = Objs_In_Image.get_objs_in_image_from_yolo_json(res2)
         img_objs.delete_intersections()
         os.remove('img.jpg')
+        return img_objs
 
     def classify(self, img):
         image_objs = self.work_image(img)
         b_list_r = any(obj.obj == 'bejickaya' for obj in image_objs.objs)
         r_list_r = any(obj.obj == 'ruzhimmash' for obj in image_objs.objs)
         if (b_list_r == False) and (r_list_r == False):
             return Rama_Prod(2)
```

### Comparing `danila-lib-1.4.2/data/neuro/Text_detect_class.py` & `danila-lib-1.4.3/data/neuro/Text_detect_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.2/data/neuro/letters_in_image.py` & `danila-lib-1.4.3/data/neuro/letters_in_image.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.2/data/neuro/models.py` & `danila-lib-1.4.3/data/neuro/models.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.2/data/neuro/objs_in_image.py` & `danila-lib-1.4.3/data/neuro/objs_in_image.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.2/data/neuro/text_recognize_yolo.py` & `danila-lib-1.4.3/data/neuro/text_recognize_yolo.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.2/data/result/Image_text_areas.py` & `danila-lib-1.4.3/data/result/Image_text_areas.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.2/data/result/Rect.py` & `danila-lib-1.4.3/data/result/Rect.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.2/data/result/Text_area.py` & `danila-lib-1.4.3/data/result/Text_area.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.2/data/result/Yolo_label_rect.py` & `danila-lib-1.4.3/data/result/Yolo_label_rect.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.2/setup.py` & `danila-lib-1.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   with open('requirements.txt', 'r') as f:
     a = f.read()
   b = a.split()
   return b
 
 setup(
   name='danila-lib',
-  version='1.4.2',
+  version='1.4.3',
   author='arseniy_zhuck',
   author_email='arseniyzhuck@mail.ru',
   description='This is the module for detecting and classifying text on rama pictures',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://github.com/Arseniy-Zhuck/danila_lib',
   packages=find_packages(),
```
