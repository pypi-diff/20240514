# Comparing `tmp/deepview_validator-3.2.2-py3-none-any.whl.zip` & `tmp/deepview_validator-3.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,59 +1,61 @@
-Zip file size: 150352 bytes, number of entries: 57
--rw-rw-r--  2.0 unx      936 b- defN 24-Feb-29 22:17 deepview/validator/__init__.py
--rw-rw-r--  2.0 unx    31800 b- defN 24-Feb-29 22:17 deepview/validator/__main__.py
--rw-rw-r--  2.0 unx    11477 b- defN 24-Feb-29 22:17 deepview/validator/exceptions.py
--rw-rw-r--  2.0 unx     5385 b- defN 24-Feb-29 22:17 deepview/validator/datasets/__init__.py
--rw-rw-r--  2.0 unx     6088 b- defN 24-Feb-29 22:17 deepview/validator/datasets/arrow.py
--rw-rw-r--  2.0 unx    12134 b- defN 24-Feb-29 22:17 deepview/validator/datasets/core.py
--rw-rw-r--  2.0 unx    20744 b- defN 24-Feb-29 22:17 deepview/validator/datasets/darknet.py
--rw-rw-r--  2.0 unx    19944 b- defN 24-Feb-29 22:17 deepview/validator/datasets/instance.py
--rw-rw-r--  2.0 unx     7530 b- defN 24-Feb-29 22:17 deepview/validator/datasets/tfrecord.py
--rw-rw-r--  2.0 unx    21516 b- defN 24-Feb-29 22:17 deepview/validator/datasets/utils.py
--rw-rw-r--  2.0 unx      735 b- defN 24-Feb-29 22:17 deepview/validator/evaluators/__init__.py
--rw-rw-r--  2.0 unx     7710 b- defN 24-Feb-29 22:17 deepview/validator/evaluators/combinedevaluator.py
--rw-rw-r--  2.0 unx    17045 b- defN 24-Feb-29 22:17 deepview/validator/evaluators/core.py
--rw-rw-r--  2.0 unx    15096 b- defN 24-Feb-29 22:17 deepview/validator/evaluators/detectionevaluator.py
--rw-rw-r--  2.0 unx    23949 b- defN 24-Feb-29 22:17 deepview/validator/evaluators/parameters.py
--rw-rw-r--  2.0 unx     8667 b- defN 24-Feb-29 22:17 deepview/validator/evaluators/poseevaluator.py
--rw-rw-r--  2.0 unx    10399 b- defN 24-Feb-29 22:17 deepview/validator/evaluators/segmentationevaluator.py
--rw-rw-r--  2.0 unx     9184 b- defN 24-Feb-29 22:17 deepview/validator/evaluators/utils.py
--rw-rw-r--  2.0 unx      952 b- defN 24-Feb-29 22:17 deepview/validator/metrics/__init__.py
--rw-rw-r--  2.0 unx     3507 b- defN 24-Feb-29 22:17 deepview/validator/metrics/core.py
--rw-rw-r--  2.0 unx    20714 b- defN 24-Feb-29 22:17 deepview/validator/metrics/detectiondata.py
--rw-rw-r--  2.0 unx    33326 b- defN 24-Feb-29 22:17 deepview/validator/metrics/detectionmatch.py
--rw-rw-r--  2.0 unx    32873 b- defN 24-Feb-29 22:17 deepview/validator/metrics/detectionmetrics.py
--rw-rw-r--  2.0 unx    26129 b- defN 24-Feb-29 22:17 deepview/validator/metrics/detectionutils.py
--rw-rw-r--  2.0 unx     9997 b- defN 24-Feb-29 22:17 deepview/validator/metrics/posedata.py
--rw-rw-r--  2.0 unx     2028 b- defN 24-Feb-29 22:17 deepview/validator/metrics/posemetrics.py
--rw-rw-r--  2.0 unx     1022 b- defN 24-Feb-29 22:17 deepview/validator/metrics/poseutils.py
--rw-rw-r--  2.0 unx    10940 b- defN 24-Feb-29 22:17 deepview/validator/metrics/segmentationdata.py
--rw-rw-r--  2.0 unx     5534 b- defN 24-Feb-29 22:17 deepview/validator/metrics/segmentationmetrics.py
--rw-rw-r--  2.0 unx     6643 b- defN 24-Feb-29 22:17 deepview/validator/metrics/segmentationutils.py
--rw-rw-r--  2.0 unx    52664 b- defN 24-Feb-29 22:17 deepview/validator/metrics/summary.py
--rw-rw-r--  2.0 unx      821 b- defN 24-Feb-29 22:17 deepview/validator/runners/__init__.py
--rw-rw-r--  2.0 unx    10089 b- defN 24-Feb-29 22:17 deepview/validator/runners/core.py
--rw-rw-r--  2.0 unx    19725 b- defN 24-Feb-29 22:17 deepview/validator/runners/deepviewrt.py
--rw-rw-r--  2.0 unx    14272 b- defN 24-Feb-29 22:17 deepview/validator/runners/keras.py
--rw-rw-r--  2.0 unx    18805 b- defN 24-Feb-29 22:17 deepview/validator/runners/offline.py
--rw-rw-r--  2.0 unx     8872 b- defN 24-Feb-29 22:17 deepview/validator/runners/onnx.py
--rw-rw-r--  2.0 unx    14653 b- defN 24-Feb-29 22:17 deepview/validator/runners/tensorrt.py
--rw-rw-r--  2.0 unx     9172 b- defN 24-Feb-29 22:17 deepview/validator/runners/tflite.py
--rw-rw-r--  2.0 unx      615 b- defN 24-Feb-29 22:17 deepview/validator/runners/modelclient/__init__.py
--rw-rw-r--  2.0 unx     3703 b- defN 24-Feb-29 22:17 deepview/validator/runners/modelclient/core.py
--rw-rw-r--  2.0 unx    25636 b- defN 24-Feb-29 22:17 deepview/validator/runners/modelclient/detection.py
--rw-rw-r--  2.0 unx     9675 b- defN 24-Feb-29 22:17 deepview/validator/runners/modelclient/segmentation.py
--rw-rw-r--  2.0 unx      314 b- defN 24-Feb-29 22:17 deepview/validator/visualize/__init__.py
--rw-rw-r--  2.0 unx    25309 b- defN 24-Feb-29 22:17 deepview/validator/visualize/detectiondraw.py
--rw-rw-r--  2.0 unx     7231 b- defN 24-Feb-29 22:17 deepview/validator/visualize/posedraw.py
--rw-rw-r--  2.0 unx     8036 b- defN 24-Feb-29 22:17 deepview/validator/visualize/segmentationdraw.py
--rw-rw-r--  2.0 unx    15063 b- defN 24-Feb-29 22:17 deepview/validator/visualize/utils.py
--rw-rw-r--  2.0 unx     2899 b- defN 24-Feb-29 22:17 deepview/validator/writers/__init__.py
--rw-rw-r--  2.0 unx     2478 b- defN 24-Feb-29 22:17 deepview/validator/writers/console.py
--rw-rw-r--  2.0 unx    17080 b- defN 24-Feb-29 22:17 deepview/validator/writers/core.py
--rw-rw-r--  2.0 unx     4884 b- defN 24-Feb-29 22:17 deepview/validator/writers/tensorboard.py
--rw-rw-r--  2.0 unx      512 b- defN 24-Feb-29 22:17 deepview_validator-3.2.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Feb-29 22:17 deepview_validator-3.2.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx       73 b- defN 24-Feb-29 22:17 deepview_validator-3.2.2.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        9 b- defN 24-Feb-29 22:17 deepview_validator-3.2.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     5542 b- defN 24-Feb-29 22:17 deepview_validator-3.2.2.dist-info/RECORD
-57 files, 662228 bytes uncompressed, 141326 bytes compressed:  78.7%
+Zip file size: 165396 bytes, number of entries: 59
+-rw-rw-r--  2.0 unx      936 b- defN 24-May-14 16:10 deepview/validator/__init__.py
+-rw-rw-r--  2.0 unx    34066 b- defN 24-May-14 16:10 deepview/validator/__main__.py
+-rw-rw-r--  2.0 unx    11375 b- defN 24-May-14 16:10 deepview/validator/exceptions.py
+-rw-rw-r--  2.0 unx     5782 b- defN 24-May-14 16:10 deepview/validator/datasets/__init__.py
+-rw-rw-r--  2.0 unx     5803 b- defN 24-May-14 16:10 deepview/validator/datasets/arrow.py
+-rw-rw-r--  2.0 unx     3276 b- defN 24-May-14 16:10 deepview/validator/datasets/base.py
+-rw-rw-r--  2.0 unx    11866 b- defN 24-May-14 16:10 deepview/validator/datasets/core.py
+-rw-rw-r--  2.0 unx    20050 b- defN 24-May-14 16:10 deepview/validator/datasets/darknet.py
+-rw-rw-r--  2.0 unx    19950 b- defN 24-May-14 16:10 deepview/validator/datasets/instance.py
+-rw-rw-r--  2.0 unx     7547 b- defN 24-May-14 16:10 deepview/validator/datasets/tfrecord.py
+-rw-rw-r--  2.0 unx    24537 b- defN 24-May-14 16:10 deepview/validator/datasets/utils.py
+-rw-rw-r--  2.0 unx      735 b- defN 24-May-14 16:10 deepview/validator/evaluators/__init__.py
+-rw-rw-r--  2.0 unx     7710 b- defN 24-May-14 16:10 deepview/validator/evaluators/combinedevaluator.py
+-rw-rw-r--  2.0 unx    17030 b- defN 24-May-14 16:10 deepview/validator/evaluators/core.py
+-rw-rw-r--  2.0 unx    14842 b- defN 24-May-14 16:10 deepview/validator/evaluators/detectionevaluator.py
+-rw-rw-r--  2.0 unx    26879 b- defN 24-May-14 16:10 deepview/validator/evaluators/parameters.py
+-rw-rw-r--  2.0 unx     8249 b- defN 24-May-14 16:10 deepview/validator/evaluators/poseevaluator.py
+-rw-rw-r--  2.0 unx    10399 b- defN 24-May-14 16:10 deepview/validator/evaluators/segmentationevaluator.py
+-rw-rw-r--  2.0 unx     9184 b- defN 24-May-14 16:10 deepview/validator/evaluators/utils.py
+-rw-rw-r--  2.0 unx      952 b- defN 24-May-14 16:10 deepview/validator/metrics/__init__.py
+-rw-rw-r--  2.0 unx     3507 b- defN 24-May-14 16:10 deepview/validator/metrics/core.py
+-rw-rw-r--  2.0 unx    20727 b- defN 24-May-14 16:10 deepview/validator/metrics/detectiondata.py
+-rw-rw-r--  2.0 unx    34156 b- defN 24-May-14 16:10 deepview/validator/metrics/detectionmatch.py
+-rw-rw-r--  2.0 unx    32369 b- defN 24-May-14 16:10 deepview/validator/metrics/detectionmetrics.py
+-rw-rw-r--  2.0 unx    26257 b- defN 24-May-14 16:10 deepview/validator/metrics/detectionutils.py
+-rw-rw-r--  2.0 unx    10009 b- defN 24-May-14 16:10 deepview/validator/metrics/posedata.py
+-rw-rw-r--  2.0 unx     2120 b- defN 24-May-14 16:10 deepview/validator/metrics/posemetrics.py
+-rw-rw-r--  2.0 unx     1022 b- defN 24-May-14 16:10 deepview/validator/metrics/poseutils.py
+-rw-rw-r--  2.0 unx    10935 b- defN 24-May-14 16:10 deepview/validator/metrics/segmentationdata.py
+-rw-rw-r--  2.0 unx     5534 b- defN 24-May-14 16:10 deepview/validator/metrics/segmentationmetrics.py
+-rw-rw-r--  2.0 unx     6643 b- defN 24-May-14 16:10 deepview/validator/metrics/segmentationutils.py
+-rw-rw-r--  2.0 unx    55204 b- defN 24-May-14 16:10 deepview/validator/metrics/summary.py
+-rw-rw-r--  2.0 unx      896 b- defN 24-May-14 16:10 deepview/validator/runners/__init__.py
+-rw-rw-r--  2.0 unx    24984 b- defN 24-May-14 16:10 deepview/validator/runners/core.py
+-rw-rw-r--  2.0 unx    21949 b- defN 24-May-14 16:10 deepview/validator/runners/deepviewrt.py
+-rw-rw-r--  2.0 unx    11086 b- defN 24-May-14 16:10 deepview/validator/runners/hailo.py
+-rw-rw-r--  2.0 unx    25984 b- defN 24-May-14 16:10 deepview/validator/runners/keras.py
+-rw-rw-r--  2.0 unx    18127 b- defN 24-May-14 16:10 deepview/validator/runners/offline.py
+-rw-rw-r--  2.0 unx    19521 b- defN 24-May-14 16:10 deepview/validator/runners/onnx.py
+-rw-rw-r--  2.0 unx    14524 b- defN 24-May-14 16:10 deepview/validator/runners/tensorrt.py
+-rw-rw-r--  2.0 unx    14547 b- defN 24-May-14 16:10 deepview/validator/runners/tflite.py
+-rw-rw-r--  2.0 unx      634 b- defN 24-May-14 16:10 deepview/validator/runners/modelclient/__init__.py
+-rw-rw-r--  2.0 unx     3685 b- defN 24-May-14 16:10 deepview/validator/runners/modelclient/core.py
+-rw-rw-r--  2.0 unx    25765 b- defN 24-May-14 16:10 deepview/validator/runners/modelclient/detection.py
+-rw-rw-r--  2.0 unx    10034 b- defN 24-May-14 16:10 deepview/validator/runners/modelclient/segmentation.py
+-rw-rw-r--  2.0 unx      314 b- defN 24-May-14 16:10 deepview/validator/visualize/__init__.py
+-rw-rw-r--  2.0 unx    25932 b- defN 24-May-14 16:10 deepview/validator/visualize/detectiondraw.py
+-rw-rw-r--  2.0 unx     7231 b- defN 24-May-14 16:10 deepview/validator/visualize/posedraw.py
+-rw-rw-r--  2.0 unx     8036 b- defN 24-May-14 16:10 deepview/validator/visualize/segmentationdraw.py
+-rw-rw-r--  2.0 unx    15087 b- defN 24-May-14 16:10 deepview/validator/visualize/utils.py
+-rw-rw-r--  2.0 unx     2899 b- defN 24-May-14 16:10 deepview/validator/writers/__init__.py
+-rw-rw-r--  2.0 unx     2478 b- defN 24-May-14 16:10 deepview/validator/writers/console.py
+-rw-rw-r--  2.0 unx    17080 b- defN 24-May-14 16:10 deepview/validator/writers/core.py
+-rw-rw-r--  2.0 unx     5021 b- defN 24-May-14 16:10 deepview/validator/writers/tensorboard.py
+-rw-rw-r--  2.0 unx     1178 b- defN 24-May-14 16:10 deepview_validator-3.3.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-May-14 16:10 deepview_validator-3.3.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       73 b- defN 24-May-14 16:10 deepview_validator-3.3.0.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        9 b- defN 24-May-14 16:10 deepview_validator-3.3.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     5732 b- defN 24-May-14 16:10 deepview_validator-3.3.0.dist-info/RECORD
+59 files, 732549 bytes uncompressed, 156078 bytes compressed:  78.7%
```

## zipnote {}

```diff
@@ -9,14 +9,17 @@
 
 Filename: deepview/validator/datasets/__init__.py
 Comment: 
 
 Filename: deepview/validator/datasets/arrow.py
 Comment: 
 
+Filename: deepview/validator/datasets/base.py
+Comment: 
+
 Filename: deepview/validator/datasets/core.py
 Comment: 
 
 Filename: deepview/validator/datasets/darknet.py
 Comment: 
 
 Filename: deepview/validator/datasets/instance.py
@@ -96,14 +99,17 @@
 
 Filename: deepview/validator/runners/core.py
 Comment: 
 
 Filename: deepview/validator/runners/deepviewrt.py
 Comment: 
 
+Filename: deepview/validator/runners/hailo.py
+Comment: 
+
 Filename: deepview/validator/runners/keras.py
 Comment: 
 
 Filename: deepview/validator/runners/offline.py
 Comment: 
 
 Filename: deepview/validator/runners/onnx.py
@@ -150,23 +156,23 @@
 
 Filename: deepview/validator/writers/core.py
 Comment: 
 
 Filename: deepview/validator/writers/tensorboard.py
 Comment: 
 
-Filename: deepview_validator-3.2.2.dist-info/METADATA
+Filename: deepview_validator-3.3.0.dist-info/METADATA
 Comment: 
 
-Filename: deepview_validator-3.2.2.dist-info/WHEEL
+Filename: deepview_validator-3.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: deepview_validator-3.2.2.dist-info/entry_points.txt
+Filename: deepview_validator-3.3.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: deepview_validator-3.2.2.dist-info/top_level.txt
+Filename: deepview_validator-3.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: deepview_validator-3.2.2.dist-info/RECORD
+Filename: deepview_validator-3.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## deepview/validator/__main__.py

```diff
@@ -51,35 +51,30 @@
 
     Raises
     ------
         ReferenceError
             This is raised if both types of thresholds 
             are set in the commandline.
     """
-    validation_score, detection_score = 0.50, 0.50
-
-    if args.validation_threshold is not None:
-        if args.validation_score is not None:
-            raise ReferenceError(
-                "Supplied two arguments for the validation score threshold.")
-        else:
-            validation_score = args.validation_threshold
-    else:
-        if args.validation_score is not None:
-            validation_score = args.validation_score
-
-    if args.detection_threshold is not None:
-        if args.detection_score is not None:
-            raise ReferenceError(
-                "Supplied two arguments for the detection score threshold.")
-        else:
-            detection_score = args.detection_threshold
-    else:
-        if args.detection_score is not None:
-            detection_score = args.detection_score
+    if args.validation_score > 0.0 and args.validation_threshold > 0.0:
+        raise RuntimeError(
+            "Only one of the validation score thresholds should be set.")
+    validation_score = (args.validation_score 
+                        if args.validation_score > 0.0 
+                        else args.validation_threshold)
+
+    detection_score = 0.50
+    if args.detection_score is not None and args.detection_threshold is not None:
+        raise RuntimeError(
+            "Only one of the detection score thresholds should be set.")
+    detection_score = (args.detection_score 
+                       if args.detection_score is not None 
+                       else args.detection_threshold 
+                       if args.detection_threshold is not None 
+                       else detection_score)
     return validation_score, detection_score
 
 
 def build_parameters(
         args, validation_score: float, detection_score: float) -> Parameters:
     """
     Store command line arguments inside the Parameters object 
@@ -119,14 +114,17 @@
     parameters.clamp_boxes = args.clamp_box
     parameters.ignore_boxes = args.ignore_box
     parameters.display = args.display
     parameters.plots = args.exclude_plots
     parameters.validate_3d = args.validate_3d
     parameters.include_background = args.include_background
     parameters.leniency_factor = args.leniency_factor
+    parameters.letterbox = args.letterbox
+    parameters.auto_offset = args.disable_auto_offset
+    parameters.class_filter = args.class_filter
 
     # Time of validation
     today = datetime.datetime.now().strftime(
         '%Y-%m-%d--%H:%M:%S').replace(":", "_")
     if args.tensorboard:
         parameters.tensorboard = os.path.join(
             args.tensorboard,
@@ -160,26 +158,26 @@
             on the dataset format that was passed in the command line. 
     """
 
     # Determine the type of the dataset either as Darknet or TFRecord.
     info_dataset = classify_dataset(
         source=args.dataset,
         labels_path=args.labels_file,
-        polar=args.polar)
+        local=args.local_reader)
     # Build the dataset class depending on the type.
     return instantiate_dataset(
         info_dataset=info_dataset,
         source=args.dataset,
         gformat=args.annotation_format,
         absolute=args.absolute_annotations,
         validate_type=args.validate,
         validate_3d=args.validate_3d,
         show_missing_annotations=args.show_missing_annotations,
         label_offset=args.gt_label_offset,
-        polar=args.polar
+        local=args.local_reader
         )
 
 
 def deepviewrt_detection_runner(
         args, labels: list, parameters: Parameters) -> Type[Runner]:
     """
     Instantiate DeepViewRT detection 
@@ -254,23 +252,25 @@
     if args.target is None:
         from deepview.validator.runners import SegmentationDeepViewRTRunner
         return SegmentationDeepViewRTRunner(args.model, parameters)
     else:
         if args.model_segmentation_type.lower() == 'modelpack':
             from deepview.validator.runners.modelclient import SegmentationModelPack
             runner = SegmentationModelPack(
-                model_path=args.model,
-                target=f'http://{args.target}/v1')
+                model=args.model,
+                target=f'http://{args.target}/v1',
+                parameters=parameters)
             return runner
 
         elif args.model_segmentation_type.lower() == 'deeplab':
             from deepview.validator.runners.modelclient import SegmentationDeepLab
             runner = SegmentationDeepLab(
-                model_path=args.model,
-                target=f'http://{args.target}/v1')
+                model=args.model,
+                target=f'http://{args.target}/v1',
+                parameters=parameters)
             return runner
 
 
 def build_deepviewrt_runner(
         args, labels: list, parameters: Parameters) -> Type[Runner]:
     """
     Instantiate DeepViewRT runners based on the different validation types.
@@ -418,14 +418,41 @@
     if args.validate.lower() == "detection":
         from deepview.validator.runners import ONNXRunner
         return ONNXRunner(args.model, parameters, labels)
     else:
         raise UnsupportedValidationTypeException(args.validate)
     
 
+def build_hailo_runner(args, labels: list, parameters: Parameters) -> Type[Runner]:
+    """
+    Instantiate Hailo runners.
+
+    Parameters
+    ----------
+        args: argsparse.NameSpace
+            The command line arguments set.
+
+        labels: list
+            This is the list of string labels from the dataset.
+
+        parameters: Parameters
+            These are the model parameters set from the command line.
+
+    Returns
+    -------
+        runner: Type[Runner]
+            This is the runner object that is used to run the model. 
+    """
+    if args.validate.lower() == "detection":
+        from deepview.validator.runners import HailoRunner
+        return HailoRunner(args.model, parameters, labels)
+    else:
+        raise UnsupportedValidationTypeException(args.validate)
+    
+
 def build_offline_runner(args, labels: list) -> Type[Runner]:
     """
     Instantiate Offline runners.
 
     Parameters
     ----------
         args: argsparse.NameSpace
@@ -474,15 +501,16 @@
     -------
         runner: Type[Runner]
             This is the runner object that is used to run the model. 
     """
     runner = None
     for root, _, files in os.walk(model):
         for file in files:
-            if os.path.basename(file) == "keras_metadata.pb":
+            if os.path.basename(file) == "keras_metadata.pb" or \
+                os.path.basename(file) == "saved_model.pb":
                 runner = build_keras_runner(
                     root, 
                     validate, 
                     labels, 
                     parameters
                 )
                 break
@@ -519,16 +547,21 @@
                         )
     parser.add_argument('-d', '--dataset',
                         help=("absolute or relative path "
                               "to the dataset folder or yaml file."),
                         required=True,
                         type=str
                         )
-    parser.add_argument('--polar',
-                        help='Specify for a polar dataset',
+    parser.add_argument('--local_reader',
+                        help=('Specify whether to use local validator methods '
+                              'for reading datasets. '
+                              'Otherwise, by default use deepview-datasets.'),
+                        action='store_true')
+    parser.add_argument('--letterbox',
+                        help='Perform letterbox image preprocessing.',
                         action='store_true')
     parser.add_argument('--labels_file',
                         help=("absolute or relative path "
                               "to the labels.txt file."),
                         type=str
                         )
     parser.add_argument('--gt_label_offset',
@@ -588,47 +621,60 @@
                         choices=['iou', 'centerpoint'],
                         default='iou',
                         type=str
                         )
     parser.add_argument('--leniency_factor',
                         help=("Specify the criteria to consider center "
                               "distances. This is the number of times the "
-                              "smallest bounding box diagonal (center to corner)"
+                              "smallest bounding box diagonal (center to corner) "
                               "should fit in the box-box center distance."),
                         default=2,
                         type=int
                         )
+    parser.add_argument('--disable_auto_offset',
+                        help=("Disable auto offset of the model indices "
+                              "based on its output shape and "
+                              "the ground truth labels."),
+                        action="store_false")
+    parser.add_argument('--class_filter',
+                        help=("Filter the model detection classes to match "
+                              "the ground truth classes. This should only "
+                              "be specified if the model has more classes than "
+                              "the dataset."),
+                        action='store_true')
     parser.add_argument('-e', '--engine',
                         help=("Compute engine for inference."
                               "'npu', 'gpu', 'cpu'"),
                         choices=['cpu', 'npu', 'gpu'],
                         default='npu',
                         type=str
                         )
     parser.add_argument('--detection_threshold',
                         help=("NMS threshold for valid scores. This parameter "
                               "will overwrite --detection_score"),
-                        type=float
+                        type=float,
                         )
     parser.add_argument('--detection_score',
                         help=('NMS threshold for valid scores. This parameter '
                               "will overwrite --detection_threshold."),
-                        type=float
+                        type=float,
                         )
     parser.add_argument('--validation_threshold',
                         help=("Validation score threshold "
                               "to filter predictions. This parameter will "
                               "overwrite --validation_score."),
-                        type=float
+                        type=float,
+                        default=0.0
                         )
     parser.add_argument('--validation_score',
                         help=("Validation score threshold "
                               "to filter predictions. This parameter will "
                               "overwrite --validation_threshold"),
-                        type=float
+                        type=float,
+                        default=0.0
                         )
     parser.add_argument('--detection_iou',
                         help='IoU threshold for NMS.',
                         default=0.50,
                         type=float
                         )
     parser.add_argument('--validation_iou',
@@ -768,14 +814,16 @@
         runner = build_tflite_runner(args, dataset.labels, parameters)
     # TensorRT Engine Evaluation
     elif os.path.splitext(args.model)[1].lower() == ".trt":
         runner = build_tensorrt_runner(args, dataset.labels, parameters)
     # ONNX EVALUATION
     elif os.path.splitext(args.model)[1].lower() == ".onnx":
         runner = build_onnx_runner(args, dataset.labels, parameters)
+    elif os.path.splitext(args.model)[1].lower() == ".hef":
+        runner = build_hailo_runner(args, dataset.labels, parameters)
     # Offline EVALUATION (TEXT FILES)
     elif os.path.splitext(args.model)[1].lower() == "":
         runner = find_keras_pb_model(
             args.model, args.validate, dataset.labels, parameters)
 
         if runner is None:
             logger("Model extension does not exist, reading text files",
```

## deepview/validator/exceptions.py

```diff
@@ -98,24 +98,20 @@
     """
     This exception will be raised when
     the dataset provided is empty.
 
     Parameters
     ----------
         info: str
-            The dataset portion that is empty (annotations or images)
-
-        source: str
-            The path to the dataset portion that fails.
+            The error message.
     """
 
-    def __init__(self, info: str, source: str):
+    def __init__(self, info: str):
         sys.tracebacklimit = 0
-        super(EmptyDatasetException, self).__init__(
-            "The are no {} at {}.".format(info, source))
+        super(EmptyDatasetException, self).__init__(info)
 
 class DatasetNotFoundException(Exception):
     """
     This exception will be raised when
     the pass path to the dataset does not exist.
 
     Parameters
@@ -160,15 +156,15 @@
 
     def __init__(self, model_extension: str):
         sys.tracebacklimit = 0
         super(
             UnsupportedModelExtensionException,
             self).__init__(
             "The given model extension {} is currently not supported. ".format(
-            model_extension) + "Can only support .rtm, .h5, or .tflite")
+            model_extension) + "Can only support .rtm, .h5, .tflite, .onnx, .hef, .trt")
 
 class UnsupportedModelTypeException(Exception):
     """
     This exception will be raised when
     the passed model has a type that is currently
     not supported.
 
@@ -197,15 +193,15 @@
             The type of engine (npu, cpu, gpu).
     """
 
     def __init__(self, engine: str):
         sys.tracebacklimit = 0
         super(UnsupportedEngineException, self).__init__(
             "The given engine type {} is not supported. ".format(engine) +
-            "Can only support 'npu', 'cpu', 'gpu'.")
+            "Can only support 'npu', 'cpu', 'gpu', 'cuda', 'deepviewrt', 'hailo'.")
 
 class UnsupportedNMSException(Exception):
     """
     This exception will be raised when
     the given NMS type is not supported.
 
     Parameters
@@ -214,15 +210,15 @@
             The type of NMS to perform.
     """
 
     def __init__(self, nms: str):
         sys.tracebacklimit = 0
         super(UnsupportedNMSException, self).__init__(
             "The given NMS {} is not supported. ".format(nms) +
-            "Can only support 'fast', 'standard', 'matrix'.")
+            "Can only support 'fast', 'standard', 'matrix', 'tensorflow', 'torch'.")
 
 class UnsupportedNormalizationException(Exception):
     """
     This exception will be raised when
     the given normalization is not supported.
 
     Parameters
@@ -372,15 +368,15 @@
     def __init__(self, validation_type: str):
         sys.tracebacklimit = 0
         super(
             UnsupportedValidationTypeException,
             self).__init__(
             "Could not recognize the type of validation, {}. ".format(
                 validation_type
-            ) + "Can only support 'detection' or 'segmentation'.")
+            ) + "Can only support 'detection', 'segmentation', or 'pose'.")
 
 class MissingLibraryException(Exception):
     """
     This exception will be raised if
     the import of a library is fails
     which could mean that the user
     needs to install the library.
```

## deepview/validator/datasets/__init__.py

```diff
@@ -10,27 +10,28 @@
 from typing import Type
 
 from deepview.validator.datasets.instance import InstanceCollection
 from deepview.validator.datasets.tfrecord import TFRecordDataset
 from deepview.validator.datasets.darknet import DarkNetDataset
 from deepview.validator.datasets.arrow import ArrowDataset
 from deepview.validator.datasets.instance import Instance
+from deepview.validator.datasets.base import BaseDataset
 from deepview.validator.datasets.core import Dataset
 from deepview.validator.writers import logger
 
 def instantiate_dataset(
-        info_dataset: dict,
+        info_dataset,
         source: str=None,
         gformat: str='yolo',
         absolute: bool=False,
         validate_type: str='detection',
         validate_3d: bool=False,
         show_missing_annotations: bool=False,
         label_offset: int=0,
-        polar: bool=False
+        local: bool=False
     ) -> Type[Dataset]:
     """
     This function instantiates either darknet or tfrecord
     format dataset objects.
 
     Parameters
     ----------
@@ -89,16 +90,17 @@
             missing annotations. Else, it will only
             print the number of missing annotations.
 
         label_offset: int
             The offset to use for the mapping of integer labels to 
             string labels. 
 
-        polar: bool
-            Specify whether reading from a polar dataset.
+        local: bool
+            Specify whether to use local validator methods for reading datasets.
+            Otherwise, by default use deepview-datasets.
 
     Returns
     -------
         Dataset object: DarknetDataset or TFRecordDataset
             This object is returned depending on the type of dataset
             provided.
 
@@ -117,45 +119,50 @@
             path to the images or annotations is not a string.
 
         EmptyDatasetException
             This exception will be raised if the provided
             path to the images or text files does not contain
             any image files or text files respectively.
     """
-    try:
-        ds_format = info_dataset.get('type')
-        if ds_format is None:
-            ds_format = info_dataset.get("dataset").get("format")
-    except AttributeError:
-        logger("Dataset was not properly read. Ensure the dataset " +
-               "structure follows images/validate and labels/validate.",
-               code="ERROR")
-    if ds_format in [None, "tfrecord"]:
-        return TFRecordDataset(
-            info_dataset=info_dataset,
-            source=source,
-            gformat=gformat,
-            absolute=absolute,
-            validate_type=validate_type,
-            label_offset=label_offset
-            )
-    elif ds_format == "darknet":
-        return DarkNetDataset(
-            info_dataset=info_dataset,
-            source=source,
-            gformat=gformat,
-            absolute=absolute,
-            validate_type=validate_type,
-            show_missing_annotations=show_missing_annotations,
-            validate_3d=validate_3d,
-            label_offset=label_offset,
-            polar=polar
+    if isinstance(info_dataset, dict):
+        try:
+            ds_format = info_dataset.get('type')
+            if ds_format is None:
+                ds_format = info_dataset.get("dataset").get("format")
+        except AttributeError:
+            logger("Dataset was not properly read. Ensure the dataset " +
+                "structure follows images/validate and labels/validate.",
+                code="ERROR")
+        if ds_format in [None, "tfrecord"]:
+            return TFRecordDataset(
+                info_dataset=info_dataset,
+                source=source,
+                gformat=gformat,
+                absolute=absolute,
+                validate_type=validate_type,
+                label_offset=label_offset
+                )
+        elif ds_format == "darknet":
+            return DarkNetDataset(
+                info_dataset=info_dataset,
+                source=source,
+                gformat=gformat,
+                absolute=absolute,
+                validate_type=validate_type,
+                show_missing_annotations=show_missing_annotations,
+                validate_3d=validate_3d,
+                label_offset=label_offset,
+                )
+        elif ds_format == "arrow":
+            return ArrowDataset(
+                info_dataset=info_dataset,
+                source=source,
+                gformat=gformat,
+                absolute=absolute,
+                validate_type=validate_type,
+                label_offset=label_offset,
             )
-    elif ds_format == "arrow":
-        return ArrowDataset(
-            info_dataset=info_dataset,
+    else:
+        return BaseDataset(
             source=source,
-            gformat=gformat,
-            absolute=absolute,
-            validate_type=validate_type,
-            label_offset=label_offset,
+            iterator=info_dataset
         )
```

## deepview/validator/datasets/arrow.py

```diff
@@ -50,22 +50,14 @@
             Specify as True if the annotations are not normalized to the
             image dimensions. By default they are normalized.
 
         validate_type: str
             The type of validation to perform that can be 'detection',
             'segmentation', or 'pose'.
 
-        validate_3d: bool
-            Specify for 3D bounding box annotations.
-
-        show_missing_annotations: bool
-            If this is True, then print on the terminal all
-            missing annotations. Else, it will only
-            print the number of missing annotations.
-
         label_offset: int
             This is the offset of the ground truths indices to be mapped
             into string labels.
 
     Raises
     ------
         InvalidDatasetSourceException
```

## deepview/validator/datasets/core.py

```diff
@@ -3,15 +3,15 @@
 # Unauthorized copying of this file, via any medium is strictly prohibited
 # Proprietary and confidential.
 #
 # This source code is provided solely for runtime interpretation by Python.
 # Modifying or copying any source code is explicitly forbidden.
 
 from deepview.validator.exceptions import UnsupportedAnnotationFormatException
-from typing import Union
+from typing import Union, List
 import numpy as np
 
 class Dataset:
     """
     Contains transformation methods for both images and annotations.
     Images can be resized and annotations can be normalized or denormalized. 
     Annotations can be converted to specific formats (yolo, coco, pascalvoc). 
@@ -53,15 +53,15 @@
         self.format = gformat.lower()
         self.absolute = absolute
         self.validate_type = validate_type.lower()
         self._labels = list()
 
         if self.format not in ['yolo', 'pascalvoc', 'coco']:
             raise UnsupportedAnnotationFormatException(self.format)
-
+        
         self.transformer = None
         if self.format == 'yolo':
             self.transformer = self.yolo2xyxy
         elif self.format == 'coco':
             self.transformer = self.xywh2xyxy
         else:
             self.transformer = None
@@ -72,41 +72,41 @@
             if validate_type.lower() == 'detection':
                 self.normalizer = self.normalize
         else:
             if validate_type.lower() == 'segmentation':
                 self.denormalizer = self.denormalize_polygon
 
     @property
-    def labels(self) -> list[str]:
+    def labels(self) -> List[str]:
         """
         Attribute to access the unique string labels.
         Can be set to :py:class:`list`.
 
         Returns
         -------
             :py:class:`list` of strings
                 This contains the unique string labels.
         """
         return self._labels
 
     @labels.setter
-    def labels(self, new_labels: list[str]):
+    def labels(self, new_labels: List[str]):
         """
         Sets the labels to a new value.
 
         Parameters
         ----------
             new_labels: :py:class:`list`.
                 These are the unique string labels in the dataset to set.
         """
         self._labels = new_labels
 
     @staticmethod
     def convert_labels(
-        labels: list[str],
+        labels: List[str],
         labels_to_convert: Union[list, np.ndarray],
         label_offset: int = 0
     ) -> list:
         """
         Converts integer lables in string labels.
 
         Parameters
@@ -126,56 +126,46 @@
         """
         if all(isinstance(label, str) for label in labels_to_convert):
             return labels_to_convert
         return [labels[int(label)+label_offset].lower() for
                 label in labels_to_convert]
 
     @staticmethod
-    def bgr2rgb(image):
+    def bgr2rgb(image: np.ndarray) -> np.ndarray:
         """
         Converts BGR image to RGB image.
 
         Parameters
         ----------
             image: (height, width, 3) np.ndarray
                 The image as a BGR numpy array.
 
         Returns
         -------
             image: (height, width, 3) np.ndarray
                 The image as a RGB image.
-
-        Raises
-        ------
-            NotImplementedError
-                This method is currently not implemented.
         """
-        raise NotImplementedError("This method is currently not implemented.")
+        return image[:, :, ::-1]
 
     @staticmethod
-    def rgb2bgr(image):
+    def rgb2bgr(image: np.ndarray) -> np.ndarray:
         """
         This method converts RGB image to BGR image.
 
         Parameters
         ----------
             image: (height, width, 3) np.ndarray
                 The image as a RGB numpy array.
 
         Returns
         -------
             image: (height, width, 3) np.ndarray
                 The image as a BGR image.
-
-        Raises
-        ------
-            NotImplementedError
-                This method is currently not implemented.
         """
-        raise NotImplementedError("This method is currently not implemented.")
+        return image[:, :, ::-1]
 
     @staticmethod
     def normalize(boxes: np.ndarray, height: int, width: int) -> np.ndarray:
         """
         Normalizes the boxes to the width and height of the 
         image or model input resolution.
```

## deepview/validator/datasets/darknet.py

```diff
@@ -14,14 +14,15 @@
     read_image
 )
 from deepview.validator.datasets.utils import (
     get_image_files, 
     get_annotation_files
 )
 from deepview.validator.writers import logger
+from typing import List, Tuple
 from PIL import ImageFile
 import numpy as np
 import warnings
 import json
 import os
 
 class DarkNetDataset(Dataset):
@@ -74,17 +75,14 @@
             missing annotations. Else, it will only
             print the number of missing annotations.
 
         label_offset: int
             This is the offset of the ground truths indices to be mapped
             into string labels.
 
-        polar: bool
-            Specify if reading a polars dataset.
-
     Raises
     ------
         InvalidDatasetSourceException
             Raised if the path to the images or annotations is None.
 
         DatasetNotFoundException
             Raised if the provided path to the images or 
@@ -105,15 +103,14 @@
         info_dataset: dict=None,
         gformat: str="yolo",
         absolute: bool=False,
         validate_type: str="detection",
         validate_3d: bool=False,
         show_missing_annotations: bool=False,
         label_offset: int=0,
-        polar: bool=False
     ):
         ImageFile.LOAD_TRUNCATED_IMAGES = True
 
         super(DarkNetDataset, self).__init__(
             source=source,
             gformat=gformat,
             absolute=absolute,
@@ -137,38 +134,22 @@
         
         self.image_source = validate_dataset_source(images_path)
         self.annotation_source = validate_dataset_source(annotations_path)
         
         labels = info_dataset.get('classes', None)
         if labels is not None:
             self.labels = [str(label) for label in labels]
-        
-        if polar:
-            try:
-                from deepview.datasets.readers import TFDarknetDetectionReader
-            except ImportError:
-                logger(
-                    "Dependency missing: deepview-datasets is needed for polar datasets.", 
-                    code="ERROR")
-            reader = TFDarknetDetectionReader(
-                images=self.image_source,
-                annotations=self.annotation_source,
-                classes=labels,
-                silent=True
-            ) 
-            self.images = reader.images
-            self.annotations = reader.annotations
-        else:
-            self.images = get_image_files(self.image_source)
-            self.annotations = get_annotation_files(self.annotation_source)
+   
+        self.images = get_image_files(self.image_source)
+        self.annotations = get_annotation_files(self.annotation_source)
 
         # This is used to map the image name to the annotation file.
         self.annotation_extension = os.path.splitext(self.annotations[0])[1]
 
-    def build_dataset(self) -> list[tuple]:
+    def build_dataset(self) -> List[tuple]:
         """
         Builds the instances to allow iteration in the dataset.
 
         Returns
         -------
             instances: list of tuples
                 One instance contains the
@@ -202,21 +183,21 @@
             logger(
                 "There were {} images without annotations. ".format(
                     missing_annotations) + "To see the names of the images, " +
                 "enable --show_missing_annotations in the command line.",
                 code="WARNING")
         return instances
 
-    def read_sample(self, sample: tuple[str, str]) -> Instance:
+    def read_sample(self, sample: Tuple[str, str]) -> Instance:
         """
         Reads one sample from the dataset.
         
         Parameters
         ----------
-            sample: tuple
+            sample: Tuple
                 This contains (image path, annotation path).
 
         Returns
         -------
             ground truth instance: Instance
                 The ground truth instance objects contains the bounding boxes
                 and the labels representing the ground truth of the image.
```

## deepview/validator/datasets/instance.py

```diff
@@ -2,15 +2,15 @@
 #
 # Unauthorized copying of this file, via any medium is strictly prohibited
 # Proprietary and confidential.
 #
 # This source code is provided solely for runtime interpretation by Python.
 # Modifying or copying any source code is explicitly forbidden.
 
-from typing import Union
+from typing import Union, List
 import numpy as np
 
 class Instance:
     """
     This is the instance object of an image that is used to store the image
     properties such as the dimensions and the path and also stores either
     the ground truth or the prediction bounding boxes (2D/3D), segmentation 
@@ -595,15 +595,15 @@
     """
 
     def __init__(self) -> None:
         self._gt_instances = list()
         self._dt_instances = list()
 
     @property
-    def gt_instances(self) -> list[Instance]:
+    def gt_instances(self) -> List[Instance]:
         """
         Attribute to access the ground truth instance objects.
         Can only be set to :py:class:`list`
 
         Returns
         -------
             :py:class:`list`: Contains ground truth instance objects.
@@ -618,15 +618,15 @@
         ----------
             instance: Instance
                 The ground truth instance object.
         """
         self._gt_instances.append(instance)
 
     @property
-    def dt_instances(self) -> list[Instance]:
+    def dt_instances(self) -> List[Instance]:
         """
         Attribute to access the prediction instance objects.
         Can only be set to :py:class:`list`
 
         Returns
         -------
             :py:class:`list`: Contains prediction instance objects.
```

## deepview/validator/datasets/tfrecord.py

```diff
@@ -7,16 +7,16 @@
 # Modifying or copying any source code is explicitly forbidden.
 
 from deepview.validator.exceptions import MissingLibraryException
 from deepview.validator.exceptions import EmptyDatasetException
 from deepview.validator.datasets.instance import Instance
 from deepview.validator.datasets.core import Dataset
 from deepview.validator.datasets.utils import (
-    classify_dataset, 
-    validate_dataset_source
+    validate_dataset_source,
+    classify_dataset
 )
 import numpy as np
 import glob
 import os
 
 class TFRecordDataset(Dataset):
     """
@@ -91,15 +91,15 @@
         
         labels = info_dataset.get('classes', None)
         if labels is not None:
             self.labels = [str(label) for label in labels]
 
         self.tfrecords = glob.glob(os.path.join(self.source, '*.tfrecord'))
         if len(self.tfrecords) == 0:
-            raise EmptyDatasetException("tfrecord files", self.source)
+            raise EmptyDatasetException(f"There are no TFRecord files in {self.source}")
 
     def py_read_data(self, example):
         """
         This method reads the from the file to extract information.
         
         Parameters
         ----------
```

## deepview/validator/datasets/utils.py

```diff
@@ -6,14 +6,15 @@
 # This source code is provided solely for runtime interpretation by Python.
 # Modifying or copying any source code is explicitly forbidden.
 
 from deepview.validator.exceptions import UnsupportedDatasetTypeException
 from deepview.validator.exceptions import DatasetNotFoundException
 from deepview.validator.exceptions import MissingLibraryException
 from deepview.validator.exceptions import EmptyDatasetException
+from deepview.validator.datasets.core import Dataset
 from deepview.validator.writers import logger
 from typing import Union, Tuple
 from PIL import Image
 import numpy as np
 import glob
 import os
 
@@ -46,27 +47,72 @@
         image = np.asarray(image)
     else:
         image.convert("RGB")
         image = np.asarray(image, dtype=np.uint8)
         image = np.stack((image,)*3, axis=-1)
     return image
 
-def resize(image: Union[str, np.ndarray], size: tuple=None):
+def letterbox_yolox(
+        image: np.ndarray, input_size: np.ndarray):
+    """
+    This function performs image letterbox using the implementation provided
+    in YOLOx: https://github.com/Megvii-BaseDetection/YOLOX/blob/main/yolox/data/data_augment.py#L142
+
+    Parameters
+    ----------
+        image: np.ndarray
+            This is the input image for letterbox transformation.
+
+        input_size: np.ndarray
+            This is the model input size (generally) or the output image 
+            resolution after letterbox transformation.
+
+    Returns
+    -------
+        image: np.ndarray
+            The image after letterbox transformation.
+
+        r: float
+            Ratio to adjust model bounding boxes due to the letterbox
+            transformations.
+    """
+    if len(image.shape) == 3:
+        padded_image = np.ones((input_size[0], input_size[1], 3), dtype=np.uint8) * 114
+    else:
+        padded_image = np.ones(input_size, dtype=np.uint8) * 114
+
+    r = min(input_size[0] / image.shape[0], input_size[1] / image.shape[1])
+    resized_image = resize(image, (int(image.shape[0] * r), int(image.shape[1] * r)), Image.BILINEAR)
+    padded_image[: int(image.shape[0] * r), : int(image.shape[1] * r)] = resized_image
+    padded_image = Dataset.rgb2bgr(padded_image) # RGB2BGR 
+    padded_image = np.ascontiguousarray(padded_image, dtype=np.float32)
+    return padded_image, r
+
+def resize(
+        image: Union[str, np.ndarray], 
+        size: tuple=None, 
+        resample: int=None
+    ) -> np.ndarray:
     """
     Resizes the images depending on the size passed.
 
     Parameters
     ----------
         image: (height, width, 3) np.ndarray or str
             The image represented as a numpy array.
             The path to the image that can be opened using pillow.
 
         size: (height, width) tuple
             Specify the size to resize.
 
+        resample: int
+            This is the type of resampling method in PIllow by default it 
+            is Image.NEAREST set to 0. However, other forms are Image.BILINEAR
+            set to 2.
+
     Returns
     -------
         image: (height, width, 3) np.ndarray
             Resized image.
 
     Raises
     ------
@@ -78,22 +124,28 @@
         return image
 
     # Resize method requires (width, height)
     size = (size[1], size[0])
     if isinstance(image, str):
         if os.path.exists(image):
             img = Image.open(image)
-            img = img.resize(size)
+            if resample is not None:
+                img = img.resize(size, resample)
+            else:
+                img = img.resize(size)
             return np.asarray(img)
         else:
             raise ValueError(
                 "The given image path does not exist at {}".format(image))
     elif isinstance(image, np.ndarray):
         img = Image.fromarray(np.uint8(image))
-        img = img.resize(size)
+        if resample is not None:
+            img = img.resize(size, resample)
+        else:
+            img = img.resize(size)
         return np.asarray(img)
     else:
         raise ValueError(
             "The image provided is neither a " +
             "numpy array or a pillow image object. " +
             "Recieved type: {}".format(type(image)))
 
@@ -124,16 +176,15 @@
     images = list()
     for ext in ['*.[pP][nN][gG]', '*.[jJ][pP][gG]', '*.[jJ][pP][eE][gG]']:
         partial = glob.glob(os.path.join(directory_path, ext))
         images += partial
 
     if check_empty and len(images) == 0:
         raise EmptyDatasetException(
-            "images",
-            directory_path
+            f"There are no images found in {directory_path}"
         )
     return sorted(images)
 
 def get_arrow_files(directory_path: str, check_empty: bool=True) -> Tuple[list, list]:
     """
     Gets all the path of the arrow boxes and images files 
     within the specified directory.
@@ -162,16 +213,15 @@
             directory.
     """
     images = glob.glob(os.path.join(directory_path, "images_*.arrow"))
     boxes = glob.glob(os.path.join(directory_path, "boxes_*.arrow"))
 
     if check_empty and (len(images) == 0 and len(boxes) == 0):
         raise EmptyDatasetException(
-            "images and boxes",
-            directory_path
+            f"There are no arrow files found in {directory_path}"
         )
     return images, boxes
     
 def contains_annotations(annotations: list) -> bool:
     """
     Checks if the detected annotation files are actual darknet annotations.
 
@@ -235,16 +285,17 @@
         annotations = glob.glob(os.path.join(directory_path, ext))
         if contains_annotations(annotations):
             break
         else:
             continue
     
     if check_empty and len(annotations) == 0:
-        raise EmptyDatasetException("annotations",
-                                    directory_path)
+        raise EmptyDatasetException(
+            f"There are no text or JSON files found in {directory_path}"
+        )
     return annotations
 
 def validate_dataset_source(source: str) -> str:
     """
     Validates the existance of the source path.
 
     Parameters
@@ -271,47 +322,59 @@
             "Recieved type: {}".format(
                 type(source)))
     
     if not os.path.exists(source):
         raise DatasetNotFoundException(source)
     return source
         
-def read_yaml_file(file_path: str):
+def read_yaml_file(file_path: str, local: bool):
     """
     Reads yaml files internal to AuZone for collecting
     dataset information.
 
     Parameters
     ----------
         file_path: str
             The path to the yaml file.
+        
+        local: bool
+            Specify if True to use local dataset readers. Otherwise,
+            use deepview-datasets by default.
 
     Returns
     -------
         info_dataset: dict
             This contains the yaml file contents.
             
     Raises
     ------
         MissingLibraryException
             Raised if the yaml library is not installed in the system.
             
         FileNotFoundError
             Raised if the provided path to the file does not exist.
     """
-    try:
-        import yaml
-    except ImportError:
-        raise MissingLibraryException(
-            "The yaml library is needed to read yaml files.")
-    if not os.path.exists(file_path):
-        raise FileNotFoundError("The yaml file is not found at: {}".format(
-            file_path))
-    with open(file_path) as file:
-        return yaml.full_load(file)
+    if local:
+        try:
+            import yaml
+        except ImportError:
+            raise MissingLibraryException(
+                "The yaml library is needed to read yaml files.")
+        if not os.path.exists(file_path):
+            raise FileNotFoundError("The yaml file is not found at: {}".format(
+                file_path))
+        with open(file_path) as file:
+            return yaml.full_load(file)
+    else:
+        from deepview.datasets.generators import ObjectDetectionGenerator
+        handler = ObjectDetectionGenerator(
+            from_config=file_path # config is the path to the yaml file
+        )
+        ds_iterator = handler.get_val_generator()
+        return ds_iterator
 
 def find_yaml_file(source: str):
     """
     Finds yaml files inside a directory. Returns the path to the yaml file
     if it exists, otherwise it returns None.
 
     Parameters
@@ -351,15 +414,15 @@
     Returns
     -------
         labels: list
             This is the list of labels that are the 
             contents of the labels file. If the label file is not found, 
             it will return an empty list.
     """
-    labels = None
+    labels = []
     # Check if labels.txt is under /dataset_path (source)/labels.txt.
     if os.path.exists(os.path.join(source, labels_file)):
         labels_path = os.path.join(source, labels_file)
     # Check if labels.txt path is explicitly provided.
     elif labels_path is not None:
         labels_path = validate_dataset_source(labels_path)
     # If labels.txt is not found, then search through the dataset.
@@ -482,30 +545,31 @@
         # There are no polar yaml representations defined yet.
         info_dataset = dict()
         info_dataset["classes"] = labels
         info_dataset["validation"] = { "path": source }
         return info_dataset
     return None
 
-def collect_darknet_files(source: str, labels: list=[], polar: bool=False):
+def collect_darknet_files(source: str, labels: list=[], local: bool=False):
     """
     Searches the source directory provided to gather images and text or json
     files for darknet datasets.
 
     Parameters
     ----------
         source: str
             The path to the directory to search for 
             images and annotation files.
 
         labels: list
             The list of string labels to include in the dataset information.
 
-        polar: bool
-            Specify when reading polar datasets.
+        local: bool
+            Specify to use local dataset readers in validator. Otherwise
+            by default, use deepview-datasets.
 
     Returns
     -------
         info_dataset: dict
             This includes the paths found for the images and the annotation 
             files and the labels. If no images were found, 
             then None is returned. 
@@ -521,44 +585,46 @@
         annotations = get_annotation_files(annotation_source, False)
         if len(annotations) > 0:
             break
     
     if len(images) == 0:
         return None
     
-    if polar:
-        return create_polar_info(
+    if local:
+        return create_info(
             image_source, 
             annotation_source, 
             "darknet",
             labels
         )
     else:
-        return create_info(
-            image_source, 
-            annotation_source, 
-            "darknet",
-            labels
+        from deepview.datasets.readers.darknet import DarknetDetectionReader
+        return DarknetDetectionReader(
+            images=image_source,
+            annotations=annotation_source,
+            classes=labels,
+            silent=True
         )
     
-def collect_arrow_files(source: str, labels: list=[], polar: bool=False):
+def collect_arrow_files(source: str, labels: list=[], local: bool=False):
     """
     Searches the source directory provided to gather images and text or json
     files for darknet datasets.
 
     Parameters
     ----------
         source: str
             The path to the directory to search for arrow files.
 
         labels: list
             The list of string labels to include in the dataset information.
 
-        polar: bool
-            Specify when reading polar datasets.
+        local: bool
+            Specify to use local dataset readers in validator. Otherwise
+            by default, use deepview-datasets.
 
     Returns
     -------
         info_dataset: dict
             This includes the paths found for the images and the boxes arrow
             files and the labels. If no arrow files were found, 
             then None is returned. 
@@ -570,31 +636,36 @@
             break
     
     if len(images) == 0 and len(boxes) == 0:
         return None
     
     image_source = os.path.join(source, "images_*.arrow")
     boxes_source = os.path.join(source, "boxes_*.arrow")
-    
-    if polar:
-        return create_polar_info(
+
+    if local:
+        return create_info(
             image_source, 
             boxes_source, 
             "arrow",
             labels
         )
     else:
-        return create_info(
-            image_source, 
-            boxes_source, 
-            "arrow",
-            labels
+        from deepview.datasets.readers.arrow import PolarsDetectionReader
+        return PolarsDetectionReader(
+            inputs=image_source,
+            annotations=boxes_source,
+            classes=labels,
+            silent=True
         )
     
-def classify_dataset(source: str, labels_path: str=None, polar: bool=False) -> dict: #NOSONAR
+def classify_dataset( #NOSONAR
+        source: str, 
+        labels_path: str=None, 
+        local: bool=False
+    ) -> dict: 
     """
     Inspects the \*.yaml file contents if it exists.
     Otherwise it will search for either images with text
     annotations (Darknet) or tfrecord files (TFRecord Dataset).
 
     Parameters
     ----------
@@ -602,24 +673,28 @@
             The validated path to the dataset.
             This can point to a yaml file or a directory containing
             tfrecords or images and text annotations.
 
         labels_path: str
             The path to the labels.txt (if provided).
 
-        polar: bool
-            Specify whether reading polar datasets.
+        local: bool
+            Specify to use the local validator reader instead of 
+            deepview-datasets.
 
     Returns
     -------
-        info_dataset: dict
+        info_dataset: dict, Iterator
             This dictionary contains the paths of the dataset files
             either the tfrecords or the images and the annotation files.
             This dictionary also contains the string labels if it exists.
 
+            This is an object from deepview-datasets that iterates through
+            the dataset, if not specifying the local reader. 
+
     Raises
     ------
         UnsupportedDatasetTypeException
             Raised if the yaml file specifies a dataset type that 
             is not recognized. Can only recognize (darknet or tfrecord).
 
         EmptyDatasetException
@@ -631,39 +706,42 @@
     """
     source = validate_dataset_source(source)
 
     if os.path.isdir(source):
         """Handle AuZoneNet and AuZoneTFRecords format."""
         # Check if a dataset yaml file is inside the directory.
         yaml_file = find_yaml_file(source)
-        if yaml_file: return read_yaml_file(yaml_file)
+        if yaml_file:
+            return read_yaml_file(yaml_file, local)
 
         # Find and read the contents of the labels file.
         labels = find_labels_file(source, labels_path)
                 
         """Handle standard TFRecord datasets."""
         info_dataset = collect_tfrecord_files(source, labels)
         if info_dataset: return info_dataset
 
         """Handle standard Darknet datasets."""
-        info_dataset = collect_darknet_files(source, labels, polar)
+        info_dataset = collect_darknet_files(source, labels, local)
         if info_dataset: return info_dataset
 
         """Handle Arrow datasets."""
-        info_dataset = collect_arrow_files(source, labels, polar)
+        info_dataset = collect_arrow_files(source, labels, local)
         if info_dataset: 
             return info_dataset
         else:
-            raise EmptyDatasetException("info_dataset returned None." + 
-                                     "Check if the path provided contains " + 
-                                     "either tfrecord files or images " +
-                                     "and annotations files.")
+            raise EmptyDatasetException(
+                "info_dataset returned None. " + 
+                f"Check if the path provided ({source}) contains " + 
+                "either tfrecord files or images and annotations files."
+            )
     elif os.path.isfile(source):
         if os.path.splitext(os.path.basename(source))[1] == ".yaml":
-            return read_yaml_file(source)
+            return read_yaml_file(source, local)
+        
         elif os.path.splitext(os.path.basename(source))[1] == ".txt":
             raise NotImplementedError(
                 "Single text file is not currently supported.")
         elif os.path.splitext(source)[1] == ".deepview":
             raise NotImplementedError(
                 "Deepview files are not currently supported.")
         else:
```

## deepview/validator/evaluators/core.py

```diff
@@ -486,15 +486,15 @@
 
         summary_dictionary = {key.lstrip('_'): value for key, value in 
             self.metric_summary.__dict__.items() if key != "_image_summaries"}
         summary_dictionary["confusion_labels"] = self.plot_summary.confusion_labels
         summary_dictionary["confusion_matrix"] = self.plot_summary.confusion_matrix
         summary_dictionary["precision"] = self.plot_summary.precision
         summary_dictionary["recall"] = self.plot_summary.recall
-        summary_dictionary["average_precision"] = self.plot_summary.average_precision
+        summary_dictionary["ap"] = self.plot_summary.average_precision
         summary_dictionary["curve_labels"] = self.plot_summary.curve_labels
 
         with open(self.parameters.json_out, 'w', encoding='utf-8') as fp:
             json.dump(
                 summary_dictionary,
                 fp, 
                 cls=NpEncoder,
```

## deepview/validator/evaluators/detectionevaluator.py

```diff
@@ -24,17 +24,17 @@
 from deepview.validator.evaluators.core import Evaluator
 from deepview.validator.visualize.detectiondraw import (
     draw_2d_bounding_boxes,
     draw_3d_bounding_boxes
 )
 from deepview.validator.datasets import Instance
 from deepview.validator.visualize.utils import (
-    plot_pr_curve,
     plot_classification_detection,
     plot_confusion_matrix,
+    plot_pr_curve,
     figure2numpy,
     close_figures
 )
 from deepview.validator.writers import logger
 from copy import deepcopy
 import numpy as np
 import os
@@ -88,15 +88,15 @@
             val_messenger: TensorBoardWriter
                 This object handles publishing of validation 
                 results into tensorboard.
         """
         if val_messenger is not None:
             self.tensorboard_writer = val_messenger
 
-    def instance_collector(self, labels: list[str] = []):
+    def instance_collector(self, labels: List[str] = []):
         """
         Collects the instances from the ground truth and the model predictions.
 
         Parameters
         ----------
             labels: list
                 This is the unique string labels that can be optionally
@@ -110,15 +110,16 @@
                 This yields one image instance from the ground
                 truth and the model predictions.
         """
         gt_instance: Instance
         for gt_instance in self.dataset.read_all_samples(
             silent=self.parameters.silent):
 
-            if os.path.splitext(self.runner.model)[1].lower() != "":
+            if (os.path.splitext(self.runner.model)[1].lower() != "" or 
+                self.runner.loaded_model is not None):
                 image = gt_instance.image
             # For offline runners, only the path to the image is needed.
             else:
                 image = gt_instance.image_path
 
             detections = self.runner.run_single_instance(image)
 
@@ -183,25 +184,33 @@
                 This object contains the detection metrics for 
                 this particular image.
         """
         gt_instance: Instance = instances.get("gt_instance")
         dt_instance: Instance = instances.get("dt_instance")
 
         # Store the ground truth and prediction instances per image.
-        self.collected_instances.append_gt_instance(gt_instance)
-        self.collected_instances.append_dt_instance(dt_instance)
+        # Too resource intensive for the EVK.
+        # self.collected_instances.append_gt_instance(gt_instance)
+        # self.collected_instances.append_dt_instance(dt_instance)
 
         image_summary = detection_evaluate(
             gt_instance,
             dt_instance,
             self.parameters,
             self.data_collection,
             self.plot_summary
         )
-        self.metric_summary.append_image_summary(image_summary)
+        self.metric_summary.add_ground_truths(image_summary.ground_truths)
+        self.metric_summary.store_centers(
+            gt_centers=image_summary.centers.get("gt_centers"),
+            dt_centers=image_summary.centers.get("dt_centers"),
+            center_distances=image_summary.centers.get("center_distances")
+        )
+        # Too resource intensive for the EVK, add_ground_truths is also inside the method below.
+        # self.metric_summary.append_image_summary(image_summary)
 
         if add_image:
             if self.parameters.visualize or self.tensorboard_writer:
                 image = self.drawer(
                     gt_instance,
                     dt_instance,
                     image_summary,
@@ -308,40 +317,19 @@
             if self.parameters.visualize:
                 self.save_metrics_disk(header, format_summary, format_timings)
         
         metric_summary_copy = deepcopy(self.metric_summary)
         self.reset()
         return metric_summary_copy
 
-    def get_plots(self) -> list[matplotlib.figure.Figure]:
+    def get_plots(self) -> List[matplotlib.figure.Figure]:
         """
         Creates Matplotlib figures based on the plot data gathered
         during validation.
 
-        Parameters
-        ----------
-            confusion_matrix: (nxn) np.ndarray
-                This is a table where the rows represents the predictions 
-                and the columns represents the ground truths. 
-
-            precision_recall_data: dict
-                The following container is formatted as follows:
-
-                .. code-block:: python
-
-                    {
-                        "precision": precision (nc, score thresholds),
-                        "recall": recall (nc, score thresholds),
-                        "average precision": average precision (nc, iou thresholds)
-                        "names": unique labels 
-                    }
-
-            unique_labels: ;ost
-                These are the unique labels needed for the confusion matrix.
-
         Returns
         -------
             plots: list
                 This contains matplotlib figures of the plots. 
         """
         fig_class_metrics = plot_classification_detection(
             self.plot_summary.class_histogram_data, self.metric_summary.model)
@@ -355,15 +343,15 @@
             self.plot_summary.precision,
             self.plot_summary.recall,
             self.plot_summary.average_precision,
             self.plot_summary.curve_labels,
             self.metric_summary.model)
         return [fig_class_metrics, fig_confusion_matrix, fig_prec_rec_curve]
 
-    def save_plots_disk(self, plots: list[matplotlib.figure.Figure]):
+    def save_plots_disk(self, plots: List[matplotlib.figure.Figure]):
         """
         Saves the validation plots as an image in the local machine.
 
         Parameters
         ----------
             plots: list
                     This contains matplotlib figures of the plots.
```

## deepview/validator/evaluators/parameters.py

```diff
@@ -7,14 +7,15 @@
 # Modifying or copying any source code is explicitly forbidden.
 
 from deepview.validator.exceptions import UnsupportedNormalizationException
 from deepview.validator.exceptions import UnsupportedBoxFormatException
 from deepview.validator.exceptions import UnsupportedEngineException
 from deepview.validator.exceptions import UnsupportedNMSException
 from deepview.validator.metrics.detectionutils import clamp
+from typing import Union
 import os
 
 class Parameters:
     """
     Default initialization parameters provided are based on the model
     parameters. Other parameters included are for validation specifications.
 
@@ -63,15 +64,15 @@
             The maximum number of detections to output per image. 
     """
 
     def __init__(
         self,
         validation_iou: float = 0.50,
         detection_iou: float = 0.50,
-        validation_score: float = 0.50,
+        validation_score: float = 0.00,
         detection_score: float = 0.50,
         engine: str = "npu",
         nms: str = "fast",
         normalization: str = "raw",
         box_format: str = "xyxy",
         warmup: int = 0,
         label_offset: int = 0,
@@ -98,14 +99,17 @@
         self._visualize = None
         self._tensorboard = None
         self._json_out = None
         self._rematching = True
         self._iou_first = True
         self._silent = False
         self._leniency_factor=2
+        self._letterbox = False
+        self._auto_offset = True
+        self._class_filter = False
 
     @property
     def validation_iou(self) -> float:
         """
         Attribute to access the validation iou. 
         This metric is used to classify if matched predictions will
         be considered as localization FPs if IoUs are below this threshold.
@@ -215,15 +219,15 @@
         Returns
         -------
             :py:class:str: The engine type.
         """
         return self._engine
 
     @engine.setter
-    def engine(self, this_engine: str | None):
+    def engine(self, this_engine: Union[str, None]):
         """
         Sets the engine type.
 
         Parameters
         ----------
             this_engine: str
                 The engine to set.
@@ -231,15 +235,15 @@
         Raises
         ------
             UnsupportedEngineException
                 Raised if the passed engine is not recognized.
         """
         if this_engine is not None:
             this_engine = this_engine.lower()
-            if this_engine not in ['npu', 'cpu', 'gpu']:
+            if this_engine not in ['npu', 'cpu', 'gpu', 'cuda', 'deepviewrt', 'hailo']:
                 raise UnsupportedEngineException(this_engine)
         self._engine = this_engine
 
     @property
     def nms(self) -> str:
         """
         Attribute to access the NMS type. 
@@ -249,15 +253,15 @@
         Returns
         -------
             :py:class:str: The NMS type.
         """
         return self._nms
 
     @nms.setter
-    def nms(self, this_nms: str | None):
+    def nms(self, this_nms: Union[str, None]):
         """
         Sets the NMS type.
 
         Parameters
         ----------
             this_nms: str
                 The NMS to set.
@@ -265,15 +269,15 @@
         Raises
         ------
             UnsupportedNMSException
                 Raised if the NMS provided is not recognized.
         """
         if this_nms is not None:
             this_nms = this_nms.lower()
-            if this_nms not in ['standard', 'fast', 'matrix', 'tensorflow']:
+            if this_nms not in ['standard', 'fast', 'matrix', 'tensorflow', 'torch']:
                 raise UnsupportedNMSException(this_nms)
         self._nms = this_nms
 
     @property
     def normalization(self) -> str:
         """
         Attribute to access the image normalization type. 
@@ -284,15 +288,15 @@
         Returns
         -------
             :py:class:str: The normalization type.
         """
         return self._normalization
 
     @normalization.setter
-    def normalization(self, norm: str | None):
+    def normalization(self, norm: Union[str, None]):
         """
         Sets the normalization type.
 
         Parameters
         ----------
             norm: str
                 The normalization to set.
@@ -318,15 +322,15 @@
         Returns
         -------
             :py:class:str: The box format type.
         """
         return self._box_format
 
     @box_format.setter
-    def box_format(self, this_box_format: str | None):
+    def box_format(self, this_box_format: Union[str, None]):
         """
         Sets the box format type.
 
         Parameters
         ----------
             this_box_format: str
                 The box format to set.
@@ -807,8 +811,93 @@
         box to box center distance does not exceed the leniency factor.
 
         Parameters
         ----------
             this_leniency_factor: int
                 The leniency_factor to set.
         """
-        self._leniency_factor = this_leniency_factor
+        self._leniency_factor = this_leniency_factor
+
+    @property
+    def letterbox(self) -> bool:
+        """
+        Attribute to access letterbox condition. 
+        Specify whether to preprocess images using letterbox transformations
+        rather than image resizing.
+        Can only be set to :py:class:bool.
+
+        Returns
+        -------
+            :py:class:bool: Condition to specify letterbox image preprocessing.
+        """
+        return self._letterbox
+
+    @letterbox.setter
+    def letterbox(self, this_letterbox: bool):
+        """
+        Specify whether to preprocess images using letterbox transformations
+        rather than image resizing.
+
+        Parameters
+        ----------
+            this_letterbox: bool
+                Condition to specify letterbox image preprocessing.
+        """
+        self._letterbox = this_letterbox
+
+    @property
+    def auto_offset(self) -> bool:
+        """
+        Attribute to access auto offset condition. 
+        Specify whether to enable auto offset of the model
+        indices based on the model output shape and the ground truth labels.
+        Can only be set to :py:class:bool.
+
+        Returns
+        -------
+            :py:class:bool: Condition to specify the auto offset property.
+        """
+        return self._auto_offset
+
+    @auto_offset.setter
+    def auto_offset(self, this_auto_offset: bool):
+        """
+        Specify whether to enable auto offset of the model
+        indices based on the model output shape and the ground truth labels.
+
+        Parameters
+        ----------
+            this_auto_offset: bool
+                Condition to specify auto offset property
+        """
+        self._auto_offset = this_auto_offset
+
+    @property
+    def class_filter(self) -> bool:
+        """
+        Attribute to access the class filter condition. 
+        Specify to filter the classes from the model detections to allow
+        only the classes present in the ground truth dataset.
+        Requires that the model detections has more classes than the 
+        ground truth dataset.
+        Can only be set to :py:class:bool.
+
+        Returns
+        -------
+            :py:class:bool: Condition to specify the class filter property.
+        """
+        return self._class_filter
+
+    @class_filter.setter
+    def class_filter(self, this_class_filter: bool):
+        """
+        Specify to filter the classes from the model detections to allow
+        only the classes present in the ground truth dataset.
+        Requires that the model detections has more classes than the 
+        ground truth dataset.
+
+        Parameters
+        ----------
+            this_class_filter: bool
+                Condition to specify class_filter property
+        """
+        self._class_filter = this_class_filter
```

## deepview/validator/evaluators/poseevaluator.py

```diff
@@ -28,37 +28,22 @@
 
 class PoseEval(Evaluator):
     """
     Performs pose evaluation for headpose models.
 
     Parameters
     ----------
-        runner: Runner object
-            This provides methods for models to generate predictions.
+        runner: Type[Runner]
+            This object provides methods to run the pose model.
 
-        dataset: Dataset object
-            This provides methods to read and parse a provided dataset.
+        dataset: Type[Dataset]
+            This object provides methods to read and parse the dataset.
 
-        visualize: str
-            The path to store images with visualizations.
-
-        tensorboard: str
-            The path to store the tfevents file that contain results of the
-            validation.
-
-        json_out: str
-            The path to store a JSON file containing the validation summary.
-
-        display: int
-            The number of images to display or save on disk.
-
-        parameters: dict
-            The model parameters.
-            See README.md (Method Parameters Format) for more information.
-            This does not apply to pose, therefore it is set as None.
+        parameters: Parameters
+            This contains the validation parameters set from the command line.
     """
     def __init__(
         self,
         parameters: Parameters,
         runner: Type[Runner] = None,
         dataset: Type[Dataset] = None,
     ):
@@ -224,14 +209,17 @@
 
         metrics = PoseMetrics(
             self.data_collection,
             self.metric_summary
         )
         metrics.run_metrics()
 
+        if self.parameters.json_out:
+            self.save_json_summary()
+
         if self.tensorboard_writer:
             self.publish_metrics(epoch, validation_type="pose")
         else:
             header, format_summary, format_timings = self.console_writer(
                 summary=self.metric_summary,
                 parameters=self.parameters,
                 validation_type="pose")
```

## deepview/validator/evaluators/utils.py

```diff
@@ -9,30 +9,30 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING, Union
 if TYPE_CHECKING:
     from deepview.validator.evaluators import Parameters
     from deepview.validator.metrics import PlotSummary
     from deepview.validator.datasets import Instance
     from deepview.validator.metrics import (
+        SegmentationDataCollection,
         DetectionDataCollection, 
-        SegmentationDataCollection
     )
 
 from deepview.validator.metrics.detectionmatch import MatchDetections
 from deepview.validator.metrics.summary import ImageSummary
 from deepview.validator.metrics.segmentationutils import (
-    create_mask_class, 
     create_mask_background, 
+    create_mask_class, 
     classify_mask
 )
 from deepview.validator.metrics.detectionutils import (
-    filter_dt, 
-    clamp_boxes, 
     ignore_boxes, 
-    get_corners
+    clamp_boxes, 
+    get_corners,
+    filter_dt
 )
 from deepview.validator.datasets.utils import resize
 from copy import deepcopy
 import numpy as np
 import os
 
 def detection_evaluate(
```

## deepview/validator/metrics/detectiondata.py

```diff
@@ -3,15 +3,15 @@
 # Unauthorized copying of this file, via any medium is strictly prohibited
 # Proprietary and confidential.
 #
 # This source code is provided solely for runtime interpretation by Python.
 # Modifying or copying any source code is explicitly forbidden.
 
 from __future__ import annotations
-from typing import TYPE_CHECKING, Union
+from typing import TYPE_CHECKING, Union, List, Tuple
 if TYPE_CHECKING:
     from deepview.validator.metrics import DetectionLabelData
 
 from deepview.validator.metrics.detectionutils import clamp
 import numpy as np
 
 class DetectionLabelData:
@@ -99,29 +99,29 @@
         ----------
             gts: int
                 The number of ground truths to add.
         """
         self._ground_truths += gts
 
     @property
-    def tps(self) -> list[tuple[float, float]]:
+    def tps(self) -> List[Tuple[float, float]]:
         """
         Attribute to access the true positives data.
         Can only be set to :py:class:`list`
 
         Returns
         -------
             :py:class:`list`
                 This contains the (IoU, score) of each 
                 true positive for this label.
         """
         return self._tps
 
     @tps.setter
-    def tps(self, this_tps: list[tuple[float, float]]):
+    def tps(self, this_tps: List[Tuple[float, float]]):
         """
         Sets the true positives data to a new value.
 
         Parameters
         ----------
             this_tps: :py:class:`list`
                 These are true positives data to set.
@@ -192,29 +192,29 @@
         if len(self.tps):
             tp_iou = np.array(self.tps)[:, 0] >= iou_threshold
             tp_score = np.array(self.tps)[:, 1] >= score_threshold
             return np.count_nonzero(tp_iou * tp_score)
         return 0
 
     @property
-    def class_fps(self) -> list[tuple[float, float]]:
+    def class_fps(self) -> List[Tuple[float, float]]:
         """
         Attribute to access the classification false positives data.
         Can only be set to :py:class:`list`
 
         Returns
         -------
             :py:class:`list`
                 This contains the (IoU, score) of each classification
                 false positive for this label.
         """
         return self._class_fps
 
     @class_fps.setter
-    def class_fps(self, this_class_fps: list[tuple[float, float]]):
+    def class_fps(self, this_class_fps: List[Tuple[float, float]]):
         """
         Sets the classification false positives data to a new value.
 
         Parameters
         ----------
             this_class_fps: :py:class:`list`
                 These are classification false positives data to set.
@@ -287,29 +287,29 @@
         if len(self.class_fps):
             fp_iou = np.array(self.class_fps)[:, 0] >= iou_threshold
             fp_score = np.array(self.class_fps)[:, 1] >= score_threshold
             return np.count_nonzero(fp_iou * fp_score)
         return 0
 
     @property
-    def local_fps(self) -> list[float]:
+    def local_fps(self) -> List[float]:
         """
         Attribute to access the localization false positives data.
         Can only be set to :py:class:`list`
 
         Returns
         -------
             :py:class:`list`
                 This contains the score of each localization
                 false positive for this label.
         """
         return self._local_fps
 
     @local_fps.setter
-    def local_fps(self, this_local_fps: list[float]):
+    def local_fps(self, this_local_fps: List[float]):
         """
         Sets the localization false positives data to a new value.
 
         Parameters
         ----------
             this_local_fps: :py:class:`list`
                 These are localization false positives data to set.
@@ -482,28 +482,28 @@
         self.tp = []
         self.conf = []
         self.pred_cls = []  # classes of detections
         self.target_cls = []  # classes of ground truths\
         self.ious = [0.5, 0.55, 0.60, 0.65, 0.70, 0.75, 0.8, 0.85, 0.9, 0.95]
 
     @property
-    def label_data_list(self) -> list[DetectionLabelData]:
+    def label_data_list(self) -> List[DetectionLabelData]:
         """
         Attribute to access the list containing DetectionLabelData objects
         Can only be set to :py:class:`list`
 
         Returns
         -------
             :py:class:`list`
                 This contains the DetectionLabelData objects.
         """
         return self._label_data_list
 
     @label_data_list.setter
-    def label_data_list(self, label_datas: list[DetectionLabelData]):
+    def label_data_list(self, label_datas: List[DetectionLabelData]):
         """
         Sets the list of DetectionLabelData objects.
 
         Parameters
         ----------
             label_datas: :py:class:`list`
                 This is the list of DetectionLabelData objects to set.
```

## deepview/validator/metrics/detectionmatch.py

```diff
@@ -3,28 +3,28 @@
 # Unauthorized copying of this file, via any medium is strictly prohibited
 # Proprietary and confidential.
 #
 # This source code is provided solely for runtime interpretation by Python.
 # Modifying or copying any source code is explicitly forbidden.
 
 from __future__ import annotations
-from typing import TYPE_CHECKING, Union
+from typing import TYPE_CHECKING, Union, List
 if TYPE_CHECKING:
     from deepview.validator.metrics import ImageSummary, PlotSummary
     from deepview.validator.metrics import DetectionDataCollection
     from deepview.validator.evaluators import Parameters
     from deepview.validator.datasets import Instance
 
 from deepview.validator.exceptions import MatchingAlgorithmException
 from deepview.validator.metrics.detectionutils import (
-    iou_2d,
-    iou_3d,
     minkowski_distance,
     localize_distance,
-    get_center_point
+    get_center_point,
+    iou_2d,
+    iou_3d,
 )
 import numpy as np
 
 class MatchDetections:
     """
     The purpose of this class is to match the model detections
     to the ground truth based on congruent labels and the highest
@@ -170,82 +170,82 @@
                 These is the predictions list. This either contains
                 bounding boxes if 2D validation or 3D box corners if
                 3D validation. 
         """
         self._predictions = this_predictions
 
     @property
-    def index_matches(self) -> list[list[int, int]]:
+    def index_matches(self) -> List[List[int, int]]:
         """
         Attribute to access the index_matches. This contains the indices
         of the ground truth and the predictions that are matched in the format
         [[gti, dti], [gti, dti], ...].
         Can be set to :py:class:`list`
 
         Returns
         -------
             :py:class:`list` 
                 The indices of the matched ground truth and the predictions.
         """
         return self._index_matches
 
     @index_matches.setter
-    def index_matches(self, this_index_matches: list[list[int, int]]):
+    def index_matches(self, this_index_matches: List[List[int, int]]):
         """
         Sets the index_matches.
 
         Parameters
         ----------
             this_index_matches: :py:class:`list` 
                 These is the index_matches.
         """
         self._index_matches = this_index_matches
 
     @property
-    def index_unmatched_dt(self) -> list[int]:
+    def index_unmatched_dt(self) -> List[int]:
         """
         Attribute to access the index_unmatched_dt. This contains the indices
         of the predictions that were unmatched.
         Can be set to :py:class:`list`
 
         Returns
         -------
             :py:class:`list` 
                 The indices of the unmatched predictions.
         """
         return self._index_unmatched_dt
 
     @index_unmatched_dt.setter
-    def index_unmatched_dt(self, this_index_unmatched_dt: list[int]):
+    def index_unmatched_dt(self, this_index_unmatched_dt: List[int]):
         """
         Sets the index_unmatched_dt.
 
         Parameters
         ----------
             this_index_unmatched_dt: :py:class:`list` 
                 The indices of the unmatched predictions.
         """
         self._index_unmatched_dt = this_index_unmatched_dt
 
     @property
-    def index_unmatched_gt(self) -> list[int]:
+    def index_unmatched_gt(self) -> List[int]:
         """
         Attribute to access the index_unmatched_gt. This contains the indices
         of the ground truths that were unmatched.
         Can be set to :py:class:`list`
 
         Returns
         -------
             :py:class:`list` 
                 The indices of the unmatched ground truths.
         """
         return self._index_unmatched_gt
 
     @index_unmatched_gt.setter
-    def index_unmatched_gt(self, this_index_unmatched_gt: list[int]):
+    def index_unmatched_gt(self, this_index_unmatched_gt: List[int]):
         """
         Sets the index_unmatched_gt.
 
         Parameters
         ----------
             this_index_unmatched_gt: :py:class:`list` 
                 The indices of the unmatched ground truths.
@@ -330,43 +330,44 @@
                     self.store_metric(gt, dt, gti, dti)
 
             idx = np.argsort(self.iou_grid, axis=None)[::-1]
             for i in idx:
                 dti = i // self.iou_grid.shape[0]
                 gti = i % self.iou_grid.shape[0]
                 match_iou = self.iou_grid[gti, dti]
-                if (match_iou > self.parameters.validation_iou
-                    and dti in self.index_unmatched_dt
-                        and gti in self.index_unmatched_gt):
+                if (match_iou > 0 and 
+                    dti in self.index_unmatched_dt and
+                    gti in self.index_unmatched_gt):
                     self.index_matches.append((dti, gti))
                     self.iou_list[dti] = match_iou
                     self.index_unmatched_dt.remove(dti)
                     self.index_unmatched_gt.remove(gti)
             return
         for gti, gt in enumerate(self.ground_truths):
             # A list of prediction indices with 
             # matching labels as the ground truth.
             dti_reflective, iou_reflective = list(), list()
+            gt_label = self.gt_instance.labels[gti]
 
             for dti, dt in enumerate(self.predictions):
                 self.store_metric(gt, dt, gti, dti)
-
-                gt_label = self.gt_instance.labels[gti]
+                
                 dt_label = self.dt_instance.labels[dti]
-
                 if dt_label == gt_label:
                     dti_reflective.append(dti)
                     iou_reflective.append(self.iou_grid[gti][dti])
-
+            
             # A potential match is the detection that produced the highest IoU.
             dti = np.argmax(self.iou_grid[gti])
             iou = max(self.iou_grid[gti])
-            if iou < self.parameters.validation_iou:
+            # If there is no intersection, it cannot be a match.
+            if iou < 0:
                 continue
-            if len(dti_reflective) and dt_label != gt_label:
+            # Only match if the IoU between matching ground truth and detection labels > 0.
+            if len(dti_reflective) and max(iou_reflective) >= self.parameters.validation_iou:
                 # The IoU of the detections with the same labels
                 # as the ground truth. A potential match is the
                 # detection with the same label as the ground truth.
                 dti = dti_reflective[np.argmax(iou_reflective)]
                 iou = max(iou_reflective)
             self.compare_matches(dti, gti, iou)
 
@@ -411,26 +412,26 @@
                 self.iou_list[dti] = iou
                 self.index_matches.append((dti, gti))
 
                 # Rematch pre_gti
                 self.iou_grid[pre_gti][dti] = 0.
                 dti = np.argmax(self.iou_grid[pre_gti])
                 iou = max(self.iou_grid[pre_gti])
-                if iou > self.parameters.validation_iou and self.parameters.rematching:
+                if iou > 0 and self.parameters.rematching:
                     self.compare_matches(dti, pre_gti, iou)
             else:
                 # Rematch gti
                 self.iou_grid[gti][dti] = 0.
                 dti = np.argmax(self.iou_grid[gti])
                 iou = max(self.iou_grid[gti])
-                if iou > self.parameters.validation_iou and self.parameters.rematching:
+                if iou > 0 and self.parameters.rematching:
                     self.compare_matches(dti, gti, iou)
 
         elif len(twice_matched) == 0:
-            if iou > self.parameters.validation_iou:
+            if iou > 0:
                 self.iou_list[dti] = iou
                 self.index_matches.append((dti, gti))
         else:
             raise MatchingAlgorithmException(
                 "Duplicate matches were unchecked.")
 
     def store_metric_all(self, eps: float=1e-7): #NOSONAR
@@ -662,19 +663,21 @@
 
             self.store_matched_centers(match)
             if self.verbose_store:
                 self.store_matches(match)
                 if score >= self.parameters.validation_score:
                     if iou >= self.parameters.validation_iou:
                         self.store_confusion_data(gt_label, dt_label)
+                    # This would become either a localization false positive or
+                    # false negative.
                     else:
                         self.store_confusion_data("background", dt_label)
                         self.store_confusion_data(gt_label, "background")
 
-    def store_matches(self, match: list[int, int]):
+    def store_matches(self, match: List[int, int]):
         """
         Stores a verbose information about the matches in the image summary.
         This includes the bounding box, iou, score of the matches.
 
         Parameters
         ----------
             match: list
@@ -737,24 +740,33 @@
         ----------
             match: list
                 This includes the index of the match 
                 [detection index, ground truth index].
         """
         score = self.dt_instance.scores[match[0]]
         iou = self.iou_list[match[0]]
+        dt_center, gt_center = None, None
 
         # Stores the centerpoint coordinates in the image summary
         if (len(self.dt_instance.centers) > 0 and 
             len(self.gt_instance.centers) > 0):
             dt_center = self.dt_instance.centers[match[0]]
             gt_center = self.gt_instance.centers[match[1]]
 
             if (score >= self.parameters.validation_score and 
                 iou >= self.parameters.validation_iou):
-                self.image_summary.append_centers(gt_center, dt_center)
+                self.image_summary.append_centers(gt_center, dt_center)      
+        else:
+            if self.parameters.metric == "centerpoint":
+                dt_center = get_center_point(self.dt_instance.boxes[match[0]])
+                gt_center = get_center_point(self.gt_instance.boxes[match[1]])
+
+                if (score >= self.parameters.validation_score and 
+                    iou >= self.parameters.validation_iou):
+                    self.image_summary.append_centers(gt_center, dt_center)
 
     def classify_extras(self):
         """
         Classifies the extra predictions into localization false positives. 
         """
         for extra in self.index_unmatched_dt:
             dt_label = self.dt_instance.labels[extra]
@@ -861,8 +873,12 @@
         ----------
             gt_label: str or int
                 This is the ground truth label.
 
             dt_label: str, int
                 This is the detection label.
         """
+        if isinstance(gt_label, np.ndarray):
+            gt_label = gt_label[0]
+        if isinstance(dt_label, np.ndarray):
+            dt_label = dt_label[0]
         self.plot_summary.append_confusion_matrix_data((gt_label, dt_label))
```

## deepview/validator/metrics/detectionmetrics.py

```diff
@@ -5,28 +5,24 @@
 #
 # This source code is provided solely for runtime interpretation by Python.
 # Modifying or copying any source code is explicitly forbidden.
 
 from __future__ import annotations
 from typing import TYPE_CHECKING, Tuple
 if TYPE_CHECKING:
+    from deepview.validator.metrics import PlotSummary, MetricSummary
     from deepview.validator.datasets import InstanceCollection
     from deepview.validator.evaluators import Parameters
     from deepview.validator.metrics import (
-        ImageSummary, PlotSummary, MetricSummary)
-    from deepview.validator.metrics import (
         DetectionDataCollection,
         DetectionLabelData
     )
-
+    
+from deepview.validator.metrics.detectionutils import nan_to_last_num
 from deepview.validator.evaluators.utils import detection_evaluate
-from deepview.validator.metrics.detectionutils import (
-    minkowski_distance,
-    nan_to_last_num
-)
 from deepview.validator.metrics.core import Metrics
 import numpy as np
 
 class DetectionMetrics(Metrics):
     """
     Provides methods to calculate::
 
@@ -118,47 +114,35 @@
                         {
                             "x-center-mae": "mean absolute error of the x-coordinate",
                             "y-center-mae": "mean absolute error of the y-coordinate",
                             "z-center-mae": "mean absolute error of the z-coordinate",
                             "distance-mae": "mean absolute error of the center distances"
                         }  
         """
-        center_distances = list()
-        complete_dt_centers, complete_gt_centers = list(), list()
         distance_metrics = {
             "x-center-mae": np.nan,
             "y-center-mae": np.nan,
             "z-center-mae": np.nan,
             "distance-mae": np.nan,
         }
+        center_distances = self.metric_summary.centers.get("center_distances")
+        gt_centers = np.array(self.metric_summary.centers.get("gt_centers"))
+        dt_centers = np.array(self.metric_summary.centers.get("dt_centers"))
 
-        # Collect the centers from each image.
-        image_summary: ImageSummary
-        for image_summary in self.metric_summary.image_summaries:
-            gt_centers = image_summary.centers.get("gt_centers")
-            dt_centers = image_summary.centers.get("dt_centers")
-
-            if len(gt_centers) + len(dt_centers) > 0:
-                for gt_center, dt_center in zip(gt_centers, dt_centers):
-                    if len(gt_center) + len(dt_center) > 0:
-                        center_distances.append(
-                            minkowski_distance(dt_center, gt_center))
-                        complete_gt_centers += [list(gt_center)]
-                        complete_dt_centers += [list(dt_center)]
-
-        gt_centers, dt_centers = np.array(
-            complete_gt_centers), np.array(complete_dt_centers)
-        if len(gt_centers) + len(dt_centers) != 0:
+        if len(gt_centers) + len(dt_centers) > 0:
             self.metric_summary.append_centers = True
             x_mae = self.mean_absolute_error(
                 gt_centers[:, 0:1], dt_centers[:, 0:1])
             y_mae = self.mean_absolute_error(
                 gt_centers[:, 1:2], dt_centers[:, 1:2])
-            z_mae = self.mean_absolute_error(
-                gt_centers[:, 2:3], dt_centers[:, 2:3])
+            if (gt_centers.shape[1] > 2 or dt_centers.shape[1] > 2):
+                z_mae = self.mean_absolute_error(
+                    gt_centers[:, 2:3], dt_centers[:, 2:3])
+            else:
+                z_mae = np.nan
             distance_mae = sum(center_distances)/len(gt_centers)
 
             distance_metrics = {
                 "x-center-mae": x_mae,
                 "y-center-mae": y_mae,
                 "z-center-mae": z_mae,
                 "distance-mae": distance_mae
@@ -641,17 +625,17 @@
                     mars[ic][it] = class_metrics[1]
                     maccs[ic][it] = class_metrics[2]
                     # This mAP computation is the average of the precision 
                     # of each class.
                     # maps[ic][it] = class_metrics[0] #NOSONAR
 
             mean_metrics = self.get_mean_average_metrics(maps, mars, maccs, nc)
-            self.metric_summary.map = {"0.50": ap50.mean(),
-                                       "0.75": ap75.mean(),
-                                       "0.50:0.95": ap.mean()}
+            self.metric_summary.map = {"0.50": 0.0 if np.isnan(ap50.mean()) else ap50.mean(),
+                                       "0.75": 0.0 if np.isnan(ap75.mean()) else ap75.mean(),
+                                       "0.50:0.95": 0.0 if np.isnan(ap.mean()) else ap.mean()}
             self.metric_summary.mar = {"0.50": mean_metrics[1][0],
                                        "0.75": mean_metrics[1][1],
                                        "0.50:0.95": mean_metrics[1][2]}
             self.metric_summary.macc = {"0.50": mean_metrics[2][0],
                                         "0.75": mean_metrics[2][1],
                                         "0.50:0.95": mean_metrics[2][2]}
 
@@ -735,15 +719,15 @@
         nc = unique_classes.shape[0]  # number of classes, number of detections
 
         # Create Precision-Recall curve and compute AP for each class
         px, py = np.linspace(0, 1, 1000), []  # for plotting
         ap, p, r = np.zeros((nc, 10)), np.zeros(
             (nc, 1000)), np.zeros((nc, 1000))
         for ci, c in enumerate(unique_classes):
-            i = pred_cls == c
+            i = np.nonzero(pred_cls == c)[0]
             n_l = nt[ci]  # number of labels
             n_p = i.sum()  # number of predictions
             if n_p == 0 or n_l == 0:
                 continue
 
             # Accumulate FPs and TPs
             fpc = (1 - tp[i]).cumsum(0)
```

## deepview/validator/metrics/detectionutils.py

```diff
@@ -208,14 +208,17 @@
     ----------
         box_a: list or np.ndarray
             This is a bounding box [xmin, ymin, xmax, ymax].
         
         box_b: list or np.ndarray
             This is a bounding box [xmin, ymin, xmax, ymax].
 
+        eps: float
+            Avoids division by zero errors.
+
     Returns
     -------
         IoU: float
             The IoU score between boxes.
 
     Exceptions
     ----------
@@ -317,14 +320,17 @@
     ----------
         box1: (Tensor[N, 4])
             Bounding boxes array.
 
         box2: (Tensor[M, 4])
             Bounding boxes array.
 
+        eps: float
+            Avoids division by zero errors.
+
     Returns
     --------
         iou: (Tensor[N, M]) 
             The NxM matrix containing the pairwise IoU values for every 
             element in boxes1 and boxes2.
     """
     # https://github.com/pytorch/vision/blob/master/torchvision/ops/boxes.py
```

## deepview/validator/metrics/posedata.py

```diff
@@ -2,15 +2,15 @@
 #
 # Unauthorized copying of this file, via any medium is strictly prohibited
 # Proprietary and confidential.
 #
 # This source code is provided solely for runtime interpretation by Python.
 # Modifying or copying any source code is explicitly forbidden.
 
-from typing import Union
+from typing import Union, List
 import numpy as np
 
 class PoseLabelData:
     """
     This is a container of angles for one specific angle 
     for both prediction and ground truth. An angle could be either yaw, 
     pitch, or roll.
@@ -49,28 +49,28 @@
         ----------
             this_label: str or int
                 The label being represented in this container.
         """
         self._label = this_label
 
     @property
-    def y_true(self) -> list[float]:
+    def y_true(self) -> List[float]:
         """
         Attribute to access the ground truth angles.
         Can only be set to :py:class:`list`
 
         Returns
         -------
             :py:class:`list`
                 This contains the ground truth angles.
         """
         return self._y_true
     
     @y_true.setter
-    def y_true(self, this_y_true: list[float]):
+    def y_true(self, this_y_true: List[float]):
         """
         Sets the ground truth angles to a new value.
 
         Parameters
         ----------
             this_y_true: :py:class:`list`
                 These are ground truth angles to set.
@@ -85,28 +85,28 @@
         ----------
             angle: float
                 The ground truth angle.
         """
         self._y_true.append(angle)
 
     @property
-    def y_pred(self) -> list[float]:
+    def y_pred(self) -> List[float]:
         """
         Attribute to access the prediction angles.
         Can only be set to :py:class:`list`
 
         Returns
         -------
             :py:class:`list`
                 This contains the prediction angles.
         """
         return self._y_pred
     
     @y_pred.setter
-    def y_pred(self, this_y_pred: list[float]):
+    def y_pred(self, this_y_pred: List[float]):
         """
         Sets the prediction angles to a new value.
 
         Parameters
         ----------
             this_y_pred: :py:class:`list`
                 These are prediction angles to set.
@@ -138,28 +138,28 @@
     """
     def __init__(self) -> None:
         
         self._pose_data_list = list()
         self._angle_names = list()
 
     @property
-    def pose_data_list(self) -> list[PoseLabelData]:
+    def pose_data_list(self) -> List[PoseLabelData]:
         """
         Attribute to access the list containing PoseLabelData objects
         Can only be set to :py:class:`list`
 
         Returns
         -------
             :py:class:`list`
                 This contains the PoseLabelData objects.
         """
         return self._pose_data_list
     
     @pose_data_list.setter
-    def pose_data_list(self, pose_datas: list[PoseLabelData]):
+    def pose_data_list(self, pose_datas: List[PoseLabelData]):
         """
         Sets the list of PoseLabelData objects.
 
         Parameters
         ----------
             pose_datas: :py:class:`list`
                 This is the list of PoseLabelData objects to set.
@@ -175,15 +175,15 @@
             label: str or int
                 The angle label to place as a data container. 
                 Can be either 'roll', 'pitch', or 'yaw'.
         """
         self._pose_data_list.append(PoseLabelData(label))
 
     def get_pose_data(
-            self, label: Union[str, int, np.integer]) -> PoseLabelData | None:
+            self, label: Union[str, int, np.integer]) -> Union[PoseLabelData, None]:
         """
         Grabs the PoseLabelData object by label.
         
         Parameters
         ----------
             label: str or int
                 The name of the angle.
```

## deepview/validator/metrics/posemetrics.py

```diff
@@ -21,14 +21,17 @@
     detection and ground truth for pose angles.
 
     Parameters
     ----------
         data_collection: PoseDataCollection
             This is a container for the prediction and 
             the ground truth angles.
+        
+        metric_summary: MetricSummary
+            Contains the metrics calculated.
     """
     def __init__(
             self, 
             data_collection: PoseDataCollection,
             metric_summary: MetricSummary
         ):
         super(PoseMetrics, self).__init__()
```

## deepview/validator/metrics/segmentationdata.py

```diff
@@ -2,15 +2,15 @@
 #
 # Unauthorized copying of this file, via any medium is strictly prohibited
 # Proprietary and confidential.
 #
 # This source code is provided solely for runtime interpretation by Python.
 # Modifying or copying any source code is explicitly forbidden.
 
-from typing import Union
+from typing import Union, List
 import numpy as np
 
 class SegmentationLabelData:
     """
     Acts a container that stores the total number of true predictions and
     false predictions for a specific label.
 
@@ -243,28 +243,28 @@
     def __init__(self):
         # A list containing the SegmentationDataLabel objects for each label.
         self._label_data_list = list()
         # A list containing the strings of unique labels.
         self.labels = list()
 
     @property
-    def label_data_list(self) -> list[SegmentationLabelData]:
+    def label_data_list(self) -> List[SegmentationLabelData]:
         """
         Attribute to access the list containing SegmentationLabelData objects
         Can only be set to :py:class:`list`
 
         Returns
         -------
             :py:class:`list`
                 This contains the SegmentationLabelData objects.
         """
         return self._label_data_list
 
     @label_data_list.setter
-    def label_data_list(self, label_datas: list[SegmentationLabelData]):
+    def label_data_list(self, label_datas: List[SegmentationLabelData]):
         """
         Sets the list of SegmentationLabelData objects.
 
         Parameters
         ----------
             label_datas: :py:class:`list`
                 This is the list of SegmentationLabelData objects to set.
@@ -281,15 +281,15 @@
                 The string label or the integer index to place as a data container.
         """
         self.label_data_list.append(SegmentationLabelData(label))
 
     def get_label_data(
         self,
         label: Union[str, int, np.integer]
-    ) -> SegmentationLabelData | None:
+    ) -> Union[SegmentationLabelData, None]:
         """
         Grabs the SegmentationLabelData object by label.
 
         Parameters
         ----------
             label: str or int
                 A unique string label or integer index from the dataset.
@@ -342,16 +342,16 @@
         self._predictions = 0
         self._union = 0
         self._true_predictions = 0
         self._false_predictions = 0
 
     def capture_class(
         self,
-        class_labels: Union[list[int], np.ndarray[np.integer]],
-        labels: list[str] = None
+        class_labels: Union[list, np.ndarray],
+        labels: List[str] = None
     ):
         """
         Records the unique labels encountered in the prediction and 
         ground truth and creates a container (SegmentationLabelData) 
         for the label found in the model predictions and ground truth.
 
         Parameters
```

## deepview/validator/metrics/summary.py

```diff
@@ -2,15 +2,16 @@
 #
 # Unauthorized copying of this file, via any medium is strictly prohibited
 # Proprietary and confidential.
 #
 # This source code is provided solely for runtime interpretation by Python.
 # Modifying or copying any source code is explicitly forbidden.
 
-from typing import Union, Tuple
+from deepview.validator.metrics.detectionutils import minkowski_distance
+from typing import Union, List
 import numpy as np
 
 class ImageSummary:
     """
     The validation summary per image.
 
     Parameters
@@ -39,14 +40,15 @@
         self._index_missed_gt = list()
         self._iou_list = list()
 
         # A container for the matched centers
         self._centers = {
             "gt_centers": [],
             "dt_centers": [],
+            "center_distances": []
         }
 
         """
         The following summary will have the format below:
         [
 			[(gt_box), (dt_box), (iou,)], # A Classification FP or a TP
 			[(gt_box),  None, 	  None],  # A False Negative
@@ -132,82 +134,82 @@
         ----------
             dts: int
                 This is the number of predictions in the image.
         """
         self._predictions = dts
 
     @property
-    def index_matches(self) -> list[list[int, int]]:
+    def index_matches(self) -> List[list]:
         """
         Attribute to access the index_matches. This contains the indices
         of the ground truth and the predictions that are matched in the format
         [[gti, dti], [gti, dti], ...].
         Can be set to :py:class:`list`
 
         Returns
         -------
             :py:class:`list` 
                 The indices of the matched ground truth and the predictions.
         """
         return self._index_matches
 
     @index_matches.setter
-    def index_matches(self, this_index_matches: list[list[int, int]]):
+    def index_matches(self, this_index_matches: List[list]):
         """
         Sets the index_matches.
 
         Parameters
         ----------
             this_index_matches: :py:class:`list` 
                 These is the index_matches.
         """
         self._index_matches = this_index_matches
 
     @property
-    def index_unmatched_dt(self) -> list[int]:
+    def index_unmatched_dt(self) -> List[int]:
         """
         Attribute to access the index_unmatched_dt. This contains the indices
         of the predictions that were unmatched.
         Can be set to :py:class:`list`
 
         Returns
         -------
             :py:class:`list` 
                 The indices of the unmatched predictions.
         """
         return self._index_unmatched_dt
 
     @index_unmatched_dt.setter
-    def index_unmatched_dt(self, this_index_unmatched_dt: list[int]):
+    def index_unmatched_dt(self, this_index_unmatched_dt: List[int]):
         """
         Sets the index_unmatched_dt.
 
         Parameters
         ----------
             this_index_unmatched_dt: :py:class:`list` 
                 The indices of the unmatched predictions.
         """
         self._index_unmatched_dt = this_index_unmatched_dt
 
     @property
-    def index_unmatched_gt(self) -> list[int]:
+    def index_unmatched_gt(self) -> List[int]:
         """
         Attribute to access the index_unmatched_gt. This contains the indices
         of the ground truths that were unmatched.
         Can be set to :py:class:`list`
 
         Returns
         -------
             :py:class:`list` 
                 The indices of the unmatched ground truths.
         """
         return self._index_unmatched_gt
 
     @index_unmatched_gt.setter
-    def index_unmatched_gt(self, this_index_unmatched_gt: list[int]):
+    def index_unmatched_gt(self, this_index_unmatched_gt: List[int]):
         """
         Sets the index_unmatched_gt.
 
         Parameters
         ----------
             this_index_unmatched_gt: :py:class:`list` 
                 The indices of the unmatched ground truths.
@@ -265,15 +267,15 @@
         Raises
         ------
             ValueError
                 This error is raised if the dictionary does not contain
                 the expected keys.
         """
         if not all(key in this_centers.keys()
-                   for key in ["gt_centers", "dt_centers"]):
+                   for key in ["gt_centers", "dt_centers", "center_distances"]):
             raise ValueError(
                 f"The following keys are expected: {this_centers.keys()}")
         self._centers = this_centers
 
     def append_centers(
         self,
         gt_center: Union[list, np.ndarray],
@@ -289,14 +291,15 @@
                 This contains the (x,y,z) center of the ground truth bounding box.
 
             dt_center: list or np.ndarray
                 This contains the (x,y,z) center of the prediction bounding box.
         """
         self._centers["gt_centers"].append(gt_center)
         self._centers["dt_centers"].append(dt_center)
+        self._centers["center_distances"].append(minkowski_distance(dt_center, gt_center))
 
     @property
     def summary(self) -> list:
         """
         Attribute to access the summary. 
         The following summary will have the format below:: 
 
@@ -505,20 +508,28 @@
             model: str = "Training Model",
             dataset: str = "Validation Dataset",
     ) -> None:
 
         self._model = model
         self._dataset = dataset
         self._save_path = None
-        self._image_summaries = list()
+        # This list becomes too resource intensive.
+        # self._image_summaries = list() # NOSONAR
         self._ground_truths = 0
         # This is used for segmentation total number of prediction pixels.
         self._predictions = 0
 
         """Detection Summaries"""
+        # A container for the matched centers
+        self._centers = {
+            "gt_centers": [],
+            "dt_centers": [],
+            "center_distances": []
+        }
+
         self._true_positives = 0
         self._false_negatives = 0
         self._classification_false_positives = 0
         self._localization_false_positives = 0
         self._overall_precision = np.nan
         self._overall_recall = np.nan
         self._overall_accuracy = np.nan
@@ -653,28 +664,28 @@
         ----------
             this_save_path: str
                 The path to save the results
         """
         self._save_path = this_save_path
 
     @property
-    def image_summaries(self) -> list[ImageSummary]:
+    def image_summaries(self) -> List[ImageSummary]:
         """
         Attribute to access the image summaries.
         Can be set to :py:class:`list` of ImageSummary
 
         Returns
         -------
             :py:class:`list` of ImageSummary
                 This contains summary of each image.
         """
         return self._image_summaries
 
     @image_summaries.setter
-    def image_summaries(self, this_summaries: list[ImageSummary]):
+    def image_summaries(self, this_summaries: List[ImageSummary]):
         """
         Sets the image summaries to a new value.
 
         Parameters
         ----------
             this_summaries: :py:class:`list` of ImageSummary
                 These are the summary objects per image
@@ -762,14 +773,77 @@
         ----------
             prd: int
                 The number of predictions to add.
         """
         self._predictions += prd
 
     @property
+    def centers(self) -> dict:
+        """
+        Attribute to access the matched center points of the bounding boxes.
+        Can only be set to :py:class:dict.
+
+        Returns
+        -------
+            :py:class:dict.: The matched center points of the bounding boxes.
+        """
+        return self._centers
+
+    @centers.setter
+    def centers(self, this_centers: dict):
+        """
+        Sets the matched center points to another dictionary.
+
+        Parameters
+        ----------
+            this_centers: dict
+                The matched center points to set.
+
+        Raises
+        ------
+            ValueError
+                This error is raised if the dictionary does not contain
+                the expected keys.
+        """
+        if not all(key in this_centers.keys()
+                   for key in ["gt_centers", "dt_centers", "center_distances"]):
+            raise ValueError(
+                f"The following keys are expected: {this_centers.keys()}")
+        self._centers = this_centers
+
+    def store_centers(
+        self,
+        gt_centers: Union[list, np.ndarray],
+        dt_centers: Union[list, np.ndarray],
+        center_distances: Union[list, np.ndarray]
+    ):
+        """
+        Appends the center points of the bounding boxes assuming gt_center
+        and dt_center are matched. Furthermore, the distance between the
+        centers is also stored.
+
+        Parameters
+        ----------
+            gt_centers: list or np.ndarray
+                This contains the [[x,y,z], ...] center of the ground truth 
+                bounding box.
+
+            dt_centers: list or np.ndarray
+                This contains the [[x,y,z], ...] center of the prediction 
+                bounding box.
+            
+            center_distances: list or np.ndarray
+                This contains the center distances between matched 
+                ground truth and prediction.
+        """
+        self._centers["gt_centers"] += gt_centers
+        self._centers["dt_centers"] += dt_centers
+        self._centers["center_distances"] += center_distances
+
+    @property
     def true_positives(self) -> int:
         """
         Attribute to access the number of true positives.
         Can only be set to :py:class:`int`
 
         Returns
         -------
@@ -1391,15 +1465,15 @@
         Returns
         -------
             :py:class:dict: The model timings.
         """
         return self._timings
 
     @timings.setter
-    def timings(self, this_timings: dict | None):
+    def timings(self, this_timings: Union[dict, None]):
         """
         Sets the timings of the model.
 
         Parameters
         ----------
             this_timings: dict
                 The model timings.
@@ -1582,28 +1656,28 @@
                             "fp": fp,
                             "gt": gt
                         }
         """
         self._class_histogram_data[label] = data
 
     @property
-    def confusion_matrix_data(self) -> list[tuple]:
+    def confusion_matrix_data(self) -> List[tuple]:
         """
         Attribute to access the confusion matrix data.
         Can only be set to :py:class:`list`
 
         Returns
         -------
             :py:class:`list`
                 This contains the data for the confusion matrix.
         """
         return self._confusion_matrix_data
 
     @confusion_matrix_data.setter
-    def confusion_matrix_data(self, data: list[tuple]):
+    def confusion_matrix_data(self, data: List[tuple]):
         """
         Sets the data for the confusion matrix to a new value.
 
         Parameters
         ----------
             data: :py:class:`list`
                 These are the confusion matrix data to set.
```

## deepview/validator/runners/__init__.py

```diff
@@ -2,16 +2,22 @@
 #
 # Unauthorized copying of this file, via any medium is strictly prohibited
 # Proprietary and confidential.
 #
 # This source code is provided solely for runtime interpretation by Python.
 # Modifying or copying any source code is explicitly forbidden.
 
-from deepview.validator.runners.deepviewrt import DeepViewRTRunner, \
-    SegmentationDeepViewRTRunner
-from deepview.validator.runners.keras import DetectionKerasRunner, \
-    SegmentationKerasRunner, PoseKerasRunner
+from deepview.validator.runners.deepviewrt import (
+    SegmentationDeepViewRTRunner,
+    DeepViewRTRunner
+)
 from deepview.validator.runners.tensorrt import TensorRTRunner
 from deepview.validator.runners.offline import OfflineRunner
 from deepview.validator.runners.tflite import TFliteRunner
+from deepview.validator.runners.hailo import HailoRunner
+from deepview.validator.runners.keras import (
+    SegmentationKerasRunner, 
+    DetectionKerasRunner, 
+    PoseKerasRunner
+)
 from deepview.validator.runners.onnx import ONNXRunner
 from deepview.validator.runners.core import Runner
```

## deepview/validator/runners/core.py

```diff
@@ -2,39 +2,60 @@
 #
 # Unauthorized copying of this file, via any medium is strictly prohibited
 # Proprietary and confidential.
 #
 # This source code is provided solely for runtime interpretation by Python.
 # Modifying or copying any source code is explicitly forbidden.
 
+from __future__ import annotations
+from typing import TYPE_CHECKING, Tuple
+if TYPE_CHECKING:
+    from deepview.validator.evaluators import Parameters
+
+from deepview.validator.exceptions import NonMatchingIndexException
 from deepview.validator.exceptions import MissingLibraryException
 from deepview.validator.metrics.detectionutils import batch_iou
 from deepview.validator.datasets.core import Dataset
 import numpy as np
 import os
 
 class Runner:
     """
     Abstract Class that provides a template for the other runner classes.
 
     Parameters
     ----------
-        model: str, tf.keras.Model
+        model: str
             This is the path to the model file, 
-            directory of prediction text files (offline), or a loaded keras
-            model.
+            directory of prediction text files (offline), or a loaded model.
+
+        model: str 
+            The path to the model.
+
+        parameters: Parameters
+            These are the model parameters set from the command line.
+
+        labels: list
+            Unique string labels.
 
     Raises
     ------
         FileNotFoundError
             Raised if the path to the model does not exist.
     """
-    def __init__(self, model):
+    def __init__(self, model, parameters: Parameters=None, labels: list=None):
         
         self.model = model
+        self.parameters = parameters
+        
+        if labels is None:
+            self.labels = []
+        else:
+            self.labels = labels
+
         self.input_shape = None
 
         self.box_timings = list()
         self.inference_timings = list()
         self.loading_input_timings = list()
 
     @staticmethod
@@ -57,14 +78,47 @@
             FileNotFoundError
                 Raised if the path to the model does not exist.
         """
         if not os.path.exists(source):
             raise FileNotFoundError(
                 "Model file is expected to be at: {}".format(source))
         return source
+    
+    def update_engine(self):
+        """
+        Updates the engine using TensorFlow or PyTorch.
+        """
+        try:
+            import torch
+            cuda = torch.cuda.is_available() and self.parameters.engine != "cpu"
+            if cuda:
+                self.parameters.engine = "cuda"
+                return
+        except ImportError:
+            pass
+
+        try:
+            import tensorflow as tf
+            if len(tf.config.list_physical_devices('GPU')):
+                self.parameters.engine = "gpu"
+            elif len(tf.config.list_physical_devices('CPU')):
+                self.parameters.engine = "cpu"
+        except ImportError:
+            pass
+
+    def update_nms(self):
+        """
+        Updates the NMS used based on the model output shape.
+        """
+        output_shape = self.get_output_shape()
+        # For COCO, yolo generates models with classes + 4 (boxes) + 1 (confidence).
+        if (output_shape[0] is None or output_shape[-1] != 85) and len(output_shape) == 3:
+            self.parameters.nms = "tensorflow"
+        elif output_shape[0] == 1 and len(output_shape) == 3:
+            self.parameters.nms = "torch"
 
     def load_model(self):
         """Abstract Method"""
         pass
 
     def run_single_instance(self, image):
         """Abstract Method"""
@@ -74,19 +128,23 @@
         """Abstract Method"""
         pass
 
     def get_input_type(self):
         """Abstract Method"""
         pass
 
+    def get_input_shape(self):
+        """Abstract Method"""
+        pass
+
     def get_output_type(self):
         """Abstract Method"""
         pass
 
-    def get_input_shape(self):
+    def get_output_shape(self):
         """Abstract Method"""
         pass
 
     @staticmethod
     def apply_normalization(
         image: np.ndarray, normalization: str, input_type: str="float32"):
         """
@@ -128,18 +186,210 @@
         -------
             x: torch.Tensor
                 This is the numpy array as a torch.Tensor type.
         """
         try:
             import torch
         except ImportError:
-            raise MissingLibraryException("pytorch is needed for Tflite models.")
+            raise MissingLibraryException(
+                "torchvision~=0.15.2 is needed to convert from NumPy.")
         return torch.from_numpy(x).to("cpu") if isinstance(x, np.ndarray) else x
+
+    def multiclass_nms(
+            self, 
+            boxes: np.ndarray, 
+            scores: np.ndarray, 
+            nms_thr: float, 
+            score_thr: float, 
+            class_agnostic: bool=True
+        ) -> np.ndarray:
+        """
+        Multiclass NMS implemented in Numpy
+        
+        Parameters
+        ----------
+            boxes: np.ndarray
+                Input boxes to the NMS (number of boxes, 4) in xyxy f
+                non-normalized ormat.
+
+            scores: np.ndarray
+                Input scores to the NMS (number of boxes, number of classes).
+
+            nms_thr: float
+                This is the IoU threshold for the NMS.
+
+            score_thr: float
+                This contains the score threshold input for the NMS.
+
+            class_agnostic: bool
+                This is to determine which type of NMS to perform.
+
+        Returns
+        -------
+            dets: np.ndarray
+                Post-NMS detections (number of detections, 6) which contains
+                (xyxy, score, class) a total of 6 columns.
+        """
+        if class_agnostic:
+            nms_method = self.multiclass_nms_class_agnostic
+        else:
+            nms_method = self.multiclass_nms_class_aware
+        return nms_method(boxes, scores, nms_thr, score_thr)
     
-    def non_max_supression( # NOSONAR
+    def multiclass_nms_class_aware(
+            self, 
+            boxes: np.ndarray, 
+            scores: np.ndarray, 
+            nms_thr: float, 
+            score_thr: float,
+        ) -> np.ndarray:
+        """
+        Multiclass NMS implemented in Numpy. Class-aware version.
+        Method taken from: https://github.com/Megvii-BaseDetection/YOLOX/blob/main/yolox/utils/demo_utils.py#L96
+
+        Parameters
+        ----------
+            boxes: np.ndarray
+                Input boxes to the NMS (number of boxes, 4) in xyxy f
+                non-normalized ormat.
+
+            scores: np.ndarray
+                Input scores to the NMS (number of boxes, number of classes).
+
+            nms_thr: float
+                This is the IoU threshold for the NMS.
+
+            score_thr: float
+                This contains the score threshold input for the NMS.
+
+        Returns
+        -------
+            dets: np.ndarray
+                Post-NMS detections (number of detections, 6) which contains
+                (xyxy, score, class) a total of 6 columns.
+        """
+        final_dets = []
+        num_classes = scores.shape[1]
+        for cls_ind in range(num_classes):
+            cls_scores = scores[:, cls_ind]
+            valid_score_mask = cls_scores > score_thr
+            if valid_score_mask.sum() == 0:
+                continue
+            else:
+                valid_scores = cls_scores[valid_score_mask]
+                valid_boxes = boxes[valid_score_mask]
+                keep = self.nms(valid_boxes, valid_scores, nms_thr)
+                if len(keep) > 0:
+                    cls_inds = np.ones((len(keep), 1)) * cls_ind
+                    dets = np.concatenate(
+                        [valid_boxes[keep], valid_scores[keep, None], cls_inds], 1
+                    )
+                    final_dets.append(dets)
+        if len(final_dets) == 0:
+            return None
+        return np.concatenate(final_dets, 0)
+
+    def multiclass_nms_class_agnostic(
+            self, 
+            boxes: np.ndarray, 
+            scores: np.ndarray, 
+            nms_thr: float, 
+            score_thr: float,
+        ) -> np.ndarray:
+        """
+        Multiclass NMS implemented in Numpy. Class-agnostic version.
+        Method taken from https://github.com/Megvii-BaseDetection/YOLOX/blob/main/yolox/utils/demo_utils.py#L120.
+        
+        Parameters
+        ----------
+            boxes: np.ndarray
+                Input boxes to the NMS (number of boxes, 4) in xyxy f
+                non-normalized ormat.
+
+            scores: np.ndarray
+                Input scores to the NMS (number of boxes, number of classes).
+
+            nms_thr: float
+                This is the IoU threshold for the NMS.
+
+            score_thr: float
+                This contains the score threshold input for the NMS.
+
+        Returns
+        -------
+            dets: np.ndarray
+                Post-NMS detections (number of detections, 6) which contains
+                (xyxy, score, class) a total of 6 columns.
+        """
+        cls_inds = scores.argmax(1)
+        cls_scores = scores[np.arange(len(cls_inds)), cls_inds]
+
+        valid_score_mask = cls_scores > score_thr
+        if valid_score_mask.sum() == 0:
+            return None
+        valid_scores = cls_scores[valid_score_mask]
+        valid_boxes = boxes[valid_score_mask]
+        valid_cls_inds = cls_inds[valid_score_mask]
+        keep = self.nms(valid_boxes, valid_scores, nms_thr)
+        if keep:
+            dets = np.concatenate(
+                [valid_boxes[keep], valid_scores[keep, None], valid_cls_inds[keep, None]], 1
+            )
+        return dets
+
+    @staticmethod
+    def nms(boxes: np.ndarray, scores: np.ndarray, nms_thr: float) -> list:
+        """
+        Single class NMS implemented in Numpy.
+        Method taken from: https://github.com/Megvii-BaseDetection/YOLOX/blob/main/yolox/utils/demo_utils.py#L57
+
+        Parameters
+        ----------
+            boxes: np.ndarray
+                Input boxes to the NMS (number of boxes, 4) in xyxy f
+                non-normalized ormat.
+
+            scores: np.ndarray
+                Input scores to the NMS (number of boxes, number of classes).
+
+            nms_thr: float
+                This is the IoU threshold for the NMS.
+
+        Returns
+        -------
+            keep: list
+                This contains the indices of the boxes to keep.
+        """
+        x1 = boxes[:, 0]
+        y1 = boxes[:, 1]
+        x2 = boxes[:, 2]
+        y2 = boxes[:, 3]
+
+        areas = (x2 - x1 + 1) * (y2 - y1 + 1)
+        order = scores.argsort()[::-1]
+
+        keep = []
+        while order.size > 0:
+            i = order[0]
+            keep.append(i)
+            xx1 = np.maximum(x1[i], x1[order[1:]])
+            yy1 = np.maximum(y1[i], y1[order[1:]])
+            xx2 = np.minimum(x2[i], x2[order[1:]])
+            yy2 = np.minimum(y2[i], y2[order[1:]])
+
+            w = np.maximum(0.0, xx2 - xx1 + 1)
+            h = np.maximum(0.0, yy2 - yy1 + 1)
+            inter = w * h
+            ovr = inter / (areas[i] + areas[order[1:]] - inter)
+
+            inds = np.nonzero(ovr <= nms_thr)[0]
+            order = order[inds + 1]
+        return keep
+    
+    def torch_nms( # NOSONAR
             self, 
             prediction,
             agnostic: bool=False,
             multi_label: bool=True,
             nm: int=0,
             max_wh: int=7680,
             max_nms: int= 30000,
@@ -155,14 +405,16 @@
         2) detection iou threshold = 0.60
         3) max detections = 300
 
         Parameters
         ----------
             prediction: torch.Tensor
                 Raw predictions from the model (inference_out, loss_out).
+                This contains shape (batch size, number of boxes, number of classes).
+
             agnostic: bool
 
             multi_label: bool
                 If validation has more than 1 labels.
 
             nm: int
 
@@ -176,29 +428,36 @@
                 Require redundant detections.
 
             merge: bool
                 Use merge NMS.
 
         Returns
         -------
-            output
+            output: list
+                Length 1 which is formatted in the following way which 
+                has a shape of (1, number of boxes, 6).
+                [[[xmin, ymin, xmax, ymax, confidence, label], [...], ...]]. 
         """
         try:
             import torchvision
             import torch
         except ImportError:
             raise MissingLibraryException(
-                "pytorch is needed for Tflite models.")
+                "torchvision~=0.15.2 is required to use torch NMS.")
+        
+        if self.parameters.max_detections is None:
+            self.parameters.max_detections = 100
 
         # YOLOv5 model in validation model.
         if isinstance(prediction, (list, tuple)):  
             # Select only inference output.
             prediction = prediction[0] 
 
         bs = prediction.shape[0]  # Batch size.
+        # Offset of -5 is explained in https://medium.com/@KrashKart/i-wish-i-knew-this-about-yolov5-2fbab3584906
         nc = prediction.shape[2] - nm - 5  # The number of classes.
         xc = prediction[..., 4] > self.parameters.detection_score # Candidates.
 
         multi_label &= nc > 1  # Multiple labels per box (adds 0.5ms/img).
         mi = 5 + nc  # Mask start index.
         output = [torch.zeros((0, 6 + nm), device="cpu")] * bs
 
@@ -235,15 +494,15 @@
             # Sort by confidence and remove excess boxes.
             x = x[x[:, 4].argsort(descending=True)[:max_nms]]  
 
             # Batched NMS.
             c = x[:, 5:6] * (0 if agnostic else max_wh)  # The classes.
             # boxes (offset by class), scores.
             boxes, scores = x[:, :4] + c, x[:, 4]  
-            
+        
             # Torchvision NMS.
             i = torchvision.ops.nms(
                 boxes, scores, self.parameters.detection_iou)  
             i = i[:self.parameters.max_detections]  # This limits detections.
             # Merge NMS (boxes merged using weighted mean).
             if merge and (1 < n < 3e3):  
                 # Update boxes as boxes(i,4) = weights(i,n) * boxes(n,4).
@@ -254,14 +513,181 @@
                 x[i, :4] = torch.mm(
                     weights, x[:, :4]).float() / weights.sum(1, keepdim=True) 
                 if redundant:
                     i = i[iou.sum(1) > 1]  # Require redundancy.
             output[xi] = x[i]
         return output
     
+    def tensorflow_nms(
+            self, 
+            boxes: np.ndarray, 
+            scores: np.ndarray, 
+            clip_boxes: bool=False
+        ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
+        """
+        Performs NMS using Tensorflow.
+
+        Parameters
+        ----------
+            boxes: np.ndarray
+                The bounding boxes from the model inference.
+
+            scores: np.ndarray
+                The detection scores from the model inference.
+
+            clip_boxes: False
+                If set to True, the boxes will be clamped within [0, 1).
+
+        Returns
+        -------
+            nms_predicted_boxes: np.ndarray
+                The detection bounding boxes after NMS.
+
+            nms_predicted_classes: np.ndarray
+                The detection labels after NMS.
+
+            nms_predicted_scores: np.ndarray
+                The detection scores after NMS.
+        """
+        try:
+            os.environ['TF_CPP_MIN_LOG_LEVEL'] = '3'
+            import tensorflow as tf
+        except ImportError:
+            raise MissingLibraryException(
+                "tensorflow>=2.8.0,<2.16.0 is needed to perform NMS.")
+        
+        if self.parameters.max_detections is None:
+            self.parameters.max_detections = 100
+        
+        nmsed_boxes, nmsed_scores, nmsed_classes, valid_boxes = \
+            tf.image.combined_non_max_suppression(
+                boxes,
+                scores,
+                self.parameters.max_detections,
+                self.parameters.max_detections,
+                iou_threshold=self.parameters.detection_iou,
+                score_threshold=self.parameters.detection_score,
+                clip_boxes=clip_boxes)
+        nmsed_classes = tf.cast(nmsed_classes, tf.int32)
+
+        return self.tensorflow_nms_filter(
+            nmsed_boxes, nmsed_scores, nmsed_classes, valid_boxes)
+    
+    def tensorflow_nms_filter(
+            self, nmsed_boxes, nmsed_scores, nmsed_classes, valid_boxes
+        ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
+        """
+        This method performs NMS filter operations.
+        
+        Parameters
+        ----------
+            nmsed_boxes: torch.Tensor
+                This is the output of TensorFlow NMS bounding boxes.
+
+            nmsed_scores: torch.Tensor
+                This is the output of TensorFlow NMS scores.
+
+            nmsed_classes: torch.Tensor
+                This is the output of TensorFlow NMS classes.
+
+            valid_boxes: torch.Tensor
+                This contains indices for valid detections.
+
+        Returns
+        -------
+            nms_predicted_boxes: np.ndarray
+                This contains only the valid bounding boxes.
+            
+            nms_predicted_classes: np.ndarray
+                This contains only the valid bounding boxes.
+            
+            nms_predicted_scores: np.ndarray
+                This contains only the valid bounding boxes.
+        """
+        nms_predicted_boxes = [nmsed_boxes.numpy()[i, :valid_boxes[i], :]
+                               for i in range(nmsed_boxes.shape[0])][0]
+        nms_predicted_classes = [nmsed_classes.numpy()[i, :valid_boxes[i]]
+                                 for i in range(nmsed_classes.shape[0])][0]
+        nms_predicted_scores = [nmsed_scores.numpy()[i, :valid_boxes[i]]
+                                for i in range(nmsed_scores.shape[0])][0]
+        return nms_predicted_boxes, nms_predicted_classes, nms_predicted_scores
+
+    def index2string(self, classes: np.ndarray) -> np.ndarray:
+        """
+        This method converts the model label indices into their string
+        representations.
+
+        Parameters
+        ----------
+            classes: np.ndarray
+                This contains the model label indices.
+
+        Returns
+        -------
+            string_classes: np.ndarray
+                This contains labels as strings. 
+        """
+        if len(self.labels) > 0:
+            string_classes = list()
+            for cls in classes:
+                try:
+                    string_classes.append(self.labels[int(cls)])
+                except IndexError:
+                    raise NonMatchingIndexException(cls)
+            return np.array(string_classes)
+        return classes
+    
+    def class_filter(
+            self, 
+            boxes: np.ndarray, 
+            classes: np.ndarray, 
+            scores: np.ndarray
+        ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
+        """
+        For dataset to model label mismatches. Filter only the 
+        bounding boxes and scores with classes that are in common between
+        the ground truth and the detections.
+
+        Parameters
+        ----------
+            boxes: np.ndarray
+                These contains boxes in any format.
+
+            classes: np.ndarray
+                These contains an array of integer indices.
+
+            scores: np.ndarray
+                These contains an array of model confidence scores. 
+        
+        Returns
+        -------
+            boxes: np.ndarray
+                These are the filtered boxes.
+
+            classes: np.ndarray
+                These are the filtered classes.
+
+            scores: np.ndarray
+                These are the filtered scores. 
+        """
+        if len(self.labels) > 0:
+            labels = np.arange(0, len(self.labels), 1)
+            # Take only the labels that are common to the ground truth labels.
+            indices = np.nonzero(np.in1d(classes, labels))[0]
+            boxes = boxes[indices]
+            scores = scores[indices]
+            classes = classes[indices]
+            # The classes may not contain indices that are larger still. 
+            # For example classes may contain [11, 9, 7]. The ground truth
+            # contains [0, 1, 2]. The classes should be mapped as [2, 1, 0].
+            if issubclass(classes.dtype.type, np.integer):
+                sorted_indices = np.argsort(classes)
+                classes = np.argsort(sorted_indices)  
+        return boxes, classes, scores
+
     def summarize(self):
         """
         Returns a summary of all the timings: 
         (mean, avg, max) of (load, inference, box).
 
         Returns
         -------
```

## deepview/validator/runners/deepviewrt.py

```diff
@@ -54,28 +54,22 @@
     """
     def __init__(
         self,
         model: str,
         parameters: Parameters,
         labels: list=None
     ):
-        super(DeepViewRTRunner, self).__init__(model)
+        super(DeepViewRTRunner, self).__init__(model, parameters, labels)
         
         try:
             import deepview.vaal as vaal # type: ignore
         except ImportError:
             raise MissingLibraryException(
                 "vaal library is needed to run DeepViewRT models.")
         
-        self.parameters = parameters
-        if labels is None:
-            self.labels = []
-        else:
-            self.labels = labels
-
         try:
             self.ctx = vaal.Context(self.parameters.engine)
         except AttributeError:
             raise EnvironmentError(
                 'Did not find Vaal Context. Try setting the environment \
                     variable VAAL_LIBRARY to the VAAL library.')
         # Change because VAAL automatically uses CPU if NPU is unavailable.
@@ -113,14 +107,78 @@
         self.ctx.load_model(model)
         if int(self.parameters.warmup) > 0:
             logger("Loading model and warmup...", code="INFO")
             t = timeit(self.ctx.run_model, number=self.parameters.warmup)
             logger("model warmup took %f seconds (%f ms avg)\n" %
                     (t, t * 1000 / self.parameters.warmup), code="INFO")
 
+        if self.parameters.label_offset == 0 and self.parameters.auto_offset:
+            self.parameters.label_offset = self.auto_offset()
+            
+    def auto_offset(self) -> int:
+        """
+        Initialize an auto offset parameter to reduce complexity for the
+        manually setting the offset of the model indices due to 
+        integer to string mapping mismatches.
+
+        This is done by comparing the number of labels in the ground truth
+        and the model outputs. Common patterns are for a playing cards model.
+
+        Properly converted.
+        ```
+        out.shape=(1, 1500, 13)   <-- number of labels
+        out.shape=(1, 1500, 1, 4)
+        ```
+
+        Improperly converted.
+        ```
+        out.shape=(1, 20, 20, 57)
+        out.shape=(1, 1500, 1, 4)
+        out.shape=(1, 1500, 14)    <-- number of labels
+        out.shape=(1, 10, 10, 57)
+        ```
+
+        Returns
+        -------
+            offset: int
+                The offset to apply towards the model indices.
+        """
+        label_count = 0
+        shape = self.get_output_shape()
+        if shape is not None:
+            label_count = shape[-1]
+        
+        if len(self.labels) == 0 or label_count == 0:
+            return 0
+        return len(self.labels) - label_count
+    
+    def apply_offset(self, label: int) -> int:
+        """
+        Apply label offset to the model output. The offset set in the command
+        line is applied if it is set. Otherwise, the auto offset feature
+        will be used. 
+
+        Parameters
+        ----------
+            label: int
+                This is the current label output of the model.
+
+        Parameters
+        ----------
+            label: int
+                This is the index with the applied offset.
+        """
+        if self.parameters.label_offset != 0:
+            label = label + self.parameters.label_offset
+
+        if label < 0:
+            raise ValueError(
+                f"The model label resulted in a negative integer: {label}")
+        return label
+
     def run_single_instance(
             self, 
             image: Union[str, np.ndarray]
         ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
         """
         Runs deepviewrt models and parses the prediction 
         bounding boxes, scores, and labels and records timings 
@@ -268,115 +326,84 @@
         Raises
         ------
             NonMatchingIndexException
                 Raised if the label index 
                 returned by the model does not match any index position in
                 either context labels or the provided labels from the dataset.
         """
-        label = box.label + self.parameters.label_offset
-        if label < 0:
-            raise ValueError(
-                f"The model label resulted in a negative integer: {label}")
-        
         if len(self.ctx.labels) > 0:
-            try:
-                if self.ctx.label(label) == "VisionPack Trial Expired":
-                    return None
-                else:
-                    dt_class = self.ctx.label(label).lower().rstrip(
-                        '\"').lstrip('\"')
-            except IndexError:
-                raise NonMatchingIndexException(label)
+            if self.ctx.label(box.label) == "VisionPack Trial Expired":
+                return None
+            else:
+                dt_class = self.ctx.label(box.label).lower().rstrip(
+                    '\"').lstrip('\"')
         elif len(self.labels) > 0:
+            label = self.apply_offset(box.label)
             try:
                 dt_class = self.labels[label].lower().rstrip(
                     '\"').lstrip('\"')
             except IndexError:
                 raise NonMatchingIndexException(label)
         else:
+            label = self.apply_offset(box.label)
             dt_class = label
         dt_box = [box.xmin, box.ymin, box.xmax, box.ymax]
         dt_score = box.score
         return dt_class, dt_box, dt_score
        
     def process_tensorflow_nms(
             self, 
             boxes: np.ndarray, 
             scores: np.ndarray
         ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
         """
-        Processes model detections using tensorflow NMS.
+        Processes model detections using TensorFlow NMS.
        
         Parameters
         ----------
             boxes: np.ndarray
                 This array contains the bounding boxes for one image.
             
             scores: np.ndarray
                 This array contains the model score per bounding box.
 
         Returns
         -------
             labels, bounding boxes, scores: np.ndarray
                 These are the model detections after being processed using
-                tensorflow NMS.
+                TensorFlow NMS.
         
         Raises
         ------
             NonMatchingIndexException
                 Raised if the model label index does
                 not match any index position in the provided labels from
                 the dataset. 
         """
         try:
             os.environ['TF_CPP_MIN_LOG_LEVEL'] = '3'
             import tensorflow as tf
         except ImportError:
             raise MissingLibraryException(
-                "tensorflow is needed to perform NMS operations.")
-
-        if self.parameters.label_offset > 0:
-            scores = scores[..., self.parameters.label_offset:]
-
-        if self.parameters.max_detections is None:
-            max_detections = 100
-        else:
-            max_detections = self.parameters.max_detections
-
-        nmsed_boxes, nmsed_scores, nmsed_classes, valid_boxes = \
-                tf.image.combined_non_max_suppression(
-                    boxes.astype(np.float32),
-                    scores.astype(np.float32),
-                    max_detections,
-                    max_detections,
-                    iou_threshold=self.parameters.detection_iou,
-                    score_threshold=self.parameters.detection_score)
-        
-        nmsed_boxes = nmsed_boxes.numpy()
-        nmsed_classes = tf.cast(nmsed_classes, tf.int32)
+                "tensorflow>=2.8.0,<2.16.0 is needed to perform NMS operations.")
 
-        nms_predicted_boxes = [nmsed_boxes[i, :valid_boxes[i], :]
-                            for i in range(nmsed_boxes.shape[0])][0]
-        nms_predicted_classes = [nmsed_classes.numpy()[i, :valid_boxes[i]]
-                                for i in range(nmsed_classes.shape[0])][0]
-        nms_predicted_scores = [nmsed_scores.numpy()[i, :valid_boxes[i]]
-                                for i in range(nmsed_scores.shape[0])][0]
-
-        if len(self.labels) > 0:
-            string_nms_predicted_classes = list()
-            format_nms_predicted_boxes = list()
-            for cls, box in zip(nms_predicted_classes, nms_predicted_boxes):
-                try:
-                    string_nms_predicted_classes.append(
-                        self.labels[int(cls)])
-                except IndexError:
-                    raise NonMatchingIndexException(cls)
-                format_nms_predicted_boxes.append(box)
-            nms_predicted_classes = np.array(string_nms_predicted_classes)
-            nms_predicted_boxes = np.array(format_nms_predicted_boxes)
+        # Negative offsets could mean that the model contains the background class,
+        # but the dataset does not.
+        if self.parameters.label_offset < 0:
+            scores = scores[..., abs(self.parameters.label_offset):]
+        # Positive offsets could mean that the dataset contains the background class,
+        # but the dataset does not.
+        # TODO: Consider cases where the offset might be positive.
+
+        nms_predicted_boxes, nms_predicted_classes, nms_predicted_scores =\
+            self.tensorflow_nms(
+                boxes.astype(np.float32), 
+                scores.astype(np.float32),
+            )
+        nms_predicted_classes = self.index2string(nms_predicted_classes)
         return nms_predicted_boxes, nms_predicted_classes, nms_predicted_scores
 
     def get_input_type(self):
         """
         Returns the model input type.
 
         Returns
@@ -387,14 +414,25 @@
         Raises
         ------
             NotImplementedError
                 raise because it has not been implemented yet.
         """
         raise NotImplementedError("has not been implemented.")
 
+    def get_input_shape(self):
+        """
+        Grabs the model input shape.
+        
+        Returns
+        -------
+            type: tuple or list
+                The model input shape.
+        """
+        return self.ctx.tensor('serving_default_input_1:0').shape
+    
     def get_output_type(self):
         """
         Returns the model output type.
 
         Returns
         -------
             type: str
@@ -403,24 +441,45 @@
         Raises
         ------
             NotImplementedError
                 raise because it has not been implemented yet.
         """
         raise NotImplementedError("has not been implemented.")
 
-    def get_input_shape(self):
+    def get_output_shape(self) -> Union[tuple, None]:
         """
-        Grabs the model input shape.
-        
+        Grabs the model output shape. Only returns shapes with lengths of 3.
+
+        Properly converted.
+        ```
+        out.shape=(1, 1500, 13)   <-- number of labels
+        out.shape=(1, 1500, 1, 4)
+        ```
+
+        Improperly converted.
+        ```
+        out.shape=(1, 20, 20, 57)
+        out.shape=(1, 1500, 1, 4)
+        out.shape=(1, 1500, 14)    <-- number of labels
+        out.shape=(1, 10, 10, 57)
+        ```
+
         Returns
         -------
-            type: tuple or list
-                The model input shape.
+            shape: tuple (1x3)
+                The output shape (batch size, number of boxes, number of labels).
         """
-        return self.ctx.tensor('serving_default_input_1:0').shape
+        for i in range(4):
+            out = self.ctx.output(index=i)
+            if out is None:
+                continue
+            shape = out.array().shape
+            if len(shape) == 3:
+                return shape
+        return None
     
 class SegmentationDeepViewRTRunner(Runner):
     """
     Runs DeepViewRT Segmentationmodels using the VAAL API.
     
     Parameters
     ----------
@@ -440,23 +499,22 @@
             does not exist and the provided image is not a numpy.ndarray.
     """
     def __init__(
         self,
         model: str,
         parameters: Parameters
     ):
-        super(SegmentationDeepViewRTRunner, self).__init__(model)
+        super(SegmentationDeepViewRTRunner, self).__init__(model, parameters)
         
         try:
             import deepview.vaal as vaal # type: ignore
         except ImportError:
             raise MissingLibraryException(
                 "vaal library is needed to run DeepViewRT models.")
 
-        self.parameters = parameters
         try:
             self.ctx = vaal.Context(self.parameters.engine)
         except AttributeError:
             raise EnvironmentError(
                 'Did not find Vaal Context. Try setting the environment \
                     variable VAAL_LIBRARY to the VAAL library.')
         
@@ -532,22 +590,22 @@
         start = clock_now()
         outputs = self.ctx.output(index=0).array()[0]
         mask = np.argmax(outputs, axis=-1).astype(np.uint8)
         boxes_ns = clock_now() - start
         self.box_timings.append(boxes_ns * 1e-6)
         return mask
 
-    def get_output_type(self):
+    def get_input_type(self):
         """
-        Returns the model output type.
-       
+        Returns the model input type.
+
         Returns
         -------
             type: str
-                The model output type
+                The model input type.
 
         Raises
         ------
             NotImplementedError
                 raise because it has not been implemented yet.
         """
         raise NotImplementedError("has not been implemented.")
@@ -557,8 +615,40 @@
         Grabs the model input shape.
         
         Returns
         -------
             type: tuple or list
                 The model input shape.
         """
-        return self.ctx.tensor('serving_default_input_1:0').shape
+        return self.ctx.tensor('serving_default_input_1:0').shape
+    
+    def get_output_type(self):
+        """
+        Returns the model output type.
+
+        Returns
+        -------
+            type: str
+                The model output type.
+
+        Raises
+        ------
+            NotImplementedError
+                raise because it has not been implemented yet.
+        """
+        raise NotImplementedError("has not been implemented.")
+
+    def get_output_shape(self) -> Union[tuple, None]:
+        """
+        Returns the model output type.
+       
+        Returns
+        -------
+            type: str
+                The model output type
+
+        Raises
+        ------
+            NotImplementedError
+                raise because it has not been implemented yet.
+        """
+        raise NotImplementedError("has not been implemented.")
```

## deepview/validator/runners/keras.py

```diff
@@ -7,25 +7,26 @@
 # Modifying or copying any source code is explicitly forbidden.
 
 from __future__ import annotations
 from typing import TYPE_CHECKING, Tuple, Union
 if TYPE_CHECKING:
     from deepview.validator.evaluators import Parameters
 
-from deepview.validator.exceptions import NonMatchingIndexException
 from deepview.validator.exceptions import MissingLibraryException
 from deepview.validator.datasets.utils import resize
 from deepview.validator.runners.core import Runner
+from deepview.validator.writers import logger
 from time import monotonic_ns as clock_now
+from timeit import timeit
 import numpy as np
 import os
 
 class DetectionKerasRunner(Runner):
     """
-    Runs the Keras (h5) models using the tensorflow library.
+    Runs the Keras (h5) models using the TensorFlow library.
     
     Parameters
     ----------
         model: str or tf.keras.Model
             The path to the model or the loaded keras model.
 
         parameters: Parameters
@@ -38,50 +39,108 @@
     ------
         NonMatchingIndexException
             Raised if the model outputs an index
             that is out of bounds to the labels list passed or the labels
             contained within the model itself.
 
         MissingLibraryException
-            Raised if the tensorflow library is not installed.
+            Raised if the TensorFlow library is not installed.
     """
     def __init__(
         self,
         model,
         parameters: Parameters,
         labels: list=None
     ):
-        super(DetectionKerasRunner, self).__init__(model)
+        super(DetectionKerasRunner, self).__init__(model, parameters, labels)
 
         try:
             os.environ['TF_CPP_MIN_LOG_LEVEL'] = '3'
             import tensorflow as tf
         except ImportError:
             raise MissingLibraryException(
-                "tensorflow is needed to load the model.")
+                "tensorflow>=2.8.0,<2.16.0 is needed to load the model.")
         
         if isinstance(model, str):
             model = self.validate_model_path(model)
-            self.loaded_model = tf.keras.models.load_model(model, compile=False)
+            if os.path.exists(os.path.join(model, "saved_model.pb")):
+                self.loaded_model = tf.saved_model.load(model)
+                self.inputs = self.loaded_model.signatures["serving_default"].inputs
+                self.outputs = self.loaded_model.signatures["serving_default"].outputs
+            else:
+                self.loaded_model = tf.keras.models.load_model(model, compile=False)
         else:
             self.loaded_model = model
             self.model = "Training Model"
         
-        self.parameters = parameters
-        self.labels = []
-        if labels is not None:
-            self.labels = labels
-        self.parameters.nms = "tensorflow"
+        self.update_nms()
+        self.update_engine()
+
+        if self.parameters.warmup > 0:
+            logger("Loading model and warmup...", code="INFO")
+            # Produce a sample image of zeros.
+            input_type = self.get_input_type()
+            height, width = self.get_input_shape()[1:3]
+            image = np.expand_dims(np.zeros((height, width, 3)), 0).astype(np.dtype(input_type))
+
+            if isinstance(self.loaded_model, tf.keras.Model):
+                t = timeit(lambda: self.loaded_model.predict(image, verbose=0), number=self.parameters.warmup)
+            else:
+                t = timeit(lambda: self.loaded_model(image), number=self.parameters.warmup)
+            logger("model warmup took %f seconds (%f ms avg)" %
+                           (t, t * 1000 / self.parameters.warmup), code="INFO")
         
-        if len(tf.config.list_physical_devices('GPU')):
-            self.parameters.engine = "gpu"
-        elif len(tf.config.list_physical_devices('CPU')):
-            self.parameters.engine = "cpu"
+        if (self.parameters.label_offset == 0 and 
+            self.parameters.auto_offset and 
+            not self.parameters.class_filter):
+            self.parameters.label_offset = self.auto_offset()
+    
+    def auto_offset(self) -> int:
+        """
+        Initialize an auto offset parameter to reduce complexity for the
+        manually setting the offset of the model indices due to 
+        integer to string mapping mismatches.
+
+        This is done by comparing the number of labels in the ground truth
+        and the model outputs. Typical shapes seen include.
+
+        ```
+        (None, None, 4)
+        (None, 6000, 3)
+        ```
+
+        Common patterns are for a coco128 YoloV5 model.
+
+        ```
+        shape=[1, 25200, 85]
+        ```
+
+        From this article https://medium.com/@KrashKart/i-wish-i-knew-this-about-yolov5-2fbab3584906,
+        the first 5 rows (index 0 to 4) indicate, the probability of bounding 
+        box coordinates (xmin, ymin, xmax, ymax) as well as the objectness per 
+        grid cell for all grid cells.
+
+        The next rows (5 to 85 in this case) are the probability of class 
+        i existing at all grid cells.
+
+        Returns
+        -------
+            offset: int
+                The offset to apply towards the model indices.
+        """
+        shape = self.get_output_shape()
+        if len(shape) == 3:
+            yolo_converted = shape[-1] - 5
+            label_count = yolo_converted if yolo_converted == len(self.labels) else shape[-1]
         else:
-            self.parameters.engine = "unknown"
+            label_count = 0
+        
+        if len(self.labels) == 0 or label_count == 0:
+            return 0
+        return len(self.labels) - label_count
 
     def run_single_instance(
             self, 
             image: Union[str, np.ndarray]
         ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
         """
         Runs the model to produce bounding box predictions on a 
@@ -101,43 +160,63 @@
             classes: np.ndarray
                 The prediction labels.. [cl1, cl2, ...].
 
             scores: np.ndarray
                 The prediction confidence scores.. [score, score, ...]
                 normalized between 0 and 1.
         """
+        """Input Preprocessing"""
         start = clock_now()
         # Take only the (height, width).
-        image = resize(image, self.get_input_shape()[1:])
-        tensor = self.apply_normalization(image, self.parameters.normalization)
+        image = resize(image, self.get_input_shape()[1:3])
+        tensor = self.apply_normalization(
+            image, self.parameters.normalization, self.get_input_type())
+        # Convert shapes (1,64,64) to (1,64,64,3)
+        if len(tensor.shape) < 4:
+            tensor = np.expand_dims(tensor, axis=3)
+            tensor = np.repeat(tensor, repeats=3, axis=3)
         load_ns = clock_now() - start
         self.loading_input_timings.append(load_ns * 1e-6)
 
-        start = clock_now()
-        outputs = self.loaded_model.predict(tensor, verbose=0)
-        infer_ns = clock_now() - start
-        self.inference_timings.append(infer_ns * 1e-6)
+        """Inference"""
+        try: # This is for a Keras saved model or H5 file.
+            start = clock_now()
+            outputs = self.loaded_model.predict(tensor, verbose=0)
+            infer_ns = clock_now() - start
+            self.inference_timings.append(infer_ns * 1e-6)
+        except AttributeError: # This is for a Tensorflow saved model.
+            start = clock_now()
+            outputs = self.loaded_model(tensor)
+            infer_ns = clock_now() - start
+            self.inference_timings.append(infer_ns * 1e-6)
 
+        """Postprocessing"""
         start = clock_now()
         boxes, classes, scores = self.postprocessing(outputs)
         boxes_ns = clock_now() - start
         self.box_timings.append(boxes_ns * 1e-6)
         return boxes, classes, scores
 
     def postprocessing(
             self, 
-            outputs: np.ndarray
+            outputs: tuple
         ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
         """
-        Extracts the boxes, labels, and scores using tensorflow NMS.
+        Extracts the boxes, labels, and scores using TensorFlow NMS.
 
         Parameters
         ----------
-            outputs: np.ndarray
-                This contains bounding boxes, scores, labels.
+            outputs: tuple
+                Internally converted models have lengths of 2 where
+                boxes = outputs[-2] and scores = outputs[-1].
+
+                YoloV5 converted models have lengths of 1 where the element
+                has the shape (1, 25200, 85) for coco models.
+
+                YoloV7 currently supports ONNX and TensorRT conversion.
 
         Returns
         -------
             boxes: np.ndarray
                 The prediction bounding boxes.. [[box1], [box2], ...].
 
             classes: np.ndarray
@@ -146,98 +225,225 @@
             scores: np.ndarray
                 The prediction confidence scores.. [score, score, ...]
                 normalized between 0 and 1.
 
         Raises
         ------
             MissingLibraryException
-                Raised if the tensorflow library is not installed.
+                Raised if the TensorFlow library is not installed.
 
             NonMatchingIndexException
                 Raised if the model label index is
                 out of bounds to the input labels list.
         """
         try:
             os.environ['TF_CPP_MIN_LOG_LEVEL'] = '3'
             import tensorflow as tf
         except ImportError:
             raise MissingLibraryException(
-                "tensorflow is needed to perform NMS operations.")
+                "tensorflow>=2.8.0,<2.16.0 is needed to perform NMS operations.")
+    
+        if len(outputs) < 2:
+            if tf.is_tensor(outputs[0]): # YoloV5 keras converted model.
+                nmsed_boxes, nmsed_classes, nmsed_scores = self.process_yolo_standard(outputs)
+            else: # YoloV5 keras converted model with NMS.
+                nmsed_boxes, nmsed_classes, nmsed_scores = self.process_yolo_nms(outputs[0])
+        else: 
+            # The outputs here is either a list or a tuple. Either of length 2 or 4.
+            # The elements are either numpy array or tf.Tensor.
+            # The difference is relied upon the shape at the last 2 element.
+            # For YoloV5 models, the shape is [1, 100] or similar for classes.
+            # Internally, the shape is [1, 6000, 1, 4], (1, 1935, 1, 4), or similar for boxes.
+            if len(outputs[-2].shape) == 4: # Internal converted model.
+                nmsed_boxes, nmsed_classes, nmsed_scores = self.process_internal(outputs)    
+            else: # YoloV5 tensorflow converted model with NMS.
+                nmsed_boxes, nmsed_classes, nmsed_scores = self.process_yolo_nms(outputs)
+
+        if self.parameters.class_filter:
+            nmsed_boxes, nmsed_classes, nmsed_scores = self.class_filter(
+                nmsed_boxes, nmsed_classes, nmsed_scores
+            )
+        nmsed_classes = self.index2string(nmsed_classes)
+        return nmsed_boxes, nmsed_classes, nmsed_scores
+    
+    def process_internal(self, outputs: tuple) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
+        """
+        This methods process model outputs that were trained internally.
+
+        Parameters
+        ----------
+            outputs: tuple
+                This has a length of either 2 or 4 which contains 
+                boxes = outputs[-2] and scores = outputs[-1] at the last indices.
 
+        Returns
+        -------
+            nmsed_boxes: np.ndarray
+                Model bounding boxes after NMS.
+            
+            nmsed_classes: np.ndarray
+                Model classes after NMS.
+            
+            nmsed_scores: np.ndarray
+                Model scores after NMS.
+        """
         boxes = outputs[-2]
-        if self.parameters.label_offset > 0:
-            scores = outputs[-1][..., self.parameters.label_offset:]
+        # Negative offsets could mean that the model contains the background class,
+        # but the dataset does not.
+        if self.parameters.label_offset < 0:
+            scores = outputs[-1][..., abs(self.parameters.label_offset):]
+        # Positive offsets could mean that the dataset contains the background class,
+        # but the dataset does not.
+        # TODO: Consider cases where the offset might be positive.
         else:
             scores = outputs[-1]
 
-        if self.parameters.max_detections is None:
-            self.parameters.max_detections = 100
+        return self.tensorflow_nms(boxes, scores)
+    
+    def process_yolo_standard(self, outputs: tuple) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
+        """
+        This method processes the outputs of the model that was converted in 
+        YoloV5.
+
+        Parameters
+        ----------
+            outputs: tuple
+                This has a length of 1 which contains a torch.Tensor of shape
+                (batch_size, number of boxes, number of classes).
+
+        Returns
+        -------
+            nmsed_boxes: np.ndarray
+                Model bounding boxes after NMS.
+            
+            nmsed_classes: np.ndarray
+                Model classes after NMS.
+            
+            nmsed_scores: np.ndarray
+                Model scores after NMS.
+        """
+        h, w = self.get_input_shape()[1:3]
+        outputs = [x if isinstance(x, np.ndarray) else x.numpy() for x in outputs]
+        # NMS requires non-normalized coordinates.
+        outputs[0][..., :4] *= [w, h, w, h]  # xywh normalized to pixels.
         
-        nmsed_boxes, nmsed_scores, nmsed_classes, valid_boxes = \
-            tf.image.combined_non_max_suppression(
-                boxes,
-                scores,
-                self.parameters.max_detections,
-                self.parameters.max_detections,
-                iou_threshold=self.parameters.detection_iou,
-                score_threshold=self.parameters.detection_score,
-                clip_boxes=False)
+        if isinstance(outputs, (list, tuple)):
+            output = self.from_numpy(outputs[0]) if len(outputs) == 1 else [
+                self.from_numpy(x) for x in outputs]
+        else:
+            output = self.from_numpy(outputs)
 
-        nmsed_boxes = nmsed_boxes.numpy()
-        nmsed_classes = tf.cast(nmsed_classes, tf.int32)
+        # Currently it is a tuple with length of 1 (YoloV5) or 2 (Internal)
+        #output = self.from_numpy(outputs[0])
+        output = self.torch_nms(output)
+
+        outputs = output[0].numpy()
+        outputs[..., :4] /= [w, h, w, h]
+        nmsed_boxes = outputs[..., :4]
+        # Single dimensional arrays gets converted to the element. 
+        # Specify the axis into 1 to prevent that.
+        nmsed_scores = np.squeeze(outputs[..., 4:5], axis=1)
+        nmsed_classes = np.squeeze(outputs[...,5:6], axis=1)
+
+        if self.parameters.label_offset != 0:
+            nmsed_classes += self.parameters.label_offset
+        return nmsed_boxes, nmsed_classes, nmsed_scores
+    
+    def process_yolo_nms(self, outputs: list) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
+        """
+        This method processes the outputs of the model that was converted in
+        YoloV5 which embeds the NMS.
+
+        Parameters
+        ----------
+            outputs: list or CombinedNonMaxSuppression
+                This can be unpacked into boxes, scores, classes, and valid boxes.
+                The output of tf.image.combined_non_max_suppression method.
 
-        nms_predicted_boxes = [nmsed_boxes[i, :valid_boxes[i], :]
-                               for i in range(nmsed_boxes.shape[0])][0]
-        nms_predicted_classes = [nmsed_classes.numpy()[i, :valid_boxes[i]]
-                                 for i in range(nmsed_classes.shape[0])][0]
-        nms_predicted_scores = [nmsed_scores.numpy()[i, :valid_boxes[i]]
-                                for i in range(nmsed_scores.shape[0])][0]
-
-        if len(self.labels) > 0:
-            string_nms_predicted_classes = list()
-            for cls in nms_predicted_classes:
-                try:
-                    string_nms_predicted_classes.append(self.labels[int(cls)])
-                except IndexError:
-                    raise NonMatchingIndexException(cls)
-            nms_predicted_classes = np.array(string_nms_predicted_classes)
-        return nms_predicted_boxes, nms_predicted_classes, nms_predicted_scores
+        Returns
+        -------
+            nms_predicted_boxes: np.ndarray
+                This contains only the valid bounding boxes.
+            
+            nms_predicted_classes: np.ndarray
+                This contains only the valid bounding boxes.
+            
+            nms_predicted_scores: np.ndarray
+                This contains only the valid bounding boxes.
+        """
+        try:
+            os.environ['TF_CPP_MIN_LOG_LEVEL'] = '3'
+            import tensorflow as tf
+        except ImportError:
+            raise MissingLibraryException(
+                "tensorflow>=2.8.0,<2.16.0 is needed for Keras models.")
+        
+        nmsed_boxes, nmsed_scores, nmsed_classes, valid_boxes = outputs
+                
+        nmsed_classes = tf.cast(nmsed_classes, tf.int32)
+        return self.tensorflow_nms_filter(
+            nmsed_boxes, nmsed_scores, nmsed_classes, valid_boxes
+        )
 
-    def get_input_type(self):
+    def get_input_type(self) -> str:
         """
         Returns the model input type.
         
         Returns
         -------
             type: str
                 The model input type.
         """
-        return 'float32'
+        try:
+            return self.loaded_model.input.dtype.as_numpy_dtype
+        except AttributeError:
+            return self.inputs[0].dtype.as_numpy_dtype
+        
+    def get_input_shape(self):
+        """
+        Grabs the model input shape.
 
+        Returns
+        -------
+            type: tuple or list
+                The model input shape.
+        """
+        try:
+            return self.loaded_model.input.shape
+        except AttributeError:
+            return self.inputs[0].shape
+        
     def get_output_type(self):
         """
-        Returns the model output type.
+        Returns the model output type of the first output.
 
         Returns
         -------
-            type: str
+            type: tf.float32
                 The model output type.
         """
-        return 'float32'
-
-    def get_input_shape(self):
+        try:
+            return self.loaded_model.output[-1].dtype.as_numpy_dtype
+        except AttributeError:
+            return self.outputs[-1].dtype.as_numpy_dtype
+    
+    def get_output_shape(self):
         """
-        Grabs the model input shape.
+        Grabs the model output shape of the first output.
 
         Returns
         -------
             type: tuple or list
-                The model input shape.
+                The model output shape.
         """
-        return self.loaded_model.input.shape
+        try:
+            return self.loaded_model.output[-1].shape
+        except AttributeError:
+            return self.outputs[-1].shape
+
 
 class SegmentationKerasRunner(Runner):
     """
     Runs Keras models to produce segmentation masks.
   
     Parameters
     -----------
@@ -247,34 +453,39 @@
         parameters: Parameters
             This object contains the model parameters configured from the
             command line.
 
     Raises
     ------
         MissingLibraryException:
-            Raised if the the tensorflow library
+            Raised if the the TensorFlow library
             which is used to load and run a keras model is not installed.
     """
     def __init__(
             self, 
             model,
             parameters: Parameters
         ):
-        super(SegmentationKerasRunner, self).__init__(model=model)
+        super(SegmentationKerasRunner, self).__init__(model, parameters)
 
         try:
             os.environ['TF_CPP_MIN_LOG_LEVEL'] = '3'
             import tensorflow as tf
         except ImportError:
             raise MissingLibraryException(
-                "Tensorflow is needed to load Keras models.")
+                "tensorflow>=2.8.0,<2.16.0 is needed to load Keras models.")
         
         if isinstance(model, str):
             model = self.validate_model_path(model)
-            self.loaded_model = tf.keras.models.load_model(model, compile=False)
+            if os.path.exists(os.path.join(model, "saved_model.pb")):
+                self.loaded_model = tf.saved_model.load(model)
+                self.inputs = self.loaded_model.signatures["serving_default"].inputs
+                self.outputs = self.loaded_model.signatures["serving_default"].outputs
+            else:
+                self.loaded_model = tf.keras.models.load_model(model, compile=False)
         else:
             self.loaded_model = model
             self.model = "Training Model"
 
         self.parameters = parameters
 
         if len(tf.config.list_physical_devices('GPU')):
@@ -301,53 +512,102 @@
                 This is the segmentation mask of the image 
                 where each pixel is represented by a class in
                 the image.
 
         Raises
         ------
             MissingLibraryException
-                Raised if the tensorflow library 
+                Raised if the TensorFlow library 
                 is not installed which is needed
                 to run a Keras model.
         """
         try:
             os.environ['TF_CPP_MIN_LOG_LEVEL'] = '3'
             import tensorflow as tf
         except ImportError:
             raise MissingLibraryException(
-                "Tensorflow i needed to load Keras models.")
+                "tensorflow>=2.8.0,<2.16.0 is needed to load Keras models.")
 
         start = clock_now()
-        image = resize(image, self.get_input_shape())
-        tensor = self.apply_normalization(image, self.parameters.normalization)
+        image = resize(image, self.get_input_shape()[1:3])
+        tensor = self.apply_normalization(
+            image, self.parameters.normalization, self.get_input_type())
         load_ns = clock_now() - start
         self.loading_input_timings.append(load_ns * 1e-6)
     
         start = clock_now()
-        output = self.loaded_model.predict(tensor, verbose=0)
+        try: # This is for a Keras saved model or H5 file.
+            outputs = self.loaded_model.predict(tensor, verbose=0)
+        except AttributeError: # This is for a Tensorflow saved model.
+            outputs = self.loaded_model(tensor)
         infer_ns = clock_now() - start
         self.inference_timings.append(infer_ns * 1e-6)
 
         start = clock_now()
-        mask = tf.argmax(output, axis=-1)[0].numpy().astype(np.uint8)
+        mask = tf.argmax(outputs, axis=-1)[0].numpy().astype(np.uint8)
         boxes_ns = clock_now() - start
         self.box_timings.append(boxes_ns * 1e-6)
         return mask
 
+    def get_input_type(self) -> str:
+        """
+        Returns the model input type.
+        
+        Returns
+        -------
+            type: str
+                The model input type.
+        """
+        try:
+            return self.loaded_model.input.dtype.as_numpy_dtype
+        except AttributeError:
+            return self.inputs[0].dtype.as_numpy_dtype
+
     def get_input_shape(self):
         """
         Returns the input shape of the Keras model.
         
         Returns
         -------
-            input shape: tuple
-                This is the model input shape (height, width).
+            input shape: tuple or list
+                This is the model input shape.
         """
-        _, model_height, model_width, _ = self.loaded_model.input.shape
-        return (model_height, model_width)
+        try:
+            return self.loaded_model.input.shape
+        except AttributeError:
+            return self.inputs[0].shape
+        
+    def get_output_type(self):
+        """
+        Returns the model output type of the first output.
+
+        Returns
+        -------
+            type: tf.float32
+                The model output type.
+        """
+        try:
+            return self.loaded_model.output[-1].dtype.as_numpy_dtype
+        except AttributeError:
+            return self.outputs[-1].dtype.as_numpy_dtype
+    
+    def get_output_shape(self):
+        """
+        Grabs the model output shape of the first output.
+
+        Returns
+        -------
+            type: tuple or list
+                The model output shape.
+        """
+        try:
+            return self.loaded_model.output[-1].shape
+        except AttributeError:
+            return self.outputs[-1].shape
+        
 
 class PoseKerasRunner(Runner):
     """
     Runs Keras pose models.
 
     Parameters
     ----------
@@ -357,33 +617,38 @@
         parameters: Parameters
             This object contains the model parameters configured from the
             command line.
 
     Raises
     -------
         MissingLibraryException
-            Raised if the tensorflow library is not installed.
+            Raised if the TensorFlow library is not installed.
     """
     def __init__(
             self, 
             model, 
             parameters: Parameters
         ):
-        super(PoseKerasRunner, self).__init__(model)
+        super(PoseKerasRunner, self).__init__(model, parameters)
 
         try:
             os.environ['TF_CPP_MIN_LOG_LEVEL'] = '3'
             import tensorflow as tf
         except ImportError:
             raise MissingLibraryException(
-                "Tensorflow is needed to load the model.")
+                "tensorflow>=2.8.0,<2.16.0 is needed to load the model.")
         
         if isinstance(model, str):
             model = self.validate_model_path(model)
-            self.loaded_model = tf.keras.models.load_model(model, compile=False)
+            if os.path.exists(os.path.join(model, "saved_model.pb")):
+                self.loaded_model = tf.saved_model.load(model)
+                self.inputs = self.loaded_model.signatures["serving_default"].inputs
+                self.outputs = self.loaded_model.signatures["serving_default"].outputs
+            else:
+                self.loaded_model = tf.keras.models.load_model(model, compile=False)
         else:
             self.loaded_model = model
             self.model = "Training Model"
 
         self.parameters = parameters
         
         if len(tf.config.list_physical_devices('GPU')):
@@ -409,32 +674,78 @@
             angles: list
                 The Euler angles roll, pitch, yaw.
 
             None
                 Place for supposed labels. TODO Replace None with actual labels.
         """
         start = clock_now()
-        image = resize(image, self.get_input_shape())
-        tensor = self.apply_normalization(image, self.parameters.normalization)
+        image = resize(image, self.get_input_shape()[1:3])
+        tensor = self.apply_normalization(
+            image, self.parameters.normalization, self.get_input_type())
         load_ns = clock_now() - start
         self.loading_input_timings.append(load_ns * 1e-6)
 
         start = clock_now()
         outputs = self.loaded_model.predict(tensor, verbose=0)
         infer_ns = clock_now() - start
         self.inference_timings.append(infer_ns * 1e-6)
 
         start = clock_now()
         boxes_ns = clock_now() - start
         self.box_timings.append(boxes_ns * 1e-6)
         return outputs[0], None
 
+    def get_input_type(self) -> str:
+        """
+        Returns the model input type.
+        
+        Returns
+        -------
+            type: str
+                The model input type.
+        """
+        try:
+            return self.loaded_model.input.dtype.as_numpy_dtype
+        except AttributeError:
+            return self.inputs[0].dtype.as_numpy_dtype
+
     def get_input_shape(self):
         """
         Returns the model input shape.
        
         Returns
         -------
             type: tuple or list
                 The model input shape.
         """
-        return self.loaded_model.input.shape[1:]
+        try:
+            return self.loaded_model.input.shape
+        except AttributeError:
+            return self.inputs[0].shape
+        
+    def get_output_type(self):
+        """
+        Returns the model output type of the first output.
+
+        Returns
+        -------
+            type: tf.float32
+                The model output type.
+        """
+        try:
+            return self.loaded_model.output[-1].dtype.as_numpy_dtype
+        except AttributeError:
+            return self.outputs[-1].dtype.as_numpy_dtype
+    
+    def get_output_shape(self):
+        """
+        Grabs the model output shape of the first output.
+
+        Returns
+        -------
+            type: tuple or list
+                The model output shape.
+        """
+        try:
+            return self.loaded_model.output[-1].shape
+        except AttributeError:
+            return self.outputs[-1].shape
```

## deepview/validator/runners/offline.py

```diff
@@ -5,15 +5,14 @@
 #
 # This source code is provided solely for runtime interpretation by Python.
 # Modifying or copying any source code is explicitly forbidden.
 
 from deepview.validator.exceptions import UnsupportedAnnotationFormatException
 from deepview.validator.exceptions import UnsupportedValidationTypeException
 from deepview.validator.metrics.segmentationutils import create_mask_image
-from deepview.validator.exceptions import NonMatchingIndexException
 from deepview.validator.datasets.core import Dataset
 from deepview.validator.runners.core import Runner
 from deepview.validator.datasets import Instance
 from typing import Tuple, Union
 import numpy as np
 import warnings
 import json
@@ -79,21 +78,17 @@
         annotation_source: str,
         labels: list=None,
         validate_type: str="detection",
         validate_3d: bool=False,
         format: str='yolo',
         label_offset: int=0
     ):
-        super(OfflineRunner, self).__init__(annotation_source)
-
-        if labels is None:
-            self.labels = list()
-        else:
-            self.labels = labels
+        super(OfflineRunner, self).__init__(annotation_source, labels=labels)
 
+        self.loaded_model = None
         self.label_offset = label_offset
         self.validate_3d = validate_3d
 
         self.define_denormalizer(validate_type)
         self.define_transformer(format)
         self.define_annotation_extension()
 
@@ -257,15 +252,15 @@
         
         elif self.validate_type == "segmentation":
             return self.process_segmentation(annotation)
         else:
             raise UnsupportedValidationTypeException(self.validate_type)
     
     def get_annotation(
-            self, annotation_path: str) -> Union[np.ndarray, dict] | None:
+            self, annotation_path: str) -> Union[Union[np.ndarray, dict], None]:
         """
         Reads the annotatation path provided to get 
         the information stored in the file.
 
         Parameters
         ----------
             annotation_path: str
@@ -316,15 +311,15 @@
             with open(annotation_path, "r") as fp:
                 return json.load(fp)
         except FileNotFoundError:
             return None
 
     def process_detection(
             self, 
-            annotation: np.ndarray | None
+            annotation: Union[np.ndarray, None]
         ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
         """
         Parses the annotation to grab the detection bounding 
         boxes, scores, and labels.
 
         Parameters
         ----------
@@ -349,35 +344,27 @@
                 that is out of bounds to the labels list passed.
         """
         if annotation is None:
             return np.array([]), np.array([]), np.array([])
         
         if len(annotation):
             annotation = annotation.reshape(-1, 6)
-            boxes = annotation[:, 2:6]
+            boxes = annotation[:, 1:5]
             boxes = self.transformer(boxes) if self.transformer else boxes
         else:
             return np.array([]), np.array([]), np.array([])
 
-        scores = annotation[:, 1:2].flatten().astype(np.float32)
+        scores = annotation[:, 5:6].flatten().astype(np.float32)
         labels = annotation[:, 0:1].flatten().astype(np.int32) + self.label_offset
-        
-        if len(self.labels) > 0:
-            string_labels = list()
-            for label in labels:
-                try:
-                    string_labels.append(self.labels[int(label)])
-                except IndexError:
-                    raise NonMatchingIndexException(label)
-            labels = np.array(string_labels)
+        labels = self.index2string(labels)
         return boxes, labels, scores
     
     def process_3d_detection(
             self, 
-            annotation: dict | None
+            annotation: Union[dict, None]
         ) -> Tuple[
             np.ndarray, np.ndarray, np.ndarray, np.ndarray, np.ndarray, np.ndarray]:
         """
         Parses the annotation to retrieve 3D bounding box information for
         the detections.
 
         Parameters
@@ -424,30 +411,22 @@
             return np.array([]), np.array([]), np.array([]), np.array([]), np.array([]), np.array([])
         
         centers = boxes_3d[:, 0:3]
         sizes = boxes_3d[:, 3:6]
         view = np.array(annotation.get("calibration"))
         boxes = np.array(annotation.get("boxes"))
         labels = boxes[:, 4:5].flatten().astype(np.int32) + self.label_offset
-  
-        if len(self.labels) > 0:
-            string_labels = list()
-            for label in labels:
-                try:
-                    string_labels.append(self.labels[int(label)])
-                except IndexError:
-                    raise NonMatchingIndexException(label)
-            labels = np.array(string_labels)
+        labels = self.index2string(labels)
         
         # This needs to be refactored to actual model scores in the future.
         scores = np.ones(len(labels))
         return centers, sizes, angles, view, labels, scores
     
     def process_pose(
-            self, annotation: dict | None) -> Tuple[np.ndarray, np.ndarray]:
+            self, annotation: Union[dict, None]) -> Tuple[np.ndarray, np.ndarray]:
         """
         Parses the annotation to get the euler angles.
 
         Parameters
         ----------
             annotation: dict
 
@@ -465,15 +444,15 @@
             labels: np.ndarray
                 The label representing each set of angles.
         """
         if annotation is None:
             return np.array([]), np.array([])
         return np.ndarray(annotation.get("angles")[0]), self.labels
     
-    def process_segmentation(self, annotation: dict | None) -> np.ndarray:
+    def process_segmentation(self, annotation: Union[dict, None]) -> np.ndarray:
         """
         Parses the annotations to get the segments and 
         create the detection mask.
 
         Parameters
         ----------
             annotation: dict
```

## deepview/validator/runners/onnx.py

```diff
@@ -7,19 +7,23 @@
 # Modifying or copying any source code is explicitly forbidden.
 
 from __future__ import annotations
 from typing import TYPE_CHECKING, Tuple, Union
 if TYPE_CHECKING:
     from deepview.validator.evaluators import Parameters
 
-from deepview.validator.exceptions import NonMatchingIndexException
 from deepview.validator.exceptions import MissingLibraryException
-from deepview.validator.datasets.utils import resize
+from deepview.validator.datasets.utils import (
+    letterbox_yolox,
+    resize, 
+)
 from deepview.validator.runners.core import Runner
+from deepview.validator.writers import logger
 from time import monotonic_ns as clock_now
+from timeit import timeit
 import numpy as np
 
 class ONNXRunner(Runner):
     """
     Runs ONNX models.
     
     Parameters
@@ -46,41 +50,98 @@
     """
     def __init__(
         self,
         model,
         parameters: Parameters,
         labels: list=None
     ):
-        super(ONNXRunner, self).__init__(model)
+        super(ONNXRunner, self).__init__(model, parameters, labels)
 
         try:
             import onnxruntime
         except ImportError:
             raise MissingLibraryException(
-                "onnxruntime or onnxruntime-gpu~=1.17.1 is needed to run ONNX models.")
+                "onnxruntime~=1.16.3 or onnxruntime-gpu~=1.16.3 is needed to run ONNX models.")
         try:
             import torch
         except ImportError:
             raise MissingLibraryException(
-                "torchvision is needed to check for cuda.")
+                "torchvision~=0.15.2 is needed to check for cuda.")
         
         if isinstance(model, str):
             model = self.validate_model_path(model)
             cuda = torch.cuda.is_available() and parameters.engine != "cpu"  # use CUDA
             providers = ["CUDAExecutionProvider", "CPUExecutionProvider"] if cuda else ["CPUExecutionProvider"]
             self.session = onnxruntime.InferenceSession(model, providers=providers)
             self.output_names = [x.name for x in self.session.get_outputs()]
+            self.graph_name = self.session.get_modelmeta().graph_name
         else:
             self.session = model
             self.model = "Training Model"
 
-        self.parameters = parameters
-        self.labels = []
-        if labels is not None:
-            self.labels = labels
+        self.update_nms()
+        self.update_engine()
+
+        if self.parameters.warmup > 0:
+            # Produce a sample image of zeros.
+            input_type = "float32" if "float" in self.get_input_type() else "uint32"
+            height, width = self.get_input_shape()[2:4]
+            image = np.expand_dims(np.zeros((height, width, 3)), 0).astype(np.dtype(input_type))
+            image = np.transpose(image, axes=[0,3,1,2])
+            logger("Loading model and warmup...", code="INFO")
+            t = timeit(lambda: self.session.run(
+                self.output_names, 
+                {self.session.get_inputs()[0].name: image}), 
+                number=self.parameters.warmup)
+            logger("model warmup took %f seconds (%f ms avg)" %
+                    (t, t * 1000 / self.parameters.warmup), code="INFO")
+        
+        # When filtering the model detection classes against the ground truth,
+        # don't perform the auto offset.
+        if (self.parameters.label_offset == 0 and 
+            self.parameters.auto_offset and 
+            not self.parameters.class_filter):
+            self.parameters.label_offset = self.auto_offset()
+            
+    def auto_offset(self) -> int:
+        """
+        Initialize an auto offset parameter to reduce complexity for the
+        manually setting the offset of the model indices due to 
+        integer to string mapping mismatches.
+
+        This is done by comparing the number of labels in the ground truth
+        and the model outputs. Common patterns are for a coco128 model.
+
+        ```
+        shape=[1, 25200, 85]
+        ```
+
+        From this article https://medium.com/@KrashKart/i-wish-i-knew-this-about-yolov5-2fbab3584906,
+        the first 5 rows (index 0 to 4) indicate, the probability of bounding 
+        box coordinates (xmin, ymin, xmax, ymax) as well as the objectness per 
+        grid cell for all grid cells.
+
+        The next rows (5 to 85 in this case) are the probability of class 
+        i existing at all grid cells.
+
+        Returns
+        -------
+            offset: int
+                The offset to apply towards the model indices.
+        """
+        shape = self.get_output_shape()
+        if len(shape) == 3:
+            yolo_converted = shape[-1] - 5
+            label_count = yolo_converted if yolo_converted == len(self.labels) else shape[-1]
+        else:
+            label_count = 0
+
+        if len(self.labels) == 0 or label_count == 0:
+            return 0
+        return len(self.labels) - label_count
 
     def run_single_instance(
         self, 
         image: Union[str, np.ndarray]
     ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
         """
         Produce ONNX inference on one image and records the timings. 
@@ -107,142 +168,346 @@
             nmsed_scores: np.ndarray
                 The prediction confidence scores.. [score, score, ...]
                 normalized between 0 and 1.
         """
 
         """Input Preprocessing"""
         start = clock_now()
-        # Take only the (height, width).
-        image = resize(image, self.get_input_shape()[2:4]) 
+        height, width, _ = image.shape
+        if self.parameters.letterbox:
+            image, ratio = letterbox_yolox(image, self.get_input_shape()[2:4])
+        else:
+            # Take only the (height, width).
+            image = resize(image, self.get_input_shape()[2:4]) 
+            ratio = 1.0
         input_type = "float32" if "float" in self.get_input_type() else "uint32"
         image = self.apply_normalization(
             image, self.parameters.normalization, input_type)
+        # Expects batch size, channel, height, width.
         image = np.transpose(image, axes=[0,3,1,2])
         load_ns = clock_now() - start
         self.loading_input_timings.append(load_ns * 1e-6)
 
         """Inference"""
         start = clock_now()
-        y = self.session.run(self.output_names, {self.session.get_inputs()[0].name: image})
-        if isinstance(y, (list, tuple)):
-            output = self.from_numpy(y[0]) if len(y) == 1 else [
-                self.from_numpy(x) for x in y]
-        else:
-            output = self.from_numpy(y)
+        outputs = self.session.run(self.output_names, {self.session.get_inputs()[0].name: image})
         infer_ns = clock_now() - start
         self.inference_timings.append(infer_ns * 1e-6)
 
         """Postprocessing"""
         start = clock_now()
         # An output with 7 columns refers to batch_id, xmin, ymin, xmax, ymax, cls, score.
         # Otherwise it is batch_size, number of boxes, number of classes which needs external NMS.
-        if output.shape[1] != 7:
-            output = self.non_max_supression(output)
-        nmsed_boxes, nmsed_classes, nmsed_scores = self.postprocessing(output)
+        nmsed_boxes, nmsed_classes, nmsed_scores = self.postprocessing(outputs, ratio, (height, width))
         decoder_ns = clock_now() - start
         self.box_timings.append(decoder_ns * 1e-6)
         return nmsed_boxes, nmsed_classes, nmsed_scores
 
     def postprocessing(
-            self, output: list) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
-        """
-        Retrieves the boxes, scores and labels.
+            self, 
+            output: Union[list, np.ndarray],
+            ratio: float,
+            image_shape: tuple,
+        ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
+        """
+        Retrieves the boxes, scores and labels. This method will perform NMS
+        operations where the outputs will be transformed into the following format.
+
+        Models converted internally will directly return the nms
+        bounding boxes, scores, and labels as described below.
+
+        Models converted in YoloV5 will be a list of length 1 which 
+        is formatted in the following way which has a shape of (1, number of boxes, 6).
+        [[[xmin, ymin, xmax, ymax, confidence, label], [...], ...]]. 
+
+        Models converted in YoloV7 will extract the bounding boxes, scores,
+        and labels from the output and directly return.
 
         Parameters
         ----------
-            outputs:
-                This contains bounding boxes, scores, labels in the format.
-                [[xmin, ymin, xmax, ymax, confidence, label], [...], ...].
+            output: list or np.ndarray
+
+                Pre NMS
+                -------
+                Models converted internally will be a list with length of 2
+                containing the bounding boxes as the first element and the scores
+                for the second element which needs to be passed to NMS.
+
+                Models converted in YoloV5 requires torch NMS which has the 
+                following shape (batch size, number of boxes, number of classes).
+                The output is a torch.Tensor.
+
+                Models converted in YoloV7 will already have NMS embedded. The
+                output will be a torch.Tensor in the following format which 
+                has a shape of (number of boxes, 7).
+                [[batch_id, xmin, ymin, xmax, ymax, cls, score], ...]
+
+            ratio: float
+                This is the ratio value from the letterbox transformation
+                to adjust the bounding boxes.
+
+            image_shape: tuple
+                This is the original resolution of the image to normalize
+                coordinates.
 
         Returns
         -------
             nmsed_boxes: np.ndarray
                 The prediction bounding boxes.. [[box1], [box2], ...].
 
             nmsed_classes: np.ndarray
                 The prediction labels.. [cl1, cl2, ...].
 
             nmsed_scores: np.ndarray
                 The prediction confidence scores.. [score, score, ...]
                 normalized between 0 and 1.
         """
-        h, w = self.get_input_shape()[2:4]
+        # Indicates YOLOv5, YOLOv7 exported models.
+        if self.graph_name == "main_graph":
+            # Convert to NumPy.
+            if isinstance(output, (list, tuple)):
+                output = self.from_numpy(output[0]) if len(output) == 1 else [
+                    self.from_numpy(x) for x in output]
+            else:
+                output = self.from_numpy(output)
 
         if isinstance(output, list):
+            if self.graph_name != "main_graph":
+                nmsed_boxes, nmsed_classes, nmsed_scores = self.process_yolox(output, ratio, image_shape)
+            else:
+                nmsed_boxes, nmsed_classes, nmsed_scores = self.process_internal(output)
+        else:
+            nmsed_boxes, nmsed_classes, nmsed_scores = self.process_yolov(output)
+
+        if self.parameters.class_filter:
+            nmsed_boxes, nmsed_classes, nmsed_scores = self.class_filter(
+                nmsed_boxes, nmsed_classes, nmsed_scores
+            )
+        if self.parameters.label_offset != 0:
+            nmsed_classes += self.parameters.label_offset
+        nmsed_classes = self.index2string(nmsed_classes)
+        return nmsed_boxes, nmsed_classes, nmsed_scores
+    
+    def process_internal(
+            self, 
+            output: Union[list, np.ndarray]
+        ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
+        """
+        Process internal exported models.
+
+        Parameters
+        ----------
+            output: list, np.ndarray
+                Models converted internally will be a list with length of 2
+                containing the bounding boxes as the first element and the scores
+                for the second element which needs to be passed to NMS.
+
+        Returns
+        -------
+            nmsed_boxes: np.ndarray
+                The prediction bounding boxes.. [[box1], [box2], ...].
+
+            nmsed_classes: np.ndarray
+                The prediction labels.. [cl1, cl2, ...].
+
+            nmsed_scores: np.ndarray
+                The prediction confidence scores.. [score, score, ...]
+                normalized between 0 and 1.
+        """
+        if len(output) == 2: # Internal converted model.
+            return self.tensorflow_nms(
+                    output[0].reshape([1,-1,1,4]) / self.get_input_shape()[2],
+                    output[1], 
+                    clip_boxes=True)
+        else:
+            logger("Postprocessing for this model output is not yet supported.", code="ERROR")
+    
+    def process_yolov(
+            self, 
+            output: Union[list, np.ndarray]
+        ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
+        """
+        Process YOLOv5 and YOLOv7 exported models.
+
+        Parameters
+        ----------
+            output: list or np.ndarray
+                Models converted in YoloV5 requires torch NMS which has the 
+                following shape (batch size, number of boxes, number of classes).
+                The output is a torch.Tensor.
+
+                Models converted in YoloV7 will already have NMS embedded. The
+                output will be a torch.Tensor in the following format which 
+                has a shape of (number of boxes, 7).
+                [[batch_id, xmin, ymin, xmax, ymax, cls, score], ...]
+
+        Returns
+        -------
+            nmsed_boxes: np.ndarray
+                The prediction bounding boxes.. [[box1], [box2], ...].
+
+            nmsed_classes: np.ndarray
+                The prediction labels.. [cl1, cl2, ...].
+
+            nmsed_scores: np.ndarray
+                The prediction confidence scores.. [score, score, ...]
+                normalized between 0 and 1.
+        """
+        h, w = self.get_input_shape()[2:4]
+        # YoloV5 converted model.
+        if output.shape[1] != 7:
+            output = self.torch_nms(output)
             outputs = output[0].numpy()
             outputs[..., :4] /= [w, h, w, h]
 
             nmsed_boxes = outputs[..., :4]
             # Single dimensional arrays gets converted to the element. 
             # Specify the axis into 1 to prevent that.
             nmsed_scores = np.squeeze(outputs[..., 4:5], axis=1)
-        else:
+        # YoloV7 converted model.
+        else: 
             outputs = output.numpy()
             outputs[..., 1:5] /= [w, h, w, h]
             nmsed_boxes = outputs[..., 1:5]
             # Single dimensional arrays gets converted to the element. 
             # Specify the axis into 1 to prevent that.
             nmsed_scores = np.squeeze(outputs[..., 6:7], axis=1)
-        
-        nmsed_classes = np.squeeze(outputs[...,5:6], axis=1) + self.parameters.label_offset
-        if len(self.labels) > 0:
-            string_nms_predicted_classes = list()
-            for cls in nmsed_classes:
-                try:
-                    string_nms_predicted_classes.append(self.labels[int(cls)])
-                except IndexError:
-                    raise NonMatchingIndexException(cls)
-            nmsed_classes = np.array(string_nms_predicted_classes)
+        nmsed_classes = np.squeeze(outputs[...,5:6], axis=1)
         return nmsed_boxes, nmsed_classes, nmsed_scores
-    
-    def get_input_type(self) -> str:
+
+    def process_yolox(
+            self, 
+            outputs: Union[list, np.ndarray], 
+            ratio: float,
+            image_shape: tuple,
+            p6: bool=False
+        ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
         """
-        This returns the input type of the model.
+        This performs postprocessing of YOLOx models.
+        Method taken from https://github.com/Megvii-BaseDetection/YOLOX/blob/main/yolox/utils/demo_utils.py#L139
+
+        Parameters
+        ----------
+            output: list or np.ndarray
+                This is the output of the model to postprocess into
+                bounding boxes, classes, scores after NMS.
+
+            ratio: float
+                This is the ratio value from the letterbox transformation
+                to adjust the bounding boxes.
+
+            image_shape: tuple
+                This is the original resolution of the image to normalize
+                coordinates.
+
+            p6: bool
 
         Returns
         -------
-            type: str
-                The input type of the model.
+            nmsed_boxes: np.ndarray
+                The prediction bounding boxes.. [[box1], [box2], ...].
+
+            nmsed_classes: np.ndarray
+                The prediction labels.. [cl1, cl2, ...].
+
+            nmsed_scores: np.ndarray
+                The prediction confidence scores.. [score, score, ...]
+                normalized between 0 and 1.
         """
-        return self.session.get_inputs()[0].type
-    
-    def get_output_type(self) -> str:
+        height, width = self.get_input_shape()[2:4]
+
+        grids = []
+        expanded_strides = []
+        strides = [8, 16, 32] if not p6 else [8, 16, 32, 64]
+
+        hsizes = [height // stride for stride in strides]
+        wsizes = [width // stride for stride in strides]
+        output = outputs[0]
+        for hsize, wsize, stride in zip(hsizes, wsizes, strides):
+            xv, yv = np.meshgrid(np.arange(wsize), np.arange(hsize))
+            grid = np.stack((xv, yv), 2).reshape(1, -1, 2)
+            grids.append(grid)
+            shape = grid.shape[:2]
+            expanded_strides.append(np.full((*shape, 1), stride))
+
+        grids = np.concatenate(grids, 1)
+        expanded_strides = np.concatenate(expanded_strides, 1)
+        output[..., :2] = (output[..., :2] + grids) * expanded_strides
+        output[..., 2:4] = np.exp(output[..., 2:4]) * expanded_strides
+        predictions = output[0]
+        boxes = predictions[:, :4]
+        scores = predictions[:, 4:5] * predictions[:, 5:]
+
+        boxes_xyxy = np.ones_like(boxes)
+        boxes_xyxy[:, 0] = boxes[:, 0] - boxes[:, 2]/2.
+        boxes_xyxy[:, 1] = boxes[:, 1] - boxes[:, 3]/2.
+        boxes_xyxy[:, 2] = boxes[:, 0] + boxes[:, 2]/2.
+        boxes_xyxy[:, 3] = boxes[:, 1] + boxes[:, 3]/2.
+        boxes_xyxy /= ratio
+
+        # Typical: nms_thr=0.45, score_thr=0.1
+        dets = self.multiclass_nms(
+            boxes_xyxy, 
+            scores, 
+            nms_thr=self.parameters.detection_iou, 
+            score_thr=self.parameters.detection_score
+        )
+        if dets is None:
+            return np.array([]), np.array([]), np.array([])
+        nmsed_boxes = dets[:, :4]
+        nmsed_scores = dets[:, 4]
+        nmsed_classes = dets[:, 5]
+        nmsed_boxes /= [image_shape[1], image_shape[0], image_shape[1], image_shape[0]]
+        return nmsed_boxes, nmsed_classes, nmsed_scores
+
+    def get_input_type(self) -> str:
         """
-        This returns the output type of the model.
+        This returns the input type of the model.
 
         Returns
         -------
             type: str
-                The output type of the model.
+                The input type of the model.
         """
-        return self.session.get_outputs()[0].type
+        return self.session.get_inputs()[0].type
 
     def get_input_shape(self) -> np.ndarray:
         """
         Grabs the model input shape.
 
         Returns
         -------
             shape: np.ndarray
                 The model input shape.
                 (batch size, channels, height, width).
         """
         return self.session.get_inputs()[0].shape
     
+    def get_output_type(self) -> str:
+        """
+        This returns the output type of the model.
+
+        Returns
+        -------
+            type: str
+                The output type of the model.
+        """
+        return self.session.get_outputs()[-1].type
+    
     def get_output_shape(self) -> np.ndarray:
         """
         Grabs the model output shape.
 
         Returns
         --------
             shape: np.ndarray
                 The model output shape.
                 (batch size, boxes, classes).
         """
-        return self.session.get_outputs()[0].shape
+        return self.session.get_outputs()[-1].shape
     
     def get_metadata(self) -> dict:
         """
         This returns the model metadata containing stride and label names
         mapping.
 
         Returns
```

## deepview/validator/runners/tensorrt.py

```diff
@@ -55,15 +55,15 @@
     def __init__(
         self,
         model: str,
         parameters: Parameters,
         labels: list=None,
         preprocessor: str="EfficientDet",
     ):
-        super(TensorRTRunner, self).__init__(model)
+        super(TensorRTRunner, self).__init__(model, parameters, labels)
 
         try:
             import tensorrt as trt
         except ImportError:
             raise MissingLibraryException(
                 "tensorrt is needed to allow running of tensorRT engines.")
         try:
@@ -79,20 +79,14 @@
             import pycuda.autoprimaryctx # type: ignore
         except ModuleNotFoundError:
             try:
                 import pycuda.autoinit # type: ignore
             except ImportError:
                 raise MissingLibraryException(
                     "supported NVIDIA GPU device is needed.")
-        
-        self.parameters = parameters
-        if labels is None:
-            self.labels = []
-        else:
-            self.labels = labels
 
         self.preprocessor = preprocessor
         self.parameters.engine = "gpu"
 
         # Load TRT engine
         self.logger = trt.Logger(trt.Logger.ERROR)
         trt.init_libnvinfer_plugins(self.logger, namespace="")
```

## deepview/validator/runners/tflite.py

```diff
@@ -7,15 +7,14 @@
 # Modifying or copying any source code is explicitly forbidden.
 
 from __future__ import annotations
 from typing import TYPE_CHECKING, Tuple, Union
 if TYPE_CHECKING:
     from deepview.validator.evaluators import Parameters
 
-from deepview.validator.exceptions import NonMatchingIndexException
 from deepview.validator.exceptions import MissingLibraryException
 from deepview.validator.datasets.utils import resize
 from deepview.validator.runners.core import Runner
 from deepview.validator.writers import logger
 from time import monotonic_ns as clock_now
 from timeit import timeit
 import numpy as np
@@ -48,50 +47,89 @@
     """
     def __init__(
         self,
         model,
         parameters: Parameters,
         labels: list=None
     ):
-        super(TFliteRunner, self).__init__(model)
+        super(TFliteRunner, self).__init__(model, parameters, labels)
         try:  # https://coral.ai/docs/edgetpu/tflite-python/#update-existing-tf-lite-code-for-the-edge-tpu
-            from tflite_runtime.interpreter import ( 
+            from tflite_runtime.interpreter import (  # type: ignore
                 Interpreter, 
                 load_delegate
             ) 
         except ImportError:
             try:
                 import tensorflow as tf
                 Interpreter, load_delegate = ( # NOSONAR
                     tf.lite.Interpreter,
                     tf.lite.experimental.load_delegate,
                 )
             except ImportError:
                 raise MissingLibraryException(
-                    "tensorflow or tflite_runtime is needed to load the model.")
+                    "tensorflow>=2.8.0,<2.16.0 or tflite_runtime is needed to load the model. ")
 
         if isinstance(model, str):
             model = self.validate_model_path(model)
             self.interpreter = Interpreter(model_path=model)  # load TFLite model
         else:
             self.interpreter = model
             self.model = "Training Model"
 
         self.interpreter.allocate_tensors()  # allocate
-        self.parameters = parameters
-
-        self.labels = []
-        if labels is not None:
-            self.labels = labels
+        self.update_nms()
+        self.update_engine()
     
         if self.parameters.warmup > 0:
             logger("Loading model and warmup...", code="INFO")
             t = timeit(self.interpreter.invoke, number=self.parameters.warmup)
             logger("model warmup took %f seconds (%f ms avg)" %
                            (t, t * 1000 / self.parameters.warmup), code="INFO")
+
+        if (self.parameters.label_offset == 0 and 
+            self.parameters.auto_offset and 
+            not self.parameters.class_filter):
+            self.parameters.label_offset = self.auto_offset()
+
+    def auto_offset(self) -> int:
+        """
+        Initialize an auto offset parameter to reduce complexity for the
+        manually setting the offset of the model indices due to 
+        integer to string mapping mismatches.
+
+        This is done by comparing the number of labels in the ground truth
+        and the model outputs. Common patterns are for a coco128 model.
+
+        ```
+        [    1, 25200,    85]
+        ```
+
+        From this article https://medium.com/@KrashKart/i-wish-i-knew-this-about-yolov5-2fbab3584906,
+        the first 5 rows (index 0 to 4) indicate, the probability of bounding 
+        box coordinates (xmin, ymin, xmax, ymax) as well as the objectness per 
+        grid cell for all grid cells.
+
+        The next rows (5 to 85 in this case) are the probability of class 
+        i existing at all grid cells.
+
+        Returns
+        -------
+            offset: int
+                The offset to apply towards the model indices.
+        """
+        shape = self.get_output_shape()
+        if len(shape) == 3:
+            yolo_converted = shape[-1] - 5
+            label_count = yolo_converted if yolo_converted == len(self.labels) else shape[-1]
+        else:
+            label_count = 0
+        
+        if len(self.labels) == 0 or label_count == 0:
+            return 0
+        return len(self.labels) - label_count
               
     def run_single_instance(
             self, 
             image: Union[str, np.ndarray]
         ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
         """
         Produce tflite predictions on one image and records the timings. 
@@ -131,124 +169,223 @@
         self.interpreter.set_tensor(input_details[0]['index'], tensor)
         load_ns = clock_now() - start
         self.loading_input_timings.append(load_ns * 1e-6)
         
         """Inference"""
         start = clock_now()
         self.interpreter.invoke()
-        y = []
+        infer_ns = clock_now() - start
+        self.inference_timings.append(infer_ns * 1e-6)
+
+        """Postprocessing"""
+        start = clock_now()
+        outputs = []
         for output in output_details:
             # is TFLite quantized uint8 model.
             int8 = input_details[0]["dtype"] == np.uint8  
             x = self.interpreter.get_tensor(output["index"])
             if int8:
                 scale, zero_point = output["quantization"]
                 x = (x.astype(np.float32) - zero_point) * scale  # re-scale
-            y.append(x)
-        y = [x if isinstance(x, np.ndarray) else x.numpy() for x in y]
-        h, w = self.get_input_shape()[1:3]
-        # NMS requires non-normalized coordinates.
-        y[0][..., :4] *= [w, h, w, h]  # xywh normalized to pixels.
-        if isinstance(y, (list, tuple)):
-            output_data = self.from_numpy(y[0]) if len(y) == 1 else [
-                self.from_numpy(x) for x in y]
-        else:
-            output_data = self.from_numpy(y)
-        infer_ns = clock_now() - start
-        self.inference_timings.append(infer_ns * 1e-6)
-
-        """Postprocessing"""
-        start = clock_now()
-        output = self.non_max_supression(output_data)
-        nmsed_boxes, nmsed_classes, nmsed_scores = self.postprocessing(output)
+            outputs.append(x)
+            
+        nmsed_boxes, nmsed_classes, nmsed_scores = self.postprocessing(outputs)
         decoder_ns = clock_now() - start
         self.box_timings.append(decoder_ns * 1e-6)
         return nmsed_boxes, nmsed_classes, nmsed_scores
 
     def postprocessing(
-            self, output: list) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
+            self, 
+            outputs: list
+        ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
         """
         Retrieves the boxes, scores and labels.
 
         Parameters
         ----------
-            outputs:
-                This contains bounding boxes, scores, labels in the format.
-                [[xmin, ymin, xmax, ymax, confidence, label], [...], ...].
+            output: list
+                This is the raw detections of the model with the following shape
+                (batch size, number of boxes, number of classes).
+
+                After NMS, it will be transformed into a list of length 1 with
+                a shape of (1, number of boxes, 6).
+                [[[xmin, ymin, xmax, ymax, confidence, label], [...], ...]]. 
 
         Returns
         -------
             nmsed_boxes: np.ndarray
                 The prediction bounding boxes.. [[box1], [box2], ...].
 
             nmsed_classes: np.ndarray
                 The prediction labels.. [cl1, cl2, ...].
 
             nmsed_scores: np.ndarray
                 The prediction confidence scores.. [score, score, ...]
                 normalized between 0 and 1.
         """
-        h, w = self.get_input_shape()[1:3]
-        outputs = output[0].numpy()
-        outputs[..., :4] /= [w, h, w, h]
-        
-        nmsed_boxes = outputs[..., :4]
-        # Single dimensional arrays gets converted to the element. 
-        # Specify the axis into 1 to prevent that.
-        nmsed_scores = np.squeeze(outputs[..., 4:5], axis=1)
-        nmsed_classes = np.squeeze(outputs[...,5:6], axis=1) + self.parameters.label_offset
-
-        if len(self.labels) > 0:
-            string_nms_predicted_classes = list()
-            for cls in nmsed_classes:
-                try:
-                    string_nms_predicted_classes.append(self.labels[int(cls)])
-                except IndexError:
-                    raise NonMatchingIndexException(cls)
-            nmsed_classes = np.array(string_nms_predicted_classes)
+        outputs = [x if isinstance(x, np.ndarray) else x.numpy() for x in outputs]
+        if len(outputs) == 2:
+            nmsed_boxes, nmsed_classes, nmsed_scores = self.process_internal(outputs)
+        else:
+            nmsed_boxes, nmsed_classes, nmsed_scores = self.process_yolov(outputs)
+
+        if self.parameters.class_filter:
+            nmsed_boxes, nmsed_classes, nmsed_scores = self.class_filter(
+                nmsed_boxes, nmsed_classes, nmsed_scores
+            )
+        if self.parameters.label_offset != 0:
+            nmsed_classes += self.parameters.label_offset
+        nmsed_classes = self.index2string(nmsed_classes)
         return nmsed_boxes, nmsed_classes, nmsed_scores
     
-    def get_input_type(self) -> str:
+    def process_internal(
+            self, 
+            outputs: list
+        ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
         """
-        This returns the input type of the model.
+        Process internal exported models.
+
+        Parameters
+        ----------
+            output: list, np.ndarray
+                Models converted internally will be a list with length of 2
+                containing the bounding boxes as the first element and the scores
+                for the second element which needs to be passed to NMS.
 
         Returns
         -------
-            type: str
-                The input type of the model.
+            nmsed_boxes: np.ndarray
+                The prediction bounding boxes.. [[box1], [box2], ...].
+
+            nmsed_classes: np.ndarray
+                The prediction labels.. [cl1, cl2, ...].
+
+            nmsed_scores: np.ndarray
+                The prediction confidence scores.. [score, score, ...]
+                normalized between 0 and 1.
         """
-        return self.interpreter.get_input_details()[0]["dtype"].__name__
+        for output in outputs:
+            if output.shape[-1] == 4:
+                boxes = output
+            else:
+                scores = output
+        return self.tensorflow_nms(
+                    boxes.reshape([1,-1,1,4]),
+                    scores, 
+                    clip_boxes=True)
     
-    def get_output_type(self) -> str:
+    def process_yolov( # NOSONAR
+            self, 
+            outputs: list
+        ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
         """
-        This returns the output type of the model.
+        Process YOLOv5 exported models.
+
+        Parameters
+        ----------
+            output: list or np.ndarray
+                Models converted in YoloV5 requires torch NMS which has the 
+                following shape (batch size, number of boxes, number of classes).
+                The output is a torch.Tensor.
+
+        Returns
+        -------
+            nmsed_boxes: np.ndarray
+                The prediction bounding boxes.. [[box1], [box2], ...].
+
+            nmsed_classes: np.ndarray
+                The prediction labels.. [cl1, cl2, ...].
+
+            nmsed_scores: np.ndarray
+                The prediction confidence scores.. [score, score, ...]
+                normalized between 0 and 1.
+        """
+        if len(outputs) == 1:
+            h, w = self.get_input_shape()[1:3]
+            # NMS requires non-normalized coordinates.
+            outputs[0][..., :4] *= [w, h, w, h]  # xywh normalized to pixels.
+            if isinstance(outputs, (list, tuple)):
+                output = self.from_numpy(outputs[0]) if len(outputs) == 1 else [
+                    self.from_numpy(x) for x in outputs]
+            else:
+                output = self.from_numpy(outputs)
+
+            output = self.torch_nms(output)
+            outputs = output[0].numpy()
+            outputs[..., :4] /= [w, h, w, h]
+            
+            nmsed_boxes = outputs[..., :4]
+            # Single dimensional arrays gets converted to the element. 
+            # Specify the axis into 1 to prevent that.
+            nmsed_scores = np.squeeze(outputs[..., 4:5], axis=1)
+            nmsed_classes = np.squeeze(outputs[...,5:6], axis=1)
+        elif len(outputs) == 4:
+            # For YOLOv5 converted models with NMS embedded.
+            # boxes = (1, 100, 4), batch_size = (1,), classes = (1, 100), scores = (1, 100).
+            nmsed_scores, nmsed_classes = None, None
+            for output in outputs:
+                if output.shape[-1] == 4:
+                    nmsed_boxes = output[0]
+                elif len(output.shape) == 2:
+                    # If all values are 0 or 1, then this could be classes.
+                    unique = np.unique(output[0])
+                    if len(unique) == 1 and (unique[0] == 0 or unique[0] == 1):
+                        nmsed_classes = output[0]
+                    # If all values are in between 0 and 1, then this could be scores.
+                    elif np.all(np.logical_and(output[0] >= 0, output[0] <= 1)):
+                        nmsed_scores = output[0]
+                    # Other combinations should just be classes.
+                    else:
+                        nmsed_classes = output[0]
+            if nmsed_scores is None or nmsed_classes is None:
+                return np.array([]), np.array([]), np.array([])
+        else:
+            logger(
+                "Postprocessing for this model output is not yet supported.", 
+                code="ERROR")
+        return nmsed_boxes, nmsed_classes, nmsed_scores
+    
+    def get_input_type(self) -> str:
+        """
+        This returns the input type of the model.
 
         Returns
         -------
             type: str
-                The output type of the model.
+                The input type of the model.
         """
-        return self.interpreter.get_output_details()[0]["dtype"].__name__
+        return self.interpreter.get_input_details()[0]["dtype"].__name__
 
     def get_input_shape(self) -> np.ndarray:
         """
         Grabs the model input shape.
 
         Returns
         -------
             shape: np.ndarray
                 The model input shape.
                 (batch size, height, width, channels).
         """
         return self.interpreter.get_input_details()[0]["shape"]
     
+    def get_output_type(self) -> str:
+        """
+        This returns the output type of the model.
+
+        Returns
+        -------
+            type: str
+                The output type of the model.
+        """
+        return self.interpreter.get_output_details()[-1]["dtype"].__name__
+    
     def get_output_shape(self) -> np.ndarray:
         """
         Grabs the model output shape.
 
         Returns
         --------
             shape: np.ndarray
                 The model output shape.
                 (batch size, boxes, classes).
         """
-        return self.interpreter.get_output_details()[0]["shape"]
+        return self.interpreter.get_output_details()[-1]["shape"]
```

## deepview/validator/runners/modelclient/__init__.py

```diff
@@ -3,11 +3,16 @@
 # Unauthorized copying of this file, via any medium is strictly prohibited
 # Proprietary and confidential.
 #
 # This source code is provided solely for runtime interpretation by Python.
 # Modifying or copying any source code is explicitly forbidden.
 
 from deepview.validator.runners.modelclient.core import ModelClientRunner
-from deepview.validator.runners.modelclient.detection import BoxesModelPack, \
+from deepview.validator.runners.modelclient.segmentation import ( 
+    SegmentationModelPack, 
+    SegmentationDeepLab,
+    SegmentationRunner
+)
+from deepview.validator.runners.modelclient.detection import (
+    BoxesModelPack,
     BoxesYolo
-from deepview.validator.runners.modelclient.segmentation import \
-    SegmentationRunner, SegmentationModelPack, SegmentationDeepLab
+)
```

## deepview/validator/runners/modelclient/core.py

```diff
@@ -40,18 +40,17 @@
     """
     def __init__(
         self,
         model: str,
         target: str,
         parameters: Parameters=None
     ):
-        self.model = model
+        super(ModelClientRunner, self).__init__(model, parameters)
         self.target = target
-        self.parameters = parameters
-        super(ModelClientRunner, self).__init__(model)
+        self.load_model()
 
     def load_model(self):
         """
         Loads the model to the modelrunner target.
       
         Raises
         ------
@@ -69,16 +68,16 @@
                 "with the modelclient server.")
 
         try:
             from deepview.rt.modelclient import ModelClient # type: ignore
             self.client = ModelClient(uri=self.target, rtm=self.model)
         except req.exceptions.ConnectionError:
             raise ModelRunnerFailedConnectionException(self.target)
-
-        self.parameters.engine = req.get(self.target).json()["engine"]
+        
+        self.parameters.engine = req.get(self.target).json()['engine']
 
         response = req.get("{}/model".format(self.target))
         self.modelclient_parameters = {}
         if response.status_code == 200:
             body = response.json()
             inputs = body['inputs']
             outputs = body['outputs']
```

## deepview/validator/runners/modelclient/detection.py

```diff
@@ -174,16 +174,19 @@
                 "tensorflow is needed to perform NMS operations.")
 
         if self.decoder:
             boxes, scores = self.build_decoder(
                 [o.astype(np.float32) for o in outputs]
             )
         else:
-            boxes = outputs[-2]
-            scores = outputs[-1]
+            for output in outputs:
+                if len(output.shape) == 4:
+                    boxes = output
+                elif len(output.shape) == 3:
+                    scores = output
 
         if self.parameters.max_detections is None:
             max_detections = 25
         else:
             max_detections = self.parameters.max_detections
 
         nmsed_boxes, nmsed_scores, nmsed_classes, valid_boxes = \
@@ -226,15 +229,15 @@
 
     def build_decoder(self, outputs: np.ndarray):
         """
         Builds the embeds decoder on the model.
 
         Parameters
         ----------
-            Outputs: np.ndarray
+            outputs: np.ndarray
                 This contains information regarding boxes,
                 labels, and scores.
 
         Returns
         -------
             boxes: np.ndarray
                 This contains the bounding boxes [[box1], [box2], ...].
```

## deepview/validator/runners/modelclient/segmentation.py

```diff
@@ -2,34 +2,42 @@
 #
 # Unauthorized copying of this file, via any medium is strictly prohibited
 # Proprietary and confidential.
 #
 # This source code is provided solely for runtime interpretation by Python.
 # Modifying or copying any source code is explicitly forbidden.
 
+from __future__ import annotations
+from typing import TYPE_CHECKING
+if TYPE_CHECKING:
+    from deepview.validator.evaluators.parameters import Parameters
+
 from deepview.validator.runners.modelclient.core import ModelClientRunner
 from deepview.validator.exceptions import MissingLibraryException
 from deepview.validator.datasets.utils import resize
 from time import monotonic_ns as clock_now
 from typing import Tuple
 import numpy as np
 import os
 
 class SegmentationRunner(ModelClientRunner):
     """
     Uploads the model to the target and runs the model per image.
 
     Parameters
     ----------
-        model_path: str
+        model: str
             The path to the model.
 
         target: str
             The modelrunner target in the EVK. Ex. 10.10.40.205:10817.
 
+        parameters: Parameters
+            This object contains the model parameters set from the command line.
+
         segmentation_model_type: str
             This is the type of segmentation model. Can either
             be "modelpack" or "deeplab".
 
     Raises
     ------
         ModelRunnerFailedConnectionException
@@ -42,26 +50,28 @@
                 Raised if the provided image_path
                 does not exist and the provided image is not a numpy.ndarray.
     """
     def __init__(
         self,
         model: str,
         target: str,
+        parameters: Parameters,
         segmentation_model_type: str="modelpack"
     ):
         try:
             import requests as re
         except ImportError:
             raise MissingLibraryException(
                 "requests is needed to communicate " +
                 "with the modelclient server.")
 
         super(SegmentationRunner,self).__init__(
             model=model,
-            target=target
+            target=target,
+            parameters=parameters
         )
         self.segmentation_model_type = segmentation_model_type.lower()
         self.outputs = list()
 
         r = re.get(self.target +
                    str('model' if self.target.endswith('/') else '/model'))
         if r.status_code == 200:
@@ -135,28 +145,42 @@
         if self.segmentation_model_type == "modelpack":
             dt_mask = cv2.warpAffine(dt_mask.astype(np.uint8), np.float32(
                 [[1, 0, 15], [0, 1, 15]]), self.get_input_shape())
 
         boxes_ns = clock_now() - start
         self.box_timings.append(boxes_ns * 1e-6)
         return dt_mask
+    
+    def get_input_shape(self) -> tuple:
+        """
+        Grabs the ModelPack input shape.
+
+        Returns
+        -------
+            shape: tuple
+                The model input shape.
+        """
+        return self.modelclient_parameters['input_shape'][0:2]
 
 class SegmentationModelPack(SegmentationRunner):
     """
     Inherits SegmentationRunner and preprocesses the input type of the MPK 
     models and decodes the output to generate the segmentation mask.
    
     Parameters
     ----------
-        model_path: str
+        model: str
             The path to the model.
 
         target: str
             The modelrunner target in the EVK. Ex. 10.10.40.205:10817.
 
+        parameters: Parameters
+            This object contains the model parameters set from the command line.
+
         segmentation_model_type: str
             This is "modelpack" type.
 
     Raises
     ------
         ModelRunnerFailedConnectionException
             Raised if connecting to modelrunner is unsuccessful.
@@ -165,20 +189,22 @@
             Raised if certain libraries are not installed.
     """
 
     def __init__(
         self,
         model: str,
         target: str,
-        segmentation_model_type: str="modelpack"
+        parameters: Parameters,
+        segmentation_model_type: str="modelpack",
     ):
         super(SegmentationModelPack, self).__init__(
             model=model,
             target=target,
-            segmentation_model_type=segmentation_model_type
+            parameters=parameters,
+            segmentation_model_type=segmentation_model_type,
         )
 
     def decode(self, outputs: dict):
         """
         Decodes the output, x and returns the numpy array segmentation 
         mask with elements containing the values of the objects ids.
 
@@ -207,40 +233,31 @@
         Returns
         -------
             img: np.ndarray
                 Expanded image with extra dimension 1.
         """
         return np.expand_dims(image, 0).astype(np.uint8)
 
-    def get_input_shape(self) -> tuple:
-        """
-        Grabs the ModelPack input shape.
-
-        Returns
-        -------
-            shape: tuple
-                The model input shape.
-        """
-        # TODO: Read from the client instead of a hardcoded value.
-        return (320, 320)
-
 class SegmentationDeepLab(SegmentationRunner):
     """
     Inherits SegmentationRunner and preprocesses the input 
     type of the Deeplab models and decodes the output to 
     generate the segmentation mask.
 
     Parameters
     ----------
         model: str
             The path to the model.
 
         target: str
             The modelrunner target in the EVK. Ex. 10.10.40.205:10817.
 
+        parameters: Parameters
+            This object contains the model parameters set from the command line.
+
         segmentation_model_type: str
             This is the type of the model. e.g. "deeplab".
 
     Raises
     ------
         ModelRunnerFailedConnectionException
             Raised if connecting to modelrunner is unsuccessful.
@@ -249,19 +266,21 @@
             Raised if certain libraries are not installed.
     """
 
     def __init__(
         self,
         model: str,
         target: str,
+        parameters: Parameters,
         segmentation_model_type: str="deeplab"
     ):
         super(SegmentationDeepLab, self).__init__(
             model=model,
             target=target,
+            parameters=parameters,
             segmentation_model_type=segmentation_model_type    
         )
 
     def decode(self, outputs: dict):
         """
         Decodes the output, x and returns the numpy array \
             segmentation mask with elements containing the values of \
@@ -309,19 +328,7 @@
 
         Returns
         -------
             img: np.ndarray
                 Expanded image with extra dimension 1.
         """
         return np.expand_dims(image.copy(), 0).astype(np.uint8)
-
-    def get_input_shape(self) -> tuple:
-        """
-        Grabs the Deeplab input shape.
-        
-        Returns
-        -------
-            shape: tuple
-                The model input shape.
-        """
-        # TODO: Read from the client instead of a hardcoded value.
-        return (513, 513)
```

## deepview/validator/visualize/detectiondraw.py

```diff
@@ -23,15 +23,16 @@
         }
 font = ImageFont.load_default()
 
 def draw_rect(
         image_draw: ImageDraw.ImageDraw, 
         selected_corners: np.ndarray, 
         color: str, 
-        width: int=2):
+        width: int=2
+    ):
     """
     This is primarily used for drawing 3D bounding boxes which consists of 
     2 rectangles and 4 lines particularly speaking.
 
     Parameters
     ----------
         image_draw: ImageDraw.ImageDraw
@@ -108,14 +109,17 @@
             ((x1, y1), (x2, y2)) position of the box.
 
         color: str
             The color of the bounding box. Typically, 
             ground truth/false negatives is set to "RoyalBlue", 
             false positives is set to "OrangeRed",
             true positives is set to "LimeGreen".
+
+        width: int
+            The width of the line to draw the bounding boxes.
     """
     image_draw.rectangle(
         box_position,
         outline=color,
         width=width)
     
 def draw_text(
@@ -171,26 +175,30 @@
         text,
         font=font,
         align=align,
         fill=color
         )
 
 def position_2d_text_background(
-        text_size: tuple, 
+        text: str, 
+        font: ImageFont,
         text_position: tuple, 
         box_position: tuple
     ) -> Tuple[tuple, tuple]:
     """
     This positions the background of the text to make it aligned with the 
     2d bounding box.
 
     Parameters
     ----------
-        text_size: tuple
-            This contains the (text width, text height).
+        text: str
+            The text that will be drawn on the image.
+
+        font: ImageFont
+            The type of font to use.
 
         text_position: tuple
             This contains the (x, y) position of the text.
 
         box_position: tuple
             This contain the ((x1, y1), (x2, y2)) position 
             of the 2D bounding box.
@@ -199,15 +207,19 @@
     -------
         background_position: tuple
             This is the ((x1, y1), (x2, y2)) position of the text background.
 
         text_position: tuple
             This is the (x,y) position of the text aligned to the background.
     """
-    text_width, text_height = text_size
+    if hasattr(font, 'getsize'): # works on older Pillow versions < 10.
+        text_width, text_height = font.getsize(text)
+    else:
+        (text_width, text_height), _ = font.font.getsize(text) # newer Pillow versions >= 10.
+
     box_text_x1 = box_position[0][0]
     box_text_x2 = box_text_x1 + text_width
 
     # This suggests a ground truth text is being drawn where the label is 
     # located in the bottom left of the bounding box.
     if text_position[1] > box_position[0][1]:
         box_text_y1 = box_position[1][1] - text_height
@@ -218,26 +230,30 @@
         # The +10 keeps the text within the bounding box.
         text_position = (text_position[0], text_position[1] + 10) 
 
     box_text_y2 = box_text_y1 + text_height
     return ((box_text_x1, box_text_y1), (box_text_x2, box_text_y2)), text_position
 
 def position_3d_text_background(
-        text_size: tuple, 
+        text: str, 
+        font: ImageFont,
         text_position: tuple, 
         color: str = "RoyalBlue"
     ) -> Tuple[tuple, tuple]:
     """
     This positions the background of the text to make it aligned to the 
     3d bounding box.
 
     Parameters
     ----------
-        text_size: tuple
-            This contains the (text width, text height).
+        text: str
+            The text that will be drawn on the image.
+
+        font: ImageFont
+            The type of font to use.
 
         text_position: tuple
             This contains the (x, y) position of the text.
 
         color: str
             The color is used to determine if the box being drawn 
             is the ground truth or the prediction.
@@ -246,15 +262,19 @@
     -------
         background_position: tuple
             This is the ((x1, y1), (x2, y2)) position of the text background.
 
         text_position: tuple
             This is the (x,y) position of the text aligned to the background.
     """
-    text_width, text_height = text_size
+    if hasattr(font, 'getsize'): # works on older Pillow versions < 10.
+        text_width, text_height = font.getsize(text)
+    else:
+        (text_width, text_height), _ = font.font.getsize(text) # newer Pillow versions >= 10.
+
     corner1, corner2, = text_position
     box_text_x1 = corner1[0] # Front, left, top corner.
     box_text_x2 = box_text_x1 + text_width
 
     if color == "RoyalBlue":
         box_text_y1 = corner2[1]
         box_text_y2 = box_text_y1 + text_height
@@ -514,15 +534,16 @@
     for label, bounding_box in zip(gt_instance.labels, gt_instance.boxes): 
         box_position = format_box_position(
             bounding_box, gt_instance.width, gt_instance.height)
         draw_2d_bounding_box(image_draw, box_position)
         
         text = str(label)
         background_position, text_position = position_2d_text_background(
-            font.getbbox(text)[2:],
+            text,
+            font,
             (box_position[0][0], box_position[1][1] - 12),
             box_position
         )
         draw_text(
             image_draw, 
             text, 
             text_position, 
@@ -538,15 +559,16 @@
         if score >= validation_score*100:
             bounding_box = dt_instance.boxes[extra]
             box_position = format_box_position(
                 bounding_box, gt_instance.width, gt_instance.height)
             draw_2d_bounding_box(image_draw, box_position, "OrangeRed")
             
             background_position, text_position = position_2d_text_background(
-                font.getbbox(text)[2:],
+                text,
+                font,
                 (box_position[0][0], box_position[0][1] - 10),
                 box_position)
             draw_text(
                 image_draw,
                 text,
                 text_position,
                 font,
@@ -571,15 +593,16 @@
         if score >= validation_score*100:
             bounding_box = dt_instance.boxes[match[0]]
             box_position = format_box_position(
                 bounding_box, gt_instance.width, gt_instance.height)
             draw_2d_bounding_box(image_draw, box_position, color)
 
             background_position, text_position = position_2d_text_background(
-                font.getbbox(text)[2:],
+                text,
+                font,
                 (box_position[0][0], box_position[0][1] - 10),
                 box_position)
             draw_text(
                 image_draw,
                 text,
                 text_position,
                 font,
@@ -656,15 +679,16 @@
         corners = corners / corners[2:3, :].repeat(3, 0).reshape(3, nbr_points)
 
         corner_position = format_corner_position(corners, angle)
         draw_3d_bounding_box(image_draw, corners)
 
         text = str(label)
         background_position, text_position = position_3d_text_background(
-            font.getbbox(text)[2:],
+            text,
+            font,
             corner_position
         )
         draw_text(
             image_draw,
             text,
             text_position,
             font,
@@ -689,15 +713,16 @@
             # Normalize.
             corners = corners / corners[2:3, :].repeat(3, 0).reshape(3, nbr_points)
             
             corner_position = format_corner_position(corners, angle)
             draw_3d_bounding_box(image_draw, corners, "OrangeRed")
 
             background_position, text_position = position_3d_text_background(
-                font.getbbox(text)[2:],
+                text,
+                font,
                 corner_position,
                 "OrangeRed"
             )
             draw_text(
                 image_draw,
                 text,
                 text_position,
@@ -733,15 +758,16 @@
             # Normalize.
             corners = corners / corners[2:3, :].repeat(3, 0).reshape(3, nbr_points)
 
             corner_position = format_corner_position(corners, angle)
             draw_3d_bounding_box(image_draw, corners, color)
 
             background_position, text_position = position_3d_text_background(
-                font.getbbox(text)[2:],
+                text,
+                font,
                 corner_position,
                 color
             )
             draw_text(
                 image_draw,
                 text,
                 text_position,
```

## deepview/validator/visualize/utils.py

```diff
@@ -4,14 +4,15 @@
 # Proprietary and confidential.
 #
 # This source code is provided solely for runtime interpretation by Python.
 # Modifying or copying any source code is explicitly forbidden.
 
 import matplotlib.pyplot as plt
 import matplotlib.figure
+from typing import List
 import numpy as np
 import matplotlib
 import io
 
 matplotlib.use('Agg')
 
 def figure2numpy(figure: matplotlib.figure.Figure) -> np.ndarray:
@@ -406,15 +407,15 @@
     plt.xticks(range(width), labels[:width], rotation="vertical")
     plt.yticks(range(height), labels[:height])
     plt.ylabel("Prediction")
     plt.xlabel("Ground Truth")
     plt.title(f"{model} Confusion Matrix")
     return fig
 
-def close_figures(figures: list[matplotlib.figure.Figure]):
+def close_figures(figures: List[matplotlib.figure.Figure]):
     """
     Closes the matplotlib figures opened to prevent 
     errors such as "Fail to allocate bitmap."
 
     Parameters
     ----------
         figures: list
```

## deepview/validator/writers/core.py

```diff
@@ -92,18 +92,18 @@
             | Classification| 0.75              |{str(round(summary.classification_fp_error.get('0.75')*100, 2)).center(14)}|
             | FP Error (%)  | 0.5-0.95          |{str(round(summary.classification_fp_error.get('0.50:0.95')*100, 2)).center(14)}|
             |_______________|___________________|______________|
         """
 
         if summary.append_centers:
             table_summary += \
-        f"""    |               | x-center          |{str(round(summary.mae_centers.get('x-center-mae'),2)).center(14)}|
-            |     Mean      | y-center          |{str(round(summary.mae_centers.get('y-center-mae'),2)).center(14)}|
-            |   Absolute    | z-center          |{str(round(summary.mae_centers.get('z-center-mae'),2)).center(14)}|
-            |    Error      | center distances  |{str(round(summary.mae_centers.get('distance-mae'),2)).center(14)}|
+        f"""    |               | x-center          |{str(round(summary.mae_centers.get('x-center-mae'),4)).center(14)}|
+            |     Mean      | y-center          |{str(round(summary.mae_centers.get('y-center-mae'),4)).center(14)}|
+            |   Absolute    | z-center          |{str(round(summary.mae_centers.get('z-center-mae'),4)).center(14)}|
+            |    Error      | center distances  |{str(round(summary.mae_centers.get('distance-mae'),4)).center(14)}|
             |_______________|___________________|______________|
         """
 
         if summary.model != "Training Model":
             table_summary += self.format_parameters(parameters)
 
         if timings is not None:
```

## deepview/validator/writers/tensorboard.py

```diff
@@ -21,14 +21,18 @@
     """
     Used to publish the images and the metrics onto TensorBoard.
     
     Parameters
     ----------
         logdir: str
             This is the path to save the tfevents file.
+
+        writer: TensorboardWriter
+            If this is provided, then this object will be used to write
+            onto Tensorboard.
     """
     def __init__(
         self,
         logdir: str=None,
         writer: TensorBoardWriter=None
         ):
         super(TensorBoardWriter, self).__init__()
```

## Comparing `deepview_validator-3.2.2.dist-info/RECORD` & `deepview_validator-3.3.0.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,57 +1,59 @@
 deepview/validator/__init__.py,sha256=H0CZJBkSPkPhL9YbYiBf8cx2fVOiyWZIPFNhtxPJHJo,936
-deepview/validator/__main__.py,sha256=LOErlY7LaQPc1cfUCXMfW-_8H63l0Fj3iOMbZSH77sc,31800
-deepview/validator/exceptions.py,sha256=Sk36_qzsX16SOAtRfv-g-MbFOuen-pxbIXnM38i2laI,11477
-deepview/validator/datasets/__init__.py,sha256=5d2yOfuwLOCXdb4fguXY3Ho9Arqk9VImZP_nSNlBhWo,5385
-deepview/validator/datasets/arrow.py,sha256=43l6pNoKQYzAiybLR9n8GLZ9ZGS5ZQm0okPWHkcnpuU,6088
-deepview/validator/datasets/core.py,sha256=0DIKWut_8xBXKG_ZyMfn19E73-jjVridCG4dRLtuXzc,12134
-deepview/validator/datasets/darknet.py,sha256=dncpXWXv2xlHpdEUSxbj7sH7hjcOjzVgkRvk6tzc2LA,20744
-deepview/validator/datasets/instance.py,sha256=rFj6y01ZNeEjmvX3ufK65I3HIaw4d94MsL2m8_riu2A,19944
-deepview/validator/datasets/tfrecord.py,sha256=SqU7F2W5l2aV58WQRkBF32GDK3U9DzQ2lPYzx0_XA5g,7530
-deepview/validator/datasets/utils.py,sha256=OUp8aML9jIJrismIoxlINj2CRy-949Zo4w90CbOuPOM,21516
+deepview/validator/__main__.py,sha256=hmgl7e0WMdrg3fRgWZkgiYVWGCuskv5AdvRfIKKBNhM,34066
+deepview/validator/exceptions.py,sha256=txpogI4iKFnaNh16rmQIhQCm-AfbIZmwGHEZIt1E3GI,11375
+deepview/validator/datasets/__init__.py,sha256=NXzUOQ3lUfh-mWrATVDIVUvZMbmkrFOD1is4ItVhnQ0,5782
+deepview/validator/datasets/arrow.py,sha256=OEy3Kvo2pWgC1pHx9FiE7xkgnXpIdpPwYehm98AhgCY,5803
+deepview/validator/datasets/base.py,sha256=rmG2VuanSEYpIpIaEcon1HDUDqrh0cVMyavLzjtjbIU,3276
+deepview/validator/datasets/core.py,sha256=adeqAw14dE-XUQFQj1CuACUtuvDJjdXxEEMYSu-hpXw,11866
+deepview/validator/datasets/darknet.py,sha256=BSIDDmWCCZx144XrHoVk5kZoD73Yyw7VhYYLdXHMvN0,20050
+deepview/validator/datasets/instance.py,sha256=gmo3ll4EH6bzbx-ninLV8tWgG_dT5EiMM93-s7T1aDc,19950
+deepview/validator/datasets/tfrecord.py,sha256=_BlRKCGp5KYGZxEmjGJswyOThzhiTH-xPsS4KSkXXZQ,7547
+deepview/validator/datasets/utils.py,sha256=aUzCrSbF5_CDKFnihGuJgHNzIPRmDRr-hZB9l-J3PAo,24537
 deepview/validator/evaluators/__init__.py,sha256=wMBjkFAc2SWK23PMg63mr8DsRbwl0A0WJCd4JJ98sNU,735
 deepview/validator/evaluators/combinedevaluator.py,sha256=2M3eNPsOJxRuFeD68iMp1a8_JHCKqhUvZN0RP3hdm_w,7710
-deepview/validator/evaluators/core.py,sha256=yR7vydeTFQET-UaQ_zkhVmNQM4-gb7Pqu3swtHzhPhk,17045
-deepview/validator/evaluators/detectionevaluator.py,sha256=HS3jbJenzzioh-tdS3hE6-OZCqk53ErjRIX6liKKC8Y,15096
-deepview/validator/evaluators/parameters.py,sha256=OideErBrFiuUVtP1Voq_T1s0mGGFKxqCggXR4eMJEng,23949
-deepview/validator/evaluators/poseevaluator.py,sha256=TVvJ-egxB0G65Wd-c8GOh4NzgsokHgOALPzS6qEp1JA,8667
+deepview/validator/evaluators/core.py,sha256=Dq5p1Pf2QCHPEiEoiHMowqdbH-ZtyxPieNv1aRKb8qk,17030
+deepview/validator/evaluators/detectionevaluator.py,sha256=jqKJzyYJkcNubgbWeunDJkdKXuHaGHUQigMevtakPOo,14842
+deepview/validator/evaluators/parameters.py,sha256=wlRn2bPCbNcppEa7ty2_6ob2B2bLgYxQGXMr5QFfWko,26879
+deepview/validator/evaluators/poseevaluator.py,sha256=E6IG7nRssH5A1aNBOqHQcIlqhhEdYji_M-H2X38c4aA,8249
 deepview/validator/evaluators/segmentationevaluator.py,sha256=Wkqoywxsb8exRAPAmrHiXF9t4DagQbkjlNQIrcuppsk,10399
-deepview/validator/evaluators/utils.py,sha256=f-r0Ah8T9VMg8AMNzCbf6QIzJhA64f9MXKHpVTatdtc,9184
+deepview/validator/evaluators/utils.py,sha256=UolhFnjlhPN77gFMK8n8zfA9I89TmaakMOG3FSYCybU,9184
 deepview/validator/metrics/__init__.py,sha256=5BQNexGp4_EdyI80zBFd7lW1BdXp7TPHoX-8wohOeZk,952
 deepview/validator/metrics/core.py,sha256=DDi632N0uKOlwurbRf08L2VFrVKbI1W1FzeLogCJBUQ,3507
-deepview/validator/metrics/detectiondata.py,sha256=Z5RDV2MI-Ac15xQERJ2ZDCCFsu9Cjern0DN4u5scmHM,20714
-deepview/validator/metrics/detectionmatch.py,sha256=0oOnpUNe_HmFQRozeNYo__RX-Jno4Hbyi2XMuBaVmdI,33326
-deepview/validator/metrics/detectionmetrics.py,sha256=02U_0DmDZ4fpTLXfD5m2kq3vci-8hoSWRCO9qImq6IA,32873
-deepview/validator/metrics/detectionutils.py,sha256=8EjY2CvagTz4ASeq4njUNjggFw56P79V5l7YgGi_qZk,26129
-deepview/validator/metrics/posedata.py,sha256=VmfpmPqtty8RwQx_cWmIGIEpwE3MvQddc5Gtm1_0Jdk,9997
-deepview/validator/metrics/posemetrics.py,sha256=2N7bAGJj_HblNUlT5XEIhb_PF33no1VUOY_GRLXnuGc,2028
+deepview/validator/metrics/detectiondata.py,sha256=AjVK1jylXbs0qxVlcAU2AhzaUukK3RQ7-yYYfjTSzQk,20727
+deepview/validator/metrics/detectionmatch.py,sha256=rTssngmt92AJRm7ib_LZspFbeIpWcJT65bNHpil6SIc,34156
+deepview/validator/metrics/detectionmetrics.py,sha256=2R60ZyxyzsiEVEKspGlTydEj3Djc7y-IWnMRKORjd50,32369
+deepview/validator/metrics/detectionutils.py,sha256=Xw3KUnaqBgJbX1TIHzU2i6l_qZVRLOZZTbJtlyCVvkA,26257
+deepview/validator/metrics/posedata.py,sha256=-4c4Vs60CcGDQ4642xrHHPqFDSXKis0vSQ6bxza0KLk,10009
+deepview/validator/metrics/posemetrics.py,sha256=_xejgPZUazXeWzaOX2z57jgRVns_7ZYzPpE8zeE-8sk,2120
 deepview/validator/metrics/poseutils.py,sha256=pk2F8zvlH1eu4iHTI38p4KV8jiyT4qFW03-15SG4GH8,1022
-deepview/validator/metrics/segmentationdata.py,sha256=u0U5RZbM80zzpAQZm2YpAdy9tDIzIn1INwyE-eusSVc,10940
+deepview/validator/metrics/segmentationdata.py,sha256=vYnpQ39jBUcKlp5HPLFb9jJXpyuTFA9FWQhArJgRUsU,10935
 deepview/validator/metrics/segmentationmetrics.py,sha256=z54DbPJRj_EbRvyCb5ZYOvW6Bq_AOlD9MEW_aIiEZAs,5534
 deepview/validator/metrics/segmentationutils.py,sha256=NDuG2qpjetlwj-HZeYPbr7Fsv_-qB0G8LZHqmeHE7E8,6643
-deepview/validator/metrics/summary.py,sha256=K6hswngwtMb053SOX6XZKcUCWU2QWy9n8CGouvBPV9s,52664
-deepview/validator/runners/__init__.py,sha256=ThlcpiYvEqECTOskeLS_g48ck7f7E22xQljfaj6PqAg,821
-deepview/validator/runners/core.py,sha256=RLMj6mMhUDlwbS8zV4GjFthIDTd9NMrOEfrFCzQfGLs,10089
-deepview/validator/runners/deepviewrt.py,sha256=IXARB6IG_kj_y45_gm-yFzujMRy0O1OA42iCoEqYLy8,19725
-deepview/validator/runners/keras.py,sha256=O0XnaSRVC1nUXvI_TC545_2i7OvItqtl3AIJybNagSM,14272
-deepview/validator/runners/offline.py,sha256=IXe0YfdRjEEg3yiEy7AfGB-jDESIbYZU1LgrK-bkySE,18805
-deepview/validator/runners/onnx.py,sha256=JY361prWJKWgZO8reV1cS6ugNx7f8mF2C-whXmYz3Ow,8872
-deepview/validator/runners/tensorrt.py,sha256=5_e5gLdnRbGEgyTo1L0CFQM_SZ3LxScPjlgQqBKJCyY,14653
-deepview/validator/runners/tflite.py,sha256=TAlhetk0PfkZfkq5V7x6B2Yk5xsSuyQaJVPNToYhQ4c,9172
-deepview/validator/runners/modelclient/__init__.py,sha256=6S6lCllYEZYdaXkUQExbQJ_XkAuDx9mjkfb8y_5LfAQ,615
-deepview/validator/runners/modelclient/core.py,sha256=Gvwu-spW0soPZSeOIJ97ancbR8nX8V73n5PBJ5evfjc,3703
-deepview/validator/runners/modelclient/detection.py,sha256=9ryMgG16NrURSVmXMEJiE5ZmKEHksQNJaim2AddkkEo,25636
-deepview/validator/runners/modelclient/segmentation.py,sha256=tNW0tRZ3tTFV7DKLsGHMpUI_qTxctV_voTJ9ML_So7g,9675
+deepview/validator/metrics/summary.py,sha256=7Gd6TTBrQsaLTJNbzKXZSRj0EtesSaarG5w383eToa4,55204
+deepview/validator/runners/__init__.py,sha256=iLhByRLIloq_MkHoBhDmQXA-T99ed-Ep6UrfYJ1gv10,896
+deepview/validator/runners/core.py,sha256=mMBUni14iPGMc7cM3S60Bhxqv4_5ESFOffOGt5IwsVE,24984
+deepview/validator/runners/deepviewrt.py,sha256=4h0x0dtRp4z5ChM-ot3A2gYOm5qSeht3FVPZe19zpKw,21949
+deepview/validator/runners/hailo.py,sha256=8pQMPDDGnCUy_2ztkwvxI5FbahIWXpCKa3HYCEOXINk,11086
+deepview/validator/runners/keras.py,sha256=V_Asq3jMK_EP583ZvtEIXR4jMw9afpVDNPzpKfh4cHY,25984
+deepview/validator/runners/offline.py,sha256=d0SKldb7efruScosGMioVHBXme8LJRFbyUCEiDkTrWU,18127
+deepview/validator/runners/onnx.py,sha256=p5NdlVxEA4AC2j8pzyN2KJmKnEc6A9W5KDcye5JpEG4,19521
+deepview/validator/runners/tensorrt.py,sha256=FjBcSPTICM_bF4-2Atf5rWRrE0J6L9QTIgbmi4QIc28,14524
+deepview/validator/runners/tflite.py,sha256=JK39rZey7vM6iD4-Sk60kiHTGAiZasJhG7_aBvznXQ0,14547
+deepview/validator/runners/modelclient/__init__.py,sha256=fNkjB4A0SXOvmqMKB1RXbeWS_-MOMZUa33gLynnpek4,634
+deepview/validator/runners/modelclient/core.py,sha256=kNV7YGLmdNJMKquYT6eQ3Z8069Qggwkrvgp4oxaBI-M,3685
+deepview/validator/runners/modelclient/detection.py,sha256=pMTvgne2axwnIZwVcIcBEsmmtZQoT9QNa3iTVCusbq0,25765
+deepview/validator/runners/modelclient/segmentation.py,sha256=j1_g3qJaXzwEAsKVWFVUpWBMogAgvqPTdFCB4Muixt8,10034
 deepview/validator/visualize/__init__.py,sha256=T_ijL0tT5Cvs8XkTjZYb2XaaykinScepFJjHgHCi7_s,314
-deepview/validator/visualize/detectiondraw.py,sha256=ATLeU8-QNXcaRdicnWNQDFVTkfNG8qz4EZjWNEE1kkk,25309
+deepview/validator/visualize/detectiondraw.py,sha256=u3anpL_rrUjiiv5m6-kiBiR67CdkH2iDtTz0_0JCHOc,25932
 deepview/validator/visualize/posedraw.py,sha256=99aGZSVgt3nsImVnwdWykyYhRz9d4eLKRjISXzLlD4s,7231
 deepview/validator/visualize/segmentationdraw.py,sha256=Zj2SSAPsEmnu8GpNPWN6TJplatE6fuFFZA0CeqwUrAE,8036
-deepview/validator/visualize/utils.py,sha256=uZ_n4rQXCR8VGPiwYLYVf1j6YcIfq8O2tuvbYv9SCAA,15063
+deepview/validator/visualize/utils.py,sha256=bOcx--Es6m9kqm_Fh6nR_6JOSVqE7HsPQ2JtPj7OydM,15087
 deepview/validator/writers/__init__.py,sha256=cFcirV22Hzyw9vi1cOL6Oyz-Z7VB-L97SDd37SGX7Cw,2899
 deepview/validator/writers/console.py,sha256=sxidknqc56hMa3k6c-yjNdm9cR2sqrqgmhs3Z4LGWW4,2478
-deepview/validator/writers/core.py,sha256=M4sZlpp8lAgZEjbgTmGogPz0ItYbJBbYz5wFTHNoBFM,17080
-deepview/validator/writers/tensorboard.py,sha256=H70xs_hHqEjzu6plczUgNlEtWdtsQ_b0PTj-ehHcZ64,4884
-deepview_validator-3.2.2.dist-info/METADATA,sha256=KK_-wGbQmlDdSwKm7CQ1ihS38jgMTtaoPRlvSENWMTM,512
-deepview_validator-3.2.2.dist-info/WHEEL,sha256=nvhOrkn7_9sGzJjxuUFjoJ6OkO7SJJqHSjq9VNu0Elc,92
-deepview_validator-3.2.2.dist-info/entry_points.txt,sha256=n4jIdEDC_mPGVLwmS21vEFC8_D7mqNuekZYdtupSSVE,73
-deepview_validator-3.2.2.dist-info/top_level.txt,sha256=FZ_uj5ZExs9dTNq5lw196yb-XR3VHKi6vS0EWgTQtXk,9
-deepview_validator-3.2.2.dist-info/RECORD,,
+deepview/validator/writers/core.py,sha256=urYKPk3Gnx3r4GW-wyd7hYDdil__ttudDupCIQYd8Nw,17080
+deepview/validator/writers/tensorboard.py,sha256=58nrwsVKqYJGtXv7bkllGi2iUl5EpFliCMHgEFZVOgs,5021
+deepview_validator-3.3.0.dist-info/METADATA,sha256=vxmaIYFwG7BUnFhgsktIbVi0yZItLV_r8oL4_ZLwcq0,1178
+deepview_validator-3.3.0.dist-info/WHEEL,sha256=nvhOrkn7_9sGzJjxuUFjoJ6OkO7SJJqHSjq9VNu0Elc,92
+deepview_validator-3.3.0.dist-info/entry_points.txt,sha256=n4jIdEDC_mPGVLwmS21vEFC8_D7mqNuekZYdtupSSVE,73
+deepview_validator-3.3.0.dist-info/top_level.txt,sha256=FZ_uj5ZExs9dTNq5lw196yb-XR3VHKi6vS0EWgTQtXk,9
+deepview_validator-3.3.0.dist-info/RECORD,,
```

