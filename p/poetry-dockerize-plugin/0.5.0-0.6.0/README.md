# Comparing `tmp/poetry_dockerize_plugin-0.5.0.tar.gz` & `tmp/poetry_dockerize_plugin-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_dockerize_plugin-0.5.0.tar", max compression
+gzip compressed data, was "poetry_dockerize_plugin-0.6.0.tar", max compression
```

## Comparing `poetry_dockerize_plugin-0.5.0.tar` & `poetry_dockerize_plugin-0.6.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1071 2024-02-01 00:00:39.791921 poetry_dockerize_plugin-0.5.0/LICENSE
--rw-r--r--   0        0        0     4271 2024-02-01 00:00:39.795921 poetry_dockerize_plugin-0.5.0/README.md
--rw-r--r--   0        0        0        0 2024-02-01 00:00:39.795921 poetry_dockerize_plugin-0.5.0/poetry_dockerize_plugin/__init__.py
--rw-r--r--   0        0        0    12934 2024-02-01 00:00:39.795921 poetry_dockerize_plugin-0.5.0/poetry_dockerize_plugin/builder.py
--rw-r--r--   0        0        0     1008 2024-02-01 00:00:39.795921 poetry_dockerize_plugin-0.5.0/poetry_dockerize_plugin/plugin.py
--rw-r--r--   0        0        0     1997 2024-02-01 00:00:39.795921 poetry_dockerize_plugin-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     6100 1970-01-01 00:00:00.000000 poetry_dockerize_plugin-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-14 09:58:29.598082 poetry_dockerize_plugin-0.6.0/LICENSE
+-rw-r--r--   0        0        0     4471 2024-05-14 09:58:29.598082 poetry_dockerize_plugin-0.6.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-14 09:58:29.598082 poetry_dockerize_plugin-0.6.0/poetry_dockerize_plugin/__init__.py
+-rw-r--r--   0        0        0    13459 2024-05-14 09:58:29.598082 poetry_dockerize_plugin-0.6.0/poetry_dockerize_plugin/builder.py
+-rw-r--r--   0        0        0     1239 2024-05-14 09:58:29.598082 poetry_dockerize_plugin-0.6.0/poetry_dockerize_plugin/plugin.py
+-rw-r--r--   0        0        0     1997 2024-05-14 09:58:29.598082 poetry_dockerize_plugin-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     6300 1970-01-01 00:00:00.000000 poetry_dockerize_plugin-0.6.0/PKG-INFO
```

### Comparing `poetry_dockerize_plugin-0.5.0/LICENSE` & `poetry_dockerize_plugin-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_dockerize_plugin-0.5.0/README.md` & `poetry_dockerize_plugin-0.6.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -82,26 +82,30 @@
 ```
 
 ## Configuration API Reference
 
 This examples shows a complete configuration of the docker image:
 
 ```toml
-[tool.docker]
+[tool.dockerize]
 name = "alternative-image-name"
 python = "3.12"
 base-image = "python:3.12-slim"
 tags = ["latest-dev"]
 entrypoint = ["python", "-m", "whatever"]
 ports = [5000]
 env = {"MY_APP_ENV" = "dev"}
 labels = {"MY_APP_LABEL" = "dev"}
 apt-packages = ["curl"]
-extra-build-instructions = ["RUN poetry config http-basic.foo <username> <password>"]
 extra-run-instructions = ["RUN curl https://huggingface.co/transformers/"]
+
+# Only for build docker layer
+build-apt-packages = ["gcc"]
+extra-build-instructions = ["RUN poetry config http-basic.foo <username> <password>"]
+
 ```
 
 * `name` customizes the docker image name. 
 * `python` python version to use. If not specified, will try to be extracted from `tool.poetry.dependencies.python`. Default is `3.11`
 * `base-image` customizes the base image. If not defined, the default base image is `python:<python-version>-slim-buster`. 
 * `tags` declares a list of tags for the image.
 * `entrypoint` customizes the entrypoint of the image. If not provided, the default entrypoint is retrieved from the `packages` configuration.
@@ -125,10 +129,18 @@
 
 To troubleshoot the plugin, you can use the `--debug` flag to get more information about the execution.
 
 ```bash
 poetry dockerize --debug
 ```
 
+## Generate Dockerfile
+
+To store the generated Dockerfile, you can use the `--generate` flag.
+
+```bash
+poetry dockerize --generate
+```
+
 ## License
 
 This project is licensed under the terms of the MIT license.
```

#### html2text {}

```diff
@@ -16,33 +16,36 @@
 poetry run pytest poetry dockerize - name: Login to Docker Hub uses: docker/
 login-action@v3 with: username: ${{ secrets.DOCKERHUB_USERNAME }} password: ${
 { secrets.DOCKERHUB_TOKEN }} - name: Push to Docker Hub run: docker push my-
 app:latest ``` ## Configuration To customize some options, you can add a `
 [tool.dockerize]` section in your `pyproject.toml` file. For example to change
 the image name: ```toml [tool.dockerize] name = "myself/myproject-app" ``` ##
 Configuration API Reference This examples shows a complete configuration of the
-docker image: ```toml [tool.docker] name = "alternative-image-name" python =
+docker image: ```toml [tool.dockerize] name = "alternative-image-name" python =
 "3.12" base-image = "python:3.12-slim" tags = ["latest-dev"] entrypoint =
 ["python", "-m", "whatever"] ports = [5000] env = {"MY_APP_ENV" = "dev"} labels
-= {"MY_APP_LABEL" = "dev"} apt-packages = ["curl"] extra-build-instructions =
-["RUN poetry config http-basic.foo "] extra-run-instructions = ["RUN curl
-https://huggingface.co/transformers/"] ``` * `name` customizes the docker image
-name. * `python` python version to use. If not specified, will try to be
-extracted from `tool.poetry.dependencies.python`. Default is `3.11` * `base-
-image` customizes the base image. If not defined, the default base image is
-`python:-slim-buster`. * `tags` declares a list of tags for the image. *
-`entrypoint` customizes the entrypoint of the image. If not provided, the
-default entrypoint is retrieved from the `packages` configuration. * `ports`
-exposes ports * `env` declares environment variables inside the docker image. *
-`labels` append labels to the docker image. Default labels are added following
-the opencontainers specification. * `apt-packages` installs apt packages inside
-the docker image. * `extra-build-instructions` adds extra instructions to the
+= {"MY_APP_LABEL" = "dev"} apt-packages = ["curl"] extra-run-instructions =
+["RUN curl https://huggingface.co/transformers/"] # Only for build docker layer
+build-apt-packages = ["gcc"] extra-build-instructions = ["RUN poetry config
+http-basic.foo "] ``` * `name` customizes the docker image name. * `python`
+python version to use. If not specified, will try to be extracted from
+`tool.poetry.dependencies.python`. Default is `3.11` * `base-image` customizes
+the base image. If not defined, the default base image is `python:-slim-
+buster`. * `tags` declares a list of tags for the image. * `entrypoint`
+customizes the entrypoint of the image. If not provided, the default entrypoint
+is retrieved from the `packages` configuration. * `ports` exposes ports * `env`
+declares environment variables inside the docker image. * `labels` append
+labels to the docker image. Default labels are added following the
+opencontainers specification. * `apt-packages` installs apt packages inside the
+docker image. * `extra-build-instructions` adds extra instructions to the
 docker build (before poetry install). Any modification to the filesystem will
 be lost after the poetry install. If you need to add files to the image, use
 the `extra-run-instructions`. * `extra-run-instructions` adds extra
 instructions to the docker run (after poetry install). Any modification to the
 filesystem will be kept after the poetry install. ## Command-Line options All
 command line options provided by the `poetry-dockerize-plugin` may be accessed
 by typing: ```bash poetry dockerize --help ``` ## Troubleshooting To
 troubleshoot the plugin, you can use the `--debug` flag to get more information
-about the execution. ```bash poetry dockerize --debug ``` ## License This
-project is licensed under the terms of the MIT license.
+about the execution. ```bash poetry dockerize --debug ``` ## Generate
+Dockerfile To store the generated Dockerfile, you can use the `--generate`
+flag. ```bash poetry dockerize --generate ``` ## License This project is
+licensed under the terms of the MIT license.
```

### Comparing `poetry_dockerize_plugin-0.5.0/poetry_dockerize_plugin/builder.py` & `poetry_dockerize_plugin-0.6.0/poetry_dockerize_plugin/builder.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     tags: List[str] = []
     entrypoint_cmd: List[str] = []
     python: str = ""
     ports: List[int] = []
     envs: dict[str, str] = {}
     labels: dict[str, str] = {}
     apt_packages: List[str] = []
+    build_apt_packages: List[str] = []
     base_image: str = ""
     extra_build_instructions: List[str] = []
     extra_runtime_instructions: List[str] = []
 
 
 class ProjectConfiguration:
     image_name: str
@@ -60,14 +61,15 @@
     config.tags = get_list_or_str_from_dict(dict, "tags")
     config.entrypoint_cmd = get_list_or_str_from_dict(dict, "entrypoint", split_by=" ")
     config.python = dict.get("python")
     config.ports = dict.get("ports")
     config.envs = dict.get("env")
     config.labels = dict.get("labels")
     config.apt_packages = dict.get("apt-packages")
+    config.build_apt_packages = dict.get("build-apt-packages")
     config.base_image = dict.get("base-image")
     config.extra_build_instructions = dict.get("extra-build-instructions")
     config.extra_runtime_instructions = dict.get("extra-runtime-instructions")
     return config
 
 
 def extract_python_version(pyversion: str) -> Optional[str]:
@@ -112,14 +114,15 @@
             name = package["include"]
             config.entrypoint = ["python", "-m", name]
 
     if not config.entrypoint:
         raise ValueError('No package found in pyproject.toml and no entrypoint specified in dockerize section')
 
     config.runtime_apt_packages = dockerize_section.apt_packages or []
+    config.build_apt_packages = dockerize_section.build_apt_packages or []
     if 'packages' in tool_poetry:
         config.app_packages += [package["include"] for package in tool_poetry['packages']]
 
     if "dependencies" in tool_poetry:
         for dep in tool_poetry["dependencies"]:
             if isinstance(tool_poetry["dependencies"][dep], dict):
                 if 'path' in tool_poetry["dependencies"][dep]:
@@ -221,19 +224,19 @@
 ENV POETRY_VIRTUALENVS_CREATE=1
 ENV POETRY_CACHE_DIR=/tmp/poetry_cache
 RUN poetry config virtualenvs.create false && poetry config virtualenvs.in-project false
 
 {generate_apt_packages_str(config.build_apt_packages)}
 {generate_add_project_toml_str(config, real_context_path)}
 
-RUN cd /app && poetry install --no-interaction --no-ansi --no-root
-
 {generate_add_packages_str(config, real_context_path)}
 {generate_extra_instructions_str(config.extra_build_instructions)}
 
+RUN cd /app && poetry install --no-interaction --no-ansi --no-root
+
 FROM {config.base_image} as runtime
 {generate_apt_packages_str(config.runtime_apt_packages)}
 {labels_str}
 
 ENV PATH="/app/.venv/bin:$PATH"
 ENV PYTHONUNBUFFERED=1
 {envs_str}
@@ -242,32 +245,38 @@
 COPY --from=builder /app/ /app/
 
 {ports_str}
 {generate_extra_instructions_str(config.extra_runtime_instructions)}
 CMD {cmd_str}"""
 
 
-def build_image(path: str, verbose: bool = False) -> None:
+def build_image(path: str, verbose: bool = False, generate: bool = False) -> None:
     config = parse_pyproject_toml(path)
-    build(config=config, root_path=path, verbose=verbose)
+    build(config=config, root_path=path, verbose=verbose, generate=generate)
 
 
 def build(
         root_path: str,
         config: ProjectConfiguration,
-        verbose: bool = False
+        verbose: bool = False,
+        generate: bool = False
 ) -> None:
     """
     Build a docker image from a poetry project.
     """
 
     with tempfile.NamedTemporaryFile() as tmp:
         dockerfile = tmp.name
         real_context_path = os.path.realpath(root_path)
         content = generate_docker_file_content(config, real_context_path)
+        if generate:
+            generate_dockerfile_path = os.path.join(real_context_path, "Dockerfile")
+            with open(generate_dockerfile_path, "w") as f:
+                f.write(content)
+            print(f"Stored Dockerfile to {generate_dockerfile_path} 📄")
         tmp.write(content.encode("utf-8"))
         tmp.flush()
         if verbose:
             print("Building with dockerfile content: \n===[Dockerfile]==\n" + content + "\n===[/Dockerfile]==\n")
 
         dockerignore = os.path.join(real_context_path, ".dockerignore")
         dockerignore_created = write_dockerignore_if_needed(dockerignore)
```

### Comparing `poetry_dockerize_plugin-0.5.0/poetry_dockerize_plugin/plugin.py` & `poetry_dockerize_plugin-0.6.0/poetry_dockerize_plugin/plugin.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,22 +17,28 @@
             "Project root path",
             flag=False,
             default=os.getcwd(),
         ),
         option(
             "debug",
             flag=True,
-            description="Debug mode",
+            description="(poetry-dockerize-plugin) Debug mode",
+        ),
+        option(
+            "generate",
+            description="(poetry-dockerize-plugin) Generate and persist Dockerfile",
+            flag=True,
         ),
     ]
 
     def handle(self) -> int:
         build_image(
             path=self.option("path"),
             verbose=self.option("debug"),
+            generate=self.option("generate"),
         )
         return 0
 
 
 def factory():
     return DockerCommand()
```

### Comparing `poetry_dockerize_plugin-0.5.0/pyproject.toml` & `poetry_dockerize_plugin-0.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-dockerize-plugin"
-version = "0.5.0"
+version = "0.6.0"
 description = "Poetry application to Docker, automatically."
 authors = ["Nicolò Boschi <boschi1997@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["poetry", "packaging", "docker"]
 repository = "https://github.com/nicoloboschi/poetry-dockerize-plugin"
 documentation = "https://github.com/nicoloboschi/poetry-dockerize-plugin"
```

### Comparing `poetry_dockerize_plugin-0.5.0/PKG-INFO` & `poetry_dockerize_plugin-0.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-dockerize-plugin
-Version: 0.5.0
+Version: 0.6.0
 Summary: Poetry application to Docker, automatically.
 Home-page: https://github.com/nicoloboschi/poetry-dockerize-plugin
 License: MIT
 Keywords: poetry,packaging,docker
 Author: Nicolò Boschi
 Author-email: boschi1997@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -121,26 +121,30 @@
 ```
 
 ## Configuration API Reference
 
 This examples shows a complete configuration of the docker image:
 
 ```toml
-[tool.docker]
+[tool.dockerize]
 name = "alternative-image-name"
 python = "3.12"
 base-image = "python:3.12-slim"
 tags = ["latest-dev"]
 entrypoint = ["python", "-m", "whatever"]
 ports = [5000]
 env = {"MY_APP_ENV" = "dev"}
 labels = {"MY_APP_LABEL" = "dev"}
 apt-packages = ["curl"]
-extra-build-instructions = ["RUN poetry config http-basic.foo <username> <password>"]
 extra-run-instructions = ["RUN curl https://huggingface.co/transformers/"]
+
+# Only for build docker layer
+build-apt-packages = ["gcc"]
+extra-build-instructions = ["RUN poetry config http-basic.foo <username> <password>"]
+
 ```
 
 * `name` customizes the docker image name. 
 * `python` python version to use. If not specified, will try to be extracted from `tool.poetry.dependencies.python`. Default is `3.11`
 * `base-image` customizes the base image. If not defined, the default base image is `python:<python-version>-slim-buster`. 
 * `tags` declares a list of tags for the image.
 * `entrypoint` customizes the entrypoint of the image. If not provided, the default entrypoint is retrieved from the `packages` configuration.
@@ -164,11 +168,19 @@
 
 To troubleshoot the plugin, you can use the `--debug` flag to get more information about the execution.
 
 ```bash
 poetry dockerize --debug
 ```
 
+## Generate Dockerfile
+
+To store the generated Dockerfile, you can use the `--generate` flag.
+
+```bash
+poetry dockerize --generate
+```
+
 ## License
 
 This project is licensed under the terms of the MIT license.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: poetry-dockerize-plugin Version: 0.5.0 Summary:
+Metadata-Version: 2.1 Name: poetry-dockerize-plugin Version: 0.6.0 Summary:
 Poetry application to Docker, automatically. Home-page: https://github.com/
 nicoloboschi/poetry-dockerize-plugin License: MIT Keywords:
 poetry,packaging,docker Author: NicolÃ² Boschi Author-email:
 boschi1997@gmail.com Requires-Python: >=3.9,<4.0 Classifier: Intended Audience
 :: Developers Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators Classifier: License ::
 OSI Approved :: MIT License Classifier: Operating System :: OS Independent
@@ -40,33 +40,36 @@
 poetry run pytest poetry dockerize - name: Login to Docker Hub uses: docker/
 login-action@v3 with: username: ${{ secrets.DOCKERHUB_USERNAME }} password: ${
 { secrets.DOCKERHUB_TOKEN }} - name: Push to Docker Hub run: docker push my-
 app:latest ``` ## Configuration To customize some options, you can add a `
 [tool.dockerize]` section in your `pyproject.toml` file. For example to change
 the image name: ```toml [tool.dockerize] name = "myself/myproject-app" ``` ##
 Configuration API Reference This examples shows a complete configuration of the
-docker image: ```toml [tool.docker] name = "alternative-image-name" python =
+docker image: ```toml [tool.dockerize] name = "alternative-image-name" python =
 "3.12" base-image = "python:3.12-slim" tags = ["latest-dev"] entrypoint =
 ["python", "-m", "whatever"] ports = [5000] env = {"MY_APP_ENV" = "dev"} labels
-= {"MY_APP_LABEL" = "dev"} apt-packages = ["curl"] extra-build-instructions =
-["RUN poetry config http-basic.foo "] extra-run-instructions = ["RUN curl
-https://huggingface.co/transformers/"] ``` * `name` customizes the docker image
-name. * `python` python version to use. If not specified, will try to be
-extracted from `tool.poetry.dependencies.python`. Default is `3.11` * `base-
-image` customizes the base image. If not defined, the default base image is
-`python:-slim-buster`. * `tags` declares a list of tags for the image. *
-`entrypoint` customizes the entrypoint of the image. If not provided, the
-default entrypoint is retrieved from the `packages` configuration. * `ports`
-exposes ports * `env` declares environment variables inside the docker image. *
-`labels` append labels to the docker image. Default labels are added following
-the opencontainers specification. * `apt-packages` installs apt packages inside
-the docker image. * `extra-build-instructions` adds extra instructions to the
+= {"MY_APP_LABEL" = "dev"} apt-packages = ["curl"] extra-run-instructions =
+["RUN curl https://huggingface.co/transformers/"] # Only for build docker layer
+build-apt-packages = ["gcc"] extra-build-instructions = ["RUN poetry config
+http-basic.foo "] ``` * `name` customizes the docker image name. * `python`
+python version to use. If not specified, will try to be extracted from
+`tool.poetry.dependencies.python`. Default is `3.11` * `base-image` customizes
+the base image. If not defined, the default base image is `python:-slim-
+buster`. * `tags` declares a list of tags for the image. * `entrypoint`
+customizes the entrypoint of the image. If not provided, the default entrypoint
+is retrieved from the `packages` configuration. * `ports` exposes ports * `env`
+declares environment variables inside the docker image. * `labels` append
+labels to the docker image. Default labels are added following the
+opencontainers specification. * `apt-packages` installs apt packages inside the
+docker image. * `extra-build-instructions` adds extra instructions to the
 docker build (before poetry install). Any modification to the filesystem will
 be lost after the poetry install. If you need to add files to the image, use
 the `extra-run-instructions`. * `extra-run-instructions` adds extra
 instructions to the docker run (after poetry install). Any modification to the
 filesystem will be kept after the poetry install. ## Command-Line options All
 command line options provided by the `poetry-dockerize-plugin` may be accessed
 by typing: ```bash poetry dockerize --help ``` ## Troubleshooting To
 troubleshoot the plugin, you can use the `--debug` flag to get more information
-about the execution. ```bash poetry dockerize --debug ``` ## License This
-project is licensed under the terms of the MIT license.
+about the execution. ```bash poetry dockerize --debug ``` ## Generate
+Dockerfile To store the generated Dockerfile, you can use the `--generate`
+flag. ```bash poetry dockerize --generate ``` ## License This project is
+licensed under the terms of the MIT license.
```

