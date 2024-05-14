# Comparing `tmp/sophosfirewall_python-0.1.37.tar.gz` & `tmp/sophosfirewall_python-0.1.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sophosfirewall_python-0.1.37.tar", max compression
+gzip compressed data, was "sophosfirewall_python-0.1.38.tar", max compression
```

## Comparing `sophosfirewall_python-0.1.37.tar` & `sophosfirewall_python-0.1.38.tar`

### file list

```diff
@@ -1,25 +1,28 @@
--rw-r--r--   0        0        0    11357 2024-05-13 21:55:02.926198 sophosfirewall_python-0.1.37/LICENSE
--rw-r--r--   0        0        0     9124 2024-05-13 21:55:02.926198 sophosfirewall_python-0.1.37/README.md
--rw-r--r--   0        0        0      675 2024-05-13 21:55:02.946198 sophosfirewall_python-0.1.37/pyproject.toml
--rw-r--r--   0        0        0    48371 2024-05-13 21:55:02.946198 sophosfirewall_python-0.1.37/sophosfirewall_python/firewallapi.py
--rw-r--r--   0        0        0     1681 2024-05-13 21:55:02.946198 sophosfirewall_python-0.1.37/sophosfirewall_python/templates/createfwrule.j2
--rw-r--r--   0        0        0      356 2024-05-13 21:55:02.946198 sophosfirewall_python-0.1.37/sophosfirewall_python/templates/createiphost.j2
--rw-r--r--   0        0        0      463 2024-05-13 21:55:02.946198 sophosfirewall_python-0.1.37/sophosfirewall_python/templates/createiphostgroup.j2
--rw-r--r--   0        0        0      397 2024-05-13 21:55:02.946198 sophosfirewall_python-0.1.37/sophosfirewall_python/templates/createipnetwork.j2
--rw-r--r--   0        0        0      402 2024-05-13 21:55:02.946198 sophosfirewall_python-0.1.37/sophosfirewall_python/templates/createiprange.j2
--rw-r--r--   0        0        0     1491 2024-05-13 21:55:02.946198 sophosfirewall_python-0.1.37/sophosfirewall_python/templates/createservice.j2
--rw-r--r--   0        0        0      406 2024-05-13 21:55:02.946198 sophosfirewall_python-0.1.37/sophosfirewall_python/templates/createurlgroup.j2
--rw-r--r--   0        0        0     2210 2024-05-13 21:55:02.946198 sophosfirewall_python-0.1.37/sophosfirewall_python/templates/createuser.j2
--rw-r--r--   0        0        0      326 2024-05-13 21:55:02.946198 sophosfirewall_python-0.1.37/sophosfirewall_python/templates/updateadminpassword.j2
--rw-r--r--   0        0        0     1432 2024-05-13 21:55:02.946198 sophosfirewall_python-0.1.37/sophosfirewall_python/templates/updatebackup.j2
--rw-r--r--   0        0        0      482 2024-05-13 21:55:02.946198 sophosfirewall_python-0.1.37/sophosfirewall_python/templates/updateiphostgroup.j2
--rw-r--r--   0        0        0     1493 2024-05-13 21:55:02.946198 sophosfirewall_python-0.1.37/sophosfirewall_python/templates/updateservice.j2
--rw-r--r--   0        0        0      615 2024-05-13 21:55:02.946198 sophosfirewall_python-0.1.37/sophosfirewall_python/templates/updateserviceacl.j2
--rw-r--r--   0        0        0      409 2024-05-13 21:55:02.946198 sophosfirewall_python-0.1.37/sophosfirewall_python/templates/updateurlgroup.j2
--rw-r--r--   0        0        0     2231 2024-05-13 21:55:02.946198 sophosfirewall_python-0.1.37/sophosfirewall_python/templates/updateuserpassword.j2
--rw-r--r--   0        0        0        0 2024-05-13 21:55:02.946198 sophosfirewall_python-0.1.37/sophosfirewall_python/tests/__init__.py
--rw-r--r--   0        0        0    16562 2024-05-13 21:55:02.946198 sophosfirewall_python-0.1.37/sophosfirewall_python/tests/functional.py
--rw-r--r--   0        0        0      103 2024-05-13 21:55:02.946198 sophosfirewall_python-0.1.37/sophosfirewall_python/tests/pytest.ini
--rw-r--r--   0        0        0    30393 2024-05-13 21:55:02.946198 sophosfirewall_python-0.1.37/sophosfirewall_python/tests/unittests.py
--rw-r--r--   0        0        0      522 2024-05-13 21:55:02.946198 sophosfirewall_python-0.1.37/sophosfirewall_python/urlgroup_example.j2
--rw-r--r--   0        0        0     9733 1970-01-01 00:00:00.000000 sophosfirewall_python-0.1.37/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-14 13:58:12.118823 sophosfirewall_python-0.1.38/LICENSE
+-rw-r--r--   0        0        0     9124 2024-05-14 13:58:12.118823 sophosfirewall_python-0.1.38/README.md
+-rw-r--r--   0        0        0      675 2024-05-14 13:58:12.138823 sophosfirewall_python-0.1.38/pyproject.toml
+-rw-r--r--   0        0        0    53144 2024-05-14 13:58:12.138823 sophosfirewall_python-0.1.38/sophosfirewall_python/firewallapi.py
+-rw-r--r--   0        0        0      570 2024-05-14 13:58:12.138823 sophosfirewall_python-0.1.38/sophosfirewall_python/templates/createfqdnhost.j2
+-rw-r--r--   0        0        0      524 2024-05-14 13:58:12.138823 sophosfirewall_python-0.1.38/sophosfirewall_python/templates/createfqdnhostgroup.j2
+-rw-r--r--   0        0        0     1681 2024-05-14 13:58:12.138823 sophosfirewall_python-0.1.38/sophosfirewall_python/templates/createfwrule.j2
+-rw-r--r--   0        0        0      356 2024-05-14 13:58:12.138823 sophosfirewall_python-0.1.38/sophosfirewall_python/templates/createiphost.j2
+-rw-r--r--   0        0        0      463 2024-05-14 13:58:12.138823 sophosfirewall_python-0.1.38/sophosfirewall_python/templates/createiphostgroup.j2
+-rw-r--r--   0        0        0      397 2024-05-14 13:58:12.138823 sophosfirewall_python-0.1.38/sophosfirewall_python/templates/createipnetwork.j2
+-rw-r--r--   0        0        0      402 2024-05-14 13:58:12.138823 sophosfirewall_python-0.1.38/sophosfirewall_python/templates/createiprange.j2
+-rw-r--r--   0        0        0     1491 2024-05-14 13:58:12.138823 sophosfirewall_python-0.1.38/sophosfirewall_python/templates/createservice.j2
+-rw-r--r--   0        0        0      406 2024-05-14 13:58:12.138823 sophosfirewall_python-0.1.38/sophosfirewall_python/templates/createurlgroup.j2
+-rw-r--r--   0        0        0     2210 2024-05-14 13:58:12.138823 sophosfirewall_python-0.1.38/sophosfirewall_python/templates/createuser.j2
+-rw-r--r--   0        0        0      326 2024-05-14 13:58:12.138823 sophosfirewall_python-0.1.38/sophosfirewall_python/templates/updateadminpassword.j2
+-rw-r--r--   0        0        0     1432 2024-05-14 13:58:12.138823 sophosfirewall_python-0.1.38/sophosfirewall_python/templates/updatebackup.j2
+-rw-r--r--   0        0        0      473 2024-05-14 13:58:12.138823 sophosfirewall_python-0.1.38/sophosfirewall_python/templates/updatefqdnhostgroup.j2
+-rw-r--r--   0        0        0      482 2024-05-14 13:58:12.138823 sophosfirewall_python-0.1.38/sophosfirewall_python/templates/updateiphostgroup.j2
+-rw-r--r--   0        0        0     1493 2024-05-14 13:58:12.138823 sophosfirewall_python-0.1.38/sophosfirewall_python/templates/updateservice.j2
+-rw-r--r--   0        0        0      615 2024-05-14 13:58:12.138823 sophosfirewall_python-0.1.38/sophosfirewall_python/templates/updateserviceacl.j2
+-rw-r--r--   0        0        0      409 2024-05-14 13:58:12.138823 sophosfirewall_python-0.1.38/sophosfirewall_python/templates/updateurlgroup.j2
+-rw-r--r--   0        0        0     2231 2024-05-14 13:58:12.138823 sophosfirewall_python-0.1.38/sophosfirewall_python/templates/updateuserpassword.j2
+-rw-r--r--   0        0        0        0 2024-05-14 13:58:12.142823 sophosfirewall_python-0.1.38/sophosfirewall_python/tests/__init__.py
+-rw-r--r--   0        0        0    19982 2024-05-14 13:58:12.142823 sophosfirewall_python-0.1.38/sophosfirewall_python/tests/functional.py
+-rw-r--r--   0        0        0      103 2024-05-14 13:58:12.142823 sophosfirewall_python-0.1.38/sophosfirewall_python/tests/pytest.ini
+-rw-r--r--   0        0        0    30393 2024-05-14 13:58:12.142823 sophosfirewall_python-0.1.38/sophosfirewall_python/tests/unittests.py
+-rw-r--r--   0        0        0      522 2024-05-14 13:58:12.142823 sophosfirewall_python-0.1.38/sophosfirewall_python/urlgroup_example.j2
+-rw-r--r--   0        0        0     9733 1970-01-01 00:00:00.000000 sophosfirewall_python-0.1.38/PKG-INFO
```

### Comparing `sophosfirewall_python-0.1.37/LICENSE` & `sophosfirewall_python-0.1.38/LICENSE`

 * *Files identical despite different names*

### Comparing `sophosfirewall_python-0.1.37/README.md` & `sophosfirewall_python-0.1.38/README.md`

 * *Files identical despite different names*

### Comparing `sophosfirewall_python-0.1.37/pyproject.toml` & `sophosfirewall_python-0.1.38/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "sophosfirewall-python"
 packages = [
     { include = "sophosfirewall_python" },
 ]
-version = "0.1.37"
+version = "0.1.38"
 description = "Python SDK for Sophos Firewall"
 authors = ["Matt Mullen <matt.mullen@sophos.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 requests = "^2.31.0"
```

### Comparing `sophosfirewall_python-0.1.37/sophosfirewall_python/firewallapi.py` & `sophosfirewall_python-0.1.38/sophosfirewall_python/firewallapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -417,14 +417,46 @@
             return self.get_tag_with_filter(
                 xml_tag="IPHost",
                 key="IPAddress",
                 value=ip_address,
                 operator=operator,
             )
         return self.get_tag(xml_tag="IPHost")
+    
+    def get_fqdn_host(
+        self, name: str = None, operator: str = "="
+    ):
+        """Get FQDN Host object(s)
+
+        Args:
+            name (str, optional): FQDN Host name. Returns all objects if not specified.
+            operator (str, optional): Operator for search. Default is "=". Valid operators: =, !=, like.
+        """
+        if name:
+            return self.get_tag_with_filter(
+                xml_tag="FQDNHost", key="Name", value=name, operator=operator
+            )
+        
+        return self.get_tag(xml_tag="FQDNHost")
+    
+    def get_fqdn_hostgroup(
+        self, name: str = None, operator: str = "="
+    ):
+        """Get FQDN HostGroup object(s)
+
+        Args:
+            name (str, optional): FQDN HostGroup name. Returns all objects if not specified.
+            operator (str, optional): Operator for search. Default is "=". Valid operators: =, !=, like.
+        """
+        if name:
+            return self.get_tag_with_filter(
+                xml_tag="FQDNHostGroup", key="Name", value=name, operator=operator
+            )
+        
+        return self.get_tag(xml_tag="FQDNHostGroup")
 
     def get_interface(self, name: str = None, operator: str = "="):
         """Get Interface object(s)
 
         Args:
             name (str, optional): Interface name. Returns all objects if not specified.
             operator (str, optional): Operator for search. Default is "=". Valid operators: =, !=, like.
@@ -460,27 +492,14 @@
                 xml_tag="IPHostGroup",
                 key="Name",
                 value=name,
                 operator=operator,
             )
         return self.get_tag(xml_tag="IPHostGroup")
 
-    def get_fqdn_host(self, name: str = None, operator: str = "="):
-        """Get FQDN object(s)
-
-        Args:
-            name (str, optional): FQDN object name. Returns all objects if not specified.
-            operator (str, optional): Operator for search. Default is "=". Valid operators: =, !=, like.
-        """
-        if name:
-            return self.get_tag_with_filter(
-                xml_tag="FQDNHost", key="Name", value=name, operator=operator
-            )
-        return self.get_tag(xml_tag="FQDNHost")
-
     def get_acl_rule(self, name: str = None, operator: str = "="):
         """Get ACL rules
 
         Args:
             name (str, optional): Name of rule to retrieve. Returns all if not specified.
             operator (str, optional): Operator for search. Default is "=". Valid operators: =, !=, like.
 
@@ -794,14 +813,58 @@
         self._validate_ip_address(ip_address)
 
         params = {"name": name, "ip_address": ip_address}
         resp = self.submit_template(
             "createiphost.j2", template_vars=params, debug=debug
         )
         return resp
+    
+    def create_fqdn_host(self, name: str,
+                         description: str,
+                         fqdn: str,
+                         fqdn_group_list: list = None,
+                         debug: bool = False):
+        """Create FQDN Host object.
+
+        Args:
+            name (str): Name of the object.
+            description (str): Description. 
+            fqdn (str): FQDN string.
+            fqdn_group_list (list, optional): List containing FQDN Host Group(s) to associate the FQDN Host.
+            debug (bool, optional): Turn on debugging. Defaults to False.
+        Returns:
+            dict: XML response converted to Python dictionary.
+        """
+
+        params = {"name": name, "description": description, "fqdn": fqdn, "fqdn_group_list": fqdn_group_list}
+        resp = self.submit_template(
+            "createfqdnhost.j2", template_vars=params, debug=debug
+        )
+        return resp
+
+    def create_fqdn_hostgroup(self, name: str,
+                         description: str,
+                         fqdn_host_list: list = None,
+                         debug: bool = False):
+        """Create FQDN HostGroup object.
+
+        Args:
+            name (str): Name of the object.
+            description (str): Description. 
+            fqdn_host_list (list, optional): List containing FQDN Host(s) to associate the FQDN Host Group.
+            debug (bool, optional): Turn on debugging. Defaults to False.
+        Returns:
+            dict: XML response converted to Python dictionary.
+        """
+
+        params = {"name": name, "description": description, "fqdn_host_list": fqdn_host_list}
+        resp = self.submit_template(
+            "createfqdnhostgroup.j2", template_vars=params, debug=debug
+        )
+        return resp
 
     def create_ip_range(
         self,
         name: str,
         start_ip: str,
         end_ip: str,
         debug: bool = False,
@@ -1160,15 +1223,15 @@
         self,
         name: str,
         host_list: list,
         description: str = None,
         action: str = "add",
         debug: bool = False,
     ):
-        """Add or remove a specified domain to/from a web URL Group
+        """Add or remove an IP Host from an IP HostGroup.
 
         Args:
             name (str): IP Host Group name.
             description (str): IP Host Group description.
             host_list (str): List of IP Hosts to be added to or removed from the Host List.
             action (str): Options are 'add', 'remove' or 'replace'. Specify None to disable updating Host List. Defaults to 'add'.
             debug (bool, optional): Enable debug mode. Defaults to False.
@@ -1215,14 +1278,78 @@
 
         params = {"name": name, "description": description, "host_list": new_host_list}
         resp = self.submit_template(
             "updateiphostgroup.j2", template_vars=params, debug=debug
         )
         return resp
 
+    def update_fqdn_hostgroup(
+        self,
+        name: str,
+        fqdn_host_list: list,
+        description: str = None,
+        action: str = "add",
+        debug: bool = False,
+    ):
+        """Add or remove a FQDN Host from an FQDN Host Group.
+
+        Args:
+            name (str): FQDN Host Group name.
+            description (str): FQDN Host Group description.
+            fqdn_host_list (str): List of FQDN Hosts to be added to or removed from the FQDN Host list.
+            action (str): Options are 'add', 'remove' or 'replace'. Specify None to disable updating FQDN Host List. Defaults to 'add'.
+            debug (bool, optional): Enable debug mode. Defaults to False.
+
+        Returns:
+            dict: XML response converted to Python dictionary
+        """
+        # Get the existing Host list first, if any
+
+        if action:
+            self._validate_arg(
+                arg_name="action",
+                arg_value=action,
+                valid_choices=["add", "remove", "replace"],
+            )
+
+        resp = self.get_fqdn_hostgroup(name=name)
+        if "FQDNHostList" in resp["Response"]["FQDNHostGroup"]:
+            exist_list = (
+                resp.get("Response").get("FQDNHostGroup").get("FQDNHostList").get("FQDNHost")
+            )
+        else:
+            exist_list = None
+
+        if action.lower() == "replace":
+            exist_list = None
+
+        new_host_list = []
+        if exist_list:
+            if isinstance(exist_list, str):
+                new_host_list.append(exist_list)
+            elif isinstance(exist_list, list):
+                new_host_list = exist_list
+        for fqdn_host in fqdn_host_list:
+            if action:
+                if action.lower() == "add" and not fqdn_host in new_host_list:
+                    new_host_list.append(fqdn_host)
+                elif action.lower() == "remove" and fqdn_host in new_host_list:
+                    new_host_list.remove(fqdn_host)
+                elif action.lower() == "replace":
+                    new_host_list.append(fqdn_host)
+        if not description:
+            description = resp.get("Response").get("FQDNHostGroup").get("Description")
+
+        params = {"name": name, "description": description, "fqdn_host_list": new_host_list}
+        resp = self.submit_template(
+            "updatefqdnhostgroup.j2", template_vars=params, debug=debug
+        )
+        return resp
+
+
     def update_backup(self, backup_params: dict, debug: bool = False):
         """Updates scheduled backup settings
 
         Args:
             backup_params (dict): Dict containing backup settings
             debug (bool, optional): Enable debug mode. Defaults to False.
```

### Comparing `sophosfirewall_python-0.1.37/sophosfirewall_python/templates/createfwrule.j2` & `sophosfirewall_python-0.1.38/sophosfirewall_python/templates/createfwrule.j2`

 * *Files identical despite different names*

### Comparing `sophosfirewall_python-0.1.37/sophosfirewall_python/templates/createservice.j2` & `sophosfirewall_python-0.1.38/sophosfirewall_python/templates/createservice.j2`

 * *Files identical despite different names*

### Comparing `sophosfirewall_python-0.1.37/sophosfirewall_python/templates/createuser.j2` & `sophosfirewall_python-0.1.38/sophosfirewall_python/templates/createuser.j2`

 * *Files identical despite different names*

### Comparing `sophosfirewall_python-0.1.37/sophosfirewall_python/templates/updatebackup.j2` & `sophosfirewall_python-0.1.38/sophosfirewall_python/templates/updatebackup.j2`

 * *Files identical despite different names*

### Comparing `sophosfirewall_python-0.1.37/sophosfirewall_python/templates/updateservice.j2` & `sophosfirewall_python-0.1.38/sophosfirewall_python/templates/updateservice.j2`

 * *Files identical despite different names*

### Comparing `sophosfirewall_python-0.1.37/sophosfirewall_python/templates/updateserviceacl.j2` & `sophosfirewall_python-0.1.38/sophosfirewall_python/templates/updateserviceacl.j2`

 * *Files identical despite different names*

### Comparing `sophosfirewall_python-0.1.37/sophosfirewall_python/templates/updateuserpassword.j2` & `sophosfirewall_python-0.1.38/sophosfirewall_python/templates/updateuserpassword.j2`

 * *Files identical despite different names*

### Comparing `sophosfirewall_python-0.1.37/sophosfirewall_python/tests/functional.py` & `sophosfirewall_python-0.1.38/sophosfirewall_python/tests/functional.py`

 * *Files 8% similar despite different names*

```diff
@@ -61,16 +61,19 @@
         print(
             f"{resp['Response']['LocalServiceACL']['Status']['@code']}: {resp['Response']['LocalServiceACL']['Status']['#text']}"
         )
         remove(tag="FirewallRule", name="FUNC_TESTRULE1")
         remove(tag="IPHost", name="FUNC_TESTNETWORK2")
         remove(tag="IPHost", name="FUNC_TESTNETWORK1")
         remove(tag="IPHostGroup", name="FUNC_TESTGROUP1")
+        remove(tag="FQDNHostGroup", name="FUNC_TESTFQDNGROUP1")
         remove(tag="IPHost", name="FUNC_TESTHOST1")
         remove(tag="IPHost", name="FUNC_TESTHOST2")
+        remove(tag="FQDNHost", name="FUNC_TESTFQDNHOST1")
+        remove(tag="FQDNHost", name="FUNC_TESTFQDNHOST2")
         remove(tag="Services", name="FUNC_TESTSVC1")
         remove(tag="WebFilterURLGroup", name="FUNC_URLGROUP1")
         remove(tag="User", name="func_testuser1")
 
     request.addfinalizer(cleanup)
 
 
@@ -146,14 +149,72 @@
             name="FUNC_TESTGROUP1",
             description="Test group created during functional test",
             host_list=["FUNC_TESTHOST1"],
         )
         == expected_result
     )
 
+def test_create_fqdn_host(setup):
+    """Test create_fqdn_host method."""
+
+    expected_result = {
+        "Response": {
+            "@APIVersion": API_VERSION,
+            "@IPS_CAT_VER": "1",
+            "Login": {"status": "Authentication Successful"},
+            "FQDNHost": {
+                "@transactionid": "",
+                "Status": {
+                    "@code": "200",
+                    "#text": "Configuration applied successfully.",
+                },
+            },
+        }
+    }
+    if float(API_VERSION) >= 2000.2:
+        expected_result["Response"]["@IS_WIFI6"] = "0"
+
+    fqdn_hosts = [
+        {"name": "FUNC_TESTFQDNHOST1", "fqdn": "*.test1.com"},
+        {"name": "FUNC_TESTFQDNHOST2", "fqdn": "*.test2.com"},
+    ]
+    for host in fqdn_hosts:
+        assert (
+            setup.create_fqdn_host(name=host["name"], description="Created during automated functional testing", fqdn=host["fqdn"])
+            == expected_result
+        )
+
+def test_create_fqdn_hostgroup(setup):
+    """Test create_fqdn_hostgroup method."""
+
+    expected_result = {
+        "Response": {
+            "@APIVersion": API_VERSION,
+            "@IPS_CAT_VER": "1",
+            "Login": {"status": "Authentication Successful"},
+            "FQDNHostGroup": {
+                "@transactionid": "",
+                "Status": {
+                    "@code": "200",
+                    "#text": "Configuration applied successfully.",
+                },
+            },
+        }
+    }
+    if float(API_VERSION) >= 2000.2:
+        expected_result["Response"]["@IS_WIFI6"] = "0"
+
+    assert (
+        setup.create_fqdn_hostgroup(
+            name="FUNC_TESTFQDNGROUP1",
+            description="Test group created during functional test",
+            fqdn_host_list=["FUNC_TESTFQDNHOST1"],
+        )
+        == expected_result
+    )
 
 def test_create_ip_network(setup):
     """Test create_ip_network method."""
 
     expected_result = {
         "Response": {
             "@APIVersion": API_VERSION,
@@ -374,14 +435,58 @@
     assert (
         setup.update_ip_hostgroup(name="FUNC_TESTGROUP1", host_list=["FUNC_TESTHOST2"])
         == update_result
     )
 
     assert setup.get_ip_hostgroup(name="FUNC_TESTGROUP1") == get_result
 
+def test_update_fqdn_hostgroup(setup):
+    """Test update_fqdn_hostgroup method."""
+
+    update_result = {
+        "Response": {
+            "@APIVersion": API_VERSION,
+            "@IPS_CAT_VER": "1",
+            "Login": {"status": "Authentication Successful"},
+            "FQDNHostGroup": {
+                "@transactionid": "",
+                "Status": {
+                    "@code": "200",
+                    "#text": "Configuration applied successfully.",
+                },
+            },
+        }
+    }
+    if float(API_VERSION) >= 2000.2:
+        update_result["Response"]["@IS_WIFI6"] = "0"
+
+    get_result = {
+        "Response": {
+            "@APIVersion": API_VERSION,
+            "@IPS_CAT_VER": "1",
+            "Login": {"status": "Authentication Successful"},
+            "FQDNHostGroup": {
+                "@transactionid": "",
+                "Name": "FUNC_TESTFQDNGROUP1",
+                "Description": "Test group created during functional test",
+                "FQDNHostList": {"FQDNHost": ["FUNC_TESTFQDNHOST1", "FUNC_TESTFQDNHOST2"]}
+            },
+        }
+    }
+    if float(API_VERSION) >= 2000.2:
+        get_result["Response"]["@IS_WIFI6"] = "0"
+
+    assert (
+        setup.update_fqdn_hostgroup(name="FUNC_TESTFQDNGROUP1", fqdn_host_list=["FUNC_TESTFQDNHOST2"])
+        == update_result
+    )
+
+    assert setup.get_fqdn_hostgroup(name="FUNC_TESTFQDNGROUP1") == get_result
+
+
 
 def test_update_urlgroup(setup):
     """Test update_urlgroup method."""
 
     update_result = {
         "Response": {
             "@APIVersion": API_VERSION,
```

### Comparing `sophosfirewall_python-0.1.37/sophosfirewall_python/tests/unittests.py` & `sophosfirewall_python-0.1.38/sophosfirewall_python/tests/unittests.py`

 * *Files identical despite different names*

### Comparing `sophosfirewall_python-0.1.37/sophosfirewall_python/urlgroup_example.j2` & `sophosfirewall_python-0.1.38/sophosfirewall_python/urlgroup_example.j2`

 * *Files identical despite different names*

### Comparing `sophosfirewall_python-0.1.37/PKG-INFO` & `sophosfirewall_python-0.1.38/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sophosfirewall-python
-Version: 0.1.37
+Version: 0.1.38
 Summary: Python SDK for Sophos Firewall
 Author: Matt Mullen
 Author-email: matt.mullen@sophos.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

