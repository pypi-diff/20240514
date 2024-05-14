# Comparing `tmp/CorePlatPy-0.0.2-py3-none-any.whl.zip` & `tmp/CorePlatPy-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,29 +1,29 @@
-Zip file size: 42679 bytes, number of entries: 27
+Zip file size: 43559 bytes, number of entries: 27
 -rw-rw-rw-  2.0 fat       26 b- defN 24-Apr-23 11:16 coreplatpy/__init__.py
--rw-rw-rw-  2.0 fat     6003 b- defN 24-May-08 14:25 coreplatpy/client.py
+-rw-rw-rw-  2.0 fat     8845 b- defN 24-May-13 11:14 coreplatpy/client.py
 -rw-rw-rw-  2.0 fat       49 b- defN 24-Apr-24 19:21 coreplatpy/account/__init__.py
--rw-rw-rw-  2.0 fat     1912 b- defN 24-May-10 09:41 coreplatpy/account/group_api.py
--rw-rw-rw-  2.0 fat       66 b- defN 24-Apr-23 13:03 coreplatpy/account/role_api.py
+-rw-rw-rw-  2.0 fat     2726 b- defN 24-May-13 11:14 coreplatpy/account/group_api.py
+-rw-rw-rw-  2.0 fat      997 b- defN 24-May-13 11:14 coreplatpy/account/role_api.py
 -rw-rw-rw-  2.0 fat     1468 b- defN 24-May-09 08:48 coreplatpy/account/user_api.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-May-10 10:53 coreplatpy/copernicus/__init__.py
 -rw-rw-rw-  2.0 fat      218 b- defN 24-May-10 10:53 coreplatpy/copernicus/copernicus.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-23 07:51 coreplatpy/globals/__init__.py
 -rw-rw-rw-  2.0 fat       61 b- defN 24-Apr-23 07:54 coreplatpy/globals/globals.py
 -rw-rw-rw-  2.0 fat      114 b- defN 24-May-10 10:53 coreplatpy/models/__init__.py
 -rw-rw-rw-  2.0 fat    42091 b- defN 24-Apr-25 12:25 coreplatpy/models/account_models.py
--rw-rw-rw-  2.0 fat     6918 b- defN 24-May-10 09:38 coreplatpy/models/api_models.py
+-rw-rw-rw-  2.0 fat     6920 b- defN 24-May-13 07:51 coreplatpy/models/api_models.py
 -rw-rw-rw-  2.0 fat      842 b- defN 24-May-10 10:53 coreplatpy/models/cop_models.py
 -rw-rw-rw-  2.0 fat      367 b- defN 24-Apr-24 10:44 coreplatpy/models/generic_models.py
 -rw-rw-rw-  2.0 fat       68 b- defN 24-May-08 10:43 coreplatpy/storage/__init__.py
 -rw-rw-rw-  2.0 fat     1171 b- defN 24-May-09 09:11 coreplatpy/storage/buckets.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-25 12:28 coreplatpy/storage/copernicus.py
--rw-rw-rw-  2.0 fat     2131 b- defN 24-May-09 11:08 coreplatpy/storage/files.py
+-rw-rw-rw-  2.0 fat     2342 b- defN 24-May-13 09:58 coreplatpy/storage/files.py
 -rw-rw-rw-  2.0 fat     1934 b- defN 24-May-09 12:00 coreplatpy/storage/folders.py
 -rw-rw-rw-  2.0 fat       22 b- defN 24-Apr-23 14:20 coreplatpy/utils/__init__.py
--rw-rw-rw-  2.0 fat     7388 b- defN 24-May-09 11:07 coreplatpy/utils/helpers.py
--rw-rw-rw-  2.0 fat     1089 b- defN 24-May-10 12:08 CorePlatPy-0.0.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      898 b- defN 24-May-10 12:08 CorePlatPy-0.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-10 12:08 CorePlatPy-0.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 24-May-10 12:08 CorePlatPy-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     2283 b- defN 24-May-10 12:08 CorePlatPy-0.0.2.dist-info/RECORD
-27 files, 77222 bytes uncompressed, 38951 bytes compressed:  49.6%
+-rw-rw-rw-  2.0 fat     7642 b- defN 24-May-14 11:30 coreplatpy/utils/helpers.py
+-rw-rw-rw-  2.0 fat     1089 b- defN 24-May-14 11:34 CorePlatPy-0.0.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      898 b- defN 24-May-14 11:34 CorePlatPy-0.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-14 11:34 CorePlatPy-0.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 24-May-14 11:34 CorePlatPy-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     2284 b- defN 24-May-14 11:34 CorePlatPy-0.0.3.dist-info/RECORD
+27 files, 82277 bytes uncompressed, 39831 bytes compressed:  51.6%
```

## zipnote {}

```diff
@@ -60,23 +60,23 @@
 
 Filename: coreplatpy/utils/__init__.py
 Comment: 
 
 Filename: coreplatpy/utils/helpers.py
 Comment: 
 
-Filename: CorePlatPy-0.0.2.dist-info/LICENSE
+Filename: CorePlatPy-0.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: CorePlatPy-0.0.2.dist-info/METADATA
+Filename: CorePlatPy-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: CorePlatPy-0.0.2.dist-info/WHEEL
+Filename: CorePlatPy-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: CorePlatPy-0.0.2.dist-info/top_level.txt
+Filename: CorePlatPy-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: CorePlatPy-0.0.2.dist-info/RECORD
+Filename: CorePlatPy-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## coreplatpy/client.py

```diff
@@ -1,105 +1,92 @@
 from .models import (
     UpdateUser, LoginParams, BearerToken, ErrorReport, UserAttrs, UserData,
-    Organization, Bucket, Folder
+    Organization, RoleUpdate, Role, Bucket, Folder
 )
 from .account import (
     authenticate_sync, update_info, get_user_data,
-    post_organization, get_user_organizations
+    post_organization, get_user_organizations,
+    post_new_group, delete_group,
+    update_role, get_role
 )
 
 from .storage import (
     create_bucket, get_folder_by_id
 )
 
 import getpass
 from jwt import decode
 from .utils import preety_print_error
 from typing import Union, List
 
+
 class Client:
     """
     A Client for the Core Platform.
 
     Parameters
     ----------
     api_url : The url of Core Platform API
     account_url: The url of Account API
     """
 
-    def __init__(self, api_url=None, account_url=None, create_logs=False) -> None:
-        if api_url:
-            self.api_url = api_url
-        else:
-            self.api_url = 'https://api-buildspace.euinno.eu/'
-
-        if account_url:
-            self.account_url = account_url
-        else:
-            self.account_url = 'https://account-buildspace.euinno.eu/'
-
+    def __init__(self, api_url=None, account_url=None) -> None:
+        self.api_url = api_url or 'https://api-buildspace.euinno.eu/'
+        self.account_url = account_url or 'https://account-buildspace.euinno.eu/'
         self.api_key = None
         self.user_id = None
 
     def __get_instance_variables__(self):
         return {k: v for k, v in self.__dict__.items() if not k.startswith('__') and not callable(v)}
 
     def authenticate(self):
         """
         Secure authentication for Core Platform.
         """
         try:
             username = input("Username: ")
             password = getpass.getpass("Password: ")
-            params = LoginParams.model_validate({
-                'username': username,
-                'password': password
-            })
-
+            params = LoginParams.model_validate({'username': username, 'password': password})
             access = authenticate_sync(self.account_url, params)
-            if access.__repr_name__() == 'ErrorReport':
+            if isinstance(access, ErrorReport):
                 preety_print_error(access)
             else:
                 self.api_key = access.access_token
-            # print("API key is set")
-            # self.user_id = jwtok.decode_jwt(self.api_key).get('sub')
         except Exception as e:
             print("Error: " + str(e))
-
-
+            raise
 
     def login(self, username: str, password: str) -> None:
         """
         Login to Core Platform.
 
         Parameters
         ----------
         username : username
         password : password
         """
         try:
-            params = LoginParams.model_validate({
-                'username': username,
-                'password': password
-            })
-
+            params = LoginParams.model_validate({'username': username, 'password': password})
             access = authenticate_sync(self.account_url, params)
             if isinstance(access, ErrorReport):
                 preety_print_error(access)
             else:
                 self.api_key = access.access_token
-            # self.user_id = jwtok.decode_jwt(self.api_key).get('sub')
         except Exception as e:
             print("Unexpected Error: " + str(e))
+            raise
 
     def get_my_user(self) -> Union[UserData, None]:
         """
-        Get the user data, once logged in
+        Get the user data, once logged in.
 
-        :return: UserData
+        Returns
+        -------
+        UserData : The user's data if successful.
+        None : If an error occurs.
         """
         resp = get_user_data(self.account_url, self.api_key)
         if isinstance(resp, ErrorReport):
             preety_print_error(resp)
             return None
         return resp
 
@@ -127,27 +114,26 @@
             update_user = UpdateUser(password=new_password)
         except Exception as e:
             print("Unexpected Error: ", str(e))
         else:
             resp = update_info(self.account_url, update_user, self.api_key)
             if isinstance(resp, ErrorReport):
                 preety_print_error(resp)
+        
+
+    def create_organization(self, organization: str, path: str = '/', sub_orgs: List[str] = [], attributes: dict = {}, org_id: str = None) -> Union[Organization, None]:
+        """
+        Create Organization.
 
-    def create_organization(self, organization: str, path: str = '/',
-                            sub_orgs: List[str] = [], attributes: dict = {},
-                            org_id: str = None) -> Union[Organization, None]:
-        """
-        Create Organization
-
-        :param organization: Name of the new organization
-        :param path: Optional (specify path when creating a sub organization)
-        :param sub_orgs: Optional list of sub groups in organization
-        :param attributes: Optional dictionary of attributes
-        :param org_id: Optional group id (only in case that ID of organization should be defined)
-        :return: Organization object
+        :param organization: Name of the new organization.
+        :param path: Optional path for sub-organization creation.
+        :param sub_orgs: Optional list of sub-groups in the organization.
+        :param attributes: Optional dictionary of attributes.
+        :param org_id: Optional group ID if predefined.
+        :return: Organization object.
         """
         new_org = Organization(name=organization, id=org_id, sub_orgs=sub_orgs,
                                     attributes=attributes, path=path)
 
         resp = post_organization(self.account_url, new_org, self.api_key)
         if isinstance(resp, ErrorReport):
             preety_print_error(resp)
@@ -157,17 +143,118 @@
         resp = create_bucket(self.api_url, bucket, self.api_key)
         if isinstance(resp, ErrorReport):
             preety_print_error(resp)
             return None
 
         return resp
 
-    def get_my_organization(self) -> Union[List[Organization], None]:
+    def get_my_organizations(self) -> Union[List[Organization], None]:
         return (get_user_organizations(self.account_url, self.api_key))
 
+    def update_user_groups(self, group_id: str, new_org_data: dict) -> Union[Organization, None]:
+        """
+        Join the user in a new group.
+
+        Parameters
+        ----------
+        group_id : str
+            ID of the referring group.
+        new_org_data : dict
+            New data for updating the organization.
+
+        Returns
+        -------
+        Organization : The updated organization if successful.
+        None : If an error occurs.
+        """
+        try:
+            org = Organization.model_validate(new_org_data)
+            resp = post_new_group(self.account_url, group_id, org, self.api_key)
+            if isinstance(resp, ErrorReport):
+                preety_print_error(resp)
+                return None
+            return resp
+        except Exception as e:
+            print("Unexpected Error: " + str(e))
+            raise
+
+    def groups_cleaning(self, group_id: str) -> bool:
+        """
+        Delete an organization by its group ID.
+
+        Parameters
+        ----------
+        group_id : str
+            ID of the organization to delete.
+
+        Returns
+        -------
+        bool : True if successful, False if an error occurs.
+        """
+        try:
+            resp = delete_group(self.account_url, group_id, self.api_key)
+            if isinstance(resp, ErrorReport):
+                preety_print_error(resp)
+                return False
+            return True
+        except Exception as e:
+            print("Unexpected Error: " + str(e))
+            raise
+
+    def update_group_role(self, group_id: str, new_role_data: dict) -> bool:
+        """
+        Update a role for a specific group by its ID.
+
+        Parameters
+        ----------
+        group_id : str
+            ID of the group to update the role for.
+        new_role_data : dict
+            Dictionary containing the updated role data.
+
+        Returns
+        -------
+        bool : True if successful, False if an error occurs.
+        """
+        try:
+            role_update = RoleUpdate.model_validate(new_role_data)
+            resp = update_role(self.account_url, group_id, role_update, self.api_key)
+            if isinstance(resp, ErrorReport):
+                preety_print_error(resp)
+                return False
+            return True
+        except Exception as e:
+            print("Unexpected Error: " + str(e))
+            raise
+
+    def get_group_role(self, group_id: str) -> Union[Role, None]:
+        """
+        Retrieve a role for a specific group by its ID.
+
+        Parameters
+        ----------
+        group_id : str
+            ID of the group to retrieve the role for.
+
+        Returns
+        -------
+        Role : The role information if successful.
+        None : If an error occurs.
+        """
+        try:
+            resp = get_role(self.account_url, group_id, self.api_key)
+            if isinstance(resp, ErrorReport):
+                preety_print_error(resp)
+                return None
+            return resp
+        except Exception as e:
+            print("Unexpected Error: " + str(e))
+            raise
+
+
     def get_folder(self, folder_id:str) -> Union[Folder, None]:
         folder = get_folder_by_id(self.api_url, folder_id, self.api_key)
         if isinstance(folder, ErrorReport):
             preety_print_error(folder)
             return None
 
         folder.client_params = self.__get_instance_variables__()
```

## coreplatpy/account/group_api.py

```diff
@@ -21,14 +21,33 @@
     head = {'Content-Type': 'application/json', 'Authorization': f'Bearer {token}'}
 
     response = safe_json_request('GET', uri, data, head)
     if isinstance(response, ErrorReport):
         return response
     return [Organization.model_validate(item) for item in response]
 
+def post_new_group(baseurl: str, group_id: str, organization: Organization, token: str) -> Union[Organization, ErrorReport]:
+    uri = baseurl + endpoint + f"{group_id}"
+    data = organization.model_dump(exclude_unset=True)
+    head = {'Content-Type': 'application/json', 'Authorization': f'Bearer {token}'}
+
+    response = safe_request('POST', uri, data, head) 
+    if isinstance(response, ErrorReport):
+        return response
+    return Organization.model_validate(response)
+
+def delete_group(baseurl: str, group_id: str, token: str) -> Union[None, ErrorReport]:
+    uri = baseurl + endpoint + f"{group_id}"
+    head = {'Authorization': f'Bearer {token}'}
+
+    response = safe_request('DELETE', uri, head)
+    if isinstance(response, ErrorReport):
+        return response
+    return None  
+
 
 def get_organization_info(baseurl: str, group_id: str, token:str) -> Union[Organization, ErrorReport]:
     uri = baseurl + endpoint + group_id
     data = None
     head = {'Content-Type': 'application/json', 'Authorization': f'Bearer {token}'}
 
     response = safe_json_request('GET', uri, data, head)
```

## coreplatpy/account/role_api.py

```diff
@@ -1,6 +1,26 @@
 import requests
-from ..models import *
+from ..models import RoleUpdate, ErrorReport, Role
+from ..utils import safe_request
+from typing import Union
 
-endpoint = "role"
+# endpoint = "role"
+endpoint = "role/group-admin/"
 
+def update_role(baseurl: str, group_id: str, role_update: RoleUpdate, token: str) -> Union[None, ErrorReport]:
+    uri = baseurl + endpoint + f"{group_id}"
+    data = role_update.model_dump(exclude_unset=True, exclude_none=True)
+    head = {'Content-Type': 'application/json', 'Authorization': f'Bearer {token}'}
+    
+    response = safe_request('PUT', uri, data, head)
+    if isinstance(response, ErrorReport):
+        return response
+    return None
 
+def get_role(baseurl: str, group_id: str, token: str) -> Union[Role, ErrorReport]:
+    uri = baseurl + endpoint + f"{group_id}"
+    head = {'Authorization': f'Bearer {token}'}
+    
+    response = safe_request('GET', uri, None, head)
+    if isinstance(response, ErrorReport):
+        return response
+    return Role.model_validate(response)
```

## coreplatpy/models/api_models.py

```diff
@@ -108,14 +108,15 @@
         threads = []
         for i in range(1, resp.total + 1):
             thread = Thread(target=send_part, args=(self.client_params['api_url'], next(chunks), i, resp.id, self.client_params['api_key']))
             thread.start()
             threads.append(thread)
 
         for thread in tqdm(threads, desc=f'Uploading {resp.meta.title}'):
+
             thread.join()
 
     def list_items(self):
         from ..storage.folders import list_folder_items
         return list_folder_items(self.client_params['api_url'], self.id, self.client_params['api_key'])
 
     def save_file(self, file_id:str, path: str):
```

## coreplatpy/storage/files.py

```diff
@@ -14,19 +14,19 @@
     response = safe_data_request('POST', uri, data, head)
     if isinstance(response, ErrorReport):
         return response
     return File.model_validate(response)
 
 def send_part(baseurl: str, part_raw: bytes, index: int, file_id, token: str) -> Union[File, ErrorReport]:
     uri = baseurl + f'{endpoint}/{file_id}?part={index}'
-    headers = {'Content-Type': 'application/octet-stream', 'Authorization': f'Bearer {token}'}
-
+    headers = {'Content-Type': 'application/octet-stream', 'Authorization': f'Bearer {token}', 'Content-Length': f'{len(part_raw)}'}
+    print(len(part_raw))
     response = safe_data_request('POST', uri, headers=headers, data=part_raw)
     if isinstance(response, ErrorReport):
-        return response
+        raise ValueError(f"HTTP Status: {response.status} \nHTTP Reason: {response.reason} \nAPI Message: {response.message} \nAPI Status Code: {response.internal_status}")
     return File.model_validate(response)
 
 def get_part(baseurl: str, file_id: str, results: list, index: int, token: str):
     uri = baseurl + f'{endpoint}/{file_id}?part={index}'
     headers = {'Content-Type': 'application/json', 'Authorization': f'Bearer {token}'}
 
     response = safe_data_request('GET', uri, headers=headers, data=None)
```

## coreplatpy/utils/helpers.py

```diff
@@ -33,20 +33,23 @@
         return ErrorReport()
     else:
         if response.status_code >= 300:
             return respond_with_error(response)
         return response.json()
 
 def safe_json_request(request: str, uri: str, data: Union[dict, None], headers: dict) -> Union[dict, ErrorReport, None]:
+    requests_max_size = 10 * 1024 * 1024  # 10 MB
+    session = requests.Session()
+    session.max_request_size = requests_max_size
     if request == 'POST':
         try:
             if data:
-                response = requests.post(uri, json=data, headers=headers)
+                response = session.post(uri, json=data, headers=headers)
             else:
-                response = requests.post(uri, headers=headers)
+                response = session.post(uri, headers=headers)
         except Exception as e:
             print("Error at request: " + str(e))
             return ErrorReport()
         else:
             if response.status_code >= 300:
                 return respond_with_error(response)
             if response.content:
@@ -55,17 +58,17 @@
                 except:
                     return response.content
             else:
                 return None
     elif request == 'GET':
         try:
             if data:
-                response = requests.get(uri, json=data, headers=headers)
+                response = session.get(uri, json=data, headers=headers)
             else:
-                response = requests.get(uri, headers=headers)
+                response = session.get(uri, headers=headers)
         except Exception as e:
             print("Error at request: " + str(e))
             return ErrorReport()
         else:
             if response.status_code >= 300:
                 return respond_with_error(response)
             if response.content:
@@ -74,17 +77,17 @@
                 except:
                     return response.content
             else:
                 return None
     elif request == 'PUT':
         try:
             if data:
-                response = requests.put(uri, json=data, headers=headers)
+                response = session.put(uri, json=data, headers=headers)
             else:
-                response = requests.put(uri, headers=headers)
+                response = session.put(uri, headers=headers)
         except Exception as e:
             print("Error at request: " + str(e))
             return ErrorReport()
         else:
             if response.status_code >= 300:
                 return respond_with_error(response)
             if response.content:
@@ -93,17 +96,17 @@
                 except:
                     return response.content
             else:
                 return None
     elif request == 'DELETE':
         try:
             if data:
-                response = requests.delete(uri, json=data, headers=headers)
+                response = session.delete(uri, json=data, headers=headers)
             else:
-                response = requests.delete(uri, headers=headers)
+                response = session.delete(uri, headers=headers)
         except Exception as e:
             print("Error at request: " + str(e))
             return ErrorReport()
         else:
             if response.status_code >= 300:
                 return respond_with_error(response)
             if response.content:
@@ -114,20 +117,23 @@
             else:
                 return None
     else:
         print("Not a valid method: " + str(e))
         return ErrorReport()
 
 def safe_data_request(request: str, uri: str, data: Union[dict, None], headers: dict) -> Union[dict, ErrorReport, None]:
+    requests_max_size = 10 * 1024 * 1024  # 10 MB
+    session = requests.Session()
+    session.max_request_size = requests_max_size
     if request == 'POST':
         try:
             if data:
-                response = requests.post(uri, data=data, headers=headers)
+                response = session.post(uri, data=data, headers=headers)
             else:
-                response = requests.post(uri, headers=headers)
+                response = session.post(uri, headers=headers)
         except Exception as e:
             print("Error at request: " + str(e))
             return ErrorReport()
         else:
             if response.status_code >= 300:
                 return respond_with_error(response)
             if response.content:
@@ -136,17 +142,17 @@
                 except:
                     return response.content
             else:
                 return None
     elif request == 'GET':
         try:
             if data:
-                response = requests.get(uri, data=data, headers=headers)
+                response = session.get(uri, data=data, headers=headers)
             else:
-                response = requests.get(uri, headers=headers)
+                response = session.get(uri, headers=headers)
         except Exception as e:
             print("Error at request: " + str(e))
             return ErrorReport()
         else:
             if response.status_code >= 300:
                 return respond_with_error(response)
             if response.content:
@@ -155,17 +161,17 @@
                 except:
                     return response.content
             else:
                 return None
     elif request == 'PUT':
         try:
             if data:
-                response = requests.put(uri, data=data, headers=headers)
+                response = session.put(uri, data=data, headers=headers)
             else:
-                response = requests.put(uri, headers=headers)
+                response = session.put(uri, headers=headers)
         except Exception as e:
             print("Error at request: " + str(e))
             return ErrorReport()
         else:
             if response.status_code >= 300:
                 return respond_with_error(response)
             if response.content:
@@ -174,17 +180,17 @@
                 except:
                     return response.content
             else:
                 return None
     elif request == 'DELETE':
         try:
             if data:
-                response = requests.delete(uri, data=data, headers=headers)
+                response = session.delete(uri, data=data, headers=headers)
             else:
-                response = requests.delete(uri, headers=headers)
+                response = session.delete(uri, headers=headers)
         except Exception as e:
             print("Error at request: " + str(e))
             return ErrorReport()
         else:
             if response.status_code >= 300:
                 return respond_with_error(response)
             if response.content:
@@ -194,15 +200,15 @@
                     return response.content
             else:
                 return None
     else:
         print("Not a valid method: " + str(e))
         return ErrorReport()
 
-def split_file_chunks(file_path, num_chunks, chunk_size_mb = 5 * 1024 * 1024 ):
+def split_file_chunks(file_path, num_chunks, chunk_size_mb = 1 * 1024 * 1024 ):
     with open(file_path, 'rb') as f:
         # Read the file in chunks
         for i in range(num_chunks):
             # Seek to the appropriate position in the file
             f.seek(i * chunk_size_mb)
             # Read the chunk
             chunk = f.read(chunk_size_mb)
```

## Comparing `CorePlatPy-0.0.2.dist-info/LICENSE` & `CorePlatPy-0.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `CorePlatPy-0.0.2.dist-info/METADATA` & `CorePlatPy-0.0.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CorePlatPy
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python client for the SLG's Core Platform
 Home-page: https://github.com/PROJECT-BUILDSPACE/CorePlatPy/tree/main
 Author-email: Iason Sotiropoulos <isotiropoulos@singularlogic.eu>, Athos Papanikolaou <apapanikolaou@singularlogic.eu>, Sotiris Aspragkathos <saspragkathos@singularlogic.eu>
 Project-URL: Homepage, https://github.com/PROJECT-BUILDSPACE/CorePlatPy/tree/main
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `CorePlatPy-0.0.2.dist-info/RECORD` & `CorePlatPy-0.0.3.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 coreplatpy/__init__.py,sha256=_5xoxBvqik7-PeMx5hwvFygQoUHpV34lQIJj__e4LaA,26
-coreplatpy/client.py,sha256=EukYJaA6W8Xrm9ZEG-dj8gVyXjNAqX82Dw08bnrFNFI,6003
+coreplatpy/client.py,sha256=JR4rJrnwEdXM2Dm0-LBZPSdPw8x661m6F1qrPNi4dWY,8845
 coreplatpy/account/__init__.py,sha256=Yr0IEm0SXfsYPmcCp7AQlIGuV-aw9En_zi2yf_aQayw,49
-coreplatpy/account/group_api.py,sha256=YGs8Kpq3Hmvy-rjzcYY2xDwpLxDafAtyF-8v6hzCRSs,1912
-coreplatpy/account/role_api.py,sha256=3cdhiHyJtAqFKrGBbHKHGAFQQDYsQEePNRXK8_5Wxfc,66
+coreplatpy/account/group_api.py,sha256=rTsGq6d599rGXvjbEHE1ck3MVPMLGnuulGZnmZc_4WY,2726
+coreplatpy/account/role_api.py,sha256=oks7UjTYv04w7bolEm7UJpyHlUPQmdSaDe-NwhLCWMM,997
 coreplatpy/account/user_api.py,sha256=JTrDhDs9YqzueOBrBbRMK10iiiHe618i7VQJiGht2BQ,1468
 coreplatpy/copernicus/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 coreplatpy/copernicus/copernicus.py,sha256=V2K7bqkj6WqsGrH6YYffWwJMvrnSmszoEQOlbg-y-iI,218
 coreplatpy/globals/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 coreplatpy/globals/globals.py,sha256=JQLiDgQfcA6O9iUH6ve2VN1Z9cM2pq44p34HakO-LhE,61
 coreplatpy/models/__init__.py,sha256=XCNMtt3MRnaCan1jna4gSgyOW00ueH66H77w0R0jBr8,114
 coreplatpy/models/account_models.py,sha256=KOUOHewUmYhwzvPuh3TKEdsR-wH_-hrpnaG8Xqcnzho,42091
-coreplatpy/models/api_models.py,sha256=Zu0vVZOe4iA3WIimqW-U1T8GeGwUDU4cBeRpg952ugw,6918
+coreplatpy/models/api_models.py,sha256=pbMwhxbWRu3OPH17va59aLUMsaNQBt6lLOCMa-H6F_o,6920
 coreplatpy/models/cop_models.py,sha256=7u0yP97oBI7a5GhBn2V65U4sasZUBaY4LecnTW3D10U,842
 coreplatpy/models/generic_models.py,sha256=liUGh-m9dbogcGU1jL9OaSAIW_o4hc-xwpdJhVxJ0aU,367
 coreplatpy/storage/__init__.py,sha256=FV6UuV5SUwpoVu-7740dDW9jy7MycViX3AIjjYH75QU,68
 coreplatpy/storage/buckets.py,sha256=D5mAoBrzSTUUt7bmdEuA_QAqbsKLnCpYZlcUWPGEvWE,1171
 coreplatpy/storage/copernicus.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-coreplatpy/storage/files.py,sha256=mF_gPgvxSV1ocleQ-q3AFKJGMteq-3NlX4GC1mpciX0,2131
+coreplatpy/storage/files.py,sha256=5-xrVYsf8b6QBOoBbz_Vr2yzENKJmKwO6rL4JVdpWPA,2342
 coreplatpy/storage/folders.py,sha256=Sj8tqPE9JaGE5jhI0Buba-cz4LUNMe5Ei3Z5IlT6tJg,1934
 coreplatpy/utils/__init__.py,sha256=D0biZ8jluo1RMV6_2qKFfl5vHnXasg1p9gRI9wNMs44,22
-coreplatpy/utils/helpers.py,sha256=pq8yQPUSxuiXdWLk6I9newtohfE9hqWl5lqudmXtT3I,7388
-CorePlatPy-0.0.2.dist-info/LICENSE,sha256=1itw0j8fnLg9xZkdzBseBFxQzO9-fIdTyZuuAfBt5Zk,1089
-CorePlatPy-0.0.2.dist-info/METADATA,sha256=W3rNWzt8_LwaO3BwN-rV3Jd_cIA_DEWY6XwnIG6Tu3s,898
-CorePlatPy-0.0.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-CorePlatPy-0.0.2.dist-info/top_level.txt,sha256=eqo5OKT6zUqwEOElmRlzlxI5Okxi3ntjeuOOvyTKYv0,11
-CorePlatPy-0.0.2.dist-info/RECORD,,
+coreplatpy/utils/helpers.py,sha256=VPol9dUHUSe4ngGp4I-kBevGuw9xKerMXdqNFyrOOgg,7642
+CorePlatPy-0.0.3.dist-info/LICENSE,sha256=1itw0j8fnLg9xZkdzBseBFxQzO9-fIdTyZuuAfBt5Zk,1089
+CorePlatPy-0.0.3.dist-info/METADATA,sha256=D2nM_q3GbZgzV2IJ3OiRxn2LoFDSZSMrpahJQ_0sL3M,898
+CorePlatPy-0.0.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+CorePlatPy-0.0.3.dist-info/top_level.txt,sha256=eqo5OKT6zUqwEOElmRlzlxI5Okxi3ntjeuOOvyTKYv0,11
+CorePlatPy-0.0.3.dist-info/RECORD,,
```

