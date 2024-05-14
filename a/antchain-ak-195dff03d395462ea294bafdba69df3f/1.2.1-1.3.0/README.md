# Comparing `tmp/antchain_ak_195dff03d395462ea294bafdba69df3f-1.2.1.tar.gz` & `tmp/antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_ak_195dff03d395462ea294bafdba69df3f-1.2.1.tar", last modified: Fri Mar 15 03:57:22 2024, max compression
+gzip compressed data, was "dist/antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0.tar", last modified: Tue May 14 02:40:03 2024, max compression
```

## Comparing `antchain_ak_195dff03d395462ea294bafdba69df3f-1.2.1.tar` & `antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 03:57:22.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.2.1/
--rw-r--r--   0 root         (0) root         (0)      600 2024-03-15 03:57:21.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-03-15 03:57:21.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2354 2024-03-15 03:57:22.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      900 2024-03-15 03:57:21.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.2.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1086 2024-03-15 03:57:21.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 03:57:22.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.2.1/antchain_ak_195dff03d395462ea294bafdba69df3f.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2354 2024-03-15 03:57:22.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.2.1/antchain_ak_195dff03d395462ea294bafdba69df3f.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      579 2024-03-15 03:57:22.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.2.1/antchain_ak_195dff03d395462ea294bafdba69df3f.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-15 03:57:22.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.2.1/antchain_ak_195dff03d395462ea294bafdba69df3f.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      108 2024-03-15 03:57:22.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.2.1/antchain_ak_195dff03d395462ea294bafdba69df3f.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       49 2024-03-15 03:57:22.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.2.1/antchain_ak_195dff03d395462ea294bafdba69df3f.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 03:57:22.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.2.1/antchain_sdk_ak_195dff03d395462ea294bafdba69df3f/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-15 03:57:21.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.2.1/antchain_sdk_ak_195dff03d395462ea294bafdba69df3f/__init__.py
--rw-r--r--   0 root         (0) root         (0)   123492 2024-03-15 03:57:21.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.2.1/antchain_sdk_ak_195dff03d395462ea294bafdba69df3f/client.py
--rw-r--r--   0 root         (0) root         (0)   185302 2024-03-15 03:57:21.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.2.1/antchain_sdk_ak_195dff03d395462ea294bafdba69df3f/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-15 03:57:22.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2651 2024-03-15 03:57:21.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 02:40:03.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0/
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-14 02:40:02.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-14 02:40:02.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2354 2024-05-14 02:40:03.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      900 2024-05-14 02:40:02.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1086 2024-05-14 02:40:02.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 02:40:03.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0/antchain_ak_195dff03d395462ea294bafdba69df3f.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2354 2024-05-14 02:40:03.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0/antchain_ak_195dff03d395462ea294bafdba69df3f.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      579 2024-05-14 02:40:03.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0/antchain_ak_195dff03d395462ea294bafdba69df3f.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 02:40:03.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0/antchain_ak_195dff03d395462ea294bafdba69df3f.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2024-05-14 02:40:03.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0/antchain_ak_195dff03d395462ea294bafdba69df3f.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2024-05-14 02:40:03.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0/antchain_ak_195dff03d395462ea294bafdba69df3f.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 02:40:03.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0/antchain_sdk_ak_195dff03d395462ea294bafdba69df3f/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-14 02:40:02.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0/antchain_sdk_ak_195dff03d395462ea294bafdba69df3f/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   131808 2024-05-14 02:40:02.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0/antchain_sdk_ak_195dff03d395462ea294bafdba69df3f/client.py
+-rw-r--r--   0 root         (0) root         (0)   201784 2024-05-14 02:40:02.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0/antchain_sdk_ak_195dff03d395462ea294bafdba69df3f/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-14 02:40:03.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2651 2024-05-14 02:40:02.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0/setup.py
```

### Comparing `antchain_ak_195dff03d395462ea294bafdba69df3f-1.2.1/LICENSE` & `antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_ak_195dff03d395462ea294bafdba69df3f-1.2.1/PKG-INFO` & `antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_ak_195dff03d395462ea294bafdba69df3f
-Version: 1.2.1
+Version: 1.3.0
 Summary: Ant Chain Ak_195dff03d395462ea294bafdba69df3f SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_195dff03d395462ea294bafdba69df3f-1.2.1/README-CN.md` & `antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_195dff03d395462ea294bafdba69df3f-1.2.1/README.md` & `antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_195dff03d395462ea294bafdba69df3f-1.2.1/antchain_ak_195dff03d395462ea294bafdba69df3f.egg-info/PKG-INFO` & `antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0/antchain_ak_195dff03d395462ea294bafdba69df3f.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-ak-195dff03d395462ea294bafdba69df3f
-Version: 1.2.1
+Version: 1.3.0
 Summary: Ant Chain Ak_195dff03d395462ea294bafdba69df3f SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_195dff03d395462ea294bafdba69df3f-1.2.1/antchain_ak_195dff03d395462ea294bafdba69df3f.egg-info/SOURCES.txt` & `antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0/antchain_ak_195dff03d395462ea294bafdba69df3f.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `antchain_ak_195dff03d395462ea294bafdba69df3f-1.2.1/antchain_sdk_ak_195dff03d395462ea294bafdba69df3f/client.py` & `antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0/antchain_sdk_ak_195dff03d395462ea294bafdba69df3f/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.2.1',
+                    'sdk_version': '1.3.0',
                     '_prod_code': 'ak_195dff03d395462ea294bafdba69df3f',
                     '_prod_channel': 'saas'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -235,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.2.1',
+                    'sdk_version': '1.3.0',
                     '_prod_code': 'ak_195dff03d395462ea294bafdba69df3f',
                     '_prod_channel': 'saas'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -2411,14 +2411,182 @@
             request.file_id = upload_resp.file_id
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             ak__195dff_03d_395462ea_294bafdba_69df_3f_models.UploadAntchainAtoSignFlowResponse(),
             await self.do_request_async('1.0', 'antchain.ato.sign.flow.upload', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
+    def create_antchain_ato_withhold_refund(
+        self,
+        request: ak__195dff_03d_395462ea_294bafdba_69df_3f_models.CreateAntchainAtoWithholdRefundRequest,
+    ) -> ak__195dff_03d_395462ea_294bafdba_69df_3f_models.CreateAntchainAtoWithholdRefundResponse:
+        """
+        Description: 创建退款请求
+        Summary: 创建退款申请
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.create_antchain_ato_withhold_refund_ex(request, headers, runtime)
+
+    async def create_antchain_ato_withhold_refund_async(
+        self,
+        request: ak__195dff_03d_395462ea_294bafdba_69df_3f_models.CreateAntchainAtoWithholdRefundRequest,
+    ) -> ak__195dff_03d_395462ea_294bafdba_69df_3f_models.CreateAntchainAtoWithholdRefundResponse:
+        """
+        Description: 创建退款请求
+        Summary: 创建退款申请
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.create_antchain_ato_withhold_refund_ex_async(request, headers, runtime)
+
+    def create_antchain_ato_withhold_refund_ex(
+        self,
+        request: ak__195dff_03d_395462ea_294bafdba_69df_3f_models.CreateAntchainAtoWithholdRefundRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ak__195dff_03d_395462ea_294bafdba_69df_3f_models.CreateAntchainAtoWithholdRefundResponse:
+        """
+        Description: 创建退款请求
+        Summary: 创建退款申请
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ak__195dff_03d_395462ea_294bafdba_69df_3f_models.CreateAntchainAtoWithholdRefundResponse(),
+            self.do_request('1.0', 'antchain.ato.withhold.refund.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def create_antchain_ato_withhold_refund_ex_async(
+        self,
+        request: ak__195dff_03d_395462ea_294bafdba_69df_3f_models.CreateAntchainAtoWithholdRefundRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ak__195dff_03d_395462ea_294bafdba_69df_3f_models.CreateAntchainAtoWithholdRefundResponse:
+        """
+        Description: 创建退款请求
+        Summary: 创建退款申请
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ak__195dff_03d_395462ea_294bafdba_69df_3f_models.CreateAntchainAtoWithholdRefundResponse(),
+            await self.do_request_async('1.0', 'antchain.ato.withhold.refund.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def query_antchain_ato_withhold_refund(
+        self,
+        request: ak__195dff_03d_395462ea_294bafdba_69df_3f_models.QueryAntchainAtoWithholdRefundRequest,
+    ) -> ak__195dff_03d_395462ea_294bafdba_69df_3f_models.QueryAntchainAtoWithholdRefundResponse:
+        """
+        Description: 退款申请结果查询
+        Summary: 退款申请结果查询
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.query_antchain_ato_withhold_refund_ex(request, headers, runtime)
+
+    async def query_antchain_ato_withhold_refund_async(
+        self,
+        request: ak__195dff_03d_395462ea_294bafdba_69df_3f_models.QueryAntchainAtoWithholdRefundRequest,
+    ) -> ak__195dff_03d_395462ea_294bafdba_69df_3f_models.QueryAntchainAtoWithholdRefundResponse:
+        """
+        Description: 退款申请结果查询
+        Summary: 退款申请结果查询
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.query_antchain_ato_withhold_refund_ex_async(request, headers, runtime)
+
+    def query_antchain_ato_withhold_refund_ex(
+        self,
+        request: ak__195dff_03d_395462ea_294bafdba_69df_3f_models.QueryAntchainAtoWithholdRefundRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ak__195dff_03d_395462ea_294bafdba_69df_3f_models.QueryAntchainAtoWithholdRefundResponse:
+        """
+        Description: 退款申请结果查询
+        Summary: 退款申请结果查询
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ak__195dff_03d_395462ea_294bafdba_69df_3f_models.QueryAntchainAtoWithholdRefundResponse(),
+            self.do_request('1.0', 'antchain.ato.withhold.refund.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def query_antchain_ato_withhold_refund_ex_async(
+        self,
+        request: ak__195dff_03d_395462ea_294bafdba_69df_3f_models.QueryAntchainAtoWithholdRefundRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ak__195dff_03d_395462ea_294bafdba_69df_3f_models.QueryAntchainAtoWithholdRefundResponse:
+        """
+        Description: 退款申请结果查询
+        Summary: 退款申请结果查询
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ak__195dff_03d_395462ea_294bafdba_69df_3f_models.QueryAntchainAtoWithholdRefundResponse(),
+            await self.do_request_async('1.0', 'antchain.ato.withhold.refund.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def notify_antchain_ato_fund_flow(
+        self,
+        request: ak__195dff_03d_395462ea_294bafdba_69df_3f_models.NotifyAntchainAtoFundFlowRequest,
+    ) -> ak__195dff_03d_395462ea_294bafdba_69df_3f_models.NotifyAntchainAtoFundFlowResponse:
+        """
+        Description: 用于资方将盖章后的合同文件上传给ISV后，ISV通过该接口通知资方已上传合同
+        Summary: 资方合同文件已上传确认接口
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.notify_antchain_ato_fund_flow_ex(request, headers, runtime)
+
+    async def notify_antchain_ato_fund_flow_async(
+        self,
+        request: ak__195dff_03d_395462ea_294bafdba_69df_3f_models.NotifyAntchainAtoFundFlowRequest,
+    ) -> ak__195dff_03d_395462ea_294bafdba_69df_3f_models.NotifyAntchainAtoFundFlowResponse:
+        """
+        Description: 用于资方将盖章后的合同文件上传给ISV后，ISV通过该接口通知资方已上传合同
+        Summary: 资方合同文件已上传确认接口
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.notify_antchain_ato_fund_flow_ex_async(request, headers, runtime)
+
+    def notify_antchain_ato_fund_flow_ex(
+        self,
+        request: ak__195dff_03d_395462ea_294bafdba_69df_3f_models.NotifyAntchainAtoFundFlowRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ak__195dff_03d_395462ea_294bafdba_69df_3f_models.NotifyAntchainAtoFundFlowResponse:
+        """
+        Description: 用于资方将盖章后的合同文件上传给ISV后，ISV通过该接口通知资方已上传合同
+        Summary: 资方合同文件已上传确认接口
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ak__195dff_03d_395462ea_294bafdba_69df_3f_models.NotifyAntchainAtoFundFlowResponse(),
+            self.do_request('1.0', 'antchain.ato.fund.flow.notify', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def notify_antchain_ato_fund_flow_ex_async(
+        self,
+        request: ak__195dff_03d_395462ea_294bafdba_69df_3f_models.NotifyAntchainAtoFundFlowRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ak__195dff_03d_395462ea_294bafdba_69df_3f_models.NotifyAntchainAtoFundFlowResponse:
+        """
+        Description: 用于资方将盖章后的合同文件上传给ISV后，ISV通过该接口通知资方已上传合同
+        Summary: 资方合同文件已上传确认接口
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ak__195dff_03d_395462ea_294bafdba_69df_3f_models.NotifyAntchainAtoFundFlowResponse(),
+            await self.do_request_async('1.0', 'antchain.ato.fund.flow.notify', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
     def create_antcloud_gatewayx_file_upload(
         self,
         request: ak__195dff_03d_395462ea_294bafdba_69df_3f_models.CreateAntcloudGatewayxFileUploadRequest,
     ) -> ak__195dff_03d_395462ea_294bafdba_69df_3f_models.CreateAntcloudGatewayxFileUploadResponse:
         """
         Description: 创建HTTP PUT提交的文件上传
         Summary: 文件上传创建
```

### Comparing `antchain_ak_195dff03d395462ea294bafdba69df3f-1.2.1/antchain_sdk_ak_195dff03d395462ea294bafdba69df3f/models.py` & `antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0/antchain_sdk_ak_195dff03d395462ea294bafdba69df3f/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -735,57 +735,65 @@
 
 class AllAntchainAtoSignTemplateRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         contract_type: str = None,
+        merchant_id: str = None,
         fund_type: str = None,
         fund_id: str = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
         # 合同类型，如果不传则返回所有
         self.contract_type = contract_type
+        # 商户统一社会信用代码，SIT环境，非融必填
+        self.merchant_id = merchant_id
         # ● FINANCE 融资
         # ● NON_FINANCE 非融资
         self.fund_type = fund_type
         # 查询融资类型时，需要传入资方统一社会信用代码
         self.fund_id = fund_id
 
     def validate(self):
-        pass
+        if self.merchant_id is not None:
+            self.validate_max_length(self.merchant_id, 'merchant_id', 42)
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
         if self.contract_type is not None:
             result['contract_type'] = self.contract_type
+        if self.merchant_id is not None:
+            result['merchant_id'] = self.merchant_id
         if self.fund_type is not None:
             result['fund_type'] = self.fund_type
         if self.fund_id is not None:
             result['fund_id'] = self.fund_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
             self.product_instance_id = m.get('product_instance_id')
         if m.get('contract_type') is not None:
             self.contract_type = m.get('contract_type')
+        if m.get('merchant_id') is not None:
+            self.merchant_id = m.get('merchant_id')
         if m.get('fund_type') is not None:
             self.fund_type = m.get('fund_type')
         if m.get('fund_id') is not None:
             self.fund_id = m.get('fund_id')
         return self
 
 
@@ -1186,14 +1194,15 @@
         order_id: str = None,
         account_id: str = None,
         status: str = None,
         flow_id: str = None,
         doc_list: str = None,
         business_scene: str = None,
         alipay_user_id: str = None,
+        sign_info: str = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
         # 结果码，一般OK表示调用成功
         self.result_code = result_code
         # 异常信息的文本描述
         self.result_msg = result_msg
@@ -1211,14 +1220,16 @@
         # 签署文件列表，参考：
         # _[{"fileItemNo":"10090801000001699892007791144960","agreementType":"COMMON","fileName":"xxx合同","fileSize":228530,"signAccountId":"fe2eb3814c4e49edba2bc012f790771f","fileId":"2c7684461a0f4d33bc02f6d77f7b3937","downloadUrl":"https://dev.oss-cn-shanghai.aliyuncs.com/ag/ord/xxx/16939683744483057_%E6%B5%8B%E8%AF%95%E6%A8%A1%E6%9D%BF%E4%B9%8B%E5%8D%8F%E8%AE%AE%E7%AD%BE%E7%BD%B2%E8%AF%81%E6%98%8E.pdf?Expires=1693971989&OSSAccessKeyId=LTAI5tR3hHiaXPAh8YsY9Dce&Signature=i%2FfAgDem33guI%2F0KjIFj24XZNCc%3D"}]_
         self.doc_list = doc_list
         # 业务场景，主要用于签署合同的标题描述
         self.business_scene = business_scene
         # 签署合同中的订单的uid。
         self.alipay_user_id = alipay_user_id
+        # 签署扩展信息，用于获取签署链接等。JSON格式字符串。
+        self.sign_info = sign_info
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -1243,14 +1254,16 @@
             result['flow_id'] = self.flow_id
         if self.doc_list is not None:
             result['doc_list'] = self.doc_list
         if self.business_scene is not None:
             result['business_scene'] = self.business_scene
         if self.alipay_user_id is not None:
             result['alipay_user_id'] = self.alipay_user_id
+        if self.sign_info is not None:
+            result['sign_info'] = self.sign_info
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('req_msg_id') is not None:
             self.req_msg_id = m.get('req_msg_id')
         if m.get('result_code') is not None:
@@ -1269,14 +1282,16 @@
             self.flow_id = m.get('flow_id')
         if m.get('doc_list') is not None:
             self.doc_list = m.get('doc_list')
         if m.get('business_scene') is not None:
             self.business_scene = m.get('business_scene')
         if m.get('alipay_user_id') is not None:
             self.alipay_user_id = m.get('alipay_user_id')
+        if m.get('sign_info') is not None:
+            self.sign_info = m.get('sign_info')
         return self
 
 
 class CreateAntchainAtoWithholdSignRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
@@ -4826,14 +4841,429 @@
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
         if m.get('file_item_no') is not None:
             self.file_item_no = m.get('file_item_no')
         return self
 
 
+class CreateAntchainAtoWithholdRefundRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        order_id: str = None,
+        period_num: int = None,
+        refund_request_no: str = None,
+        refund_money: int = None,
+        refund_reason: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 订单id
+        self.order_id = order_id
+        # 第几期
+        # 针对用户履约的第几期进行退款申请
+        self.period_num = period_num
+        # 外部系统传入的退款请求号
+        self.refund_request_no = refund_request_no
+        # 本次请求的退款金额，单位为分
+        # 1234=12.34元
+        self.refund_money = refund_money
+        # 退款原因
+        self.refund_reason = refund_reason
+
+    def validate(self):
+        self.validate_required(self.order_id, 'order_id')
+        if self.order_id is not None:
+            self.validate_max_length(self.order_id, 'order_id', 128)
+        self.validate_required(self.period_num, 'period_num')
+        if self.period_num is not None:
+            self.validate_minimum(self.period_num, 'period_num', 1)
+        self.validate_required(self.refund_request_no, 'refund_request_no')
+        if self.refund_request_no is not None:
+            self.validate_max_length(self.refund_request_no, 'refund_request_no', 128)
+        self.validate_required(self.refund_money, 'refund_money')
+        if self.refund_money is not None:
+            self.validate_minimum(self.refund_money, 'refund_money', 1)
+        if self.refund_reason is not None:
+            self.validate_max_length(self.refund_reason, 'refund_reason', 200)
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.order_id is not None:
+            result['order_id'] = self.order_id
+        if self.period_num is not None:
+            result['period_num'] = self.period_num
+        if self.refund_request_no is not None:
+            result['refund_request_no'] = self.refund_request_no
+        if self.refund_money is not None:
+            result['refund_money'] = self.refund_money
+        if self.refund_reason is not None:
+            result['refund_reason'] = self.refund_reason
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('order_id') is not None:
+            self.order_id = m.get('order_id')
+        if m.get('period_num') is not None:
+            self.period_num = m.get('period_num')
+        if m.get('refund_request_no') is not None:
+            self.refund_request_no = m.get('refund_request_no')
+        if m.get('refund_money') is not None:
+            self.refund_money = m.get('refund_money')
+        if m.get('refund_reason') is not None:
+            self.refund_reason = m.get('refund_reason')
+        return self
+
+
+class CreateAntchainAtoWithholdRefundResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        refund_request_no: str = None,
+        status: str = None,
+        refund_order_no: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 外部系统传入的退款请求号
+        self.refund_request_no = refund_request_no
+        # ACCEPT : 受理成功
+        self.status = status
+        # 请求支付宝的退款单据号
+        self.refund_order_no = refund_order_no
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.refund_request_no is not None:
+            result['refund_request_no'] = self.refund_request_no
+        if self.status is not None:
+            result['status'] = self.status
+        if self.refund_order_no is not None:
+            result['refund_order_no'] = self.refund_order_no
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('refund_request_no') is not None:
+            self.refund_request_no = m.get('refund_request_no')
+        if m.get('status') is not None:
+            self.status = m.get('status')
+        if m.get('refund_order_no') is not None:
+            self.refund_order_no = m.get('refund_order_no')
+        return self
+
+
+class QueryAntchainAtoWithholdRefundRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        order_id: str = None,
+        period_num: int = None,
+        refund_request_no: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 订单id
+        self.order_id = order_id
+        # 几期
+        # 针对用户履约的第几期进行退款申请
+        self.period_num = period_num
+        # 外部系统传入的退款请求号
+        self.refund_request_no = refund_request_no
+
+    def validate(self):
+        self.validate_required(self.order_id, 'order_id')
+        if self.order_id is not None:
+            self.validate_max_length(self.order_id, 'order_id', 128)
+        self.validate_required(self.period_num, 'period_num')
+        if self.period_num is not None:
+            self.validate_minimum(self.period_num, 'period_num', 1)
+        self.validate_required(self.refund_request_no, 'refund_request_no')
+        if self.refund_request_no is not None:
+            self.validate_max_length(self.refund_request_no, 'refund_request_no', 128)
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.order_id is not None:
+            result['order_id'] = self.order_id
+        if self.period_num is not None:
+            result['period_num'] = self.period_num
+        if self.refund_request_no is not None:
+            result['refund_request_no'] = self.refund_request_no
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('order_id') is not None:
+            self.order_id = m.get('order_id')
+        if m.get('period_num') is not None:
+            self.period_num = m.get('period_num')
+        if m.get('refund_request_no') is not None:
+            self.refund_request_no = m.get('refund_request_no')
+        return self
+
+
+class QueryAntchainAtoWithholdRefundResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        refund_request_no: str = None,
+        refund_order_no: str = None,
+        status: str = None,
+        refund_error_msg: str = None,
+        total_refund_amount: int = None,
+        send_back_amount: int = None,
+        gmt_refund_pay: int = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 外部系统传入的退款请求号
+        self.refund_request_no = refund_request_no
+        # 请求支付宝的退款单据号
+        self.refund_order_no = refund_order_no
+        # 退款请求状态
+        # ● ACCEPT: 受理成功
+        # ● PENDING: 需人工介入
+        # ● SUCCESS: 成功
+        # ● FAILED : 失败
+        self.status = status
+        # 退款失败原因
+        self.refund_error_msg = refund_error_msg
+        # 本笔交易总退款金额，单位为分
+        # 12300=123元
+        self.total_refund_amount = total_refund_amount
+        # 本次退款申请的实际退款金额，单位为分
+        # 12300=123元
+        self.send_back_amount = send_back_amount
+        # 实际退款时间,13位时间戳（毫秒）
+        self.gmt_refund_pay = gmt_refund_pay
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.refund_request_no is not None:
+            result['refund_request_no'] = self.refund_request_no
+        if self.refund_order_no is not None:
+            result['refund_order_no'] = self.refund_order_no
+        if self.status is not None:
+            result['status'] = self.status
+        if self.refund_error_msg is not None:
+            result['refund_error_msg'] = self.refund_error_msg
+        if self.total_refund_amount is not None:
+            result['total_refund_amount'] = self.total_refund_amount
+        if self.send_back_amount is not None:
+            result['send_back_amount'] = self.send_back_amount
+        if self.gmt_refund_pay is not None:
+            result['gmt_refund_pay'] = self.gmt_refund_pay
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('refund_request_no') is not None:
+            self.refund_request_no = m.get('refund_request_no')
+        if m.get('refund_order_no') is not None:
+            self.refund_order_no = m.get('refund_order_no')
+        if m.get('status') is not None:
+            self.status = m.get('status')
+        if m.get('refund_error_msg') is not None:
+            self.refund_error_msg = m.get('refund_error_msg')
+        if m.get('total_refund_amount') is not None:
+            self.total_refund_amount = m.get('total_refund_amount')
+        if m.get('send_back_amount') is not None:
+            self.send_back_amount = m.get('send_back_amount')
+        if m.get('gmt_refund_pay') is not None:
+            self.gmt_refund_pay = m.get('gmt_refund_pay')
+        return self
+
+
+class NotifyAntchainAtoFundFlowRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        merchant_id: str = None,
+        order_id: str = None,
+        sign_no: str = None,
+        file_item_no: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 订单所属商户的统一社会信用代码
+        self.merchant_id = merchant_id
+        # 商户的订单号
+        self.order_id = order_id
+        # 签署合同单号
+        self.sign_no = sign_no
+        # 返回的文件fileItemNo编号
+        self.file_item_no = file_item_no
+
+    def validate(self):
+        self.validate_required(self.merchant_id, 'merchant_id')
+        self.validate_required(self.order_id, 'order_id')
+        self.validate_required(self.sign_no, 'sign_no')
+        self.validate_required(self.file_item_no, 'file_item_no')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.merchant_id is not None:
+            result['merchant_id'] = self.merchant_id
+        if self.order_id is not None:
+            result['order_id'] = self.order_id
+        if self.sign_no is not None:
+            result['sign_no'] = self.sign_no
+        if self.file_item_no is not None:
+            result['file_item_no'] = self.file_item_no
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('merchant_id') is not None:
+            self.merchant_id = m.get('merchant_id')
+        if m.get('order_id') is not None:
+            self.order_id = m.get('order_id')
+        if m.get('sign_no') is not None:
+            self.sign_no = m.get('sign_no')
+        if m.get('file_item_no') is not None:
+            self.file_item_no = m.get('file_item_no')
+        return self
+
+
+class NotifyAntchainAtoFundFlowResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        return self
+
+
 class CreateAntcloudGatewayxFileUploadRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         api_code: str = None,
         file_label: str = None,
         file_metadata: str = None,
```

### Comparing `antchain_ak_195dff03d395462ea294bafdba69df3f-1.2.1/setup.py` & `antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_ak_195dff03d395462ea294bafdba69df3f.
 
-Created on 15/03/2024
+Created on 14/05/2024
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_ak_195dff03d395462ea294bafdba69df3f"
 NAME = "antchain_ak_195dff03d395462ea294bafdba69df3f" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain Ak_195dff03d395462ea294bafdba69df3f SDK Library for Python"
 AUTHOR = "Ant Chain SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/alipay/antchain-openapi-prod-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "antchain_alipay_util>=1.0.1, <2.0.0",
-    "alibabacloud_tea_util>=0.3.11, <1.0.0",
+    "alibabacloud_tea_util>=0.3.12, <1.0.0",
     "alibabacloud_rpc_util>=0.0.4, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

