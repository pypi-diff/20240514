# Comparing `tmp/document_image_utils-0.1.6.tar.gz` & `tmp/document_image_utils-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "document_image_utils-0.1.6.tar", max compression
+gzip compressed data, was "document_image_utils-0.1.7.tar", max compression
```

## Comparing `document_image_utils-0.1.6.tar` & `document_image_utils-0.1.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2024-03-12 20:00:48.000000 document_image_utils-0.1.6/document_image_utils/__init__.py
--rw-r--r--   0        0        0    11476 2024-02-13 16:43:52.000000 document_image_utils-0.1.6/document_image_utils/box.py
--rw-r--r--   0        0        0    14342 2024-05-06 16:21:30.740290 document_image_utils-0.1.6/document_image_utils/image.py
--rw-r--r--   0        0        0      505 2024-05-06 16:24:58.201809 document_image_utils-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      879 2024-03-15 17:34:42.000000 document_image_utils-0.1.6/README.md
--rw-r--r--   0        0        0     1351 1970-01-01 00:00:00.000000 document_image_utils-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-03-12 20:00:48.000000 document_image_utils-0.1.7/document_image_utils/__init__.py
+-rw-r--r--   0        0        0    11098 2024-05-14 19:43:48.244212 document_image_utils-0.1.7/document_image_utils/box.py
+-rw-r--r--   0        0        0    18389 2024-05-14 19:40:21.969761 document_image_utils-0.1.7/document_image_utils/image.py
+-rw-r--r--   0        0        0      505 2024-05-14 19:46:33.854780 document_image_utils-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      879 2024-03-15 17:34:42.000000 document_image_utils-0.1.7/README.md
+-rw-r--r--   0        0        0     1351 1970-01-01 00:00:00.000000 document_image_utils-0.1.7/PKG-INFO
```

### Comparing `document_image_utils-0.1.6/document_image_utils/box.py` & `document_image_utils-0.1.7/document_image_utils/box.py`

 * *Files 13% similar despite different names*

```diff
@@ -34,22 +34,25 @@
         self.height = bottom - top
 
     def load_json(self,json_dict:dict):
         self.left = json_dict['left']
         self.right = json_dict['right']
         self.top = json_dict['top']
         self.bottom = json_dict['bottom']
-        self.width = json_dict['width']
-        self.height = json_dict['height']
+        self.width = self.right - self.left
+        self.height = self.bottom - self.top
 
     def copy(self):
         return Box(self.left,self.right,self.top,self.bottom)
 
     def __str__(self):
-        return f'left:{self.left} right:{self.right} top:{self.top} bottom:{self.bottom}'
+        return f'left:{self.left} right:{self.right} top:{self.top} bottom:{self.bottom} width:{self.width} height:{self.height}'
+    
+    def __dict__(self):
+        return self.to_dict()
 
     def to_json(self):
         return {
             'left':self.left,
             'right':self.right,
             'top':self.top,
             'bottom':self.bottom,
@@ -63,74 +66,76 @@
             'right':self.right,
             'top':self.top,
             'bottom':self.bottom,
             'width':self.width,
             'height':self.height
         }
     
+
+    def update(self, left:int=None, right:int=None, top:int=None, bottom:int=None):
+        if left is not None:
+            self.left = left
+        if right is not None:
+            self.right = right
+        if top is not None:
+            self.top = top
+        if bottom is not None:
+            self.bottom = bottom
+
+        self.width = self.right - self.left
+        self.height = self.bottom - self.top
+
+    
     def valid(self):
         '''Check if box is valid'''
         if self.left is None or self.right is None or self.top is None or self.bottom is None or self.left>self.right or self.top>self.bottom:
             return False
         return True
     
-    def within_vertical_boxes(self,box,range=0):
-        '''Check if boxes are within each other vertically, considering a range'''
-        # avoid division by zero
-        topmost = min(self.top,box.top)
-        topleast = max(self.top,box.top)
-        bottommost = max(self.bottom,box.bottom)
-        bottomlest = min(self.bottom,box.bottom)
-
-        # avoid division by zero
-        top_ratio = abs(topleast / topmost - 1) if topmost != 0 else abs(topleast / 0.1 - 1)
-        bottom_ratio = abs(bottomlest / bottommost - 1) if bottommost != 0 else abs(bottomlest / 0.1 - 1)
 
+    def area(self):
+        return self.width * self.height
+    
+    def within_vertical_boxes(self,box: 'Box',range:float=0):
+        '''Check if boxes are within each other vertically, considering a range (0-1)'''
+        
+        # check if box is within self with range
+        if (self.top - self.height*range <= box.top and self.bottom + self.height*range >= box.bottom):
+            return True
+        
         # check if self is within box with range
-        if (topmost == topleast or self.top <= box.top or top_ratio <= range) and (bottommost == bottomlest or self.bottom >= box.bottom or bottom_ratio <= range):
+        if (box.top - box.height*range <= self.top and box.bottom + box.height*range >= self.bottom):
             return True
 
-        # check if box is within self with range
-        elif (topmost == topleast or box.top <= self.top or top_ratio<= range) and (bottommost == bottomlest or box.bottom >= self.bottom or bottom_ratio <= range):
-            return True
+
         return False
             
 
-    def within_horizontal_boxes(self, box, range=0):
-        '''Check if boxes are within each other horizontally, considering a range'''
-        # avoid division by zero
-        leftmost = min(self.left, box.left)
-        leftleast = max(self.left, box.left)
-        rightmost = max(self.right, box.right)
-        rightleast = min(self.right, box.right)
-
+    def within_horizontal_boxes(self, box: 'Box', range:float=0):
+        '''Check if boxes are within each other horizontally, considering a range (0-1)'''
         
-        # avoid division by zero
-        left_ratio = abs(leftleast / leftmost - 1) if leftmost != 0 else abs(leftleast / 0.1 - 1)
-        right_ratio = abs(rightleast / rightmost - 1) if rightmost != 0 else abs(rightleast / 0.1 - 1)
-
         # check if box is within self with range
-        if (self.left <= box.left or left_ratio <= range) and (self.right >= box.right or right_ratio <= range):
+        if (self.left - self.width*range <= box.left and self.right + self.width*range >= box.right):
             return True
-
+        
         # check if self is within box with range
-        if (box.left <= self.left or left_ratio <= range) and (box.right >= self.right or right_ratio <= range):
+        if (box.left - box.width*range <= self.left and box.right + box.width*range >= self.right):
             return True
 
         return False
 
 
-    def same_level_box(self,box):
+    def same_level_box(self,box:'Box'):
         '''Check if two boxes are in the same level (horizontal and/or vertical)'''
         if self.within_horizontal_boxes(box) or self.within_vertical_boxes(box):
             return True
         return False
 
 
-    def is_inside_box(self,box):
+    def is_inside_box(self,box:'Box'):
         '''Check if box is inside container'''
         if self.left >= box.left and self.right <= box.right and self.top >= box.top and self.bottom <= box.bottom:
             return True
         return False
 
 
     def intersects_box(self,box,extend_vertical:bool=False,extend_horizontal:bool=False,inside:bool=False):
```

### Comparing `document_image_utils-0.1.6/document_image_utils/image.py` & `document_image_utils-0.1.7/document_image_utils/image.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import os
 import cv2
 from .box import *
 from scipy import ndimage
 import numpy as np
-
+from scipy.signal import *
+from whittaker_eilers import WhittakerSmoother
+from matplotlib import pyplot as plt
 
 def get_concat_h(im1, im2,margin=0):
     '''Concatenate images horizontally'''
     dst = np.zeros((im1.shape[0], im1.shape[1] + im2.shape[1] + margin, 3), dtype=np.uint8)
     dst[:, :im1.shape[1], :] = im1
     dst[:, im1.shape[1] + margin:, :] = im2
     return dst
@@ -400,13 +402,127 @@
             cv2.circle(og_img, (p[0]+50, p[1]), 7, (255, 0, 0), -1)
 
         cv2.imwrite(test_path + '_points.png', og_img)
 
     return img
         
 
+
+
+def divide_columns(image_path:str,method:str='WhittakerSmoother',logs:bool=False)->list[Box]:
+    '''Get areas of columns based on black pixel frequency.\n
+    Frequencies are then inverted to find white peaks.
+    Frequency graph is smoothened using chosen method.
+    
+    Available methods:
+        - WhittakerSmoother
+        - savgol_filter'''
+    columns = []
+
+    methods = ['WhittakerSmoother','savgol_filter']
+    if method not in methods:
+        method = 'WhittakerSmoother'
+
+    if not os.path.exists(image_path):
+        print('Image not found')
+        return columns
+
+    image = cv2.imread(image_path)
+    # cut possible header and footer (cut 30% from top and 10% from bottom)
+    image = image[round(image.shape[0]*0.3):round(image.shape[0]*0.9)]
+
+    # black and white
+    gray = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
+    # clean noise
+    se=cv2.getStructuringElement(cv2.MORPH_RECT , (8,8))
+    bg=cv2.morphologyEx(gray, cv2.MORPH_DILATE, se)
+    gray=cv2.divide(gray, bg, scale=255)
+    # binarize
+    binarized = cv2.threshold(gray, 0, 255, cv2.THRESH_BINARY_INV + cv2.THRESH_OTSU)[1]
+
+    # get frequency of white pixels per column
+    x_axis_freq = np.zeros(binarized.shape[1])
+
+    # count when column neighbours (above,bellow and right) are also white
+    mask = np.logical_and(
+        np.logical_and(binarized[1:,:-1] == 255, binarized[:-1,:-1] == 255),
+        binarized[:-1,1:] == 255
+    )
+    x_axis_freq = np.add.reduce(mask, axis=0)
+
+
+    if x_axis_freq.any():
+        # invert frequencies
+        max_freq = max(x_axis_freq)
+        x_axis_freq = np.array([max_freq - i for i in x_axis_freq])
+
+        if method == 'WhittakerSmoother':
+            whittaker_smoother = WhittakerSmoother(lmbda=2e4, order=2, data_length = len(x_axis_freq))
+            x_axis_freq_smooth = whittaker_smoother.smooth(x_axis_freq)
+        elif method == 'savgol_filter':
+            x_axis_freq_smooth = savgol_filter(x_axis_freq, round(len(x_axis_freq)*0.1), 2)
+
+        x_axis_freq_smooth = [i if i > 0 else 0 for i in x_axis_freq_smooth ]
+
+
+
+        peaks,_ = find_peaks(x_axis_freq_smooth,prominence=0.2*(max(x_axis_freq_smooth)- min(x_axis_freq_smooth)))
+
+        x_axis_freq_smooth = np.array(x_axis_freq_smooth)
+
+        # average of frequency
+        average_smooth_frequency = np.average(x_axis_freq_smooth)
+
+        if logs:
+            
+            # create 4 plots
+            plt.subplot(2, 2, 1)
+            plt.plot(peaks, x_axis_freq[peaks], "ob"); plt.plot(x_axis_freq); plt.legend(['prominence'])
+            plt.title('Frequency')
+
+
+            plt.subplot(2, 2, 2)
+            plt.plot(peaks, x_axis_freq_smooth[peaks], "ob"); plt.plot(x_axis_freq_smooth); plt.legend(['prominence'])
+            # average line
+            plt.plot([0,len(x_axis_freq_smooth)], [average_smooth_frequency, average_smooth_frequency], "r--");
+            plt.title('Frequency Smooth')
+
+            # binarized image
+            plt.subplot(2, 2, 3)
+            plt.imshow(binarized, cmap='gray')
+            plt.title('Binarized Image')
+
+            plt.show()
+
+
+        print('cleaned peaks',peaks)
+
+        # estimate columns
+        ## for each two peaks, decide if possible column, if middle frequencies are mostly above average
+        potential_columns = []
+        next_column = [0,None]
+        for i in range(len(peaks)):
+
+            if next_column[0] != None:
+                next_column[1] = peaks[i]
+
+            if next_column[0] != None and next_column[1] != None:
+                potential_columns.append([next_column[0],next_column[1]])
+
+            next_column = [peaks[i],None]
+
+        # create columns
+        if potential_columns:
+            print('potential columns',potential_columns)
+            for column in potential_columns:
+                c = Box({'left':column[0],'right':column[1],'top':0,'bottom':binarized.shape[0]})
+                columns.append(c)
+        
+
+    return columns
+
```

### Comparing `document_image_utils-0.1.6/README.md` & `document_image_utils-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `document_image_utils-0.1.6/PKG-INFO` & `document_image_utils-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: document_image_utils
-Version: 0.1.6
+Version: 0.1.7
 Summary: Toolkit for document image processing
 Author: Gonçalo Afonso
 Author-email: brazafonso2001@gmail.com
 Requires-Python: >=3.10.11,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

