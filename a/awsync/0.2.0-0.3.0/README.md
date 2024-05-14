# Comparing `tmp/awsync-0.2.0.tar.gz` & `tmp/awsync-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awsync-0.2.0.tar", max compression
+gzip compressed data, was "awsync-0.3.0.tar", max compression
```

## Comparing `awsync-0.2.0.tar` & `awsync-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11357 2024-05-01 04:32:50.769212 awsync-0.2.0/LICENSE
--rw-r--r--   0        0        0     2118 2024-05-07 05:46:47.639367 awsync-0.2.0/README.md
--rw-r--r--   0        0        0        0 2024-05-01 04:07:11.855130 awsync-0.2.0/awsync/__init__.py
--rw-r--r--   0        0        0      677 2024-05-07 05:46:54.896367 awsync-0.2.0/awsync/__main__.py
--rw-r--r--   0        0        0     7326 2024-05-07 05:14:49.519264 awsync-0.2.0/awsync/client.py
--rw-r--r--   0        0        0        0 2024-05-01 04:07:11.852130 awsync-0.2.0/awsync/models/__init__.py
--rw-r--r--   0        0        0     2573 2024-05-07 05:32:14.863320 awsync-0.2.0/awsync/models/aws.py
--rw-r--r--   0        0        0     1433 2024-05-01 19:56:43.825054 awsync-0.2.0/awsync/models/http.py
--rw-r--r--   0        0        0      283 2024-05-01 19:56:06.559052 awsync-0.2.0/awsync/models/strenum.py
--rw-r--r--   0        0        0        0 2024-05-01 20:49:43.288001 awsync-0.2.0/awsync/py.typed
--rw-r--r--   0        0        0     9350 2024-05-07 05:35:13.709330 awsync-0.2.0/awsync/request.py
--rw-r--r--   0        0        0     1071 2024-05-07 05:30:02.627313 awsync-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3088 1970-01-01 00:00:00.000000 awsync-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-01 04:32:50.769212 awsync-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2082 2024-05-14 01:49:11.328354 awsync-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-01 04:07:11.855130 awsync-0.3.0/awsync/__init__.py
+-rw-r--r--   0        0        0      592 2024-05-14 05:43:47.995003 awsync-0.3.0/awsync/__main__.py
+-rw-r--r--   0        0        0     6934 2024-05-14 05:28:33.978012 awsync-0.3.0/awsync/client.py
+-rw-r--r--   0        0        0        0 2024-05-01 04:07:11.852130 awsync-0.3.0/awsync/models/__init__.py
+-rw-r--r--   0        0        0     3062 2024-05-10 03:09:12.698260 awsync-0.3.0/awsync/models/aws.py
+-rw-r--r--   0        0        0     1433 2024-05-01 19:56:43.825054 awsync-0.3.0/awsync/models/http.py
+-rw-r--r--   0        0        0      282 2024-05-10 04:58:06.020609 awsync-0.3.0/awsync/models/strenum.py
+-rw-r--r--   0        0        0        0 2024-05-01 20:49:43.288001 awsync-0.3.0/awsync/py.typed
+-rw-r--r--   0        0        0     9350 2024-05-07 05:35:13.709330 awsync-0.3.0/awsync/request.py
+-rw-r--r--   0        0        0     1376 2024-05-14 05:50:54.263025 awsync-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3052 1970-01-01 00:00:00.000000 awsync-0.3.0/PKG-INFO
```

### Comparing `awsync-0.2.0/LICENSE` & `awsync-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `awsync-0.2.0/README.md` & `awsync-0.3.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -8,34 +8,32 @@
 Only a few API methods currently implemented for testing and development.
 
 ## Usage
 
 ```python
 "Module main."
 from asyncio import run
-from datetime import datetime, UTC
 from httpx import AsyncClient
 
 from awsync.client import Client
 from awsync.models.aws import Region, Credentials
 
 
 async def main() -> int:
     "Main function."
     async with AsyncClient() as httpx_client:
         client = Client(
             credentials=Credentials.from_environment(),
             httpx_client=httpx_client,
-            utcnow=lambda: datetime.now(UTC),
         )
         response = await client.list_stack_resources(
             region=Region.us_east_1, stack_name="Example-Stack-Name"
         )
         print(response)
-        return 0
+    return 0
 
 
 if __name__ == "__main__":
     run(main())
 ```
 
 ## Local Developer Setup
@@ -61,16 +59,14 @@
 - `make pr` runs all pull request pre-checks below.
 - `make format` runs code formatter.
 - `make lint` checks code linting.
 - `make test` runs tests.
 
 ## Repository TODO:
 
-- Logging
-- Test Coverage
+- Code generation [from JSON](https://github.com/boto/botocore/tree/develop/botocore/data)
 - Automatic Publish CICD
 - Documentation with [mkDocs](https://squidfunk.github.io/mkdocs-material/)
-- Issue template
-- Repository Template variables?
 - Test Makefile replacements
+  - [mise](https://mise.jdx.dev/)
   - [Poetry run](https://python-poetry.org/docs/cli/#run)
   - [doit](https://pydoit.org/)
```

### Comparing `awsync-0.2.0/awsync/__main__.py` & `awsync-0.3.0/awsync/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 "Module main."
 from asyncio import run
-from datetime import datetime, UTC
 from httpx import AsyncClient
 
 from awsync.client import Client
 from awsync.models.aws import Region, Credentials
 
 
 async def main() -> int:
     "Main function."
     async with AsyncClient() as httpx_client:
         client = Client(
             credentials=Credentials.from_environment(),
             httpx_client=httpx_client,
-            utcnow=lambda: datetime.now(UTC),
         )
         response = await client.list_stack_resources(
             region=Region.us_east_1, stack_name="Example-Stack-Name"
         )
         print(response)
-        return 0
+    return 0
 
 
 if __name__ == "__main__":
     run(main())
```

### Comparing `awsync-0.2.0/awsync/client.py` & `awsync-0.3.0/awsync/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 "Middle level abstraction async AWS client for API requests."
 import asyncio
 from dataclasses import dataclass
-from datetime import datetime
+import datetime
 import json
 from typing import Any, Callable, Dict, List, Optional
+import logging
 
 from httpx import AsyncClient
 
 from awsync.models.aws import Credentials, Region
 from awsync.models.http import Method
 from awsync.request import Request
 
@@ -28,95 +29,78 @@
 class StatusError(Exception):
     "API responded with a non-2XX status code."
 
 
 async def request_with_retry(
     client: AsyncClient,
     request: Request,
+    logger: logging.Logger,
     retries: int = 3,
 ) -> Response:
     """
     Make an async HTTP request with retries and exponential backoff.
     Will only retry if request fails due to throttling or a server error.
     """
-    attempt = 0
+    logger.debug(f"Sending request to AWS API: '{request}'")
+    attempt = 1
     client_response = await client.request(
         method=request.method,
         url=request.get_url(),
         headers=request.headers,
         params=request.query,
         json=request.body,
     )
+
+    # Retry if remote error or throttling with exponential backoff
     while client_response.status_code >= 500 or (
         client_response.status_code == 400 and "Throttling" in client_response.text
     ):
         # Base case
         if attempt > retries:
             raise MaxRetriesException(
-                f"Maximum number of retries '{retries}' exceeded.\n"
-                f"Response: {client_response}"
+                f"Maximum number of retries '{retries}' exceeded. "
+                f"Response: '{client_response}'"
             )
-        # Retry if remote error or throttling - exponential backoff
         await asyncio.sleep(2**attempt)
+        logger.warn(f"Attempting retry '{attempt}' of '{retries}'...")
         client_response = await client.request(
             method=request.method,
             url=request.get_url(),
             headers=request.headers,
             params=request.query,
             json=request.body,
         )
         attempt += 1
+
     response = Response(status=client_response.status_code, text=client_response.text)
+    logger.debug(f"Recieved response: '{response}'")
     if response.status < 200 or response.status >= 300:
-        raise StatusError(f"Recieved non-2XX response code.\n" f"Response: {response}")
+        raise StatusError(
+            f"Recieved non-2XX response code from AWS API. " f"Response: '{response}'"
+        )
     return response
 
 
+def utcnow() -> datetime.datetime:
+    "A zero argument callable function that returns the current datetime in UTC."
+    return datetime.datetime.now(datetime.UTC)
+
+
 @dataclass(frozen=True)
 class Client:
     "An AWS API client."
     credentials: Credentials
     "AWS credentials."
     httpx_client: AsyncClient
     "The httpx AsyncClient to use for async reqeusts."
-    utcnow: Callable[[], datetime]
+    logger: logging.Logger = logging.getLogger(__name__)
+    "The logger to use for logging, can be set to control log level and format."
+    utcnow: Callable[[], datetime.datetime] = utcnow
     "A zero argument callable function that returns the current datetime in UTC."
 
-    async def assume_role(
-        self,
-        role_arn: str,
-    ) -> Dict[str, Any]:
-        "Get AWS Role credentials with STS AssumeRole."
-        service = "sts"
-        region = Region.us_east_1
-        request = Request(
-            credentials=self.credentials,
-            method=Method.POST,
-            host=f"{service}.amazonaws.com",
-            body={
-                "Action": "AssumeRole",
-                "RoleArn": role_arn,
-                "RoleSessionName": "AsyncSession",
-                "Version": "2011-06-15",
-            },
-            headers={
-                "Accept": "application/json",
-                "Content-Type": "application/x-www-form-urlencoded; charset=utf-8",
-            },
-        )
-        signed_request = request.sign(
-            utc_now=self.utcnow(), service=service, region=region
-        )
-        response = await request_with_retry(
-            self.httpx_client,
-            request=signed_request,
-        )
-        json_response: Dict[str, Any] = json.loads(response.text)
-        return json_response
-
     async def list_stack_resources(
         self,
         region: Region,
         stack_name: str,
         next_token: Optional[str] = None,
     ) -> List[Dict[str, Any]]:
         "List all resources in a CloudFormation stack asynchronously."
@@ -142,14 +126,15 @@
 
         signed_request = request.sign(
             utc_now=self.utcnow(), service=service, region=region
         )
         response = await request_with_retry(
             self.httpx_client,
             request=signed_request,
+            logger=self.logger,
         )
 
         json_response = json.loads(response.text)
         result = json_response["ListStackResourcesResponse"]["ListStackResourcesResult"]
         resources: List[Dict[str, Any]] = result["StackResourceSummaries"]
 
         # Handle pagination
@@ -189,14 +174,15 @@
         )
         signed_request = request.sign(
             utc_now=self.utcnow(), service=service, region=region
         )
         response = await request_with_retry(
             self.httpx_client,
             request=signed_request,
+            logger=self.logger,
         )
         json_response = json.loads(response.text)
         properties = json_response["ResourceDescription"]["Properties"]
         resource: Dict[str, Any] = json.loads(properties)
         return resource
 
     async def invoke(
@@ -222,9 +208,10 @@
         )
         signed_request = request.sign(
             utc_now=self.utcnow(), service=service, region=region
         )
         response = await request_with_retry(
             self.httpx_client,
             request=signed_request,
+            logger=self.logger,
         )
         return response.text
```

### Comparing `awsync-0.2.0/awsync/models/aws.py` & `awsync-0.3.0/awsync/models/aws.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 "AWS type models."
 from awsync.models.strenum import StrEnum
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from typing import Optional
 import os
 
 
 @dataclass(frozen=True)
 class Credentials:
     "AWS Credentials."
     access_key_id: str
     "The Access Key ID."
-    secret_access_key: str
+    secret_access_key: str = field(repr=False)  # Avoid logging secret values.
     "The Secret Access Key."
     session_token: Optional[str] = None
     "(Optional) The session security token if using temporary credentials."
 
     @classmethod
     def from_environment(cls) -> "Credentials":
-        return cls(
-            access_key_id=os.environ["AWS_ACCESS_KEY_ID"],
-            secret_access_key=os.environ["AWS_SECRET_ACCESS_KEY"],
-            session_token=os.environ.get("AWS_SESSION_TOKEN"),
-        )
+        try:
+            return cls(
+                access_key_id=os.environ["AWS_ACCESS_KEY_ID"],
+                secret_access_key=os.environ["AWS_SECRET_ACCESS_KEY"],
+                session_token=os.environ.get("AWS_SESSION_TOKEN"),
+            )
+        except KeyError as exc:
+            raise KeyError(
+                "Unable to find AWS credentials in environment variables when calling Credentials.from_environment(). "
+                "Ensure environment variables 'AWS_ACCESS_KEY_ID' and 'AWS_SECRET_ACCESS_KEY' are set before calling Credentials.from_environment() or use Credentials() to set values directly."
+            ) from exc
 
 
 class Region(StrEnum):
     """
     An AWS Region.
     See: https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/using-regions-availability-zones.html#concepts-available-regions
     """
```

### Comparing `awsync-0.2.0/awsync/models/http.py` & `awsync-0.3.0/awsync/models/http.py`

 * *Files identical despite different names*

### Comparing `awsync-0.2.0/awsync/request.py` & `awsync-0.3.0/awsync/request.py`

 * *Files identical despite different names*

### Comparing `awsync-0.2.0/pyproject.toml` & `awsync-0.3.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "awsync"
-version = "0.2.0"
+version = "0.3.0"
 description = "An asynchronous, fully-typed AWS API library with a focus on being understandable, reliable, and maintainable."
 license = "Apache-2.0"
 authors = ["JKCT <jkct@visceralfx.com>"]
 readme = "README.md"
 packages = [{include = "awsync"}]
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -21,21 +21,33 @@
 python = "^3.8"
 httpx = "^0.27.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.4.0"
 mypy = "^1.9.0"
 pytest = "^8.1.1"
+pytest-cov = "^5.0.0"
+pytest-asyncio = "^0.23.6"
 
 [tool.mypy]
 strict = true
 color_output = true
 cache_dir = "/tmp/cache/.mypy_cache"
 
+[tool.coverage.run]
+omit = ["__main__.py"]
+
+[tool.coverage.report]
+exclude_also = [
+    "async def list_stack_resources",
+    "async def get_resource",
+    "async def invoke",
+    ]
+
 [tool.pytest.ini_options]
 testpaths = "tests"
 cache_dir = "/tmp/cache/.pytest_cache"
-addopts = "-vv"
+addopts = "-vv --cov=awsync --cov-report term-missing:skip-covered --cov-fail-under=100"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `awsync-0.2.0/PKG-INFO` & `awsync-0.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awsync
-Version: 0.2.0
+Version: 0.3.0
 Summary: An asynchronous, fully-typed AWS API library with a focus on being understandable, reliable, and maintainable.
 Home-page: https://github.com/JKCT/awsync
 License: Apache-2.0
 Keywords: aws,async,boto,request,sdk,typed
 Author: JKCT
 Author-email: jkct@visceralfx.com
 Requires-Python: >=3.8,<4.0
@@ -32,34 +32,32 @@
 Only a few API methods currently implemented for testing and development.
 
 ## Usage
 
 ```python
 "Module main."
 from asyncio import run
-from datetime import datetime, UTC
 from httpx import AsyncClient
 
 from awsync.client import Client
 from awsync.models.aws import Region, Credentials
 
 
 async def main() -> int:
     "Main function."
     async with AsyncClient() as httpx_client:
         client = Client(
             credentials=Credentials.from_environment(),
             httpx_client=httpx_client,
-            utcnow=lambda: datetime.now(UTC),
         )
         response = await client.list_stack_resources(
             region=Region.us_east_1, stack_name="Example-Stack-Name"
         )
         print(response)
-        return 0
+    return 0
 
 
 if __name__ == "__main__":
     run(main())
 ```
 
 ## Local Developer Setup
@@ -85,17 +83,15 @@
 - `make pr` runs all pull request pre-checks below.
 - `make format` runs code formatter.
 - `make lint` checks code linting.
 - `make test` runs tests.
 
 ## Repository TODO:
 
-- Logging
-- Test Coverage
+- Code generation [from JSON](https://github.com/boto/botocore/tree/develop/botocore/data)
 - Automatic Publish CICD
 - Documentation with [mkDocs](https://squidfunk.github.io/mkdocs-material/)
-- Issue template
-- Repository Template variables?
 - Test Makefile replacements
+  - [mise](https://mise.jdx.dev/)
   - [Poetry run](https://python-poetry.org/docs/cli/#run)
   - [doit](https://pydoit.org/)
```

