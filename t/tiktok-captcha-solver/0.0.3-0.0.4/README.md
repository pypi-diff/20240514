# Comparing `tmp/tiktok_captcha_solver-0.0.3.tar.gz` & `tmp/tiktok_captcha_solver-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiktok_captcha_solver-0.0.3.tar", last modified: Sat May 11 04:36:02 2024, max compression
+gzip compressed data, was "tiktok_captcha_solver-0.0.4.tar", last modified: Tue May 14 04:00:52 2024, max compression
```

## Comparing `tiktok_captcha_solver-0.0.3.tar` & `tiktok_captcha_solver-0.0.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 gregb     (1000) gregb     (1000)        0 2024-05-11 04:36:02.220627 tiktok_captcha_solver-0.0.3/
--rw-r--r--   0 gregb     (1000) gregb     (1000)     3415 2024-05-11 04:36:02.219627 tiktok_captcha_solver-0.0.3/PKG-INFO
--rw-r--r--   0 gregb     (1000) gregb     (1000)     2411 2024-05-11 04:35:04.000000 tiktok_captcha_solver-0.0.3/README.md
--rw-r--r--   0 gregb     (1000) gregb     (1000)     1087 2024-05-11 04:35:39.000000 tiktok_captcha_solver-0.0.3/pyproject.toml
--rw-r--r--   0 gregb     (1000) gregb     (1000)       38 2024-05-11 04:36:02.220627 tiktok_captcha_solver-0.0.3/setup.cfg
-drwxr-xr-x   0 gregb     (1000) gregb     (1000)        0 2024-05-11 04:36:02.216627 tiktok_captcha_solver-0.0.3/src/
-drwxr-xr-x   0 gregb     (1000) gregb     (1000)        0 2024-05-11 04:36:02.218627 tiktok_captcha_solver-0.0.3/src/tiktok_captcha_solver/
--rw-r--r--   0 gregb     (1000) gregb     (1000)      120 2024-05-11 04:30:20.000000 tiktok_captcha_solver-0.0.3/src/tiktok_captcha_solver/__init__.py
--rw-r--r--   0 gregb     (1000) gregb     (1000)     1895 2024-05-11 04:30:20.000000 tiktok_captcha_solver-0.0.3/src/tiktok_captcha_solver/api.py
--rw-r--r--   0 gregb     (1000) gregb     (1000)      350 2024-05-11 04:30:20.000000 tiktok_captcha_solver-0.0.3/src/tiktok_captcha_solver/downloader.py
--rw-r--r--   0 gregb     (1000) gregb     (1000)      335 2024-05-05 06:12:30.000000 tiktok_captcha_solver-0.0.3/src/tiktok_captcha_solver/models.py
--rw-r--r--   0 gregb     (1000) gregb     (1000)     7911 2024-05-11 04:30:20.000000 tiktok_captcha_solver-0.0.3/src/tiktok_captcha_solver/playwrightsolver.py
--rw-r--r--   0 gregb     (1000) gregb     (1000)     7704 2024-05-11 04:30:20.000000 tiktok_captcha_solver-0.0.3/src/tiktok_captcha_solver/seleniumsolver.py
--rw-r--r--   0 gregb     (1000) gregb     (1000)     1521 2024-05-11 04:30:20.000000 tiktok_captcha_solver-0.0.3/src/tiktok_captcha_solver/solver.py
-drwxr-xr-x   0 gregb     (1000) gregb     (1000)        0 2024-05-11 04:36:02.219627 tiktok_captcha_solver-0.0.3/src/tiktok_captcha_solver/tests/
--rw-r--r--   0 gregb     (1000) gregb     (1000)        0 2024-05-05 16:49:30.000000 tiktok_captcha_solver-0.0.3/src/tiktok_captcha_solver/tests/__init__.py
--rw-r--r--   0 gregb     (1000) gregb     (1000)     1264 2024-05-05 17:22:04.000000 tiktok_captcha_solver-0.0.3/src/tiktok_captcha_solver/tests/test_api.py
--rw-r--r--   0 gregb     (1000) gregb     (1000)      189 2024-05-05 17:34:44.000000 tiktok_captcha_solver-0.0.3/src/tiktok_captcha_solver/tests/test_downloader.py
--rw-r--r--   0 gregb     (1000) gregb     (1000)     1062 2024-05-11 04:35:06.000000 tiktok_captcha_solver-0.0.3/src/tiktok_captcha_solver/tests/test_playwrightsolver.py
--rw-r--r--   0 gregb     (1000) gregb     (1000)     1930 2024-05-11 04:33:34.000000 tiktok_captcha_solver-0.0.3/src/tiktok_captcha_solver/tests/test_seleniumsolver.py
-drwxr-xr-x   0 gregb     (1000) gregb     (1000)        0 2024-05-11 04:36:02.219627 tiktok_captcha_solver-0.0.3/src/tiktok_captcha_solver.egg-info/
--rw-r--r--   0 gregb     (1000) gregb     (1000)     3415 2024-05-11 04:36:02.000000 tiktok_captcha_solver-0.0.3/src/tiktok_captcha_solver.egg-info/PKG-INFO
--rw-r--r--   0 gregb     (1000) gregb     (1000)      792 2024-05-11 04:36:02.000000 tiktok_captcha_solver-0.0.3/src/tiktok_captcha_solver.egg-info/SOURCES.txt
--rw-r--r--   0 gregb     (1000) gregb     (1000)        1 2024-05-11 04:36:02.000000 tiktok_captcha_solver-0.0.3/src/tiktok_captcha_solver.egg-info/dependency_links.txt
--rw-r--r--   0 gregb     (1000) gregb     (1000)      106 2024-05-11 04:36:02.000000 tiktok_captcha_solver-0.0.3/src/tiktok_captcha_solver.egg-info/requires.txt
--rw-r--r--   0 gregb     (1000) gregb     (1000)       22 2024-05-11 04:36:02.000000 tiktok_captcha_solver-0.0.3/src/tiktok_captcha_solver.egg-info/top_level.txt
+drwxr-xr-x   0 gregb     (1000) gregb     (1000)        0 2024-05-14 04:00:52.974847 tiktok_captcha_solver-0.0.4/
+-rw-r--r--   0 gregb     (1000) gregb     (1000)     3533 2024-05-14 04:00:52.974847 tiktok_captcha_solver-0.0.4/PKG-INFO
+-rw-r--r--   0 gregb     (1000) gregb     (1000)     2529 2024-05-14 04:00:19.000000 tiktok_captcha_solver-0.0.4/README.md
+-rw-r--r--   0 gregb     (1000) gregb     (1000)     1087 2024-05-14 04:00:39.000000 tiktok_captcha_solver-0.0.4/pyproject.toml
+-rw-r--r--   0 gregb     (1000) gregb     (1000)       38 2024-05-14 04:00:52.974847 tiktok_captcha_solver-0.0.4/setup.cfg
+drwxr-xr-x   0 gregb     (1000) gregb     (1000)        0 2024-05-14 04:00:52.969847 tiktok_captcha_solver-0.0.4/src/
+drwxr-xr-x   0 gregb     (1000) gregb     (1000)        0 2024-05-14 04:00:52.971847 tiktok_captcha_solver-0.0.4/src/tiktok_captcha_solver/
+-rw-r--r--   0 gregb     (1000) gregb     (1000)      120 2024-05-11 04:30:20.000000 tiktok_captcha_solver-0.0.4/src/tiktok_captcha_solver/__init__.py
+-rw-r--r--   0 gregb     (1000) gregb     (1000)     1895 2024-05-12 21:58:21.000000 tiktok_captcha_solver-0.0.4/src/tiktok_captcha_solver/api.py
+-rw-r--r--   0 gregb     (1000) gregb     (1000)      350 2024-05-11 04:30:20.000000 tiktok_captcha_solver-0.0.4/src/tiktok_captcha_solver/downloader.py
+-rw-r--r--   0 gregb     (1000) gregb     (1000)      335 2024-05-05 06:12:30.000000 tiktok_captcha_solver-0.0.4/src/tiktok_captcha_solver/models.py
+-rw-r--r--   0 gregb     (1000) gregb     (1000)     7982 2024-05-14 03:53:36.000000 tiktok_captcha_solver-0.0.4/src/tiktok_captcha_solver/playwrightsolver.py
+-rw-r--r--   0 gregb     (1000) gregb     (1000)     7865 2024-05-14 03:54:51.000000 tiktok_captcha_solver-0.0.4/src/tiktok_captcha_solver/seleniumsolver.py
+-rw-r--r--   0 gregb     (1000) gregb     (1000)     1688 2024-05-14 03:54:52.000000 tiktok_captcha_solver-0.0.4/src/tiktok_captcha_solver/solver.py
+drwxr-xr-x   0 gregb     (1000) gregb     (1000)        0 2024-05-14 04:00:52.973847 tiktok_captcha_solver-0.0.4/src/tiktok_captcha_solver/tests/
+-rw-r--r--   0 gregb     (1000) gregb     (1000)        0 2024-05-05 16:49:30.000000 tiktok_captcha_solver-0.0.4/src/tiktok_captcha_solver/tests/__init__.py
+-rw-r--r--   0 gregb     (1000) gregb     (1000)     1264 2024-05-05 17:22:04.000000 tiktok_captcha_solver-0.0.4/src/tiktok_captcha_solver/tests/test_api.py
+-rw-r--r--   0 gregb     (1000) gregb     (1000)      189 2024-05-05 17:34:44.000000 tiktok_captcha_solver-0.0.4/src/tiktok_captcha_solver/tests/test_downloader.py
+-rw-r--r--   0 gregb     (1000) gregb     (1000)     1608 2024-05-14 03:57:25.000000 tiktok_captcha_solver-0.0.4/src/tiktok_captcha_solver/tests/test_playwrightsolver.py
+-rw-r--r--   0 gregb     (1000) gregb     (1000)     2356 2024-05-14 03:57:24.000000 tiktok_captcha_solver-0.0.4/src/tiktok_captcha_solver/tests/test_seleniumsolver.py
+drwxr-xr-x   0 gregb     (1000) gregb     (1000)        0 2024-05-14 04:00:52.973847 tiktok_captcha_solver-0.0.4/src/tiktok_captcha_solver.egg-info/
+-rw-r--r--   0 gregb     (1000) gregb     (1000)     3533 2024-05-14 04:00:52.000000 tiktok_captcha_solver-0.0.4/src/tiktok_captcha_solver.egg-info/PKG-INFO
+-rw-r--r--   0 gregb     (1000) gregb     (1000)      792 2024-05-14 04:00:52.000000 tiktok_captcha_solver-0.0.4/src/tiktok_captcha_solver.egg-info/SOURCES.txt
+-rw-r--r--   0 gregb     (1000) gregb     (1000)        1 2024-05-14 04:00:52.000000 tiktok_captcha_solver-0.0.4/src/tiktok_captcha_solver.egg-info/dependency_links.txt
+-rw-r--r--   0 gregb     (1000) gregb     (1000)      106 2024-05-14 04:00:52.000000 tiktok_captcha_solver-0.0.4/src/tiktok_captcha_solver.egg-info/requires.txt
+-rw-r--r--   0 gregb     (1000) gregb     (1000)       22 2024-05-14 04:00:52.000000 tiktok_captcha_solver-0.0.4/src/tiktok_captcha_solver.egg-info/top_level.txt
```

### Comparing `tiktok_captcha_solver-0.0.3/PKG-INFO` & `tiktok_captcha_solver-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiktok-captcha-solver
-Version: 0.0.3
+Version: 0.0.4
 Summary: This package integrates with Selenium or Playwright to solve any TikTok captcha in one line of code.
 Author-email: Toughdata LLC <greg@toughdata.net>
 Project-URL: Homepage, https://www.sadcaptcha.com
 Project-URL: Source, https://github.com/gbiz123/tiktok-captcha-solver/
 Keywords: tiktok,captcha,solver,selenium,rotate,puzzle,3d
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -28,26 +28,27 @@
 The purpose is to make integrating SadCaptcha into your Selenium or Playwright app as simple as one line of code.
 
 
 Instructions for integrating with Selenium and Playwright are described below in their respective sections.
 
 ## Requirements
 - Python >= 3.10
-- Selenium properly installed and in `PATH`
+- **If using Selenium** - Selenium properly installed and in `PATH`
+- **If using Playwright** - Playwright must be properly installed with `playwright install`
 
 ## Installation
 This project can be installed with `pip`. Just run the following command:
 ```
 pip install tiktok-captcha-solver
 ```
 
 ## Selenium Client 
 Import the package, set up the SadCaptcha class, and call it whenever you need.
 This turns the entire captcha detection, solution, retry, and verification process into a single line of code.
-It is the recommended method if you are using Selenium.
+It is the recommended method if you are using Playwright.
 
 ```py
 from tiktok_captcha_solver import SeleniumSolver
 import undetected_chromedriver as uc
 
 driver = uc.Chrome(headless=False)
 api_key = "YOUR_API_KEY_HERE"
@@ -73,21 +74,21 @@
 
 with sync_playwright() as p:
     browser = p.chromium.launch(headless=False)
     page = browser.new_page()
     
     # Playwright code that causes a TikTok captcha...
 
-    sadcaptcha = PlaywrightSolver(page, os.environ["API_KEY"])
+    sadcaptcha = PlaywrightSolver(page, api_key)
     sadcaptcha.solve_captcha_if_present()
 ```
 That's it!
 
 ## API Client
-If you are not using Selenium, you can still import and use the API client to help you make calls to SadCaptcha
+If you are not using Selenium or Playwright, you can still import and use the API client to help you make calls to SadCaptcha
 ```py
 from tiktok_captcha_solver import ApiClient
 
 api_key = "YOUR_API_KEY_HERE"
 client = ApiClient(api_key)
 
 # Rotate
```

### Comparing `tiktok_captcha_solver-0.0.3/README.md` & `tiktok_captcha_solver-0.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,26 +3,27 @@
 The purpose is to make integrating SadCaptcha into your Selenium or Playwright app as simple as one line of code.
 
 
 Instructions for integrating with Selenium and Playwright are described below in their respective sections.
 
 ## Requirements
 - Python >= 3.10
-- Selenium properly installed and in `PATH`
+- **If using Selenium** - Selenium properly installed and in `PATH`
+- **If using Playwright** - Playwright must be properly installed with `playwright install`
 
 ## Installation
 This project can be installed with `pip`. Just run the following command:
 ```
 pip install tiktok-captcha-solver
 ```
 
 ## Selenium Client 
 Import the package, set up the SadCaptcha class, and call it whenever you need.
 This turns the entire captcha detection, solution, retry, and verification process into a single line of code.
-It is the recommended method if you are using Selenium.
+It is the recommended method if you are using Playwright.
 
 ```py
 from tiktok_captcha_solver import SeleniumSolver
 import undetected_chromedriver as uc
 
 driver = uc.Chrome(headless=False)
 api_key = "YOUR_API_KEY_HERE"
@@ -48,21 +49,21 @@
 
 with sync_playwright() as p:
     browser = p.chromium.launch(headless=False)
     page = browser.new_page()
     
     # Playwright code that causes a TikTok captcha...
 
-    sadcaptcha = PlaywrightSolver(page, os.environ["API_KEY"])
+    sadcaptcha = PlaywrightSolver(page, api_key)
     sadcaptcha.solve_captcha_if_present()
 ```
 That's it!
 
 ## API Client
-If you are not using Selenium, you can still import and use the API client to help you make calls to SadCaptcha
+If you are not using Selenium or Playwright, you can still import and use the API client to help you make calls to SadCaptcha
 ```py
 from tiktok_captcha_solver import ApiClient
 
 api_key = "YOUR_API_KEY_HERE"
 client = ApiClient(api_key)
 
 # Rotate
```

### Comparing `tiktok_captcha_solver-0.0.3/pyproject.toml` & `tiktok_captcha_solver-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"  # If not defined, then legacy behavior can happen.
 
 [project]
 name = "tiktok-captcha-solver"
-version = "0.0.3"
+version = "0.0.4"
 
 description = "This package integrates with Selenium or Playwright to solve any TikTok captcha in one line of code."
 readme = "README.md"
 requires-python = ">=3.10"
 
 keywords = ["tiktok", "captcha", "solver", "selenium", "rotate", "puzzle", "3d"]
```

### Comparing `tiktok_captcha_solver-0.0.3/src/tiktok_captcha_solver/api.py` & `tiktok_captcha_solver-0.0.4/src/tiktok_captcha_solver/api.py`

 * *Files identical despite different names*

### Comparing `tiktok_captcha_solver-0.0.3/src/tiktok_captcha_solver/playwrightsolver.py` & `tiktok_captcha_solver-0.0.4/src/tiktok_captcha_solver/playwrightsolver.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,18 @@
 
     def __init__(self, page: Page, sadcaptcha_api_key: str) -> None:
         self.page = page
         self.client = ApiClient(sadcaptcha_api_key)
 
     def captcha_is_present(self, timeout: int = 15) -> bool:
         for _ in range(timeout):
-            if len(self.page.locator("div#captcha_container").all()) > 0:
-                logging.debug("Detected captcha")
-                return True
+            for wrapper in self.captcha_wrappers:
+                if len(self.page.locator(wrapper).all()) > 0:
+                    logging.debug("Detected captcha with wrapper: " + wrapper)
+                    return True
             time.sleep(1)
         logging.debug("Did not detect captcha")
         return False
 
     def identify_captcha(self) -> Literal["puzzle", "shapes", "rotate"]:
         rotate_selector = "[data-testid=whirl-inner-img]"
         puzzle_selector = "img.captcha_verify_img_slide"
```

### Comparing `tiktok_captcha_solver-0.0.3/src/tiktok_captcha_solver/seleniumsolver.py` & `tiktok_captcha_solver-0.0.4/src/tiktok_captcha_solver/seleniumsolver.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,17 +21,20 @@
 
     def __init__(self, chromedriver: Chrome, sadcaptcha_api_key: str) -> None:
         self.chromedriver = chromedriver
         self.client = ApiClient(sadcaptcha_api_key)
 
     def captcha_is_present(self, timeout: int = 15) -> bool:
         for _ in range(timeout):
-            if len(self.chromedriver.find_elements(By.CSS_SELECTOR, "div#captcha_container")) > 0:
-                return True
+            for wrapper in self.captcha_wrappers:
+                if len(self.chromedriver.find_elements(By.CSS_SELECTOR, wrapper)) > 0:
+                    logging.debug("Found captcha with wrapper: " + wrapper)
+                    return True
             time.sleep(1)
+        logging.debug("Captcha not found")
         return False
 
     def identify_captcha(self) -> Literal["puzzle", "shapes", "rotate"]:
         rotate_selector = "[data-testid=whirl-inner-img]"
         puzzle_selector = "img.captcha_verify_img_slide"
         shapes_selector = "#verify-points"
         for _ in range(15):
```

### Comparing `tiktok_captcha_solver-0.0.3/src/tiktok_captcha_solver/solver.py` & `tiktok_captcha_solver-0.0.4/src/tiktok_captcha_solver/solver.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,21 @@
 from abc import ABC, abstractmethod
 from typing import Literal
 
 from undetected_chromedriver import logging
 
 class Solver(ABC):
 
+    @property
+    def captcha_wrappers(self) -> list[str]:
+        return [
+            "div#captcha_container",
+            "div.captcha_verify_container"
+        ]
+
     def solve_captcha_if_present(self, captcha_detect_timeout: int = 15, retries: int = 3) -> None:
         """Solves any captcha that is present, if one is detected
 
         Args:
             captcha_detect_timeout: return if no captcha is detected in this many seconds
             retries: number of times to retry captcha
         """
```

### Comparing `tiktok_captcha_solver-0.0.3/src/tiktok_captcha_solver/tests/test_api.py` & `tiktok_captcha_solver-0.0.4/src/tiktok_captcha_solver/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `tiktok_captcha_solver-0.0.3/src/tiktok_captcha_solver/tests/test_playwrightsolver.py` & `tiktok_captcha_solver-0.0.4/src/tiktok_captcha_solver/tests/test_playwrightsolver.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,15 +16,29 @@
     time.sleep(2);
     write_password = page.locator('xpath=//input[contains(@type,"password")]')
     write_password.type(os.environ["TIKTOK_PASSWORD"]);
     time.sleep(2)
     login_btn = page.locator('//button[contains(@data-e2e,"login-button")]').click();
     time.sleep(8)
 
-def test_solve_captcha(caplog):
+def open_tiktok_search(page: Page) -> None:
+    search_query = "davidteather"
+    page.goto(f"https://www.tiktok.com/search/user?q={search_query}&t=1715558822399")
+
+def test_solve_captcha_at_login(caplog):
     caplog.set_level(logging.DEBUG)
     with sync_playwright() as p:
         browser = p.chromium.launch(headless=False)
         page = browser.new_page()
+        stealth_sync(page)
         open_tiktkok_login(page)
         sadcaptcha = PlaywrightSolver(page, os.environ["API_KEY"])
         sadcaptcha.solve_captcha_if_present()
+
+def test_solve_captcha_at_search(caplog):
+    caplog.set_level(logging.DEBUG)
+    with sync_playwright() as p:
+        browser = p.chromium.launch(headless=False)
+        page = browser.new_page()
+        open_tiktok_search(page) 
+        sadcaptcha = PlaywrightSolver(page, os.environ["API_KEY"])
+        sadcaptcha.solve_captcha_if_present()
```

### Comparing `tiktok_captcha_solver-0.0.3/src/tiktok_captcha_solver/tests/test_seleniumsolver.py` & `tiktok_captcha_solver-0.0.4/src/tiktok_captcha_solver/tests/test_seleniumsolver.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,13 +37,24 @@
     time.sleep(2);
     write_password = driver.find_element(By.XPATH, '//input[contains(@type,"password")]');
     write_password.send_keys(os.environ["TIKTOK_PASSWORD"]);
     time.sleep(2)
     login_btn = driver.find_element(By.XPATH, '//button[contains(@data-e2e,"login-button")]').click();
     time.sleep(8)
 
-def test_solve_captcha(caplog):
+def open_tiktkok_search(driver: uc.Chrome) -> None:
+    search_query = "davidteather"
+    driver.get(f"https://www.tiktok.com/search/user?q={search_query}&t=1715558822399")
+
+def test_solve_captcha_at_login(caplog):
     caplog.set_level(logging.DEBUG)
     driver = make_driver()
     open_tiktkok_login(driver)
     sadcaptcha = SeleniumSolver(driver, os.environ["API_KEY"])
     sadcaptcha.solve_captcha_if_present()
+
+def test_solve_captcha_at_search(caplog):
+    caplog.set_level(logging.DEBUG)
+    driver = make_driver()
+    open_tiktkok_search(driver)
+    sadcaptcha = SeleniumSolver(driver, os.environ["API_KEY"])
+    sadcaptcha.solve_captcha_if_present()
```

### Comparing `tiktok_captcha_solver-0.0.3/src/tiktok_captcha_solver.egg-info/PKG-INFO` & `tiktok_captcha_solver-0.0.4/src/tiktok_captcha_solver.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiktok-captcha-solver
-Version: 0.0.3
+Version: 0.0.4
 Summary: This package integrates with Selenium or Playwright to solve any TikTok captcha in one line of code.
 Author-email: Toughdata LLC <greg@toughdata.net>
 Project-URL: Homepage, https://www.sadcaptcha.com
 Project-URL: Source, https://github.com/gbiz123/tiktok-captcha-solver/
 Keywords: tiktok,captcha,solver,selenium,rotate,puzzle,3d
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -28,26 +28,27 @@
 The purpose is to make integrating SadCaptcha into your Selenium or Playwright app as simple as one line of code.
 
 
 Instructions for integrating with Selenium and Playwright are described below in their respective sections.
 
 ## Requirements
 - Python >= 3.10
-- Selenium properly installed and in `PATH`
+- **If using Selenium** - Selenium properly installed and in `PATH`
+- **If using Playwright** - Playwright must be properly installed with `playwright install`
 
 ## Installation
 This project can be installed with `pip`. Just run the following command:
 ```
 pip install tiktok-captcha-solver
 ```
 
 ## Selenium Client 
 Import the package, set up the SadCaptcha class, and call it whenever you need.
 This turns the entire captcha detection, solution, retry, and verification process into a single line of code.
-It is the recommended method if you are using Selenium.
+It is the recommended method if you are using Playwright.
 
 ```py
 from tiktok_captcha_solver import SeleniumSolver
 import undetected_chromedriver as uc
 
 driver = uc.Chrome(headless=False)
 api_key = "YOUR_API_KEY_HERE"
@@ -73,21 +74,21 @@
 
 with sync_playwright() as p:
     browser = p.chromium.launch(headless=False)
     page = browser.new_page()
     
     # Playwright code that causes a TikTok captcha...
 
-    sadcaptcha = PlaywrightSolver(page, os.environ["API_KEY"])
+    sadcaptcha = PlaywrightSolver(page, api_key)
     sadcaptcha.solve_captcha_if_present()
 ```
 That's it!
 
 ## API Client
-If you are not using Selenium, you can still import and use the API client to help you make calls to SadCaptcha
+If you are not using Selenium or Playwright, you can still import and use the API client to help you make calls to SadCaptcha
 ```py
 from tiktok_captcha_solver import ApiClient
 
 api_key = "YOUR_API_KEY_HERE"
 client = ApiClient(api_key)
 
 # Rotate
```

### Comparing `tiktok_captcha_solver-0.0.3/src/tiktok_captcha_solver.egg-info/SOURCES.txt` & `tiktok_captcha_solver-0.0.4/src/tiktok_captcha_solver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

