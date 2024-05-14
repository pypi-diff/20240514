# Comparing `tmp/pisahkan_ktp-0.1.8.tar.gz` & `tmp/pisahkan_ktp-0.2.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pisahkan_ktp-0.1.8.tar", max compression
+gzip compressed data, was "pisahkan_ktp-0.2.10.tar", max compression
```

## Comparing `pisahkan_ktp-0.1.8.tar` & `pisahkan_ktp-0.2.10.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0     1097 2024-05-07 03:55:25.046040 pisahkan_ktp-0.1.8/LICENSE
--rwxr-xr-x   0        0        0     4971 2024-05-13 03:45:24.672426 pisahkan_ktp-0.1.8/README.md
--rwxr-xr-x   0        0        0      690 2024-05-13 03:56:17.118171 pisahkan_ktp-0.1.8/pyproject.toml
--rwxr-xr-x   0        0        0        0 2024-05-07 03:58:19.125178 pisahkan_ktp-0.1.8/src/pisahkan_ktp/__init__.py
--rwxr-xr-x   0        0        0    17220 2024-05-13 03:55:43.595029 pisahkan_ktp-0.1.8/src/pisahkan_ktp/ktp_segmenter.py
--rw-r--r--   0        0        0     5676 1970-01-01 00:00:00.000000 pisahkan_ktp-0.1.8/PKG-INFO
+-rwxr-xr-x   0        0        0     1097 2024-05-07 03:55:25.046040 pisahkan_ktp-0.2.10/LICENSE
+-rwxr-xr-x   0        0        0     5857 2024-05-14 06:42:10.332905 pisahkan_ktp-0.2.10/README.md
+-rwxr-xr-x   0        0        0      826 2024-05-14 06:43:03.403749 pisahkan_ktp-0.2.10/pyproject.toml
+-rwxr-xr-x   0        0        0        0 2024-05-07 03:58:19.125178 pisahkan_ktp-0.2.10/src/pisahkan_ktp/__init__.py
+-rwxr-xr-x   0        0        0    20414 2024-05-14 06:23:11.367664 pisahkan_ktp-0.2.10/src/pisahkan_ktp/ktp_segmenter.py
+-rw-r--r--   0        0        0     6670 1970-01-01 00:00:00.000000 pisahkan_ktp-0.2.10/PKG-INFO
```

### Comparing `pisahkan_ktp-0.1.8/LICENSE` & `pisahkan_ktp-0.2.10/LICENSE`

 * *Files identical despite different names*

### Comparing `pisahkan_ktp-0.1.8/README.md` & `pisahkan_ktp-0.2.10/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -32,30 +32,50 @@
 1. Installation
     ```sh
     pip install pisahkan-ktp
     ```
 ### Inference
 1. Usage
     - Text Area
-        ```py
-        # Input ==> Image Path
-        from pisahkan_ktp.ktp_segmenter import segmenter
-
-        image_path = "./tests/sample.jpg"
-        result = segmenter(image_path)
-        print(result)
-
-        # Input ==> Numpy Array Image ==> cv2.imread(image_path)
-        from pisahkan_ktp.ktp_segmenter import segmenter_ndarray
+        - Standard Segmenter
+            ```py
+            # Input ==> Image Path
+            from pisahkan_ktp.ktp_segmenter import segmenter
+
+            image_path = "./tests/sample.jpg"
+            result = segmenter(image_path)
+            print(result)
+
+            # Input ==> Numpy Array Image ==> cv2.imread(image_path)
+            from pisahkan_ktp.ktp_segmenter import segmenter_ndarray
+
+            image_path = "./tests/sample.jpg"
+            image = cv2.imread(image_path)
+            result = segmenter_ndarray(image)
+            print(result)
+            ```
+        
+        - Adaptive Segmenter (Adjust contrast level in preprocessing)
+            ```py
+            # Input ==> Image Path
+            from pisahkan_ktp.ktp_segmenter import adaptive_segmenter
+    
+            image_path = "./tests/sample.jpg"
+            result = adaptive_segmenter(image_path, contrast_factor=1.7, delta_contrast=0.7, gamma_factor=1.0)
+            print(result)
+    
+            # Input ==> Numpy Array Image ==> cv2.imread(image_path)
+            from pisahkan_ktp.ktp_segmenter import adaptive_segmenter_ndarray
+    
+            image_path = "./tests/sample.jpg"
+            image = cv2.imread(image_path)
+            result = adaptive_segmenter_ndarray(image, contrast_factor=1.7, delta_contrast=0.7, gamma_factor=1.0)
+            print(result)
+            ```
 
-        image_path = "./tests/sample.jpg"
-        image = cv2.imread(image_path)
-        result = segmenter_ndarray(image)
-        print(result)
-        ```
     - Pass-Photo & Signature
         ```py
         # Input ==> Image Path
         from pisahkan_ktp.ktp_segmenter import getPassPhoto, getSignature
 
         image_path = "./tests/sample.jpg"
         result = getPassPhoto(image_path)
@@ -97,15 +117,15 @@
     - Detail Area Cropped
         
         <img src="./assets/8-7-detail.jpg" alt="Beautiful Landscape" width="500">
 
 ## How to Show in Matplotlib
 ### Input ==> Image Path
 ```py
-from src.pisahkan_ktp.ktp_segmenter import segmenter
+from pisahkan_ktp.ktp_segmenter import segmenter
 import matplotlib.pyplot as plt
 import cv2
 
 def show_result(result_dict):
     num_boxes = len(result_dict)
     fig, axes = plt.subplots(num_boxes, 1)
     if num_boxes == 1:
@@ -125,15 +145,15 @@
 show_result(result["provinsiArea"])
 show_result(result["nikArea"])
 show_result(result["detailArea"])
 ```
 
 ### Input ==> Numpy Array Image ==> cv2.imread(image_path)
 ```py
-from src.pisahkan_ktp.ktp_segmenter import segmenter_ndarray
+from pisahkan_ktp.ktp_segmenter import segmenter_ndarray
 import matplotlib.pyplot as plt
 import cv2
 
 def show_result(result_dict):
     num_boxes = len(result_dict)
     fig, axes = plt.subplots(num_boxes, 1)
     if num_boxes == 1:
```

### Comparing `pisahkan_ktp-0.1.8/pyproject.toml` & `pisahkan_ktp-0.2.10/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pisahkan-ktp"
-version = "0.1.8"
+version = "0.2.10"
 authors = ["Hanif Yuli Abdillah P <hanifabd23@gmail.com>"]
+repository = "https://github.com/hanifabd/pisahkan-ktp"
+keywords = ["ktp", "segmentation", "segmentasi", "id-card", "identity-card"]
 description = "Python package for detecting entities in text based on a dictionary and fuzzy similarity"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `pisahkan_ktp-0.1.8/src/pisahkan_ktp/ktp_segmenter.py` & `pisahkan_ktp-0.2.10/src/pisahkan_ktp/ktp_segmenter.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 import os
 import cv2
 import numpy as np
 import math
 from pythonRLSA.rlsa_fast import rlsa_fast
 
 def add_white_block_signature(image, block_width, block_height):
+    '''
+    This function will cover offside signature in detail area
+    '''
     # Get the dimensions of the original image
     height, width, _ = image.shape
 
     # Create a white block image
     white_block = np.full((block_height, block_width, 3), 255, dtype=np.uint8)
 
     # Place the white block in front of the original image
     image_with_block_front = np.copy(image)
     image_with_block_front[height-block_height:, width-block_width:] = white_block
 
     return image_with_block_front
 
 def add_white_block_provinsi(image, block_width, block_height):
+    '''
+    This function will create white block in upper left, upper left, and upper center of provinsi area
+    '''
     # Get the dimensions of the original image
     height, width, _ = image.shape
 
     # Create a white block image
     white_block = np.full((block_height, block_width, 3), 255, dtype=np.uint8)
     upper_height = 5
     white_block_upper = np.full((upper_height, width, 3), 255, dtype=np.uint8)
@@ -33,14 +39,17 @@
     image_with_block_front[:block_height, width - block_width:] = white_block
     # Place the white block in the upper center of the original image
     image_with_block_front[:upper_height, :] = white_block_upper
 
     return image_with_block_front
 
 def prepareRecognitionArea(image_path):
+    '''
+    This function will crop image to provinsi, nik, and detail area
+    '''
     assert isinstance(image_path, str), "Image Path for OCR Process"
     try:
       # Open Image
       img = cv2.imread(image_path)
 
       # Resize Image to Standard Preprocessing Size
       imgResize = cv2.resize(img, (1000, 700))
@@ -58,14 +67,17 @@
 
       return imgResize, provinsi_area, nik_area, detail_area
     except Exception as e:
       print(f"ERROR: {e}")
       return None
 
 def prepareRecognitionAreaNdarray(image):
+    '''
+    This function will crop image to provinsi, nik, and detail area
+    '''
     assert isinstance(image, np.ndarray), "image can be ndarray type only"
     try:
       # Resize Image to Standard Preprocessing Size
       imgResize = cv2.resize(image, (1000, 700))
 
       # Segment Identity Card (Indonesian IC) based on Image Ratio
       imgHeight, imgWidth = imgResize.shape[:2]
@@ -80,34 +92,40 @@
 
       return imgResize, provinsi_area, nik_area, detail_area
     except Exception as e:
       print(f"ERROR: {e}")
       return None
 
 def apply_clahe_to_channels(image, clip_limit=2.0, tile_grid_size=(8, 8)):
+    '''
+    This function will do clahe operation
+    '''
     # Split the image into individual channels
     channels = cv2.split(image)
 
     # Apply CLAHE to each channel
     clahe = cv2.createCLAHE(clipLimit=clip_limit, tileGridSize=tile_grid_size)
     clahe_channels = [clahe.apply(channel) for channel in channels]
 
     # Merge the CLAHE-enhanced channels back into an image
     clahe_image = cv2.merge(clahe_channels)
 
     return clahe_image
 
-def preprocessRecognitionArea(image):
+def preprocessRecognitionArea(image, contrast_factor=1.7, gamma_factor=1.0):
+    '''
+    This function will preprocess the image of each area
+    '''
     # Adjust Image Contrast
-    factor = 1.7 # 1.7
+    factor = contrast_factor # 1.7
     imgAdjustedContrast = image.astype(float)*factor
     imgAdjustedContrast = np.clip(imgAdjustedContrast, 0, 255).astype(np.uint8)
 
     # Gamma Correction - gamma correction can strengthen or weaken dark colors depending on the gamma value used
-    gamma = 1.0 # 1.0
+    gamma = gamma_factor # 1.0
     gamma_corrected = np.clip(imgAdjustedContrast ** (1 / gamma), 0, 255).astype(np.uint8)
 
     # Standarize Image Channel
     imageClahe = apply_clahe_to_channels(gamma_corrected, clip_limit=3.0, tile_grid_size=(8, 8))
 
     # Denoise Image
     imgDenoise = cv2.fastNlMeansDenoisingColored(imageClahe, None, 12, 12, 2, 20)
@@ -117,14 +135,17 @@
 
     # Thresholding Image
     imgThresh = cv2.threshold(imgGray, 220, 255, cv2.THRESH_TRUNC)[1]
 
     return imgThresh
 
 def add_black_block_details(image, x_position, block_width):
+    '''
+    This function will create black block the left of detail area
+    '''
     # Get image dimensions
     height, width = image.shape
 
     # Calculate the starting and ending x coordinates of the block
     start_x = x_position
     end_x = start_x + block_width
 
@@ -134,26 +155,32 @@
 
     # Create a white block
     image[:, start_x:end_x] = 0
 
     return image
 
 def add_black_block_border(image, top, bottom, left, right):
+    '''
+    This function will create black block in the edge of the image
+    '''
     # Get image dimensions
     height, width = image.shape
 
     # Create a black border
     image[:top, :] = 0  # Top border
     image[-bottom:, :] = 0  # Bottom border
     image[:, :left] = 0  # Left border
     image[:, -right:] = 0  # Right border
 
     return image
 
 def findTextPattern(image, typeImage):
+    '''
+    This function will create text line pattern for each row in the image
+    '''
     # Thresholding Image
     threshImage = cv2.threshold(image, 220, 255, cv2.THRESH_BINARY | cv2.THRESH_OTSU)[1]
 
     # RLSA Operation to extract out the ROI(region of interest) like block-of-text/title/content with applied heuristics.
     rlsaValue = max(math.ceil(image.shape[0]/100),math.ceil(image.shape[1]/100))+20
     rlsaImage = rlsa_fast(threshImage, True, False, rlsaValue)
 
@@ -198,14 +225,17 @@
 
     # Reverse Monochrome Color
     patternImage = cv2.bitwise_not(thinDilateImage)
 
     return patternImage
 
 def provinsiCreateBoudingBox(image, min_area_threshold):
+    '''
+    This function will create bounding box for provinsi area
+    '''
     # Thresholding Image
     imgThresh = cv2.adaptiveThreshold(image, 255, cv2.ADAPTIVE_THRESH_GAUSSIAN_C, cv2.THRESH_BINARY_INV, 11, 5)
 
     # Find contours
     contours, _ = cv2.findContours(imgThresh, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE)
 
     # Get bounding boxes
@@ -216,14 +246,17 @@
             bounding_boxes.append((0, max(y-20, 0), min(x+w, int(image.shape[1])), y+h+20))
 
     bounding_boxes.sort(key=lambda bbox: (bbox[1], bbox[0]))
 
     return bounding_boxes
 
 def nikCreateBoudingBox(image, min_area_threshold):
+    '''
+    This function will create bounding box for nik area
+    '''
     # Thresholding Image
     imgThresh = cv2.adaptiveThreshold(image, 255, cv2.ADAPTIVE_THRESH_GAUSSIAN_C, cv2.THRESH_BINARY_INV, 11, 5)
 
     # Find contours
     contours, _ = cv2.findContours(imgThresh, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE)
 
     # Get bounding boxes
@@ -234,14 +267,17 @@
             bounding_boxes.append((0, max(y-30, 0), min(x+image.shape[1], int(image.shape[1])), y+h+30))
 
     bounding_boxes.sort(key=lambda bbox: (bbox[1], bbox[0]))
 
     return bounding_boxes
 
 def detailCreateBoudingBox(image, min_area_threshold):
+    '''
+    This function will create bounding box for detail area
+    '''
     # Thresholding Image
     imgThresh = cv2.adaptiveThreshold(image, 255, cv2.ADAPTIVE_THRESH_GAUSSIAN_C, cv2.THRESH_BINARY_INV, 11, 5)
 
     # Find contours
     contours, _ = cv2.findContours(imgThresh, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE)
 
     # Get bounding boxes
@@ -251,31 +287,31 @@
         if w * h >= min_area_threshold:
             bounding_boxes.append((0, max(y-12, 0), min(x+image.shape[1], int(image.shape[1])), y+h+12))
 
     bounding_boxes.sort(key=lambda bbox: (bbox[1], bbox[0]))
 
     return bounding_boxes
 
-def segmenter(image_path):
+def segmenter(image_path, contrast_factor=1.7, gamma_factor=1.0):
     '''
      This function identifies and isolates sections of Indonesian identity cards from images. 
      By detecting text and photo areas, it creates boundaries for province, nik, and personal information.
     '''
     assert isinstance(image_path, str), "image_path can be str() type only"
 
     try:
         # Attempt to open the file in read mode
         with open(image_path, "r"):
             # Original Image
             originalImage, provinsiArea, nikArea, detailArea = prepareRecognitionArea(image_path)
 
             # Preprocessed Image
-            provinsiAreaPreprocessed = preprocessRecognitionArea(provinsiArea)
-            nikAreaPreprocessed = preprocessRecognitionArea(nikArea)
-            detailAreaPreprocessed = preprocessRecognitionArea(detailArea)
+            provinsiAreaPreprocessed = preprocessRecognitionArea(provinsiArea, contrast_factor=contrast_factor, gamma_factor=gamma_factor)
+            nikAreaPreprocessed = preprocessRecognitionArea(nikArea, contrast_factor=contrast_factor, gamma_factor=gamma_factor)
+            detailAreaPreprocessed = preprocessRecognitionArea(detailArea, contrast_factor=contrast_factor, gamma_factor=gamma_factor)
 
             # Pattern Image
             provinsiAreaPattern = findTextPattern(provinsiAreaPreprocessed, "provinsi")
             nikAreaPattern = findTextPattern(nikAreaPreprocessed, "nik")
             detailAreaPattern = findTextPattern(detailAreaPreprocessed, "detail")
 
             # Draw bounding boxes on the original image
@@ -303,28 +339,28 @@
                 "nikArea": segmented_nik,
                 "detailArea": segmented_detail,
             }
     except FileNotFoundError:
         # If the file does not exist, FileNotFoundError is raised
         raise FileNotFoundError("File does not exist.")
 
-def segmenter_ndarray(image):
+def segmenter_ndarray(image, contrast_factor=1.7, gamma_factor=1.0):
     '''
      This function identifies and isolates sections of Indonesian identity cards from images. 
      By detecting text and photo areas, it creates boundaries for province, nik, and personal information.
     '''
     assert isinstance(image, np.ndarray), "image can be ndarray type only"
 
     try:
         # Original Image
         originalImage, provinsiArea, nikArea, detailArea = prepareRecognitionAreaNdarray(image)
         # Preprocessed Image
-        provinsiAreaPreprocessed = preprocessRecognitionArea(provinsiArea)
-        nikAreaPreprocessed = preprocessRecognitionArea(nikArea)
-        detailAreaPreprocessed = preprocessRecognitionArea(detailArea)
+        provinsiAreaPreprocessed = preprocessRecognitionArea(provinsiArea, contrast_factor=contrast_factor, gamma_factor=gamma_factor)
+        nikAreaPreprocessed = preprocessRecognitionArea(nikArea, contrast_factor=contrast_factor, gamma_factor=gamma_factor)
+        detailAreaPreprocessed = preprocessRecognitionArea(detailArea, contrast_factor=contrast_factor, gamma_factor=gamma_factor)
         # Pattern Image
         provinsiAreaPattern = findTextPattern(provinsiAreaPreprocessed, "provinsi")
         nikAreaPattern = findTextPattern(nikAreaPreprocessed, "nik")
         detailAreaPattern = findTextPattern(detailAreaPreprocessed, "detail")
         # Draw bounding boxes on the original image
         segmented_provinsi = []
         boundingBoxesRowsProvinsi = provinsiCreateBoudingBox(provinsiAreaPattern, 450)
@@ -347,15 +383,52 @@
             "nikArea": segmented_nik,
             "detailArea": segmented_detail,
         }
     except Exception as e:
         # If the file does not exist, FileNotFoundError is raised
         raise f"ERROR: {e}"
 
+def detect_empty_list_in_dict(input_dict):
+    '''
+    Detects if any value in the given dictionary is an empty list.
+    '''
+    # Iterate over the values of the dictionary
+    for value in input_dict.values():
+        if isinstance(value, list) and not value:
+            return True
+    return False
+
+def adaptive_segmenter(image_path, contrast_factor=1.7, delta_contrast=0.1, gamma_factor=1.0):
+    '''
+    This function will execute segmenter() with operation of contrast_factor if result contain []. contrast_factor will be reduced by delta_contrast
+    '''
+    contrast_factor = contrast_factor
+    while (contrast_factor >= 1.0):
+        result = segmenter(image_path, contrast_factor=contrast_factor, gamma_factor=gamma_factor)
+        if detect_empty_list_in_dict(result):
+            contrast_factor = round(contrast_factor - delta_contrast, 1)
+        else:
+            return result 
+
+def adaptive_segmenter_ndarray(image, contrast_factor=1.7, delta_contrast=0.1, gamma_factor=1.0):
+    '''
+    This function will execute segmenter_ndarray() with operation of contrast_factor if result contain []. contrast_factor will be reduced by delta_contrast
+    '''
+    contrast_factor = contrast_factor
+    while (contrast_factor >= 1.0):
+        result = segmenter_ndarray(image, contrast_factor=contrast_factor, gamma_factor=gamma_factor)
+        if detect_empty_list_in_dict(result):
+            contrast_factor = round(contrast_factor - delta_contrast, 1)
+        else:
+            return result 
+
 def getPassPhoto(image_path):
+    '''
+    This function will crop pass-photo from the image
+    '''
     assert isinstance(image_path, str), "Image Path"
     try:
         # Open Image
         img = cv2.imread(image_path)
 
         # Resize Image to Standard Preprocessing Size
         imgResize = cv2.resize(img, (1000, 700))
@@ -368,14 +441,17 @@
         
         return passphoto
     except Exception as e:
         print(f"ERROR: {e}")
         return None
 
 def getSignature(image_path):
+    '''
+    This function will crop signature from the image
+    '''
     assert isinstance(image_path, str), "Image Path"
     try:
         # Open Image
         img = cv2.imread(image_path)
 
         # Resize Image to Standard Preprocessing Size
         imgResize = cv2.resize(img, (1000, 700))
```

### Comparing `pisahkan_ktp-0.1.8/PKG-INFO` & `pisahkan_ktp-0.2.10/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: pisahkan-ktp
-Version: 0.1.8
+Version: 0.2.10
 Summary: Python package for detecting entities in text based on a dictionary and fuzzy similarity
+Home-page: https://github.com/hanifabd/pisahkan-ktp
+Keywords: ktp,segmentation,segmentasi,id-card,identity-card
 Author: Hanif Yuli Abdillah P
 Author-email: hanifabd23@gmail.com
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: opencv-contrib-python (==4.9.0.80)
 Requires-Dist: opencv-python (==4.8.0.76)
 Requires-Dist: pythonRLSA (==1.0.0)
+Project-URL: Repository, https://github.com/hanifabd/pisahkan-ktp
 Description-Content-Type: text/markdown
 
 # **PISAHKAN KTP: Indonesian ID Card (KTP) Information Segmentation**
 
 <center><img src="./assets/OIG1.jpg" alt="Beautiful Landscape" width="250"></center>
 
 
@@ -53,30 +55,50 @@
 1. Installation
     ```sh
     pip install pisahkan-ktp
     ```
 ### Inference
 1. Usage
     - Text Area
-        ```py
-        # Input ==> Image Path
-        from pisahkan_ktp.ktp_segmenter import segmenter
-
-        image_path = "./tests/sample.jpg"
-        result = segmenter(image_path)
-        print(result)
-
-        # Input ==> Numpy Array Image ==> cv2.imread(image_path)
-        from pisahkan_ktp.ktp_segmenter import segmenter_ndarray
+        - Standard Segmenter
+            ```py
+            # Input ==> Image Path
+            from pisahkan_ktp.ktp_segmenter import segmenter
+
+            image_path = "./tests/sample.jpg"
+            result = segmenter(image_path)
+            print(result)
+
+            # Input ==> Numpy Array Image ==> cv2.imread(image_path)
+            from pisahkan_ktp.ktp_segmenter import segmenter_ndarray
+
+            image_path = "./tests/sample.jpg"
+            image = cv2.imread(image_path)
+            result = segmenter_ndarray(image)
+            print(result)
+            ```
+        
+        - Adaptive Segmenter (Adjust contrast level in preprocessing)
+            ```py
+            # Input ==> Image Path
+            from pisahkan_ktp.ktp_segmenter import adaptive_segmenter
+    
+            image_path = "./tests/sample.jpg"
+            result = adaptive_segmenter(image_path, contrast_factor=1.7, delta_contrast=0.7, gamma_factor=1.0)
+            print(result)
+    
+            # Input ==> Numpy Array Image ==> cv2.imread(image_path)
+            from pisahkan_ktp.ktp_segmenter import adaptive_segmenter_ndarray
+    
+            image_path = "./tests/sample.jpg"
+            image = cv2.imread(image_path)
+            result = adaptive_segmenter_ndarray(image, contrast_factor=1.7, delta_contrast=0.7, gamma_factor=1.0)
+            print(result)
+            ```
 
-        image_path = "./tests/sample.jpg"
-        image = cv2.imread(image_path)
-        result = segmenter_ndarray(image)
-        print(result)
-        ```
     - Pass-Photo & Signature
         ```py
         # Input ==> Image Path
         from pisahkan_ktp.ktp_segmenter import getPassPhoto, getSignature
 
         image_path = "./tests/sample.jpg"
         result = getPassPhoto(image_path)
@@ -118,15 +140,15 @@
     - Detail Area Cropped
         
         <img src="./assets/8-7-detail.jpg" alt="Beautiful Landscape" width="500">
 
 ## How to Show in Matplotlib
 ### Input ==> Image Path
 ```py
-from src.pisahkan_ktp.ktp_segmenter import segmenter
+from pisahkan_ktp.ktp_segmenter import segmenter
 import matplotlib.pyplot as plt
 import cv2
 
 def show_result(result_dict):
     num_boxes = len(result_dict)
     fig, axes = plt.subplots(num_boxes, 1)
     if num_boxes == 1:
@@ -146,15 +168,15 @@
 show_result(result["provinsiArea"])
 show_result(result["nikArea"])
 show_result(result["detailArea"])
 ```
 
 ### Input ==> Numpy Array Image ==> cv2.imread(image_path)
 ```py
-from src.pisahkan_ktp.ktp_segmenter import segmenter_ndarray
+from pisahkan_ktp.ktp_segmenter import segmenter_ndarray
 import matplotlib.pyplot as plt
 import cv2
 
 def show_result(result_dict):
     num_boxes = len(result_dict)
     fig, axes = plt.subplots(num_boxes, 1)
     if num_boxes == 1:
```

