# Comparing `tmp/danila-lib-1.4.3.tar.gz` & `tmp/danila-lib-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danila-lib-1.4.3.tar", last modified: Tue May 14 11:45:43 2024, max compression
+gzip compressed data, was "danila-lib-1.4.4.tar", last modified: Tue May 14 12:37:52 2024, max compression
```

## Comparing `danila-lib-1.4.3.tar` & `danila-lib-1.4.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 11:45:43.029764 danila-lib-1.4.3/
--rw-rw-rw-   0        0        0     9615 2024-05-14 11:45:43.029764 danila-lib-1.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     5060 2024-04-22 21:01:41.000000 danila-lib-1.4.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-14 11:45:43.014145 danila-lib-1.4.3/danila/
--rw-rw-rw-   0        0        0        0 2024-04-15 11:55:56.000000 danila-lib-1.4.3/danila/__init__.py
--rw-rw-rw-   0        0        0     1896 2024-05-14 11:10:44.000000 danila-lib-1.4.3/danila/danila.py
--rw-rw-rw-   0        0        0     9741 2024-05-06 15:01:57.000000 danila-lib-1.4.3/danila/danila_v1.py
--rw-rw-rw-   0        0        0    10159 2024-05-07 07:31:38.000000 danila-lib-1.4.3/danila/danila_v2.py
--rw-rw-rw-   0        0        0    10591 2024-05-14 11:34:55.000000 danila-lib-1.4.3/danila/danila_v3.py
-drwxrwxrwx   0        0        0        0 2024-05-14 11:45:43.014145 danila-lib-1.4.3/danila_lib.egg-info/
--rw-rw-rw-   0        0        0     9615 2024-05-14 11:45:42.000000 danila-lib-1.4.3/danila_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      920 2024-05-14 11:45:42.000000 danila-lib-1.4.3/danila_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 11:45:42.000000 danila-lib-1.4.3/danila_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1879 2024-05-14 11:45:42.000000 danila-lib-1.4.3/danila_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-14 11:45:42.000000 danila-lib-1.4.3/danila_lib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-14 11:45:43.014145 danila-lib-1.4.3/data/
--rw-rw-rw-   0        0        0        0 2024-04-15 12:01:57.000000 danila-lib-1.4.3/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 11:45:43.029764 danila-lib-1.4.3/data/neuro/
--rw-rw-rw-   0        0        0     5722 2024-04-22 21:09:12.000000 danila-lib-1.4.3/data/neuro/Letters_recognize.py
--rw-rw-rw-   0        0        0     2754 2024-04-22 10:33:16.000000 danila-lib-1.4.3/data/neuro/Rama_classify_class.py
--rw-rw-rw-   0        0        0     2121 2024-04-22 11:59:10.000000 danila-lib-1.4.3/data/neuro/Rama_detect_class.py
--rw-rw-rw-   0        0        0     2595 2024-05-14 11:45:22.000000 danila-lib-1.4.3/data/neuro/Rama_prod_classify_class.py
--rw-rw-rw-   0        0        0     3159 2024-04-22 19:35:07.000000 danila-lib-1.4.3/data/neuro/Text_detect_class.py
--rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.4.3/data/neuro/__init__.py
--rw-rw-rw-   0        0        0     6373 2024-05-06 15:05:03.000000 danila-lib-1.4.3/data/neuro/letters_in_image.py
--rw-rw-rw-   0        0        0      830 2024-05-14 11:12:36.000000 danila-lib-1.4.3/data/neuro/models.py
--rw-rw-rw-   0        0        0     2975 2024-05-14 11:04:15.000000 danila-lib-1.4.3/data/neuro/objs_in_image.py
--rw-rw-rw-   0        0        0     4337 2024-05-07 07:39:22.000000 danila-lib-1.4.3/data/neuro/text_recognize_yolo.py
-drwxrwxrwx   0        0        0        0 2024-05-14 11:45:43.029764 danila-lib-1.4.3/data/result/
--rw-rw-rw-   0        0        0       89 2023-11-28 06:30:22.000000 danila-lib-1.4.3/data/result/Class_im.py
--rw-rw-rw-   0        0        0      108 2023-12-12 16:53:34.000000 danila-lib-1.4.3/data/result/Class_text.py
--rw-rw-rw-   0        0        0     2811 2024-04-22 19:35:07.000000 danila-lib-1.4.3/data/result/Image_text_areas.py
--rw-rw-rw-   0        0        0      311 2024-04-22 18:52:56.000000 danila-lib-1.4.3/data/result/Label_area.py
--rw-rw-rw-   0        0        0      105 2024-05-14 11:34:55.000000 danila-lib-1.4.3/data/result/Rama_prod.py
--rw-rw-rw-   0        0        0     3233 2024-04-22 18:17:45.000000 danila-lib-1.4.3/data/result/Rect.py
--rw-rw-rw-   0        0        0      539 2024-04-22 18:52:56.000000 danila-lib-1.4.3/data/result/Text_area.py
--rw-rw-rw-   0        0        0      716 2024-04-22 10:33:16.000000 danila-lib-1.4.3/data/result/Yolo_label_rect.py
--rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.4.3/data/result/__init__.py
--rw-rw-rw-   0        0        0      126 2024-05-14 11:04:15.000000 danila-lib-1.4.3/data/result/prod_classify_result.py
--rw-rw-rw-   0        0        0      122 2024-05-06 08:55:07.000000 danila-lib-1.4.3/data/result/word_compare_result.py
--rw-rw-rw-   0        0        0       42 2024-05-14 11:45:43.029764 danila-lib-1.4.3/setup.cfg
--rw-rw-rw-   0        0        0      983 2024-05-14 11:45:40.000000 danila-lib-1.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 12:37:52.149118 danila-lib-1.4.4/
+-rw-rw-rw-   0        0        0     9615 2024-05-14 12:37:52.149118 danila-lib-1.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5060 2024-04-22 21:01:41.000000 danila-lib-1.4.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 12:37:52.117878 danila-lib-1.4.4/danila/
+-rw-rw-rw-   0        0        0        0 2024-04-15 11:55:56.000000 danila-lib-1.4.4/danila/__init__.py
+-rw-rw-rw-   0        0        0     1896 2024-05-14 11:10:44.000000 danila-lib-1.4.4/danila/danila.py
+-rw-rw-rw-   0        0        0     9741 2024-05-06 15:01:57.000000 danila-lib-1.4.4/danila/danila_v1.py
+-rw-rw-rw-   0        0        0    10159 2024-05-07 07:31:38.000000 danila-lib-1.4.4/danila/danila_v2.py
+-rw-rw-rw-   0        0        0    10693 2024-05-14 12:37:43.000000 danila-lib-1.4.4/danila/danila_v3.py
+drwxrwxrwx   0        0        0        0 2024-05-14 12:37:52.133504 danila-lib-1.4.4/danila_lib.egg-info/
+-rw-rw-rw-   0        0        0     9615 2024-05-14 12:37:52.000000 danila-lib-1.4.4/danila_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      920 2024-05-14 12:37:52.000000 danila-lib-1.4.4/danila_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 12:37:52.000000 danila-lib-1.4.4/danila_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1879 2024-05-14 12:37:52.000000 danila-lib-1.4.4/danila_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-14 12:37:52.000000 danila-lib-1.4.4/danila_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 12:37:52.133504 danila-lib-1.4.4/data/
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:01:57.000000 danila-lib-1.4.4/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 12:37:52.133504 danila-lib-1.4.4/data/neuro/
+-rw-rw-rw-   0        0        0     5722 2024-04-22 21:09:12.000000 danila-lib-1.4.4/data/neuro/Letters_recognize.py
+-rw-rw-rw-   0        0        0     2754 2024-04-22 10:33:16.000000 danila-lib-1.4.4/data/neuro/Rama_classify_class.py
+-rw-rw-rw-   0        0        0     2121 2024-04-22 11:59:10.000000 danila-lib-1.4.4/data/neuro/Rama_detect_class.py
+-rw-rw-rw-   0        0        0     2614 2024-05-14 12:37:43.000000 danila-lib-1.4.4/data/neuro/Rama_prod_classify_class.py
+-rw-rw-rw-   0        0        0     3159 2024-04-22 19:35:07.000000 danila-lib-1.4.4/data/neuro/Text_detect_class.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.4.4/data/neuro/__init__.py
+-rw-rw-rw-   0        0        0     6373 2024-05-06 15:05:03.000000 danila-lib-1.4.4/data/neuro/letters_in_image.py
+-rw-rw-rw-   0        0        0      830 2024-05-14 11:12:36.000000 danila-lib-1.4.4/data/neuro/models.py
+-rw-rw-rw-   0        0        0     2975 2024-05-14 11:04:15.000000 danila-lib-1.4.4/data/neuro/objs_in_image.py
+-rw-rw-rw-   0        0        0     4337 2024-05-07 07:39:22.000000 danila-lib-1.4.4/data/neuro/text_recognize_yolo.py
+drwxrwxrwx   0        0        0        0 2024-05-14 12:37:52.149118 danila-lib-1.4.4/data/result/
+-rw-rw-rw-   0        0        0       89 2023-11-28 06:30:22.000000 danila-lib-1.4.4/data/result/Class_im.py
+-rw-rw-rw-   0        0        0      108 2023-12-12 16:53:34.000000 danila-lib-1.4.4/data/result/Class_text.py
+-rw-rw-rw-   0        0        0     2811 2024-04-22 19:35:07.000000 danila-lib-1.4.4/data/result/Image_text_areas.py
+-rw-rw-rw-   0        0        0      311 2024-04-22 18:52:56.000000 danila-lib-1.4.4/data/result/Label_area.py
+-rw-rw-rw-   0        0        0      105 2024-05-14 11:34:55.000000 danila-lib-1.4.4/data/result/Rama_prod.py
+-rw-rw-rw-   0        0        0     3233 2024-04-22 18:17:45.000000 danila-lib-1.4.4/data/result/Rect.py
+-rw-rw-rw-   0        0        0      539 2024-04-22 18:52:56.000000 danila-lib-1.4.4/data/result/Text_area.py
+-rw-rw-rw-   0        0        0      716 2024-04-22 10:33:16.000000 danila-lib-1.4.4/data/result/Yolo_label_rect.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.4.4/data/result/__init__.py
+-rw-rw-rw-   0        0        0      126 2024-05-14 11:04:15.000000 danila-lib-1.4.4/data/result/prod_classify_result.py
+-rw-rw-rw-   0        0        0      122 2024-05-06 08:55:07.000000 danila-lib-1.4.4/data/result/word_compare_result.py
+-rw-rw-rw-   0        0        0       42 2024-05-14 12:37:52.149118 danila-lib-1.4.4/setup.cfg
+-rw-rw-rw-   0        0        0      983 2024-05-14 12:37:49.000000 danila-lib-1.4.4/setup.py
```

### Comparing `danila-lib-1.4.3/PKG-INFO` & `danila-lib-1.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danila-lib
-Version: 1.4.3
+Version: 1.4.4
 Summary: This is the module for detecting and classifying text on rama pictures
 Home-page: https://github.com/Arseniy-Zhuck/danila_lib
 Author: arseniy_zhuck
 Author-email: arseniyzhuck@mail.ru
 Project-URL: GitHub, https://github.com/Arseniy-Zhuck/danila_lib
 Keywords: rama detect machine-learning computer-vision
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `danila-lib-1.4.3/README.md` & `danila-lib-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.3/danila/danila.py` & `danila-lib-1.4.4/danila/danila.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.3/danila/danila_v1.py` & `danila-lib-1.4.4/danila/danila_v1.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.3/danila/danila_v2.py` & `danila-lib-1.4.4/danila/danila_v2.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.3/danila/danila_v3.py` & `danila-lib-1.4.4/danila/danila_v3.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,27 +36,27 @@
         self.rama_no_spring_bejickaya_text_detect_model = Text_detect_class(rama_no_spring_bejickaya_text_detect_model_path,
                                                                             'rama_no_spring_bejickaya_text_detect', yolo_path)
         text_recognize_yolo_model_path = TEXT_RECOGNIZE_YOLO_MODEL_ADDRESS
         self.text_recognize_model = Text_Recognize_yolo(text_recognize_yolo_model_path, yolo_path)
     # returns string - class of rama using CNN network
     # img - openCV frame
 
-    def rama_classify(self, img):
+    def rama_classify(self, img, size = 256):
         """rama_classify(Img : openCv frame): String - returns class of rama using CNN network"""
         """rama_classify uses Rama_classify_class method - classify(Img)"""
         # img = cv2.imread(img_path)
-        rama_prod = self.rama_prod_classify_model.classify(img)
+        rama_prod = self.rama_prod_classify_model.classify(img, size)
         return rama_prod.name
 
     # returns openCV frame with rama from openCV frame\
-    def rama_detect(self, img):
+    def rama_detect(self, img, size = 256):
         """rama_detect(img : openCV img) -> openCV image with drawn rama rectangle"""
         initial_image_path = 'initial_image.jpg'
         cv2.imwrite(initial_image_path, img)
-        rama_prod = self.rama_prod_classify_model.classify(img)
+        rama_prod = self.rama_prod_classify_model.classify(img, size)
         if rama_prod == Rama_Prod.no_rama:
             return img
         rect = Rect()
         if (rama_prod == Rama_Prod.ruzhimmash):
             rect = self.rama_spring_detect_model.rama_detect(initial_image_path)
         else:
             rect = self.rama_no_spring_detect_model.rama_detect(initial_image_path)
@@ -65,18 +65,18 @@
         if rect is None:
             return img
         cv2.rectangle(new_img, (rect.xmin, rect.ymin), (rect.xmax, rect.ymax), (0, 0, 255), 2)
         cv2.putText(new_img, rama_prod.name, (rect.xmin, rect.ymin), cv2.FONT_HERSHEY_SIMPLEX, 0.5, (0,0,255), 2)
         return new_img
 
     # returns openCV image with cut_rama
-    def rama_cut(self, img):
+    def rama_cut(self, img, size = 256):
         """rama_cut(img : openCV img) -> openCV image of rama rectangle"""
         initial_image_path = 'initial_image.jpg'
-        cv2.imwrite(initial_image_path, img)
+        cv2.imwrite(initial_image_path, img, size)
         rama_prod = self.rama_prod_classify_model.classify(img)
         if rama_prod == Rama_Prod.no_rama:
             return img
         rect = Rect()
         if (rama_prod == Rama_Prod.ruzhimmash):
             rect = self.rama_spring_detect_model.rama_detect(initial_image_path)
         else:
@@ -84,15 +84,15 @@
         if rect is None:
             return img
         img_res = img[rect.ymin:rect.ymax, rect.xmin:rect.xmax]
         os.remove('initial_image.jpg')
         return img_res
     #
     # returns openCV cut rama with drawn text areas
-    def text_detect_cut(self, img):
+    def text_detect_cut(self, img, size = 256):
         """returns openCV cut rama with drawn text areas"""
         initial_image_path = 'initial_image.jpg'
         cv2.imwrite(initial_image_path, img)
         rama_prod = self.rama_prod_classify_model.classify(img)
         if rama_prod == Rama_Prod.no_rama:
             return img
         rect = Rect()
@@ -118,19 +118,19 @@
             image_text_areas = self.rama_no_spring_bejickaya_text_detect_model.text_detect(img_cut_path)
             image_drawn_text_areas = self.rama_no_spring_bejickaya_text_detect_model.draw_text_areas_in_opencv(image_text_areas, img_cut)
             os.remove(initial_image_path)
             os.remove(img_cut_path)
             return image_drawn_text_areas
 
     # returns openCV img with drawn text areas
-    def text_detect(self, img):
+    def text_detect(self, img, size = 256):
         """returns openCV img with drawn text areas"""
         initial_image_path = 'initial_image.jpg'
         cv2.imwrite(initial_image_path, img)
-        rama_prod = self.rama_prod_classify_model.classify(img)
+        rama_prod = self.rama_prod_classify_model.classify(img, size)
         if rama_prod == Rama_Prod.no_rama:
             return img
         rect = Rect()
         if (rama_prod == Rama_Prod.ruzhimmash):
             rect = self.rama_spring_detect_model.rama_detect(initial_image_path)
             if rect is None:
                 return img
@@ -154,19 +154,19 @@
             image_text_areas.explore_to_whole_image(rect)
             image_drawn_text_areas = self.rama_no_spring_bejickaya_text_detect_model.draw_text_areas_in_opencv(image_text_areas, img)
             os.remove(initial_image_path)
             os.remove(img_cut_path)
             return image_drawn_text_areas
 
     # returns dict {'number', 'prod', 'year'} for openCV rama img or 'no_rama'
-    def text_recognize(self, img):
+    def text_recognize(self, img, size = 256):
         """returns dict {'number', 'prod', 'year'} for openCV rama img or 'no_rama'"""
         initial_image_path = 'initial_image.jpg'
         cv2.imwrite(initial_image_path, img)
-        rama_prod = self.rama_prod_classify_model.classify(img)
+        rama_prod = self.rama_prod_classify_model.classify(img, size)
         if rama_prod == Rama_Prod.no_rama:
             return {'result': 'no_rama'}
         rect = Rect()
         if (rama_prod == Rama_Prod.ruzhimmash):
             rect = self.rama_spring_detect_model.rama_detect(initial_image_path)
             if rect is None:
                 return {'result': 'no_rama'}
```

### Comparing `danila-lib-1.4.3/danila_lib.egg-info/PKG-INFO` & `danila-lib-1.4.4/danila_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danila-lib
-Version: 1.4.3
+Version: 1.4.4
 Summary: This is the module for detecting and classifying text on rama pictures
 Home-page: https://github.com/Arseniy-Zhuck/danila_lib
 Author: arseniy_zhuck
 Author-email: arseniyzhuck@mail.ru
 Project-URL: GitHub, https://github.com/Arseniy-Zhuck/danila_lib
 Keywords: rama detect machine-learning computer-vision
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `danila-lib-1.4.3/danila_lib.egg-info/SOURCES.txt` & `danila-lib-1.4.4/danila_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.3/danila_lib.egg-info/requires.txt` & `danila-lib-1.4.4/danila_lib.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.3/data/neuro/Letters_recognize.py` & `danila-lib-1.4.4/data/neuro/Letters_recognize.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.3/data/neuro/Rama_classify_class.py` & `danila-lib-1.4.4/data/neuro/Rama_classify_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.3/data/neuro/Rama_detect_class.py` & `danila-lib-1.4.4/data/neuro/Rama_detect_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.3/data/neuro/Rama_prod_classify_class.py` & `danila-lib-1.4.4/data/neuro/Rama_prod_classify_class.py`

 * *Files 23% similar despite different names*

```diff
@@ -35,26 +35,26 @@
             zip_ref.extractall()
         # weights_file_path = model_name + '_weights.pt'
         self.model = torch.hub.load(yolo_path, 'custom', 'prod_classify.pt', source='local')
 
         # for every text_class try to recognize text from all areas of text_class, length is depends on class and prod, returns string
 
 
-    def work_image(self, img):
+    def work_image(self, img, size):
         cv2.imwrite('img.jpg', img)
-        results = self.model(['img.jpg'], size = 256)
+        results = self.model(['img.jpg'], size = size)
         json_res = results.pandas().xyxy[0].to_json(orient="records")
         res2 = json.loads(json_res)
         img_objs = Objs_In_Image.get_objs_in_image_from_yolo_json(res2)
         img_objs.delete_intersections()
         os.remove('img.jpg')
         return img_objs
 
-    def classify(self, img):
-        image_objs = self.work_image(img)
+    def classify(self, img, size):
+        image_objs = self.work_image(img, size)
         b_list_r = any(obj.obj == 'bejickaya' for obj in image_objs.objs)
         r_list_r = any(obj.obj == 'ruzhimmash' for obj in image_objs.objs)
         if (b_list_r == False) and (r_list_r == False):
             return Rama_Prod(2)
         else:
             if b_list_r and r_list_r:
                 return Rama_Prod(2)
```

### Comparing `danila-lib-1.4.3/data/neuro/Text_detect_class.py` & `danila-lib-1.4.4/data/neuro/Text_detect_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.3/data/neuro/letters_in_image.py` & `danila-lib-1.4.4/data/neuro/letters_in_image.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.3/data/neuro/models.py` & `danila-lib-1.4.4/data/neuro/models.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.3/data/neuro/objs_in_image.py` & `danila-lib-1.4.4/data/neuro/objs_in_image.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.3/data/neuro/text_recognize_yolo.py` & `danila-lib-1.4.4/data/neuro/text_recognize_yolo.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.3/data/result/Image_text_areas.py` & `danila-lib-1.4.4/data/result/Image_text_areas.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.3/data/result/Rect.py` & `danila-lib-1.4.4/data/result/Rect.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.3/data/result/Text_area.py` & `danila-lib-1.4.4/data/result/Text_area.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.3/data/result/Yolo_label_rect.py` & `danila-lib-1.4.4/data/result/Yolo_label_rect.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.3/setup.py` & `danila-lib-1.4.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   with open('requirements.txt', 'r') as f:
     a = f.read()
   b = a.split()
   return b
 
 setup(
   name='danila-lib',
-  version='1.4.3',
+  version='1.4.4',
   author='arseniy_zhuck',
   author_email='arseniyzhuck@mail.ru',
   description='This is the module for detecting and classifying text on rama pictures',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://github.com/Arseniy-Zhuck/danila_lib',
   packages=find_packages(),
```

