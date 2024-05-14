# Comparing `tmp/friendly_captcha_client-0.0.2.tar.gz` & `tmp/friendly_captcha_client-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "friendly_captcha_client-0.0.2.tar", max compression
+gzip compressed data, was "friendly_captcha_client-0.0.3.tar", max compression
```

## Comparing `friendly_captcha_client-0.0.2.tar` & `friendly_captcha_client-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1073 2024-01-17 16:23:35.069927 friendly_captcha_client-0.0.2/LICENSE
--rw-r--r--   0        0        0     2594 2024-01-17 16:23:35.070191 friendly_captcha_client-0.0.2/README.md
--rw-r--r--   0        0        0        0 2024-01-17 16:23:35.071096 friendly_captcha_client-0.0.2/friendly_captcha_client/__init__.py
--rw-r--r--   0        0        0     9868 2024-01-24 10:49:42.489792 friendly_captcha_client-0.0.2/friendly_captcha_client/client.py
--rw-r--r--   0        0        0      738 2024-01-24 16:00:21.925615 friendly_captcha_client-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3474 1970-01-01 00:00:00.000000 friendly_captcha_client-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-14 08:34:25.255338 friendly_captcha_client-0.0.3/LICENSE
+-rw-r--r--   0        0        0     3861 2024-05-14 08:34:25.255338 friendly_captcha_client-0.0.3/README.md
+-rw-r--r--   0        0        0        0 2024-05-14 08:34:25.255338 friendly_captcha_client-0.0.3/friendly_captcha_client/__init__.py
+-rw-r--r--   0        0        0     9868 2024-05-14 08:34:25.255338 friendly_captcha_client-0.0.3/friendly_captcha_client/client.py
+-rw-r--r--   0        0        0      670 2024-05-14 08:34:25.255338 friendly_captcha_client-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4741 1970-01-01 00:00:00.000000 friendly_captcha_client-0.0.3/PKG-INFO
```

### Comparing `friendly_captcha_client-0.0.2/LICENSE` & `friendly_captcha_client-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `friendly_captcha_client-0.0.2/README.md` & `friendly_captcha_client-0.0.3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,77 +1,107 @@
-# Friendly Captcha SDK
-A Python client for the Friendly Captcha service. This client allows for easy integration and verification of captcha responses with the Friendly Captcha API.
+# Friendly Captcha Python SDK
+
+A Python client for the [Friendly Captcha](https://friendlycaptcha.com) service. This client allows for easy integration and verification of captcha responses with the Friendly Captcha API.
+
+> This library is for [Friendly Captcha V2](https://developer.friendlycaptcha.com) only. If you are looking for V1, look [here](https://docs.friendlycaptcha.com)
+
+## Installation
 
-# Installation
 ```bash
 pip install friendly-captcha-client
 ```
 
-# Usage
+## Usage
+
+Below are some basic examples of how to use the client.
+
+For a more detailed example, take a look at the [example](./example) directory.
+
 ### Initialization
+
 To start using the client:
-```
+
+```python
 from friendly_client import FriendlyCaptchaClient
+
 client = FriendlyCaptchaClient(
-    api_key="YOUR_API_KEY", 
+    api_key="YOUR_API_KEY",
     sitekey="YOUR_SITEKEY"
-    )
+)
 ```
 
 ### Verifying a Captcha Response
-- To verify a captcha response:
-```
-result: FriendlyCaptchaResult = client.verify_captcha_response("CAPTCHA_RESPONSE_HERE")
-print(result.should_accept) # True
+
+After calling `verify_captcha_response` with the captcha response there are two functions on the result object that you should check:
+
+- `was_able_to_verify` indicates whether we were able to verify the captcha response. This will be `False` in case there was an issue with the network/our service or if there was a mistake in the configuration.
+- `should_accept` indicates whether the captcha response was correct. If the client is running in non-strict mode (default) and `was_able_to_verify` returned `False`, this will be `True`.
+
+Below are some examples of this behaviour.
+
+#### Verifying a correct captcha response without issues when veryfing:
+
+```python
+result = client.verify_captcha_response("CORRECT?CAPTCHA_RESPONSE_HERE")
 print(result.was_able_to_verify) # True
+print(result.should_accept) # True
 ```
 
-- Verify with bad configuration in non-strict (default) mode
-```
-client.set_siteverify_endpoint("https://incorrect.endpoint.com")
-result: FriendlyCaptchaResult = client.verify_captcha_response("CAPTCHA_RESPONSE_HERE")
-print(result.should_accept)  # True
-print(result.was_able_to_verify)  # False
+#### Verifying an incorrect captcha response without issues when veryfing:
+
+```python
+result = client.verify_captcha_response("INCORRECT_CAPTCHA_RESPONSE_HERE")
+print(result.was_able_to_verify) # True
+print(result.should_accept) # False
 ```
 
-- Verify with bad configuration in strict (default) mode
+#### Verifying an incorrect captcha response with issues (network issues or bad configuration) when veryfing in non-strict mode (default):
+
+```python
+result = client.verify_captcha_response("INCORRECT_CAPTCHA_RESPONSE_HERE")
+print(result.was_able_to_verify) # False
+print(result.should_accept) # True
 ```
+
+#### Verifying an incorrect captcha response with issues (network/service issues or bad configuration) when veryfing in strict mode:
+
+```python
 client.strict = True
-client.set_siteverify_endpoint("https://incorrect.endpoint.com")
-result: FriendlyCaptchaResult = client.verify_captcha_response("CAPTCHA_RESPONSE_HERE")
+result = client.verify_captcha_response("INCORRECT_CAPTCHA_RESPONSE_HERE")
 print(result.should_accept)  # False
 print(result.was_able_to_verify)  # False
 ```
 
-
-
 ### Configuration
+
 The client offers several configuration options:
 
 - **api_key**: Your Friendly Captcha API key.
-- **sitekey**: Your Friendly Captcha site key.
-- **strict**: (Optional) In case the client was not able to verify the captcha response at all, for example if there is a network failure or a mistake in configuration, by default the `verify_captcha_response` returns True regardless. By passing `strict=true`, it will be false instead: every response needs to be strictly verified.
-- **siteverify_endpoint**: (Optional) The endpoint URL for the site verification API.
-- **verbose**: (Optional) Default is False. Turn on basic logging. 
+- **sitekey**: Your Friendly Captcha sitekey.
+- **strict**: (Optional) In case the client was not able to verify the captcha response at all (for example if there is a network failure or a mistake in configuration), by default the `verify_captcha_response` returns `True` regardless. By passing `strict=True`, it will return `False` instead: every response needs to be strictly verified.
+- **siteverify_endpoint**: (Optional) The endpoint URL for the site verification API. Shorthands `eu` or `global` are also accepted. Default is `global`.
+- **verbose**: (Optional) Default is False. Turn on basic logging.
 - Error Handling: The client has built-in error handling mechanisms. In case of unexpected responses or errors from the Friendly Captcha API, the client will log the error and provide a default response.
 
-### Development  
+## Development
+
 To install it locally:
+
 ```bash
 pip install -e .
-pip install requests_mock
+pip install -r requirements-dev.txt
 ```
 
 Run the tests:
+
 ```bash
 # Run the unit tests
 python -m pytest
 
 # Run the SDK integration tests (requires that you have the SDK test mock server running)
+docker run -p 1090:1090 friendlycaptcha/sdk-testserver:latest
 python -m pytest integration_tests
 ```
 
+## License
 
-## Contributing
-Contributions are welcome! If you'd like to contribute to this project, please submit a pull request with your changes.
-
-
+Open source under [MIT](./LICENSE).
```

### Comparing `friendly_captcha_client-0.0.2/friendly_captcha_client/client.py` & `friendly_captcha_client-0.0.3/friendly_captcha_client/client.py`

 * *Files identical despite different names*

### Comparing `friendly_captcha_client-0.0.2/pyproject.toml` & `friendly_captcha_client-0.0.3/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "friendly-captcha-client"
-version = "0.0.2"
+version = "0.0.3"
 description = "A client for Friendly Captcha."
 authors = [
     "Antal Nagy <dev@friendlycaptcha.com>",
     "Friendly Captcha GmbH <dev@friendlycaptcha.com>"
 ]
 readme = "README.md"
 homepage = "https://developer.friendlycaptcha.com/"
@@ -19,13 +19,7 @@
 python = "^3.6"
 requests = "2.31.0"
 pydantic = "2.1.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "7.4.0"
 requests-mock = "1.11.0"
-
-[build]
-exclude = [
-    "examples/*",
-    "integration_tests/*",
-]
```

