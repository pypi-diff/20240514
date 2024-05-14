# Comparing `tmp/pyawsopstoolkit.exceptions-0.1.0-py3-none-any.whl.zip` & `tmp/pyawsopstoolkit.exceptions-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4764 bytes, number of entries: 8
--rw-r--r--  2.0 unx      537 b- defN 24-May-13 20:56 pyawsopstoolkit/exceptions/__init__.py
--rw-r--r--  2.0 unx     1755 b- defN 24-May-13 20:56 pyawsopstoolkit/exceptions/__main__.py
--rw-r--r--  2.0 unx      780 b- defN 24-May-13 20:56 pyawsopstoolkit/exceptions/__validations__.py
--rw-r--r--  2.0 unx     1069 b- defN 24-May-13 20:56 pyawsopstoolkit.exceptions-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     2316 b- defN 24-May-13 20:56 pyawsopstoolkit.exceptions-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-13 20:56 pyawsopstoolkit.exceptions-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 24-May-13 20:56 pyawsopstoolkit.exceptions-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      771 b- defN 24-May-13 20:56 pyawsopstoolkit.exceptions-0.1.0.dist-info/RECORD
-8 files, 7336 bytes uncompressed, 3384 bytes compressed:  53.9%
+Zip file size: 5024 bytes, number of entries: 8
+-rw-r--r--  2.0 unx      577 b- defN 24-May-14 07:22 pyawsopstoolkit/exceptions/__init__.py
+-rw-r--r--  2.0 unx     3165 b- defN 24-May-14 07:22 pyawsopstoolkit/exceptions/__main__.py
+-rw-r--r--  2.0 unx      780 b- defN 24-May-14 07:22 pyawsopstoolkit/exceptions/__validations__.py
+-rw-r--r--  2.0 unx     1069 b- defN 24-May-14 07:22 pyawsopstoolkit.exceptions-0.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2678 b- defN 24-May-14 07:22 pyawsopstoolkit.exceptions-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-14 07:22 pyawsopstoolkit.exceptions-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 24-May-14 07:22 pyawsopstoolkit.exceptions-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      771 b- defN 24-May-14 07:22 pyawsopstoolkit.exceptions-0.1.1.dist-info/RECORD
+8 files, 9148 bytes uncompressed, 3644 bytes compressed:  60.2%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: pyawsopstoolkit/exceptions/__main__.py
 Comment: 
 
 Filename: pyawsopstoolkit/exceptions/__validations__.py
 Comment: 
 
-Filename: pyawsopstoolkit.exceptions-0.1.0.dist-info/LICENSE
+Filename: pyawsopstoolkit.exceptions-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: pyawsopstoolkit.exceptions-0.1.0.dist-info/METADATA
+Filename: pyawsopstoolkit.exceptions-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: pyawsopstoolkit.exceptions-0.1.0.dist-info/WHEEL
+Filename: pyawsopstoolkit.exceptions-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: pyawsopstoolkit.exceptions-0.1.0.dist-info/top_level.txt
+Filename: pyawsopstoolkit.exceptions-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: pyawsopstoolkit.exceptions-0.1.0.dist-info/RECORD
+Filename: pyawsopstoolkit.exceptions-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyawsopstoolkit/exceptions/__init__.py

```diff
@@ -1,13 +1,14 @@
 __all__ = [
-    "AssumeRoleError"
+    "AssumeRoleError",
+    "ValidationError"
 ]
 __name__ = "pyawsopstoolkit.exceptions"
 __description__ = """
 This package offers a collection of exception classes tailored for handling errors within the AWS Ops Toolkit.
 These exceptions are specifically designed to address different scenarios and errors that may occur during the
 execution of pyawsopstoolkit operations, providing comprehensive support for error handling and debugging within
 the toolkit.
 """
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 
-from pyawsopstoolkit.exceptions.__main__ import AssumeRoleError
+from pyawsopstoolkit.exceptions.__main__ import AssumeRoleError, ValidationError
```

## pyawsopstoolkit/exceptions/__main__.py

```diff
@@ -51,7 +51,51 @@
     def message(self) -> str:
         """
         Getter for message attribute.
         :return: The error message.
         :rtype: str
         """
         return self._message
+
+
+class ValidationError(Exception):
+    """
+    The ValidationError exception class serves a precise purpose within the AWS Ops Toolkit framework.
+    It diligently emerges when validation processes falter within the pyawsopstoolkit.validators package.
+    """
+
+    def __init__(
+            self,
+            message: str,
+            exception: Optional[Exception] = None
+    ) -> None:
+        """
+        Constructor for the ValidationError class.
+        :param message: The error message.
+        :type message: str
+        :param exception: The exception that occurred, if any.
+        :type exception: Exception
+        """
+        Validation.validate_type(message, str, 'message should be a string.')
+        Validation.validate_type(exception, Union[Exception, None], 'exception should be of Exception type.')
+
+        self._exception = exception
+        self._message = f'ERROR: {message}.{f" {exception}." if exception else ""}'
+        super().__init__(self.message)
+
+    @property
+    def message(self) -> str:
+        """
+        Getter for message attribute.
+        :return: The error message.
+        :rtype: str
+        """
+        return self._message
+
+    @property
+    def exception(self) -> Optional[Exception]:
+        """
+        Getter for exception attribute.
+        :return: The exception that occurred, if any.
+        :rtype: Exception
+        """
+        return self._exception
```

## Comparing `pyawsopstoolkit.exceptions-0.1.0.dist-info/LICENSE` & `pyawsopstoolkit.exceptions-0.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyawsopstoolkit.exceptions-0.1.0.dist-info/METADATA` & `pyawsopstoolkit.exceptions-0.1.1.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyawsopstoolkit.exceptions
-Version: 0.1.0
+Version: 0.1.1
 Summary: This package offers a collection of exception classes tailored for handling errors within the AWS Ops Toolkit.
 Home-page: https://github.com/coldsofttech/pyawsopstoolkit.exceptions
 Author: coldsofttech
 License: MIT
 Keywords: aws,toolkit,exceptions,amazon-web-services,awsopstoolkit,aws-ops-toolkit
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -54,14 +54,23 @@
 The **AssumeRoleError** exception class is specifically designed for the AWS Ops Toolkit. It's raised when the assume
 role session fails.
 
 #### Methods
 
 - `__init__(self, role_arn: str, exception: Optional[Exception] = None)`: Constructor for the **AssumeRoleError** class.
 
+### ValidationError
+
+The **ValidationError** exception class serves a precise purpose within the AWS Ops Toolkit framework. It diligently
+emerges when validation processes falter within the **pyawsopstoolkit.validators** package.
+
+#### Methods
+
+- `__init__(self, message: str, exception: Optional[Exception] = None)`: Constructor for the ValidationError class.
+
 # License
 
 Please refer to the [MIT license](LICENSE) within the project for more information.
 
 # Contributing
 
 We welcome contributions from the community! Whether you have ideas for new features, bug fixes, or enhancements, feel
```

## Comparing `pyawsopstoolkit.exceptions-0.1.0.dist-info/RECORD` & `pyawsopstoolkit.exceptions-0.1.1.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-pyawsopstoolkit/exceptions/__init__.py,sha256=tlW3ab-4_272ltJ6HrBe7D0REpDDntnOrTvGG6pQYdU,537
-pyawsopstoolkit/exceptions/__main__.py,sha256=3w94l_GhkgA5fxGh8hLMwOrHvwVAWWtXij6ga99lQg4,1755
+pyawsopstoolkit/exceptions/__init__.py,sha256=VAh5q_IW2Ly4XszoNWvXLXvnbGPONQgVgxtuV3PvtqA,577
+pyawsopstoolkit/exceptions/__main__.py,sha256=nOFYIDTnOEEIXvw-OgnGAD2gooCz11a1jHbgTX_-HtM,3165
 pyawsopstoolkit/exceptions/__validations__.py,sha256=RFgQuG2EuIxoD3INJBY-QnPwuEbBSG2IXxGnySjceOY,780
-pyawsopstoolkit.exceptions-0.1.0.dist-info/LICENSE,sha256=QDd-5ssO5cRVguOaD889uNuqyZlNg2DQS6VjttE-8Dk,1069
-pyawsopstoolkit.exceptions-0.1.0.dist-info/METADATA,sha256=ECu8V6-mo9DemX75M9J92MjmeDJEH1tFiW2yXDAtKGg,2316
-pyawsopstoolkit.exceptions-0.1.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-pyawsopstoolkit.exceptions-0.1.0.dist-info/top_level.txt,sha256=Sf9U8aiv7IzpPAt3wJmc0sUFQ7q_PyyOqUmugSJpwbA,16
-pyawsopstoolkit.exceptions-0.1.0.dist-info/RECORD,,
+pyawsopstoolkit.exceptions-0.1.1.dist-info/LICENSE,sha256=QDd-5ssO5cRVguOaD889uNuqyZlNg2DQS6VjttE-8Dk,1069
+pyawsopstoolkit.exceptions-0.1.1.dist-info/METADATA,sha256=BtJDQ7l4_Gl8MzEB5FgJyu4vSFwcfp4w4b0JKhhXkyw,2678
+pyawsopstoolkit.exceptions-0.1.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+pyawsopstoolkit.exceptions-0.1.1.dist-info/top_level.txt,sha256=Sf9U8aiv7IzpPAt3wJmc0sUFQ7q_PyyOqUmugSJpwbA,16
+pyawsopstoolkit.exceptions-0.1.1.dist-info/RECORD,,
```

