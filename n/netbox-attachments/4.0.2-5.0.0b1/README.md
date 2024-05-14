# Comparing `tmp/netbox-attachments-4.0.2.tar.gz` & `tmp/netbox_attachments-5.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-attachments-4.0.2.tar", last modified: Mon Feb 19 14:23:14 2024, max compression
+gzip compressed data, was "netbox_attachments-5.0.0b1.tar", last modified: Tue May 14 11:56:54 2024, max compression
```

## Comparing `netbox-attachments-4.0.2.tar` & `netbox_attachments-5.0.0b1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:23:14.842580 netbox-attachments-4.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-19 14:23:07.000000 netbox-attachments-4.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-02-19 14:23:14.842580 netbox-attachments-4.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-02-19 14:23:07.000000 netbox-attachments-4.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:23:14.838580 netbox-attachments-4.0.2/netbox_attachments/
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-02-19 14:23:07.000000 netbox-attachments-4.0.2/netbox_attachments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:23:14.838580 netbox-attachments-4.0.2/netbox_attachments/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 14:23:07.000000 netbox-attachments-4.0.2/netbox_attachments/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-02-19 14:23:07.000000 netbox-attachments-4.0.2/netbox_attachments/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-02-19 14:23:07.000000 netbox-attachments-4.0.2/netbox_attachments/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-02-19 14:23:07.000000 netbox-attachments-4.0.2/netbox_attachments/api/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-02-19 14:23:07.000000 netbox-attachments-4.0.2/netbox_attachments/filtersets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-02-19 14:23:07.000000 netbox-attachments-4.0.2/netbox_attachments/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:23:14.838580 netbox-attachments-4.0.2/netbox_attachments/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-02-19 14:23:07.000000 netbox-attachments-4.0.2/netbox_attachments/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-02-19 14:23:07.000000 netbox-attachments-4.0.2/netbox_attachments/migrations/0002_alter_netboxattachment_options_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-02-19 14:23:07.000000 netbox-attachments-4.0.2/netbox_attachments/migrations/0003_alter_netboxattachment_name.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-02-19 14:23:07.000000 netbox-attachments-4.0.2/netbox_attachments/migrations/0004_netboxattachment_size_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-02-19 14:23:07.000000 netbox-attachments-4.0.2/netbox_attachments/migrations/0005_netboxattachment_description.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 14:23:07.000000 netbox-attachments-4.0.2/netbox_attachments/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3920 2024-02-19 14:23:07.000000 netbox-attachments-4.0.2/netbox_attachments/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-02-19 14:23:07.000000 netbox-attachments-4.0.2/netbox_attachments/navigation.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-02-19 14:23:07.000000 netbox-attachments-4.0.2/netbox_attachments/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-02-19 14:23:07.000000 netbox-attachments-4.0.2/netbox_attachments/tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     6366 2024-02-19 14:23:07.000000 netbox-attachments-4.0.2/netbox_attachments/template_content.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:23:14.834580 netbox-attachments-4.0.2/netbox_attachments/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:23:14.842580 netbox-attachments-4.0.2/netbox_attachments/templates/netbox_attachments/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 14:23:07.000000 netbox-attachments-4.0.2/netbox_attachments/templates/netbox_attachments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-02-19 14:23:07.000000 netbox-attachments-4.0.2/netbox_attachments/templates/netbox_attachments/add_attachment_button.html
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-02-19 14:23:07.000000 netbox-attachments-4.0.2/netbox_attachments/templates/netbox_attachments/generic_tab_list.html
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-02-19 14:23:07.000000 netbox-attachments-4.0.2/netbox_attachments/templates/netbox_attachments/netbox_attachment_edit.html
--rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-02-19 14:23:07.000000 netbox-attachments-4.0.2/netbox_attachments/templates/netbox_attachments/netbox_attachment_panel.html
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-02-19 14:23:07.000000 netbox-attachments-4.0.2/netbox_attachments/templates/netbox_attachments/netboxattachment.html
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-02-19 14:23:07.000000 netbox-attachments-4.0.2/netbox_attachments/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-02-19 14:23:07.000000 netbox-attachments-4.0.2/netbox_attachments/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-19 14:23:07.000000 netbox-attachments-4.0.2/netbox_attachments/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-02-19 14:23:07.000000 netbox-attachments-4.0.2/netbox_attachments/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:23:14.842580 netbox-attachments-4.0.2/netbox_attachments.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-02-19 14:23:14.000000 netbox-attachments-4.0.2/netbox_attachments.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-02-19 14:23:14.000000 netbox-attachments-4.0.2/netbox_attachments.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 14:23:14.000000 netbox-attachments-4.0.2/netbox_attachments.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 14:23:14.000000 netbox-attachments-4.0.2/netbox_attachments.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-19 14:23:14.000000 netbox-attachments-4.0.2/netbox_attachments.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-19 14:23:14.842580 netbox-attachments-4.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-02-19 14:23:07.000000 netbox-attachments-4.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:54.255107 netbox_attachments-5.0.0b1/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3894 2024-05-14 11:56:54.251108 netbox_attachments-5.0.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:54.251108 netbox_attachments-5.0.0b1/netbox_attachments/
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/netbox_attachments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:54.251108 netbox_attachments-5.0.0b1/netbox_attachments/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/netbox_attachments/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/netbox_attachments/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/netbox_attachments/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/netbox_attachments/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/netbox_attachments/filtersets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/netbox_attachments/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:54.251108 netbox_attachments-5.0.0b1/netbox_attachments/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/netbox_attachments/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/netbox_attachments/migrations/0002_alter_netboxattachment_options_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/netbox_attachments/migrations/0003_alter_netboxattachment_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/netbox_attachments/migrations/0004_netboxattachment_size_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/netbox_attachments/migrations/0005_netboxattachment_description.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/netbox_attachments/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3920 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/netbox_attachments/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/netbox_attachments/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/netbox_attachments/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/netbox_attachments/tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6365 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/netbox_attachments/template_content.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:54.247107 netbox_attachments-5.0.0b1/netbox_attachments/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:54.251108 netbox_attachments-5.0.0b1/netbox_attachments/templates/netbox_attachments/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/netbox_attachments/templates/netbox_attachments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/netbox_attachments/templates/netbox_attachments/add_attachment_button.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/netbox_attachments/templates/netbox_attachments/generic_tab_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/netbox_attachments/templates/netbox_attachments/netbox_attachment_edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/netbox_attachments/templates/netbox_attachments/netbox_attachment_panel.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/netbox_attachments/templates/netbox_attachments/netboxattachment.html
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/netbox_attachments/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/netbox_attachments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/netbox_attachments/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/netbox_attachments/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:54.251108 netbox_attachments-5.0.0b1/netbox_attachments.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3894 2024-05-14 11:56:54.000000 netbox_attachments-5.0.0b1/netbox_attachments.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-14 11:56:54.000000 netbox_attachments-5.0.0b1/netbox_attachments.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 11:56:54.000000 netbox_attachments-5.0.0b1/netbox_attachments.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 11:56:54.000000 netbox_attachments-5.0.0b1/netbox_attachments.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-14 11:56:54.000000 netbox_attachments-5.0.0b1/netbox_attachments.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 11:56:54.255107 netbox_attachments-5.0.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/setup.py
```

### Comparing `netbox-attachments-4.0.2/PKG-INFO` & `netbox_attachments-5.0.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-attachments
-Version: 4.0.2
+Version: 5.0.0b1
 Summary: Netbox plugin to manage attachments for any model
 Home-page: https://github.com/Kani999/netbox-attachments
 Author: Jan Krupa
 Keywords: netbox,netbox-plugin
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
@@ -25,15 +25,16 @@
 | Netbox   | Plugin          |
 | -------- | --------------- |
 | >= 3.3.4 | 0.0.0 <-> 0.0.5 |
 | >= 3.4.0 | 0.0.6 <-> 1.0.6 |
 | >= 3.4.3 | 1.0.7 <-> 1.1.X |
 | >= 3.5.0 | 2.0.0           |
 | >= 3.6.0 | 3.0.0           |
-| >= 3.7.0 | 4.0.0 
+| >= 3.7.0 | 4.0.0           |
+| >= 4.0.0 | 5.0.0-beta1     |
 
 ## Installation
 
 The plugin is available as a Python package in pypi and can be installed with pip
 
 ```
 pip install netbox-attachments
```

### Comparing `netbox-attachments-4.0.2/README.md` & `netbox_attachments-5.0.0b1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 | Netbox   | Plugin          |
 | -------- | --------------- |
 | >= 3.3.4 | 0.0.0 <-> 0.0.5 |
 | >= 3.4.0 | 0.0.6 <-> 1.0.6 |
 | >= 3.4.3 | 1.0.7 <-> 1.1.X |
 | >= 3.5.0 | 2.0.0           |
 | >= 3.6.0 | 3.0.0           |
-| >= 3.7.0 | 4.0.0 
+| >= 3.7.0 | 4.0.0           |
+| >= 4.0.0 | 5.0.0-beta1     |
 
 ## Installation
 
 The plugin is available as a Python package in pypi and can be installed with pip
 
 ```
 pip install netbox-attachments
```

### Comparing `netbox-attachments-4.0.2/netbox_attachments/__init__.py` & `netbox_attachments-5.0.0b1/netbox_attachments/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from extras.plugins import PluginConfig
-
+from netbox.plugins import PluginConfig
 from .version import __version__
 
 
 class NetBoxAttachmentsConfig(PluginConfig):
     name = 'netbox_attachments'
     verbose_name = 'Netbox Attachments'
     description = 'Netbox plugin to manage attachments for any model'
@@ -12,12 +11,12 @@
     base_url = 'netbox-attachments'
     default_settings = {
         'apps': ['dcim', 'ipam', 'circuits', 'tenancy', 'virtualization', 'wireless'],
         'display_default': "additional_tab",
         'display_setting': {}
     }
     required_settings = []
-    min_version = '3.5.0'
-    max_version = '3.7.99'
+    min_version = '4.0.0'
+    max_version = '4.0.99'
 
 
 config = NetBoxAttachmentsConfig
```

### Comparing `netbox-attachments-4.0.2/netbox_attachments/api/serializers.py` & `netbox_attachments-5.0.0b1/netbox_attachments/api/serializers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from django.contrib.contenttypes.models import ContentType
 from django.core.exceptions import ObjectDoesNotExist
-#from drf_yasg.utils import swagger_serializer_method
+# from drf_yasg.utils import swagger_serializer_method
 from netbox.api.fields import ContentTypeField
 from netbox.api.serializers import NetBoxModelSerializer
 from netbox.constants import NESTED_SERIALIZER_PREFIX
 from rest_framework import serializers
 from utilities.api import get_serializer_for_model
 
 from ..models import NetBoxAttachment
@@ -19,14 +19,15 @@
     parent = serializers.SerializerMethodField(read_only=True)
 
     class Meta:
         model = NetBoxAttachment
         fields = [
             'id', 'url', 'display', 'content_type', 'object_id', 'parent', 'name', 'description', 'file', 'created', 'last_updated', 'comments',
         ]
+        brief_fields = ('id', 'url', 'display', 'name', 'description', 'file')
 
     def validate(self, data):
         # Validate that the parent object exists
         try:
             if 'content_type' in data and 'object_id' in data:
                 data['content_type'].get_object_for_this_type(
                     id=data['object_id'])
@@ -37,15 +38,15 @@
             )
 
         # Enforce model validation
         super().validate(data)
 
         return data
 
-    #@swagger_serializer_method(serializer_or_field=serializers.JSONField)
+    # @swagger_serializer_method(serializer_or_field=serializers.JSONField)
     def get_parent(self, obj):
         if obj.parent:
             serializer = get_serializer_for_model(
                 obj.parent, prefix=NESTED_SERIALIZER_PREFIX)
             return serializer(obj.parent, context={'request': self.context['request']}).data
         else:
             return None
```

### Comparing `netbox-attachments-4.0.2/netbox_attachments/filtersets.py` & `netbox_attachments-5.0.0b1/netbox_attachments/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox-attachments-4.0.2/netbox_attachments/forms.py` & `netbox_attachments-5.0.0b1/netbox_attachments/forms.py`

 * *Files identical despite different names*

### Comparing `netbox-attachments-4.0.2/netbox_attachments/migrations/0001_initial.py` & `netbox_attachments-5.0.0b1/netbox_attachments/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-attachments-4.0.2/netbox_attachments/migrations/0002_alter_netboxattachment_options_and_more.py` & `netbox_attachments-5.0.0b1/netbox_attachments/migrations/0002_alter_netboxattachment_options_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-attachments-4.0.2/netbox_attachments/migrations/0004_netboxattachment_size_and_more.py` & `netbox_attachments-5.0.0b1/netbox_attachments/migrations/0004_netboxattachment_size_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-attachments-4.0.2/netbox_attachments/models.py` & `netbox_attachments-5.0.0b1/netbox_attachments/models.py`

 * *Files identical despite different names*

### Comparing `netbox-attachments-4.0.2/netbox_attachments/tables.py` & `netbox_attachments-5.0.0b1/netbox_attachments/tables.py`

 * *Files identical despite different names*

### Comparing `netbox-attachments-4.0.2/netbox_attachments/template_content.py` & `netbox_attachments-5.0.0b1/netbox_attachments/template_content.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 
 from django.conf import settings
 from django.contrib.contenttypes.models import ContentType
 from django.db.utils import OperationalError
-from extras.plugins import PluginTemplateExtension
+from netbox.plugins import PluginTemplateExtension
+
 from netbox.views import generic
 from utilities.views import ViewTab, register_model_view
 from netbox.context import current_request
 
 from . import filtersets, models, tables
 from .models import NetBoxAttachment
 
@@ -95,15 +96,15 @@
         tab = ViewTab(
             label="Attachments",
             badge=lambda obj: models.NetBoxAttachment.objects.filter(
                 content_type=ContentType.objects.get_for_model(obj),
                 object_id=obj.id,
             ).restrict(current_request.get().user, 'view').count(),
             hide_if_empty=False,
-            permission = "netbox_attachments.view_netboxattachment"
+            permission="netbox_attachments.view_netboxattachment"
         )
 
         def get_children(self, request, parent):
             childrens = self.child_model.objects.filter(
                 content_type=ContentType.objects.get_for_model(parent),
                 object_id=parent.id,
             ).restrict(request.user, 'view')
```

### Comparing `netbox-attachments-4.0.2/netbox_attachments/templates/netbox_attachments/generic_tab_list.html` & `netbox_attachments-5.0.0b1/netbox_attachments/templates/netbox_attachments/generic_tab_list.html`

 * *Files identical despite different names*

### Comparing `netbox-attachments-4.0.2/netbox_attachments/templates/netbox_attachments/netbox_attachment_edit.html` & `netbox_attachments-5.0.0b1/netbox_attachments/templates/netbox_attachments/netbox_attachment_edit.html`

 * *Files identical despite different names*

### Comparing `netbox-attachments-4.0.2/netbox_attachments/templates/netbox_attachments/netbox_attachment_panel.html` & `netbox_attachments-5.0.0b1/netbox_attachments/templates/netbox_attachments/netbox_attachment_panel.html`

 * *Files identical despite different names*

### Comparing `netbox-attachments-4.0.2/netbox_attachments/templates/netbox_attachments/netboxattachment.html` & `netbox_attachments-5.0.0b1/netbox_attachments/templates/netbox_attachments/netboxattachment.html`

 * *Files identical despite different names*

### Comparing `netbox-attachments-4.0.2/netbox_attachments/urls.py` & `netbox_attachments-5.0.0b1/netbox_attachments/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-attachments-4.0.2/netbox_attachments/views.py` & `netbox_attachments-5.0.0b1/netbox_attachments/views.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,15 +7,20 @@
 
 class NetBoxAttachmentView(generic.ObjectView):
     controls = []
     queryset = models.NetBoxAttachment.objects.all()
 
 
 class NetBoxAttachmentListView(generic.ObjectListView):
-    actions = ['export']
+    actions = {
+        'import': {'add'},
+        'export': set(),
+        'bulk_edit': {'change'},
+        'bulk_delete': {'delete'},
+    }
     queryset = models.NetBoxAttachment.objects.all()
     table = tables.NetBoxAttachmentTable
     filterset = filtersets.NetBoxAttachmentFilterSet
     filterset_form = forms.NetBoxAttachmentFilterForm
 
 
 class NetBoxAttachmentEditView(generic.ObjectEditView):
```

### Comparing `netbox-attachments-4.0.2/netbox_attachments.egg-info/PKG-INFO` & `netbox_attachments-5.0.0b1/netbox_attachments.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-attachments
-Version: 4.0.2
+Version: 5.0.0b1
 Summary: Netbox plugin to manage attachments for any model
 Home-page: https://github.com/Kani999/netbox-attachments
 Author: Jan Krupa
 Keywords: netbox,netbox-plugin
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
@@ -25,15 +25,16 @@
 | Netbox   | Plugin          |
 | -------- | --------------- |
 | >= 3.3.4 | 0.0.0 <-> 0.0.5 |
 | >= 3.4.0 | 0.0.6 <-> 1.0.6 |
 | >= 3.4.3 | 1.0.7 <-> 1.1.X |
 | >= 3.5.0 | 2.0.0           |
 | >= 3.6.0 | 3.0.0           |
-| >= 3.7.0 | 4.0.0 
+| >= 3.7.0 | 4.0.0           |
+| >= 4.0.0 | 5.0.0-beta1     |
 
 ## Installation
 
 The plugin is available as a Python package in pypi and can be installed with pip
 
 ```
 pip install netbox-attachments
```

### Comparing `netbox-attachments-4.0.2/netbox_attachments.egg-info/SOURCES.txt` & `netbox_attachments-5.0.0b1/netbox_attachments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox-attachments-4.0.2/setup.py` & `netbox_attachments-5.0.0b1/setup.py`

 * *Files identical despite different names*

