# Comparing `tmp/civipy-0.0.2.tar.gz` & `tmp/civipy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "civipy-0.0.2.tar", last modified: Sun Jan 14 00:13:44 2024, max compression
+gzip compressed data, was "civipy-0.0.3.tar", last modified: Tue May 14 19:55:07 2024, max compression
```

## Comparing `civipy-0.0.2.tar` & `civipy-0.0.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 00:13:44.629760 civipy-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    34916 2024-01-14 00:13:36.000000 civipy-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-01-14 00:13:36.000000 civipy-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-01-14 00:13:44.629760 civipy-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-01-14 00:13:36.000000 civipy-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-14 00:13:36.000000 civipy-0.0.2/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 00:13:44.625760 civipy-0.0.2/civipy/
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-01-14 00:13:36.000000 civipy-0.0.2/civipy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-01-14 00:13:36.000000 civipy-0.0.2/civipy/address.py
--rw-r--r--   0 runner    (1001) docker     (127)    10350 2024-01-14 00:13:36.000000 civipy-0.0.2/civipy/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-01-14 00:13:36.000000 civipy-0.0.2/civipy/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-01-14 00:13:36.000000 civipy-0.0.2/civipy/contact.py
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-01-14 00:13:36.000000 civipy-0.0.2/civipy/contribution.py
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-01-14 00:13:36.000000 civipy-0.0.2/civipy/country.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-14 00:13:36.000000 civipy-0.0.2/civipy/custom_field.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-01-14 00:13:36.000000 civipy-0.0.2/civipy/event.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-01-14 00:13:36.000000 civipy-0.0.2/civipy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-01-14 00:13:36.000000 civipy-0.0.2/civipy/membership.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-01-14 00:13:36.000000 civipy-0.0.2/civipy/note.py
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-01-14 00:13:36.000000 civipy-0.0.2/civipy/option_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-01-14 00:13:36.000000 civipy-0.0.2/civipy/order.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-01-14 00:13:36.000000 civipy-0.0.2/civipy/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 00:13:44.629760 civipy-0.0.2/civipy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-01-14 00:13:44.000000 civipy-0.0.2/civipy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-01-14 00:13:44.000000 civipy-0.0.2/civipy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-14 00:13:44.000000 civipy-0.0.2/civipy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-01-14 00:13:44.000000 civipy-0.0.2/civipy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-14 00:13:44.000000 civipy-0.0.2/civipy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-01-14 00:13:36.000000 civipy-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-14 00:13:44.629760 civipy-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 00:13:44.629760 civipy-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-01-14 00:13:36.000000 civipy-0.0.2/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-01-14 00:13:36.000000 civipy-0.0.2/tests/test_contact.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-01-14 00:13:36.000000 civipy-0.0.2/tests/test_contribution.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:55:07.141111 civipy-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    34916 2024-05-14 19:55:02.000000 civipy-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-14 19:55:02.000000 civipy-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-05-14 19:55:07.137111 civipy-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-05-14 19:55:02.000000 civipy-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-14 19:55:02.000000 civipy-0.0.3/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:55:07.137111 civipy-0.0.3/civipy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-05-14 19:55:02.000000 civipy-0.0.3/civipy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-14 19:55:02.000000 civipy-0.0.3/civipy/activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-05-14 19:55:02.000000 civipy-0.0.3/civipy/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5770 2024-05-14 19:55:02.000000 civipy-0.0.3/civipy/contact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-14 19:55:02.000000 civipy-0.0.3/civipy/contribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-14 19:55:02.000000 civipy-0.0.3/civipy/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-14 19:55:02.000000 civipy-0.0.3/civipy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-14 19:55:02.000000 civipy-0.0.3/civipy/financial.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-14 19:55:02.000000 civipy-0.0.3/civipy/grant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-14 19:55:02.000000 civipy-0.0.3/civipy/mailing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-05-14 19:55:02.000000 civipy-0.0.3/civipy/membership.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-14 19:55:02.000000 civipy-0.0.3/civipy/note.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-14 19:55:02.000000 civipy-0.0.3/civipy/option_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-14 19:55:02.000000 civipy-0.0.3/civipy/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-14 19:55:02.000000 civipy-0.0.3/civipy/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:55:07.137111 civipy-0.0.3/civipy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-05-14 19:55:07.000000 civipy-0.0.3/civipy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-14 19:55:07.000000 civipy-0.0.3/civipy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 19:55:07.000000 civipy-0.0.3/civipy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-14 19:55:07.000000 civipy-0.0.3/civipy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 19:55:07.000000 civipy-0.0.3/civipy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-14 19:55:02.000000 civipy-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 19:55:07.141111 civipy-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:55:07.137111 civipy-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-14 19:55:02.000000 civipy-0.0.3/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-05-14 19:55:02.000000 civipy-0.0.3/tests/test_contact.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-14 19:55:02.000000 civipy-0.0.3/tests/test_contribution.py
```

### Comparing `civipy-0.0.2/LICENSE` & `civipy-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `civipy-0.0.2/civipy/address.py` & `civipy-0.0.3/civipy/address.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,67 +1,59 @@
-from civipy.base import CiviCRMBase
-from civipy.base import get_unique
-from civipy.config import logger
+from civipy.base.base import CiviCRMBase
+from civipy.base.config import logger
 
 
-class CiviStateProvince(CiviCRMBase):
-    pass
+class CiviCountry(CiviCRMBase):
+    civicrm_entity_table = "country"
 
+    @classmethod
+    def find_by_country_code(cls, country_code: str, select: list[str] | None = None):
+        return cls.find(select=select, iso_code=country_code)
 
-class CiviCountry(CiviCRMBase):
+
+class CiviStateProvince(CiviCRMBase):
     pass
 
 
 class CiviLocationType(CiviCRMBase):
     pass
 
 
 class CiviAddress(CiviCRMBase):
     country_iso_code_cache = {}
     state_province_abbreviation_cache = {}
 
     @classmethod
-    def _create(cls, entity=None, **kwargs):
-        """
-        Calls the CiviCRM API create action and returns parsed JSON on success.
+    def create(cls, **kwargs):
+        """Calls the CiviCRM API create action and returns parsed JSON on success.
 
         Accepts field country_iso_code and will convert this to country_id
-        Accepts field state_province_abbreviation and will convert this to state_province_id
-        """
+        Accepts field state_province_abbreviation and will convert this to state_province_id"""
         if "country_iso_code" in kwargs:
             country_iso_code = kwargs["country_iso_code"]
+            del kwargs["country_iso_code"]
             if country_iso_code in cls.country_iso_code_cache:
                 country = cls.country_iso_code_cache[country_iso_code]
             else:
-                country = CiviCountry.find(**{"iso_code": country_iso_code})
+                country = CiviCountry.find_by_country_code(country_iso_code)
                 cls.country_iso_code_cache[country_iso_code] = country
 
-            del kwargs["country_iso_code"]
             kwargs["country_id"] = country.civi_id
 
             if country.civi_id not in cls.state_province_abbreviation_cache:
                 cls.state_province_abbreviation_cache[country.civi_id] = {}
 
-            if country.is_province_abbreviated and "state_province_abbreviation" in kwargs:
-                state_province_abbreviation = kwargs["state_province_abbreviation"]
-                if state_province_abbreviation in cls.state_province_abbreviation_cache[country.civi_id]:
-                    logger.debug("using cache for %s" % state_province_abbreviation)
-                    state_province_id = cls.state_province_abbreviation_cache[country.civi_id][
-                        state_province_abbreviation
-                    ]
-                else:
-                    response = CiviStateProvince._get(
-                        **{"country_id": country.civi_id, "abbreviation": state_province_abbreviation}
-                    )
-                    state_province_id = get_unique(response)["id"]
-                    cls.state_province_abbreviation_cache[country.civi_id][
-                        state_province_abbreviation
-                    ] = state_province_id
-
+            if "state_province_abbreviation" in kwargs:
+                abbreviation = kwargs["state_province_abbreviation"]
                 del kwargs["state_province_abbreviation"]
-                kwargs["state_province_id"] = state_province_id
-            elif not country.is_province_abbreviated and "state_province_abbreviation" in kwargs:
-                kwargs["supplemental_address_3"] = kwargs["state_province_abbreviation_cache"]
-
-            assert ("state_province_id" in kwargs) or ("supplemental_address_3" in kwargs)
-            assert "country_id" in kwargs
-        return CiviCRMBase._post_method()("create", "Address", kwargs)
+                if country.is_province_abbreviated:
+                    if abbreviation in cls.state_province_abbreviation_cache[country.civi_id]:
+                        logger.debug("Using cache for %s" % abbreviation)
+                        state_province_id = cls.state_province_abbreviation_cache[country.civi_id][abbreviation]
+                    else:
+                        state_province = CiviStateProvince.find(country_id=country.civi_id, abbreviation=abbreviation)
+                        state_province_id = state_province["id"]
+                        cls.state_province_abbreviation_cache[country.civi_id][abbreviation] = state_province_id
+                    kwargs["state_province_id"] = state_province_id
+                else:
+                    kwargs["supplemental_address_3"] = abbreviation
+        return super().create(**kwargs)
```

### Comparing `civipy-0.0.2/civipy/contribution.py` & `civipy-0.0.3/civipy/contribution.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,84 +1,67 @@
-from civipy.base import CiviCRMBase
-from civipy.base import get_unique
+from civipy.base.base import CiviCRMBase
+from civipy.base.base import get_unique
 from civipy.contact import CiviContact
-from civipy.exceptions import NonUniqueSelectorException
 
 
 class CiviContribution(CiviCRMBase):
     civicrm_entity_table = "contribution"
 
     def complete_transaction(self, **kwargs):
-        """
-        Calls the CiviCRM API completetransaction action and returns parsed JSON on success.
-        """
+        """Calls the CiviCRM API completetransaction action and returns parsed JSON on success."""
         kwargs["id"] = self.civi_id
-        response = self._post_method()("completetransaction", None, kwargs)
+        response = self.action("completetransaction", **kwargs)
         if not isinstance(response.get("values"), int):
             value = get_unique(response)
             return self.__class__(value)
         else:
             return response
 
     @classmethod
-    def find_by_transaction_id(cls, trxn_id: str):
-        """
-        Find a contribution by payment transaction ID
-        """
-        found = cls._get(trxn_id=trxn_id)
-        if not found or found.get("count") == 0:
-            return
-        if found and found.get("count") == 1:
-            return cls(get_unique(found))
-        raise NonUniqueSelectorException(f"Multiple Civi contribution records found for Payment ID {trxn_id}!")
+    def find_by_transaction_id(cls, trxn_id: str, select: list[str] | None = None):
+        """Find a contribution by payment transaction ID"""
+        return cls.find(select=select, trxn_id=trxn_id)
 
     @classmethod
-    def find_by_invoice_id(cls, invoice_id: str):
-        found = cls._get(invoice_id=invoice_id)
-        if not found or found.get("count") == 0:
-            return
-        if found and found.get("count") == 1:
-            return cls(get_unique(found))
-        raise NonUniqueSelectorException(f"Multiple Civi contribution records found for Invoice ID {invoice_id}!")
+    def find_by_invoice_id(cls, invoice_id: str, select: list[str] | None = None):
+        return cls.find(select=select, invoice_id=invoice_id)
 
     @classmethod
-    def find_by_donor(cls, display_name: str, total_amount=None, receive_date=None):
-        """
-        Find a contribution by donor's display name, and optionally
-        by amount and/or date received (yyyy-mm-dd).
-        """
-        result = CiviContact._get(display_name=display_name)
-        if result["count"] == 0:
-            return
-        elif result["count"] > 1:
-            raise NonUniqueSelectorException(f"Multiple donors named {display_name}")
-        contact_obj = get_unique(result)
-        return cls.find_by_donor_id(contact_obj["contact_id"], total_amount, receive_date)
+    def find_by_donor(
+        cls,
+        display_name: str,
+        total_amount: float | None = None,
+        receive_date: str | None = None,
+        select: list[str] | None = None,
+    ):
+        """Find a contribution by donor's display name, and optionally
+        by amount and/or date received (yyyy-mm-dd)."""
+        contact = CiviContact.find(select=["contact_id"], display_name=display_name)
+        return cls.find_by_donor_id(contact["contact_id"], total_amount, receive_date, select)
 
     @classmethod
-    def find_by_donor_id(cls, contact_id: int, total_amount=None, receive_date=None):
-        """
-        Find a contribution by donor's contact ID, and optionally
-        by amount and/or date received (yyyy-mm-dd).
-        """
+    def find_by_donor_id(
+        cls,
+        contact_id: int,
+        total_amount: float | None = None,
+        receive_date: str | None = None,
+        select: list[str] | None = None,
+    ):
+        """Find a contribution by donor's contact ID, and optionally
+        by amount and/or date received (yyyy-mm-dd)."""
         query = {"contact_id": contact_id}
         if total_amount is not None:
             query["total_amount"] = total_amount
         if receive_date is not None:
             query["receive_date"] = {"BETWEEN": [receive_date, f"{receive_date} 23:59:59"]}
-        return cls.find(**query)
+        return cls.find(select=select, **query)
 
 
 class CiviContributionRecur(CiviCRMBase):
     civicrm_entity_table = "contributionrecur"
 
     @classmethod
-    def find_by_transaction_id(cls, trxn_id: str):
+    def find_by_transaction_id(cls, trxn_id: str, select: list[str] | None = None):
         """
         Find a recurring contribution by subscription transaction ID
         """
-        found = cls._get(trxn_id=trxn_id)
-        if not found or found.get("count") == 0:
-            return
-        if found and found.get("count") == 1:
-            return cls(get_unique(found))
-        raise NonUniqueSelectorException(f"Multiple ContributionRecur records found for Subscription ID {trxn_id}!")
+        return cls.find(select=select, trxn_id=trxn_id)
```

### Comparing `civipy-0.0.2/civipy/exceptions.py` & `civipy-0.0.3/civipy/exceptions.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,22 +8,27 @@
     pass
 
 
 class CiviProgrammingError(CivipyException):
     pass
 
 
-class NonUniqueSelectorException(CivipyException):
+class NoResultError(CivipyException):
+    pass
+
+
+class NonUniqueResultError(CivipyException):
     pass
 
 
 class CiviHTTPError(CivipyException):
     def __init__(self, r: "BaseHTTPResponse"):
         self.r = r
         self.status_code = r.status
         self.message = r.data.decode("utf-8", errors="replace")
+        super().__init__(f"{self.status_code}: {self.message}")
 
 
 class CiviAPIError(CivipyException):
     def __init__(self, data):
         self.code = data.get("error_code")
         self.message = data.get("error_message")
```

### Comparing `civipy-0.0.2/civipy/option_group.py` & `civipy-0.0.3/civipy/option_group.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,22 @@
-from civipy.base import CiviCRMBase
-from civipy.base import get_unique
+from civipy.base.base import CiviCRMBase
 
 
 class CiviOptionValue(CiviCRMBase):
     pass
 
 
 class CiviOptionGroup(CiviCRMBase):
     @classmethod
-    def find_options_by_group_name(cls, option_group_name):
+    def find_options_by_group_name(cls, option_group_name: str):
         """
         Taking an option_group_name, looks up the group and its members.
         """
-        response = CiviOptionGroup._get(name=option_group_name)
-        og = get_unique(response)
-        values_response = CiviOptionValue._get(option_group_id=og["id"])
-        return values_response["values"]
+        og = CiviOptionGroup.find(name=option_group_name)
+        return CiviOptionValue.find_all(option_group_id=og["id"])
 
     @classmethod
     def option_values_dict_by_group_name(cls, option_group_name):
         """
         Taking an option_group_name, looks up the group and its members.
         """
         option_values_list = cls.find_options_by_group_name(option_group_name)
@@ -30,22 +27,19 @@
 
 class CiviCustomValue(CiviCRMBase):
     pass
 
 
 class CiviCustomField(CiviCRMBase):
     @classmethod
-    def find_field_by_label(cls, field_label):
-        response = CiviCustomField._get(label=field_label)
-        field = get_unique(response)
-        return field
+    def find_field_by_label(cls, field_label: str):
+        return CiviCustomField.find(label=field_label)
 
     @classmethod
-    def find_options_by_field_label(cls, label):
+    def find_options_by_field_label(cls, label: str):
         custom_field = cls.find(label=label)
-        values_response = CiviOptionValue._get(option_group_id=custom_field.civi_option_group_id)
-        return values_response["values"]
+        return CiviOptionValue.find_all(option_group_id=custom_field.civi_option_group_id)
 
     @classmethod
-    def options_label_map(cls, label):
+    def options_label_map(cls, label: str):
         option_values = cls.find_options_by_field_label(label)
         return dict((ov["label"], ov["value"]) for ov in option_values)
```

### Comparing `civipy-0.0.2/civipy/user.py` & `civipy-0.0.3/civipy/user.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,53 @@
-from civipy.base import CiviCRMBase
+from civipy.base.base import CiviCRMBase
+from civipy.exceptions import NoResultError, NonUniqueResultError
 
 
-class CiviUFField(CiviCRMBase):
-    ...
+class CiviUFField(CiviCRMBase): ...
 
 
-class CiviUFGroup(CiviCRMBase):
-    ...
+class CiviUFGroup(CiviCRMBase): ...
 
 
-class CiviUFJoin(CiviCRMBase):
-    ...
+class CiviUFJoin(CiviCRMBase): ...
 
 
 class CiviUFMatch(CiviCRMBase):
-    """This is the table that matches WordPress users to CiviCRM Contacts.
+    """This is the table that matches host system users to CiviCRM Contacts.
 
     create requires uf_id, uf_name, and contact_id
 
     Attributes:
         id: str e.g. "24392"
         domain_id: str e.g. "1"
         uf_id: str e.g. "46914"
         uf_name: str e.g. "user@example.com"
         contact_id: str e.g. "367872"
     """
 
     @classmethod
-    def find_wp(cls, contact_ids):
+    def find_system_users(cls, contact_ids: list[int]) -> list["CiviUFMatch"]:
         result = []
         for contact_id in set(contact_ids):
-            found = cls.find(search_key_name="contact_id", contact_id=contact_id)
+            found = cls.find(contact_id=contact_id)
             if not found:
                 continue
             result.append(found)
         if not result:
-            raise ValueError("No result found!")
+            raise NoResultError("No result found!")
         if len(result) != 1:
             views = [f"{r.civi}\n" for r in result]
-            raise ValueError(f"Too many results:\n {''.join(views)}")
+            raise NonUniqueResultError(f"Too many results:\n {''.join(views)}")
         result = result[0]
         for attr in ("id", "domain_id", "uf_id", "contact_id"):
             result.civi[attr] = int(result.civi[attr])
         return result
 
-    def update_wp_user(self, wp_user_id):
-        payload = self.civi
-        payload["uf_id"] = wp_user_id
-        self.update(**payload)
+    def update_system_user(self, user_id: int):
+        return self.update(**self.civi, uf_id=user_id)
+
+    @classmethod
+    def connect(cls, host_user: int, contact_id: int, domain_id: int = 1):
+        return cls.objects.create(domain_id=domain_id, uf_id=host_user, contact_id=contact_id)
 
 
-class CiviUser(CiviCRMBase):
-    ...
+class CiviUser(CiviCRMBase): ...
```

### Comparing `civipy-0.0.2/civipy.egg-info/SOURCES.txt` & `civipy-0.0.3/civipy.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 LICENSE
 MANIFEST.in
 README.md
 VERSION
 pyproject.toml
 civipy/__init__.py
+civipy/activity.py
 civipy/address.py
-civipy/base.py
-civipy/config.py
 civipy/contact.py
 civipy/contribution.py
-civipy/country.py
-civipy/custom_field.py
 civipy/event.py
 civipy/exceptions.py
+civipy/financial.py
+civipy/grant.py
+civipy/mailing.py
 civipy/membership.py
 civipy/note.py
 civipy/option_group.py
 civipy/order.py
 civipy/user.py
 civipy.egg-info/PKG-INFO
 civipy.egg-info/SOURCES.txt
```

### Comparing `civipy-0.0.2/pyproject.toml` & `civipy-0.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,53 +2,55 @@
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "civipy"
 description = "CiviCRM v3/v4 REST API Python wrapper"
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 license = {text = "GPLv3"}
 authors = [ {name = "Joe Carey", email = "joecarey001@gmail.com"}, {name = "Ana Nelson", email = "ana@ananelson.com"} ]
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
 urls = {Homepage = "https://github.com/indepndnt/civipy"}
 dynamic = ["version"]
 dependencies = [
     "urllib3",
 ]
+optional-dependencies.pyproject = [
+    "tomli>=1.1.0; python_version < '3.11'",
+]
 optional-dependencies.dev = [
     "black",
     "coverage[toml]",
     "pytest",
     "pytest-cov",
     "ruff",
 ]
 
 [tool.setuptools]
 packages = ["civipy"]
 dynamic.version = {file = "VERSION"}
 
 [tool.cibuildwheel]
-build = ["cp38-*", "cp39-*", "cp310-*", "cp311-*", "cp312-*", "cp313-*"]
+build = ["cp39-*", "cp310-*", "cp311-*", "cp312-*", "cp313-*"]
 build-frontend = "build"
 test-command = "pytest {project}/tests --color yes"
 test-requires = "pytest"
 
 [tool.black]
 line-length = 120
-target-version = ["py38", "py39", "py310", "py311", "py312"]
+target-version = ["py39", "py310", "py311", "py312"]
 
 [tool.coverage]
 run.source = ["civipy"]
 report.skip_empty = true
 
 [tool.pytest.ini_options]
 addopts = "--cov --cov-report=xml -l -rN --color=yes --code-highlight=yes"
@@ -56,12 +58,14 @@
 python_files = "*.py"
 log_auto_indent = true
 log_cli = true
 norecursedirs = ["__pycache__", "*.egg-info", ".*", "dist"]
 
 [tool.ruff]
 src = ["src"]
-select = ["E", "F", "PL"]
 line-length = 120
 target-version = "py310"
 extend-exclude = ["react"]
+
+[tool.ruff.lint]
+select = ["E", "F", "PL"]
 ignore = ["PLR2004"]
```

