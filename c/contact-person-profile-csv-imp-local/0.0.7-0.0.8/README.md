# Comparing `tmp/contact_person_profile_csv_imp_local-0.0.7.tar.gz` & `tmp/contact_person_profile_csv_imp_local-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contact_person_profile_csv_imp_local-0.0.7.tar", last modified: Fri May 10 04:47:58 2024, max compression
+gzip compressed data, was "contact_person_profile_csv_imp_local-0.0.8.tar", last modified: Tue May 14 20:50:52 2024, max compression
```

## Comparing `contact_person_profile_csv_imp_local-0.0.7.tar` & `contact_person_profile_csv_imp_local-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:47:58.539374 contact_person_profile_csv_imp_local-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-10 04:47:58.539374 contact_person_profile_csv_imp_local-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-10 04:47:36.000000 contact_person_profile_csv_imp_local-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:47:58.535374 contact_person_profile_csv_imp_local-0.0.7/contact_person_profile_csv_imp_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:47:58.539374 contact_person_profile_csv_imp_local-0.0.7/contact_person_profile_csv_imp_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)    21321 2024-05-10 04:47:36.000000 contact_person_profile_csv_imp_local-0.0.7/contact_person_profile_csv_imp_local/src/CSVToContactPersonProfile.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 04:47:36.000000 contact_person_profile_csv_imp_local-0.0.7/contact_person_profile_csv_imp_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10459 2024-05-10 04:47:36.000000 contact_person_profile_csv_imp_local-0.0.7/contact_person_profile_csv_imp_local/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:47:58.539374 contact_person_profile_csv_imp_local-0.0.7/contact_person_profile_csv_imp_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-10 04:47:58.000000 contact_person_profile_csv_imp_local-0.0.7/contact_person_profile_csv_imp_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-10 04:47:58.000000 contact_person_profile_csv_imp_local-0.0.7/contact_person_profile_csv_imp_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 04:47:58.000000 contact_person_profile_csv_imp_local-0.0.7/contact_person_profile_csv_imp_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-10 04:47:58.000000 contact_person_profile_csv_imp_local-0.0.7/contact_person_profile_csv_imp_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-10 04:47:58.000000 contact_person_profile_csv_imp_local-0.0.7/contact_person_profile_csv_imp_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-10 04:47:36.000000 contact_person_profile_csv_imp_local-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 04:47:58.539374 contact_person_profile_csv_imp_local-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-10 04:47:36.000000 contact_person_profile_csv_imp_local-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:50:52.304778 contact_person_profile_csv_imp_local-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-14 20:50:52.304778 contact_person_profile_csv_imp_local-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-14 20:50:12.000000 contact_person_profile_csv_imp_local-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:50:52.300778 contact_person_profile_csv_imp_local-0.0.8/contact_person_profile_csv_imp_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:50:52.304778 contact_person_profile_csv_imp_local-0.0.8/contact_person_profile_csv_imp_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    50693 2024-05-14 20:50:12.000000 contact_person_profile_csv_imp_local-0.0.8/contact_person_profile_csv_imp_local/src/CSVToContactPersonProfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 20:50:12.000000 contact_person_profile_csv_imp_local-0.0.8/contact_person_profile_csv_imp_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10655 2024-05-14 20:50:12.000000 contact_person_profile_csv_imp_local-0.0.8/contact_person_profile_csv_imp_local/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:50:52.304778 contact_person_profile_csv_imp_local-0.0.8/contact_person_profile_csv_imp_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-14 20:50:52.000000 contact_person_profile_csv_imp_local-0.0.8/contact_person_profile_csv_imp_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-14 20:50:52.000000 contact_person_profile_csv_imp_local-0.0.8/contact_person_profile_csv_imp_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 20:50:52.000000 contact_person_profile_csv_imp_local-0.0.8/contact_person_profile_csv_imp_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-14 20:50:52.000000 contact_person_profile_csv_imp_local-0.0.8/contact_person_profile_csv_imp_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-14 20:50:52.000000 contact_person_profile_csv_imp_local-0.0.8/contact_person_profile_csv_imp_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-14 20:50:12.000000 contact_person_profile_csv_imp_local-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 20:50:52.304778 contact_person_profile_csv_imp_local-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-14 20:50:12.000000 contact_person_profile_csv_imp_local-0.0.8/setup.py
```

### Comparing `contact_person_profile_csv_imp_local-0.0.7/PKG-INFO` & `contact_person_profile_csv_imp_local-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contact-person-profile-csv-imp-local
-Version: 0.0.7
+Version: 0.0.8
 Summary: PyPI Package for Circles CSVToContactPersonProfile-local Local/Remote Python
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `contact_person_profile_csv_imp_local-0.0.7/README.md` & `contact_person_profile_csv_imp_local-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `contact_person_profile_csv_imp_local-0.0.7/contact_person_profile_csv_imp_local/src/utils.py` & `contact_person_profile_csv_imp_local-0.0.8/contact_person_profile_csv_imp_local/src/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import List, Tuple
 
 from circles_local_database_python.generic_mapping import GenericMapping
 from dotenv import load_dotenv
+# TODO from group_remote.groups_remote
 from group_remote.group_remote import GroupsRemote
 from phone_local.phones_local import PhonesLocal
 
+# TODO Can we avoid the src.
 from src.CSVToContactPersonProfile import logger
 
 load_dotenv()
 
 
 # TODO def process_email_address( email_address: str)
 #          """ Returned email_address_id, domain_name, organization_name """
@@ -149,14 +151,15 @@
         if job_title in group:
             groups_to_link.append(group)
 
     # If no matching groups found based on job_title
     if len(groups_to_link) == 0:
         # Creating a new group with the job_title
         title = job_title
+        # TODO Why do we need the 1st parameter?
         group_id = GroupsRemote.create_group(GroupsRemote(), title=title,
                                              titleLangCode=logger.user_context.get_effective_profile_preferred_lang_code(),
                                              isInterest=True)
         # Inserting mapping between contact and the newly created group
         GenericMapping.insert_mapping(GenericMapping(), 'contact', 'group', contact_id, group_id)
         groups_linked.append((group_id, title))
     else:
@@ -166,14 +169,15 @@
                 GroupsRemote(), groupName=group).json()['data'][0]['id']
             generec_mapping.insert_mapping(
                 'contact', 'group', contact_id, group_id)
             groups_linked.append((group_id, group))
 
     # Logging the success of processing job title and returning linked group IDs and titles
     logger.end("success processing job title", object={
+        #TODO Please add a suffix to all relevant variables i.e. groups_linked
         'groups_linked': groups_linked})
     return groups_linked
 
 
 def get_all_groups_names():
     group_remote = GroupsRemote()
     groups = group_remote.get_all_groups().json()
```

### Comparing `contact_person_profile_csv_imp_local-0.0.7/contact_person_profile_csv_imp_local.egg-info/PKG-INFO` & `contact_person_profile_csv_imp_local-0.0.8/contact_person_profile_csv_imp_local.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contact-person-profile-csv-imp-local
-Version: 0.0.7
+Version: 0.0.8
 Summary: PyPI Package for Circles CSVToContactPersonProfile-local Local/Remote Python
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `contact_person_profile_csv_imp_local-0.0.7/pyproject.toml` & `contact_person_profile_csv_imp_local-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `contact_person_profile_csv_imp_local-0.0.7/setup.py` & `contact_person_profile_csv_imp_local-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = 'contact-person-profile-csv-imp-local'
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.7',  # https://pypi.org/project/contact-person-profile-csv-imp-local/
+    version='0.0.8',  # https://pypi.org/project/contact-person-profile-csv-imp-local/
     author="Circles",
     author_email="info@circles.ai",
     description="PyPI Package for Circles CSVToContactPersonProfile-local Local/Remote Python",
     long_description="This is a package for sharing common XXX function used in different repositories",
     long_description_content_type="text/markdown",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
```

