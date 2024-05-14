# Comparing `tmp/pyreqwest_impersonate-0.4.4.tar.gz` & `tmp/pyreqwest_impersonate-0.4.5.tar.gz`

## Comparing `pyreqwest_impersonate-0.4.4.tar` & `pyreqwest_impersonate-0.4.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      947 1970-01-01 00:00:00.000000 pyreqwest_impersonate-0.4.4/Cargo.toml
--rw-r--r--   0     1001      127     8111 2024-05-13 00:13:53.000000 pyreqwest_impersonate-0.4.4/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      766 2024-05-13 00:13:53.000000 pyreqwest_impersonate-0.4.4/.gitignore
--rw-r--r--   0     1001      127     8529 2024-05-13 00:13:53.000000 pyreqwest_impersonate-0.4.4/README.md
--rw-r--r--   0     1001      127      343 2024-05-13 00:13:53.000000 pyreqwest_impersonate-0.4.4/benchmark/README.md
--rw-r--r--   0     1001      127     3484 2024-05-13 00:13:53.000000 pyreqwest_impersonate-0.4.4/benchmark/benchmark.py
--rw-r--r--   0     1001      127     3719 2024-05-13 00:13:53.000000 pyreqwest_impersonate-0.4.4/benchmark/generate_image.py
--rw-r--r--   0     1001      127      144 2024-05-13 00:13:53.000000 pyreqwest_impersonate-0.4.4/benchmark/requirements.txt
--rw-r--r--   0     1001      127      990 2024-05-13 00:13:53.000000 pyreqwest_impersonate-0.4.4/benchmark/server.py
--rw-r--r--   0     1001      127   112102 2024-05-13 00:13:53.000000 pyreqwest_impersonate-0.4.4/benchmark.jpg
--rw-r--r--   0     1001      127    29788 2024-05-13 00:13:53.000000 pyreqwest_impersonate-0.4.4/src/lib.rs
--rw-r--r--   0     1001      127     3036 2024-05-13 00:13:53.000000 pyreqwest_impersonate-0.4.4/src/response.rs
--rw-r--r--   0     1001      127     6232 2024-05-13 00:13:53.000000 pyreqwest_impersonate-0.4.4/tests/test_client.py
--rw-r--r--   0     1001      127     8287 2024-05-13 00:13:53.000000 pyreqwest_impersonate-0.4.4/tests/test_defs.py
--rw-r--r--   0     1001      127    41270 2024-05-13 00:13:53.000000 pyreqwest_impersonate-0.4.4/Cargo.lock
--rw-r--r--   0     1001      127     1151 2024-05-13 00:13:53.000000 pyreqwest_impersonate-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     9598 1970-01-01 00:00:00.000000 pyreqwest_impersonate-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1010 1970-01-01 00:00:00.000000 pyreqwest_impersonate-0.4.5/Cargo.toml
+-rw-r--r--   0     1001      127     8780 2024-05-14 11:45:15.000000 pyreqwest_impersonate-0.4.5/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      766 2024-05-14 11:45:15.000000 pyreqwest_impersonate-0.4.5/.gitignore
+-rw-r--r--   0     1001      127     8546 2024-05-14 11:45:15.000000 pyreqwest_impersonate-0.4.5/README.md
+-rw-r--r--   0     1001      127      343 2024-05-14 11:45:15.000000 pyreqwest_impersonate-0.4.5/benchmark/README.md
+-rw-r--r--   0     1001      127     3484 2024-05-14 11:45:15.000000 pyreqwest_impersonate-0.4.5/benchmark/benchmark.py
+-rw-r--r--   0     1001      127     3719 2024-05-14 11:45:15.000000 pyreqwest_impersonate-0.4.5/benchmark/generate_image.py
+-rw-r--r--   0     1001      127      144 2024-05-14 11:45:15.000000 pyreqwest_impersonate-0.4.5/benchmark/requirements.txt
+-rw-r--r--   0     1001      127      990 2024-05-14 11:45:15.000000 pyreqwest_impersonate-0.4.5/benchmark/server.py
+-rw-r--r--   0     1001      127   112327 2024-05-14 11:45:15.000000 pyreqwest_impersonate-0.4.5/benchmark.jpg
+-rw-r--r--   0     1001      127    29872 2024-05-14 11:45:15.000000 pyreqwest_impersonate-0.4.5/src/lib.rs
+-rw-r--r--   0     1001      127     3036 2024-05-14 11:45:15.000000 pyreqwest_impersonate-0.4.5/src/response.rs
+-rw-r--r--   0     1001      127     6232 2024-05-14 11:45:15.000000 pyreqwest_impersonate-0.4.5/tests/test_client.py
+-rw-r--r--   0     1001      127     8287 2024-05-14 11:45:15.000000 pyreqwest_impersonate-0.4.5/tests/test_defs.py
+-rw-r--r--   0     1001      127    41306 2024-05-14 11:45:15.000000 pyreqwest_impersonate-0.4.5/Cargo.lock
+-rw-r--r--   0     1001      127     1151 2024-05-14 11:45:15.000000 pyreqwest_impersonate-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0     9615 1970-01-01 00:00:00.000000 pyreqwest_impersonate-0.4.5/PKG-INFO
```

### Comparing `pyreqwest_impersonate-0.4.4/Cargo.toml` & `pyreqwest_impersonate-0.4.5/Cargo.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 [package]
 name = "pyreqwest_impersonate"
-version = "0.4.4"
+version = "0.4.5"
 edition = "2021"
 description = "HTTP client that can impersonate web browsers, mimicking their headers and `TLS/JA3/JA4/HTTP2` fingerprints"
 authors = ["deedy5"]
 
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "pyreqwest_impersonate"
 crate-type = ["cdylib"]
 
 [dependencies]
-pyo3 = { version = "0.21", features = ["extension-module", "abi3-py38"] }
+pyo3 = { version = "0.21", features = ["extension-module", "abi3-py38", "indexmap"] }
 reqwest-impersonate = { version = "0.11", default-features = false, features = [
     "cookies",
     "boring-tls",
     "impersonate",
     "json",
     "multipart",  # to send a multipart/form-data body
     "socks",
     "gzip",
     "brotli",
     "deflate",
 ] }
 encoding_rs = { version = "0.8" }
+indexmap = { version = "2", features = ["serde"] }
 pythonize = "0.21"
 serde_json = "1"
 tokio = { version = "1", features = ["fs", "rt"] }
 
 [profile.release]
 codegen-units = 1
 lto = "fat"
```

### Comparing `pyreqwest_impersonate-0.4.4/.github/workflows/CI.yml` & `pyreqwest_impersonate-0.4.5/.github/workflows/CI.yml`

 * *Files 10% similar despite different names*

```diff
@@ -247,16 +247,29 @@
           pip install -r benchmark/requirements.txt
       - name: Start Uvicorn server
         run: |
           uvicorn benchmark.server:app --host 0.0.0.0 --port 8000 &
           sleep 10
       - name: Run benchmark
         run: python benchmark/benchmark.py
-      - name: Generate image and commit
+      - name: Generate image and commit to the new branch
         run: |
           python benchmark/generate_image.py
           git config --global user.name 'GitHub Actions'
           git config --global user.email 'actions@github.com'
           git add \*.jpg
           git diff --quiet && git diff --staged --quiet || git commit -m "Update generated image"
-          # Attempt to push changes only if there are changes to commit
-          git push https://${{ secrets.PUSH_TOKEN }}@github.com/${{ github.repository }} || echo "No changes to push"
+          # Create a new branch and switch to it
+          git checkout -b update-generated-image
+          # Attempt to push changes to the new branch
+          git push https://${{ secrets.PUSH_TOKEN }}@github.com/deedy5/pyreqwest_impersonate.git update-generated-image || echo "No changes to push"
+      - name: Merge changes into main and delete temporary branch
+        run: |
+          # Fetch the latest changes from the remote repository
+          git fetch origin
+          # Merge the temporary branch into main
+          git checkout main
+          git merge update-generated-image
+          # Push the changes to the main branch
+          git push https://${{ secrets.PUSH_TOKEN }}@github.com/deedy5/pyreqwest_impersonate.git main
+          # Delete the temporary branch
+          git push origin --delete update-generated-image
```

### Comparing `pyreqwest_impersonate-0.4.4/.gitignore` & `pyreqwest_impersonate-0.4.5/.gitignore`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.4.4/README.md` & `pyreqwest_impersonate-0.4.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -59,18 +59,18 @@
             in additional requests. Default is True.
         referer (bool, optional): Enable or disable automatic setting of the `Referer` header. Default is True.
         proxy (str, optional): Proxy URL for HTTP requests. Example: "socks5://127.0.0.1:9150". Default is None.
         impersonate (str, optional): Entity to impersonate. Example: "chrome_124". Default is None.
             Chrome: "chrome_99","chrome_100","chrome_101","chrome_104","chrome_105","chrome_106","chrome_108", 
                 "chrome_107","chrome_109","chrome_114","chrome_116","chrome_117","chrome_118","chrome_119", 
                 "chrome_120","chrome_123","chrome_124"
-            Safari: "safari_ios_17.2","safari_15.3","safari_15.5","safari_15.6.1","safari_16","safari_16.5","safari_17.2.1", 
-                "safari_17.4.1"
+            Safari: "safari_ios_16.5","safari_ios_17.2","safari_15.3","safari_15.5","safari_15.6.1","safari_16",
+                "safari_16.5","safari_17.2.1","safari_17.4.1"
             OkHttp: "okhttp_3.9","okhttp_3.11","okhttp_3.13","okhttp_3.14","okhttp_4.9","okhttp_4.10","okhttp_5"
-            Edge: "edge_99","edge_101","edge_120"
+            Edge: "edge_99","edge_101","edge_122"
         follow_redirects (bool, optional): Whether to follow redirects. Default is True.
         max_redirects (int, optional): Maximum redirects to follow. Default 20. Applies if `follow_redirects` is True.
         verify (bool, optional): Verify SSL certificates. Default is True.
         http1 (bool, optional): Use only HTTP/1.1. Default is None.
         http2 (bool, optional): Use only HTTP/2. Default is None.
          
     """
```

### Comparing `pyreqwest_impersonate-0.4.4/benchmark/benchmark.py` & `pyreqwest_impersonate-0.4.5/benchmark/benchmark.py`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.4.4/benchmark/generate_image.py` & `pyreqwest_impersonate-0.4.5/benchmark/generate_image.py`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.4.4/benchmark/server.py` & `pyreqwest_impersonate-0.4.5/benchmark/server.py`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.4.4/benchmark.jpg` & `pyreqwest_impersonate-0.4.5/benchmark.jpg`

 * *Files 20% similar despite different names*

#### Image content

```diff
@@ -1,21 +1,21 @@
    ;:;;@88888X88888S8888X%X888@8@88@88@S88@88X888@@X8@@8;;::
- ::88;XS:%8tSSttS%X%X:@8X%SSt.8%SSXSt%@%SS%S%.  .  %;  8;t %
-S:;t      .           ..     .  .          .      S8 . X%8 t
-8.:%  . .    .    .S8   ;;        .   . S .  t; . S8   @8S %
-S ;%  .:S;@  :X ;;S88  ;8. ..t.@  :%.%8S8X.tX.@.t8S8 .8 8X.t
-  :% X@ t8 8@ttS.%:@8t.S. @:.8@ @8  t8@ %8@88 @XSX88SS888@.t
-  ;;;;;XX@8X8Xt:t;S%@88X%888X88@8888XX@8X888SSt.:@X@8@S%:;;:
-   ;:;;888888888888%88@88XS@88X8@888888%8@@888888@@X8@@@t:;:
- . 88;XS:S8%XX%tXtS%X;88@%SSS:8SSSSS;;8tS%S@X...  . .  88S %
-S;%t  .. .            .:  .       . .    .      .     .t;8 t
-8t%%     .  .        .  :.   .  .      .   . @%    .  .%X. %
-S t%  .  ..  S8.   ;% .;S: .      :S ..t88.;% 8. .:t8 @% X t
-  :% %@8X@%8SXtX@%t88  X8S;X8X:XS8:8St;888X@X:S:@:@8@S88:8 %
- .;;;;tS8X8X8Xt;:%X8X888S888@@8888@8@XX888@8@S;;t88@8S8St;;:
-   :;:X88888888@8@8%88S8888X888S88@8@88X8@S88X88@8@8@88X%;::
- ;%88tSX:;8:XSSt8;S%X:88@SXSS.8SS%XStt@%S%S@X.: . ..   8%S.t
-S.:t    .             .:   . .      .  .    .    . .  .%8S %
-8;;%   .     .%      . .:8:   . .  .    .  .  ..   .   %8S.t
-S %%    .:. %;8% .:;%8@8.8 .      :% .:St ;;8:8. .: 8 S;8t.t
-  :t.tXXS8 @.88X; @88X888X;8X8;8X8  t;t@88@8@.%;8.88@ 88 X %
-  ;;;;tS@88888;::tX8X@XXS88888888888@XX88@88X%t;t88X8X@%;;;:
+ ::88;XS:%8tSSttS%X%X:@8X%SSt.8%SSXSt%@%SS%S%.  .  %: .8:% %
+S:;t      .           ..     .  .          .      S8 : X%8 t
+8.:%  . .    .    .S8   ;; .     .  .  .S .  %t . S8   @8S %
+S ;%  .:S;8  .S ;;%8@  t8 . .t 8  .t S8S8X.%X @ t8SX :8 8X.t
+  :% XX t8 8SS;S S:88..S: @:.8@ @8. %88 %8@88:SSX8 @8 .888.t
+  ;;;:;SX@8X8X%:tt%SX88X%888X88X8888XX@8X888XSt.;88888@ttt;:
+   ;:;;@88888@88888S88@88@S@88X8@88@888%8@@88@8888@S8@X@t:;:
+ ..88;XS:S8tXS%tXtS%X;88@%SSS:@SS%SXt;8tS%X@X...   .. .8XS %
+S;tt  .. .            ::     .   .  .   .       .   . .%8% t
+8t%%      .  .          :..    .     .      .8S   .    S8X.%
+S t%  .  : . SX.   ;t..;S; .     ..% ..t8X.t% 8. .;:8 8 8t.t
+  :% tX8@X%8%XtX@%;88X S8S;8@@:8S8:8Xt;8888@@:S;@:@8XS88 X t
+ .;;;;tS8X8@8Xt;:%S88888S888888888@8@XX8@@8@XS;;;88@8S8%;;;:
+   ;:;X88888888@8@8%88%8888X@88S88@@@88X8@X8@S88X8S8@8@X%;;:
+ ;%88;SX.:8.XSSt8;%%X:88@SXS%:8SS%XStt@%X%X@S.......   8%S t
+S.:t   .              .:    . .      .        .    .  .S8S %
+8;;%   .     :t       . .8:  .  .  .   . .  .%:   . .  %8S.%
+S %%   . ;. %t8%. :;%888.@.       .t .:%% :%@.8. .: 8 St8t.t
+  :t.tXXSX:8.88X;.888X888%;8@@%8X8  t;t;%888@88:8.88X 88.X %
+  ;;;;tSX88@@X;::tX8@@XS:88888888888@XX8@@888@%;t88X8X@%;;;:
```

#### Image metadata

```diff
@@ -10,10 +10,10 @@
 Interlace mode: None
 Rendering intent: Perceptual
 X resolution: 100
 Y resolution: 100
 Resolution units: PixelsPerInch
 Transparency channel enabled: False
 Gamma: 0.454545
-Number of unique colors: 18576
+Number of unique colors: 18791
 Comment: 
 EXIF data:
```

### Comparing `pyreqwest_impersonate-0.4.4/src/lib.rs` & `pyreqwest_impersonate-0.4.5/src/lib.rs`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-use std::collections::HashMap;
 use std::str::FromStr;
 use std::sync::{Arc, OnceLock};
 use std::time::Duration;
 
+use indexmap::IndexMap;
 use pyo3::exceptions;
 use pyo3::prelude::*;
 use pyo3::types::{PyBool, PyBytes, PyDict, PyString};
 use reqwest_impersonate::header::{HeaderMap, HeaderName, HeaderValue};
 use reqwest_impersonate::impersonate::Impersonate;
 use reqwest_impersonate::multipart;
 use reqwest_impersonate::redirect::Policy;
@@ -51,15 +51,15 @@
 
 #[pyclass]
 /// HTTP client that can impersonate web browsers.
 pub struct Client {
     client: Arc<reqwest_impersonate::Client>,
     auth: Option<(String, Option<String>)>,
     auth_bearer: Option<String>,
-    params: Option<HashMap<String, String>>,
+    params: Option<IndexMap<String, String>>,
 }
 
 #[pymethods]
 impl Client {
     #[new]
     /// Initializes an HTTP client that can impersonate web browsers.
     ///
@@ -105,16 +105,16 @@
     ///     http1=True,
     ///     http2=False,
     /// )
     /// ```
     fn new(
         auth: Option<(String, Option<String>)>,
         auth_bearer: Option<String>,
-        params: Option<HashMap<String, String>>,
-        headers: Option<HashMap<String, String>>,
+        params: Option<IndexMap<String, String>>,
+        headers: Option<IndexMap<String, String>>,
         cookie_store: Option<bool>,
         referer: Option<bool>,
         proxy: Option<&str>,
         timeout: Option<f64>,
         impersonate: Option<&str>,
         follow_redirects: Option<bool>,
         max_redirects: Option<usize>,
@@ -129,17 +129,25 @@
         }
 
         // Client builder
         let mut client_builder = reqwest_impersonate::Client::builder()
             .enable_ech_grease()
             .permute_extensions();
 
+        // Impersonate
+        if let Some(impersonation_type) = impersonate {
+            let impersonation = Impersonate::from_str(impersonation_type).map_err(|_| {
+                PyErr::new::<exceptions::PyValueError, _>("Invalid impersonate param")
+            })?;
+            client_builder = client_builder.impersonate(impersonation);
+        }
+
         // Headers
         if let Some(headers) = headers {
-            let mut headers_new = HeaderMap::new();
+            let mut headers_new = HeaderMap::with_capacity(headers.len());
             for (key, value) in headers {
                 headers_new.insert(
                     HeaderName::from_bytes(key.as_bytes()).map_err(|_| {
                         PyErr::new::<exceptions::PyValueError, _>("Invalid header name")
                     })?,
                     HeaderValue::from_str(&value).map_err(|_| {
                         PyErr::new::<exceptions::PyValueError, _>("Invalid header value")
@@ -167,22 +175,14 @@
         }
 
         // Timeout
         if let Some(seconds) = timeout {
             client_builder = client_builder.timeout(Duration::from_secs_f64(seconds));
         }
 
-        // Impersonate
-        if let Some(impersonation_type) = impersonate {
-            let impersonation = Impersonate::from_str(impersonation_type).map_err(|_| {
-                PyErr::new::<exceptions::PyValueError, _>("Invalid impersonate param")
-            })?;
-            client_builder = client_builder.impersonate(impersonation);
-        }
-
         // Redirects
         let max_redirects = max_redirects.unwrap_or(20); // Default to 20 if not provided
         if follow_redirects.unwrap_or(true) {
             client_builder = client_builder.redirect(Policy::limited(max_redirects));
         } else {
             client_builder = client_builder.redirect(Policy::none());
         }
@@ -243,20 +243,20 @@
     ///
     /// * `PyException` - If there is an error making the request.
     fn request(
         &self,
         py: Python,
         method: &str,
         url: &str,
-        params: Option<HashMap<String, String>>,
-        headers: Option<HashMap<String, String>>,
+        params: Option<IndexMap<String, String>>,
+        headers: Option<IndexMap<String, String>>,
         content: Option<Vec<u8>>,
         data: Option<&Bound<'_, PyDict>>,
         json: Option<&Bound<'_, PyDict>>,
-        files: Option<HashMap<String, String>>,
+        files: Option<IndexMap<String, String>>,
         auth: Option<(String, Option<String>)>,
         auth_bearer: Option<String>,
         timeout: Option<f64>,
     ) -> PyResult<Response> {
         let client = Arc::clone(&self.client);
         let auth = auth.or(self.auth.clone());
         let auth_bearer = auth_bearer.or(self.auth_bearer.clone());
@@ -294,15 +294,15 @@
             // Params
             if let Some(params) = params {
                 request_builder = request_builder.query(&params);
             }
 
             // Headers
             if let Some(headers) = headers {
-                let mut headers_new = HeaderMap::new();
+                let mut headers_new = HeaderMap::with_capacity(headers.len());
                 for (key, value) in headers {
                     headers_new.insert(
                         HeaderName::from_bytes(key.as_bytes()).map_err(|_| {
                             PyErr::new::<exceptions::PyValueError, _>("Invalid header name")
                         })?,
                         HeaderValue::from_str(&value).map_err(|_| {
                             PyErr::new::<exceptions::PyValueError, _>("Invalid header value")
@@ -370,15 +370,15 @@
 
             // Send the request and await the response
             let resp = request_builder.send().await.map_err(|e| {
                 PyErr::new::<exceptions::PyException, _>(format!("Error in request: {}", e))
             })?;
 
             // Response items
-            let cookies: HashMap<String, String> = resp
+            let cookies: IndexMap<String, String> = resp
                 .cookies()
                 .map(|cookie| (cookie.name().to_string(), cookie.value().to_string()))
                 .collect();
             // Encoding from "Content-Type" header or "UTF-8"
             let encoding = resp
                 .headers()
                 .get("Content-Type")
@@ -392,15 +392,15 @@
                             Some(value.to_string())
                         } else {
                             None
                         }
                     })
                 })
                 .unwrap_or("UTF-8".to_string());
-            let headers: HashMap<String, String> = resp
+            let headers: IndexMap<String, String> = resp
                 .headers()
                 .iter()
                 .map(|(k, v)| (k.as_str().to_string(), v.to_str().unwrap_or("").to_string()))
                 .collect();
             let status_code = resp.status().as_u16();
             let url = resp.url().to_string();
             let buf = resp.bytes().await.map_err(|e| {
@@ -446,16 +446,16 @@
         })
     }
 
     fn get(
         &self,
         py: Python,
         url: &str,
-        params: Option<HashMap<String, String>>,
-        headers: Option<HashMap<String, String>>,
+        params: Option<IndexMap<String, String>>,
+        headers: Option<IndexMap<String, String>>,
         auth: Option<(String, Option<String>)>,
         auth_bearer: Option<String>,
         timeout: Option<f64>,
     ) -> PyResult<Response> {
         self.request(
             py,
             "GET",
@@ -471,16 +471,16 @@
             timeout,
         )
     }
     fn head(
         &self,
         py: Python,
         url: &str,
-        params: Option<HashMap<String, String>>,
-        headers: Option<HashMap<String, String>>,
+        params: Option<IndexMap<String, String>>,
+        headers: Option<IndexMap<String, String>>,
         auth: Option<(String, Option<String>)>,
         auth_bearer: Option<String>,
         timeout: Option<f64>,
     ) -> PyResult<Response> {
         self.request(
             py,
             "HEAD",
@@ -496,16 +496,16 @@
             timeout,
         )
     }
     fn options(
         &self,
         py: Python,
         url: &str,
-        params: Option<HashMap<String, String>>,
-        headers: Option<HashMap<String, String>>,
+        params: Option<IndexMap<String, String>>,
+        headers: Option<IndexMap<String, String>>,
         auth: Option<(String, Option<String>)>,
         auth_bearer: Option<String>,
         timeout: Option<f64>,
     ) -> PyResult<Response> {
         self.request(
             py,
             "OPTIONS",
@@ -521,16 +521,16 @@
             timeout,
         )
     }
     fn delete(
         &self,
         py: Python,
         url: &str,
-        params: Option<HashMap<String, String>>,
-        headers: Option<HashMap<String, String>>,
+        params: Option<IndexMap<String, String>>,
+        headers: Option<IndexMap<String, String>>,
         auth: Option<(String, Option<String>)>,
         auth_bearer: Option<String>,
         timeout: Option<f64>,
     ) -> PyResult<Response> {
         self.request(
             py,
             "DELETE",
@@ -547,20 +547,20 @@
         )
     }
 
     fn post(
         &self,
         py: Python,
         url: &str,
-        params: Option<HashMap<String, String>>,
-        headers: Option<HashMap<String, String>>,
+        params: Option<IndexMap<String, String>>,
+        headers: Option<IndexMap<String, String>>,
         content: Option<Vec<u8>>,
         data: Option<&Bound<'_, PyDict>>,
         json: Option<&Bound<'_, PyDict>>,
-        files: Option<HashMap<String, String>>,
+        files: Option<IndexMap<String, String>>,
         auth: Option<(String, Option<String>)>,
         auth_bearer: Option<String>,
         timeout: Option<f64>,
     ) -> PyResult<Response> {
         self.request(
             py,
             "POST",
@@ -576,20 +576,20 @@
             timeout,
         )
     }
     fn put(
         &self,
         py: Python,
         url: &str,
-        params: Option<HashMap<String, String>>,
-        headers: Option<HashMap<String, String>>,
+        params: Option<IndexMap<String, String>>,
+        headers: Option<IndexMap<String, String>>,
         content: Option<Vec<u8>>,
         data: Option<&Bound<'_, PyDict>>,
         json: Option<&Bound<'_, PyDict>>,
-        files: Option<HashMap<String, String>>,
+        files: Option<IndexMap<String, String>>,
         auth: Option<(String, Option<String>)>,
         auth_bearer: Option<String>,
         timeout: Option<f64>,
     ) -> PyResult<Response> {
         self.request(
             py,
             "PUT",
@@ -605,20 +605,20 @@
             timeout,
         )
     }
     fn patch(
         &self,
         py: Python,
         url: &str,
-        params: Option<HashMap<String, String>>,
-        headers: Option<HashMap<String, String>>,
+        params: Option<IndexMap<String, String>>,
+        headers: Option<IndexMap<String, String>>,
         content: Option<Vec<u8>>,
         data: Option<&Bound<'_, PyDict>>,
         json: Option<&Bound<'_, PyDict>>,
-        files: Option<HashMap<String, String>>,
+        files: Option<IndexMap<String, String>>,
         auth: Option<(String, Option<String>)>,
         auth_bearer: Option<String>,
         timeout: Option<f64>,
     ) -> PyResult<Response> {
         self.request(
             py,
             "PATCH",
@@ -638,20 +638,20 @@
 
 /// Convenience functions that use a default Client instance under the hood
 #[pyfunction]
 fn request(
     py: Python,
     method: &str,
     url: &str,
-    params: Option<HashMap<String, String>>,
-    headers: Option<HashMap<String, String>>,
+    params: Option<IndexMap<String, String>>,
+    headers: Option<IndexMap<String, String>>,
     content: Option<Vec<u8>>,
     data: Option<&Bound<'_, PyDict>>,
     json: Option<&Bound<'_, PyDict>>,
-    files: Option<HashMap<String, String>>,
+    files: Option<IndexMap<String, String>>,
     auth: Option<(String, Option<String>)>,
     auth_bearer: Option<String>,
     timeout: Option<f64>,
     impersonate: Option<&str>,
     verify: Option<bool>,
 ) -> PyResult<Response> {
     let client = Client::new(
@@ -686,16 +686,16 @@
     )
 }
 
 #[pyfunction]
 fn get(
     py: Python,
     url: &str,
-    params: Option<HashMap<String, String>>,
-    headers: Option<HashMap<String, String>>,
+    params: Option<IndexMap<String, String>>,
+    headers: Option<IndexMap<String, String>>,
     auth: Option<(String, Option<String>)>,
     auth_bearer: Option<String>,
     timeout: Option<f64>,
     impersonate: Option<&str>,
     verify: Option<bool>,
 ) -> PyResult<Response> {
     let client = Client::new(
@@ -717,16 +717,16 @@
     client.get(py, url, params, headers, auth, auth_bearer, timeout)
 }
 
 #[pyfunction]
 fn head(
     py: Python,
     url: &str,
-    params: Option<HashMap<String, String>>,
-    headers: Option<HashMap<String, String>>,
+    params: Option<IndexMap<String, String>>,
+    headers: Option<IndexMap<String, String>>,
     auth: Option<(String, Option<String>)>,
     auth_bearer: Option<String>,
     timeout: Option<f64>,
     impersonate: Option<&str>,
     verify: Option<bool>,
 ) -> PyResult<Response> {
     let client = Client::new(
@@ -748,16 +748,16 @@
     client.head(py, url, params, headers, auth, auth_bearer, timeout)
 }
 
 #[pyfunction]
 fn options(
     py: Python,
     url: &str,
-    params: Option<HashMap<String, String>>,
-    headers: Option<HashMap<String, String>>,
+    params: Option<IndexMap<String, String>>,
+    headers: Option<IndexMap<String, String>>,
     auth: Option<(String, Option<String>)>,
     auth_bearer: Option<String>,
     timeout: Option<f64>,
     impersonate: Option<&str>,
     verify: Option<bool>,
 ) -> PyResult<Response> {
     let client = Client::new(
@@ -779,16 +779,16 @@
     client.options(py, url, params, headers, auth, auth_bearer, timeout)
 }
 
 #[pyfunction]
 fn delete(
     py: Python,
     url: &str,
-    params: Option<HashMap<String, String>>,
-    headers: Option<HashMap<String, String>>,
+    params: Option<IndexMap<String, String>>,
+    headers: Option<IndexMap<String, String>>,
     auth: Option<(String, Option<String>)>,
     auth_bearer: Option<String>,
     timeout: Option<f64>,
     impersonate: Option<&str>,
     verify: Option<bool>,
 ) -> PyResult<Response> {
     let client = Client::new(
@@ -810,20 +810,20 @@
     client.delete(py, url, params, headers, auth, auth_bearer, timeout)
 }
 
 #[pyfunction]
 fn post(
     py: Python,
     url: &str,
-    params: Option<HashMap<String, String>>,
-    headers: Option<HashMap<String, String>>,
+    params: Option<IndexMap<String, String>>,
+    headers: Option<IndexMap<String, String>>,
     content: Option<Vec<u8>>,
     data: Option<&Bound<'_, PyDict>>,
     json: Option<&Bound<'_, PyDict>>,
-    files: Option<HashMap<String, String>>,
+    files: Option<IndexMap<String, String>>,
     auth: Option<(String, Option<String>)>,
     auth_bearer: Option<String>,
     timeout: Option<f64>,
     impersonate: Option<&str>,
     verify: Option<bool>,
 ) -> PyResult<Response> {
     let client = Client::new(
@@ -857,20 +857,20 @@
     )
 }
 
 #[pyfunction]
 fn put(
     py: Python,
     url: &str,
-    params: Option<HashMap<String, String>>,
-    headers: Option<HashMap<String, String>>,
+    params: Option<IndexMap<String, String>>,
+    headers: Option<IndexMap<String, String>>,
     content: Option<Vec<u8>>,
     data: Option<&Bound<'_, PyDict>>,
     json: Option<&Bound<'_, PyDict>>,
-    files: Option<HashMap<String, String>>,
+    files: Option<IndexMap<String, String>>,
     auth: Option<(String, Option<String>)>,
     auth_bearer: Option<String>,
     timeout: Option<f64>,
     impersonate: Option<&str>,
     verify: Option<bool>,
 ) -> PyResult<Response> {
     let client = Client::new(
@@ -904,20 +904,20 @@
     )
 }
 
 #[pyfunction]
 fn patch(
     py: Python,
     url: &str,
-    params: Option<HashMap<String, String>>,
-    headers: Option<HashMap<String, String>>,
+    params: Option<IndexMap<String, String>>,
+    headers: Option<IndexMap<String, String>>,
     content: Option<Vec<u8>>,
     data: Option<&Bound<'_, PyDict>>,
     json: Option<&Bound<'_, PyDict>>,
-    files: Option<HashMap<String, String>>,
+    files: Option<IndexMap<String, String>>,
     auth: Option<(String, Option<String>)>,
     auth_bearer: Option<String>,
     timeout: Option<f64>,
     impersonate: Option<&str>,
     verify: Option<bool>,
 ) -> PyResult<Response> {
     let client = Client::new(
```

### Comparing `pyreqwest_impersonate-0.4.4/src/response.rs` & `pyreqwest_impersonate-0.4.5/src/response.rs`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.4.4/tests/test_client.py` & `pyreqwest_impersonate-0.4.5/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.4.4/tests/test_defs.py` & `pyreqwest_impersonate-0.4.5/tests/test_defs.py`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.4.4/Cargo.lock` & `pyreqwest_impersonate-0.4.5/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -556,14 +556,15 @@
 name = "indexmap"
 version = "2.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "168fb715dda47215e360912c096649d23d58bf392ac62f73919e831745e40f26"
 dependencies = [
  "equivalent",
  "hashbrown",
+ "serde",
 ]
 
 [[package]]
 name = "indoc"
 version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
@@ -826,14 +827,15 @@
 [[package]]
 name = "pyo3"
 version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a5e00b96a521718e08e03b1a622f01c8a8deb50719335de3f60b3b3950f069d8"
 dependencies = [
  "cfg-if",
+ "indexmap",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "portable-atomic",
  "pyo3-build-config",
  "pyo3-ffi",
@@ -884,17 +886,18 @@
  "pyo3-build-config",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyreqwest_impersonate"
-version = "0.4.4"
+version = "0.4.5"
 dependencies = [
  "encoding_rs",
+ "indexmap",
  "pyo3",
  "pythonize",
  "reqwest-impersonate",
  "serde_json",
  "tokio",
 ]
 
@@ -953,17 +956,17 @@
 name = "regex-syntax"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
 
 [[package]]
 name = "reqwest-impersonate"
-version = "0.11.79"
+version = "0.11.84"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1b3ef1d8a08ef2150db45aae7e85dce08b96747357857fe4537cddd59624dc74"
+checksum = "281893b5f8d18e013d5998df9ac657d2a82402add22253048660516f35ed40d5"
 dependencies = [
  "async-compression",
  "base64",
  "boring-imp",
  "boring-sys-imp",
  "bytes",
  "cookie",
```

### Comparing `pyreqwest_impersonate-0.4.4/pyproject.toml` & `pyreqwest_impersonate-0.4.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.4.4/PKG-INFO` & `pyreqwest_impersonate-0.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyreqwest_impersonate
-Version: 0.4.4
+Version: 0.4.5
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -83,18 +83,18 @@
             in additional requests. Default is True.
         referer (bool, optional): Enable or disable automatic setting of the `Referer` header. Default is True.
         proxy (str, optional): Proxy URL for HTTP requests. Example: "socks5://127.0.0.1:9150". Default is None.
         impersonate (str, optional): Entity to impersonate. Example: "chrome_124". Default is None.
             Chrome: "chrome_99","chrome_100","chrome_101","chrome_104","chrome_105","chrome_106","chrome_108", 
                 "chrome_107","chrome_109","chrome_114","chrome_116","chrome_117","chrome_118","chrome_119", 
                 "chrome_120","chrome_123","chrome_124"
-            Safari: "safari_ios_17.2","safari_15.3","safari_15.5","safari_15.6.1","safari_16","safari_16.5","safari_17.2.1", 
-                "safari_17.4.1"
+            Safari: "safari_ios_16.5","safari_ios_17.2","safari_15.3","safari_15.5","safari_15.6.1","safari_16",
+                "safari_16.5","safari_17.2.1","safari_17.4.1"
             OkHttp: "okhttp_3.9","okhttp_3.11","okhttp_3.13","okhttp_3.14","okhttp_4.9","okhttp_4.10","okhttp_5"
-            Edge: "edge_99","edge_101","edge_120"
+            Edge: "edge_99","edge_101","edge_122"
         follow_redirects (bool, optional): Whether to follow redirects. Default is True.
         max_redirects (int, optional): Maximum redirects to follow. Default 20. Applies if `follow_redirects` is True.
         verify (bool, optional): Verify SSL certificates. Default is True.
         http1 (bool, optional): Use only HTTP/1.1. Default is None.
         http2 (bool, optional): Use only HTTP/2. Default is None.
          
     """
```

