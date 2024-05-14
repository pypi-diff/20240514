# Comparing `tmp/partnero-0.2.0.tar.gz` & `tmp/partnero-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "partnero-0.2.0.tar", max compression
+gzip compressed data, was "partnero-0.3.0.tar", max compression
```

## Comparing `partnero-0.2.0.tar` & `partnero-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     3206 2024-05-11 01:49:12.829698 partnero-0.2.0/README.md
--rw-r--r--   0        0        0      434 2024-05-11 01:49:12.829698 partnero-0.2.0/partnero/__init__.py
--rw-r--r--   0        0        0      712 2024-05-11 01:49:12.829698 partnero-0.2.0/partnero/authentication.py
--rw-r--r--   0        0        0     1892 2024-05-11 01:49:12.829698 partnero-0.2.0/partnero/base_api.py
--rw-r--r--   0        0        0     1284 2024-05-11 01:49:12.829698 partnero-0.2.0/partnero/coupon_api.py
--rw-r--r--   0        0        0     2701 2024-05-11 01:49:12.833698 partnero-0.2.0/partnero/customer_api.py
--rw-r--r--   0        0        0     1607 2024-05-11 01:49:12.833698 partnero-0.2.0/partnero/partner_api.py
--rw-r--r--   0        0        0      960 2024-05-11 01:49:12.833698 partnero-0.2.0/partnero/promotion_code_api.py
--rw-r--r--   0        0        0      863 2024-05-11 01:49:12.833698 partnero-0.2.0/partnero/transaction_api.py
--rw-r--r--   0        0        0      320 2024-05-11 01:49:12.833698 partnero-0.2.0/partnero/utils.py
--rw-r--r--   0        0        0     1140 2024-05-11 01:49:12.833698 partnero-0.2.0/partnero/webhook_api.py
--rw-r--r--   0        0        0      919 2024-05-11 01:49:12.833698 partnero-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3684 1970-01-01 00:00:00.000000 partnero-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2760 2024-05-14 21:02:24.474753 partnero-0.3.0/README.md
+-rw-r--r--   0        0        0      666 2024-05-14 21:02:24.474753 partnero-0.3.0/partnero/__init__.py
+-rw-r--r--   0        0        0      698 2024-05-14 21:02:24.478752 partnero-0.3.0/partnero/authentication.py
+-rw-r--r--   0        0        0     1892 2024-05-14 21:02:24.478752 partnero-0.3.0/partnero/base_api.py
+-rw-r--r--   0        0        0     1284 2024-05-14 21:02:24.478752 partnero-0.3.0/partnero/coupon_api.py
+-rw-r--r--   0        0        0     2701 2024-05-14 21:02:24.478752 partnero-0.3.0/partnero/customer_api.py
+-rw-r--r--   0        0        0     1607 2024-05-14 21:02:24.478752 partnero-0.3.0/partnero/partner_api.py
+-rw-r--r--   0        0        0      960 2024-05-14 21:02:24.478752 partnero-0.3.0/partnero/promotion_code_api.py
+-rw-r--r--   0        0        0      863 2024-05-14 21:02:24.478752 partnero-0.3.0/partnero/transaction_api.py
+-rw-r--r--   0        0        0      320 2024-05-14 21:02:24.478752 partnero-0.3.0/partnero/utils.py
+-rw-r--r--   0        0        0     1140 2024-05-14 21:02:24.478752 partnero-0.3.0/partnero/webhook_api.py
+-rw-r--r--   0        0        0     1012 2024-05-14 21:02:24.478752 partnero-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3373 1970-01-01 00:00:00.000000 partnero-0.3.0/PKG-INFO
```

### Comparing `partnero-0.2.0/README.md` & `partnero-0.3.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,97 +1,90 @@
 # Partnero SDK
 
-The Partnero SDK provides a simple and powerful Python interface to the Partnero API, allowing developers to manage customers, partners, transactions, webhooks, coupons, and promotion codes programmatically.
+The Partnero SDK provides a simple and powerful Python interface to the Partnero API, allowing developers to manage customers, partners, transactions, webhooks, coupons, and promotion codes programmatically. It simplifies interactions by providing a centralized client (`PartneroClient`) that handles configuration and request management.
+
 [Partnero API Documentation](https://developers.partnero.com/reference/general.html)
+
 ## Installation
 
 To install the Partnero SDK, run the following command:
 
 ```bash
 pip install partnero
 ```
 
 ## Configuration
 
-Before using the SDK, you need to set up authentication:
+Before using the SDK, configure the `PartneroClient` with your API token:
 
 ```python
-from partnero import Authentication
+from partnero import PartneroClient
 
 # Replace 'your_api_token_here' with your actual API token
-auth = Authentication.configure(api_token='your_api_token_here')
+client = PartneroClient(api_key='your_api_token_here')
 ```
 
 ## Usage
 
-Here's how you can use different components of the SDK:
+With `PartneroClient`, you can easily access different parts of the Partnero API. Here's how you can use it to manage customers, partners, transactions, and webhooks:
 
 ### Customer Management
 
 **List Customers**
 
 ```python
-from partnero import CustomerAPI
-
-customer_api = CustomerAPI()
-customers = customer_api.list_customers(limit=10, page=1)
+customers = client.customers.list_customers(limit=10, page=1)
 print(customers)
 ```
 
 **Create a New Customer**
 
 ```python
-new_customer = customer_api.create_customer(
+new_customer = client.customers.create_customer(
     partner_key='your_partner_key',
     customer_key='unique_customer_key',
     email='customer@example.com',
     name='Customer Name'
 )
 print(new_customer)
 ```
 
 ### Partner Management
 
 **List Partners**
 
 ```python
-from partnero import PartnerAPI
-
-partner_api = PartnerAPI()
-partners = partner_api.list_partners(limit=5, page=1)
+partners = client.partners.list_partners(limit=5, page=1)
 print(partners)
 ```
 
 **Register a New Partner**
 
 ```python
-new_partner = partner_api.create_partner(
+new_partner = client.partners.create_partner(
     email='newpartner@example.com',
     name='New Partner',
     password='securepassword123'
 )
 print(new_partner)
 ```
 
 ### Transaction Management
 
 **List Transactions**
 
 ```python
-from partnero import TransactionAPI
-
-transaction_api = TransactionAPI()
-transactions = transaction_api.list_transactions(limit=5, page=1)
+transactions = client.transactions.list_transactions(limit=5, page=1)
 print(transactions)
 ```
 
 **Create a Transaction**
 
 ```python
-new_transaction = transaction_api.create_transaction(
+new_transaction = client.transactions.create_transaction(
     customer_key='customer_key',
     transaction_key='unique_transaction_key',
     amount=39.99,
     product_id='product_id',
     product_type='type',
     action='purchase'
 )
@@ -99,25 +92,22 @@
 ```
 
 ### Webhook Management
 
 **List Webhooks**
 
 ```python
-from partnero import WebhookAPI
-
-webhook_api = WebhookAPI()
-webhooks = webhook_api.list_webhooks(limit=5, page=1)
+webhooks = client.webhooks.list_webhooks(limit=5, page=1)
 print(webhooks)
 ```
 
 **Create a Webhook**
 
 ```python
-new_webhook = webhook_api.create_webhook(
+new_webhook = client.webhooks.create_webhook(
     name='Order Placed',
     url='https://yourdomain.com/webhooks/order_placed',
     events=['order_placed'],
     is_active=True
 )
 print(new_webhook)
 ```
@@ -125,14 +115,9 @@
 ## Contributions
 
 Contributions are welcome! For major changes, please open an issue first to discuss what you would like to change.
 
 ## License
 
 This SDK is released under the MIT License. See the LICENSE file for more details.
-```
-
-This README includes basic examples of how to use each part of your SDK. It also guides the user on error handling and encourages community contributions, which are important aspects of maintaining an open-source project.
 
-**Suggestions for your next steps:**
-- **a.** Consider adding a `Contributing.md` file to guide potential contributors on how to help develop the SDK further.
-- **b.** Regularly update the documentation as you add features or make changes to the SDK.
+---
```

### Comparing `partnero-0.2.0/partnero/authentication.py` & `partnero-0.3.0/partnero/authentication.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,20 +8,20 @@
         if cls not in cls._instances:
             instance = super().__call__(*args, **kwargs)
             cls._instances[cls] = instance
         return cls._instances[cls]
 
 
 class Authentication(metaclass=SingletonMeta):
-    api_token = None
+    api_key = None
 
     @classmethod
-    def configure(cls, api_token):
-        cls.api_token = api_token
+    def configure(cls, api_key):
+        cls.api_key = api_key
 
     def get_headers(self) -> Dict[str, str]:
-        if not self.api_token:
-            raise ValueError("API token has not been set.")
+        if not self.api_key:
+            raise ValueError("API key has not been set.")
         return {
-            'Authorization': f'Bearer {self.api_token}',
+            'Authorization': f'Bearer {self.api_key}',
             'Content-Type': 'application/json'
         }
```

### Comparing `partnero-0.2.0/partnero/base_api.py` & `partnero-0.3.0/partnero/base_api.py`

 * *Files identical despite different names*

### Comparing `partnero-0.2.0/partnero/coupon_api.py` & `partnero-0.3.0/partnero/coupon_api.py`

 * *Files identical despite different names*

### Comparing `partnero-0.2.0/partnero/customer_api.py` & `partnero-0.3.0/partnero/customer_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         validate_key(partner_key, "partner_key")
         validate_key(customer_key, "customer_key")
         data = {'partner': {'key': partner_key}, 'key': customer_key, 'email': email, 'name': name}
         return self.send_request('POST', 'customers', data=data)
 
     def get_customer(self, email: str = None, customer_key: str = None) -> dict:
         """
-        Search for partners based on provided parameters. Parameters are optional.
+        Search for customer based on provided parameters. Parameters are optional.
         :param email: Email of the customer to search for.
         :param customer_key: ID of the customer to search for.
         """
         params = {k: v for k, v in [('email', email), ('key', customer_key)] if v is not None}
         return self.send_request('GET', 'customers:search', params=params)
 
     def get_customer_transactions(self, customer_key: str, limit: int = 15, page: int = 1) -> dict:
```

### Comparing `partnero-0.2.0/partnero/partner_api.py` & `partnero-0.3.0/partnero/partner_api.py`

 * *Files identical despite different names*

### Comparing `partnero-0.2.0/partnero/promotion_code_api.py` & `partnero-0.3.0/partnero/promotion_code_api.py`

 * *Files identical despite different names*

### Comparing `partnero-0.2.0/partnero/transaction_api.py` & `partnero-0.3.0/partnero/transaction_api.py`

 * *Files identical despite different names*

### Comparing `partnero-0.2.0/partnero/webhook_api.py` & `partnero-0.3.0/partnero/webhook_api.py`

 * *Files identical despite different names*

### Comparing `partnero-0.2.0/pyproject.toml` & `partnero-0.3.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 [tool.poetry]
 name = "partnero"
-version = "0.2.0"
+version = "0.3.0"
 description = "A Python SDK designed to wrap around the Partnero API."
-authors = ["Your Name <you@example.com>"]
 readme = "README.md"
+license = "MIT"
+
+authors = [
+    "Simon Mahfoud <simon@offerwell.com>",
+]
+
+maintainers = [
+    "James Garcia <james@offerwell.com>",
+]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 requests = "^2.31.0"
 
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `partnero-0.2.0/PKG-INFO` & `partnero-0.3.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,111 +1,108 @@
 Metadata-Version: 2.1
 Name: partnero
-Version: 0.2.0
+Version: 0.3.0
 Summary: A Python SDK designed to wrap around the Partnero API.
-Author: Your Name
-Author-email: you@example.com
+License: MIT
+Author: Simon Mahfoud
+Author-email: simon@offerwell.com
+Maintainer: James Garcia
+Maintainer-email: james@offerwell.com
 Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Partnero SDK
 
-The Partnero SDK provides a simple and powerful Python interface to the Partnero API, allowing developers to manage customers, partners, transactions, webhooks, coupons, and promotion codes programmatically.
+The Partnero SDK provides a simple and powerful Python interface to the Partnero API, allowing developers to manage customers, partners, transactions, webhooks, coupons, and promotion codes programmatically. It simplifies interactions by providing a centralized client (`PartneroClient`) that handles configuration and request management.
+
 [Partnero API Documentation](https://developers.partnero.com/reference/general.html)
+
 ## Installation
 
 To install the Partnero SDK, run the following command:
 
 ```bash
 pip install partnero
 ```
 
 ## Configuration
 
-Before using the SDK, you need to set up authentication:
+Before using the SDK, configure the `PartneroClient` with your API token:
 
 ```python
-from partnero import Authentication
+from partnero import PartneroClient
 
 # Replace 'your_api_token_here' with your actual API token
-auth = Authentication.configure(api_token='your_api_token_here')
+client = PartneroClient(api_key='your_api_token_here')
 ```
 
 ## Usage
 
-Here's how you can use different components of the SDK:
+With `PartneroClient`, you can easily access different parts of the Partnero API. Here's how you can use it to manage customers, partners, transactions, and webhooks:
 
 ### Customer Management
 
 **List Customers**
 
 ```python
-from partnero import CustomerAPI
-
-customer_api = CustomerAPI()
-customers = customer_api.list_customers(limit=10, page=1)
+customers = client.customers.list_customers(limit=10, page=1)
 print(customers)
 ```
 
 **Create a New Customer**
 
 ```python
-new_customer = customer_api.create_customer(
+new_customer = client.customers.create_customer(
     partner_key='your_partner_key',
     customer_key='unique_customer_key',
     email='customer@example.com',
     name='Customer Name'
 )
 print(new_customer)
 ```
 
 ### Partner Management
 
 **List Partners**
 
 ```python
-from partnero import PartnerAPI
-
-partner_api = PartnerAPI()
-partners = partner_api.list_partners(limit=5, page=1)
+partners = client.partners.list_partners(limit=5, page=1)
 print(partners)
 ```
 
 **Register a New Partner**
 
 ```python
-new_partner = partner_api.create_partner(
+new_partner = client.partners.create_partner(
     email='newpartner@example.com',
     name='New Partner',
     password='securepassword123'
 )
 print(new_partner)
 ```
 
 ### Transaction Management
 
 **List Transactions**
 
 ```python
-from partnero import TransactionAPI
-
-transaction_api = TransactionAPI()
-transactions = transaction_api.list_transactions(limit=5, page=1)
+transactions = client.transactions.list_transactions(limit=5, page=1)
 print(transactions)
 ```
 
 **Create a Transaction**
 
 ```python
-new_transaction = transaction_api.create_transaction(
+new_transaction = client.transactions.create_transaction(
     customer_key='customer_key',
     transaction_key='unique_transaction_key',
     amount=39.99,
     product_id='product_id',
     product_type='type',
     action='purchase'
 )
@@ -113,25 +110,22 @@
 ```
 
 ### Webhook Management
 
 **List Webhooks**
 
 ```python
-from partnero import WebhookAPI
-
-webhook_api = WebhookAPI()
-webhooks = webhook_api.list_webhooks(limit=5, page=1)
+webhooks = client.webhooks.list_webhooks(limit=5, page=1)
 print(webhooks)
 ```
 
 **Create a Webhook**
 
 ```python
-new_webhook = webhook_api.create_webhook(
+new_webhook = client.webhooks.create_webhook(
     name='Order Placed',
     url='https://yourdomain.com/webhooks/order_placed',
     events=['order_placed'],
     is_active=True
 )
 print(new_webhook)
 ```
@@ -139,14 +133,9 @@
 ## Contributions
 
 Contributions are welcome! For major changes, please open an issue first to discuss what you would like to change.
 
 ## License
 
 This SDK is released under the MIT License. See the LICENSE file for more details.
-```
-
-This README includes basic examples of how to use each part of your SDK. It also guides the user on error handling and encourages community contributions, which are important aspects of maintaining an open-source project.
 
-**Suggestions for your next steps:**
-- **a.** Consider adding a `Contributing.md` file to guide potential contributors on how to help develop the SDK further.
-- **b.** Regularly update the documentation as you add features or make changes to the SDK.
+---
```

