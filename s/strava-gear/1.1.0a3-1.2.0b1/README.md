# Comparing `tmp/strava-gear-1.1.0a3.tar.gz` & `tmp/strava_gear-1.2.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strava-gear-1.1.0a3.tar", last modified: Mon Dec  4 18:06:37 2023, max compression
+gzip compressed data, was "strava_gear-1.2.0b1.tar", last modified: Mon May 13 22:05:07 2024, max compression
```

## Comparing `strava-gear-1.1.0a3.tar` & `strava_gear-1.2.0b1.tar`

### file list

```diff
@@ -1,45 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 18:06:37.779179 strava-gear-1.1.0a3/
--rw-r--r--   0 runner    (1001) docker     (127)      325 2023-12-04 18:06:09.000000 strava-gear-1.1.0a3/.cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 18:06:37.771179 strava-gear-1.1.0a3/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2023-12-04 18:06:09.000000 strava-gear-1.1.0a3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 18:06:37.775179 strava-gear-1.1.0a3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     4479 2023-12-04 18:06:09.000000 strava-gear-1.1.0a3/.github/workflows/check.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2023-12-04 18:06:09.000000 strava-gear-1.1.0a3/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       68 2023-12-04 18:06:09.000000 strava-gear-1.1.0a3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2023-12-04 18:06:09.000000 strava-gear-1.1.0a3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3357 2023-12-04 18:06:09.000000 strava-gear-1.1.0a3/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    14304 2023-12-04 18:06:37.779179 strava-gear-1.1.0a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12735 2023-12-04 18:06:09.000000 strava-gear-1.1.0a3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2023-12-04 18:06:09.000000 strava-gear-1.1.0a3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       93 2023-12-04 18:06:37.779179 strava-gear-1.1.0a3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 18:06:37.771179 strava-gear-1.1.0a3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 18:06:37.775179 strava-gear-1.1.0a3/src/strava_gear/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2023-12-04 18:06:09.000000 strava-gear-1.1.0a3/src/strava_gear/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2023-12-04 18:06:09.000000 strava-gear-1.1.0a3/src/strava_gear/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3064 2023-12-04 18:06:09.000000 strava-gear-1.1.0a3/src/strava_gear/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2023-12-04 18:06:09.000000 strava-gear-1.1.0a3/src/strava_gear/cli_strava_offline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2023-12-04 18:06:09.000000 strava-gear-1.1.0a3/src/strava_gear/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     6905 2023-12-04 18:06:09.000000 strava-gear-1.1.0a3/src/strava_gear/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 18:06:37.775179 strava-gear-1.1.0a3/src/strava_gear/input/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-04 18:06:09.000000 strava-gear-1.1.0a3/src/strava_gear/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2023-12-04 18:06:09.000000 strava-gear-1.1.0a3/src/strava_gear/input/activities.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2023-12-04 18:06:09.000000 strava-gear-1.1.0a3/src/strava_gear/input/date.py
--rw-r--r--   0 runner    (1001) docker     (127)     5069 2023-12-04 18:06:09.000000 strava-gear-1.1.0a3/src/strava_gear/input/rules.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-04 18:06:09.000000 strava-gear-1.1.0a3/src/strava_gear/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2023-12-04 18:06:09.000000 strava-gear-1.1.0a3/src/strava_gear/report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 18:06:37.779179 strava-gear-1.1.0a3/src/strava_gear.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14304 2023-12-04 18:06:37.000000 strava-gear-1.1.0a3/src/strava_gear.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      888 2023-12-04 18:06:37.000000 strava-gear-1.1.0a3/src/strava_gear.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-04 18:06:37.000000 strava-gear-1.1.0a3/src/strava_gear.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      122 2023-12-04 18:06:37.000000 strava-gear-1.1.0a3/src/strava_gear.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      283 2023-12-04 18:06:37.000000 strava-gear-1.1.0a3/src/strava_gear.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-12-04 18:06:37.000000 strava-gear-1.1.0a3/src/strava_gear.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 18:06:37.779179 strava-gear-1.1.0a3/tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)      142 2023-12-04 18:06:09.000000 strava-gear-1.1.0a3/tests/cram-noescape.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2023-12-04 18:06:09.000000 strava-gear-1.1.0a3/tests/csv.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      452 2023-12-04 18:06:09.000000 strava-gear-1.1.0a3/tests/include.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 18:06:37.779179 strava-gear-1.1.0a3/tests/readme/
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2023-12-04 18:06:09.000000 strava-gear-1.1.0a3/tests/readme/help.md
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2023-12-04 18:06:09.000000 strava-gear-1.1.0a3/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2023-12-04 18:06:09.000000 strava-gear-1.1.0a3/tests/test_input_date.py
--rw-r--r--   0 runner    (1001) docker     (127)     3967 2023-12-04 18:06:09.000000 strava-gear-1.1.0a3/tests/test_input_rules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:05:07.834190 strava_gear-1.2.0b1/
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-13 22:04:39.000000 strava_gear-1.2.0b1/.cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:05:07.826189 strava_gear-1.2.0b1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-13 22:04:39.000000 strava_gear-1.2.0b1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:05:07.826189 strava_gear-1.2.0b1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-05-13 22:04:39.000000 strava_gear-1.2.0b1/.github/workflows/check.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-13 22:04:39.000000 strava_gear-1.2.0b1/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-13 22:04:39.000000 strava_gear-1.2.0b1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-13 22:04:39.000000 strava_gear-1.2.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-05-13 22:04:39.000000 strava_gear-1.2.0b1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    14995 2024-05-13 22:05:07.830190 strava_gear-1.2.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13062 2024-05-13 22:04:39.000000 strava_gear-1.2.0b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-05-13 22:04:39.000000 strava_gear-1.2.0b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-13 22:05:07.834190 strava_gear-1.2.0b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:05:07.822189 strava_gear-1.2.0b1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:05:07.826189 strava_gear-1.2.0b1/src/strava_gear/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-13 22:04:39.000000 strava_gear-1.2.0b1/src/strava_gear/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-13 22:04:39.000000 strava_gear-1.2.0b1/src/strava_gear/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4429 2024-05-13 22:04:39.000000 strava_gear-1.2.0b1/src/strava_gear/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-13 22:04:39.000000 strava_gear-1.2.0b1/src/strava_gear/cli_strava_offline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-05-13 22:04:39.000000 strava_gear-1.2.0b1/src/strava_gear/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7187 2024-05-13 22:04:39.000000 strava_gear-1.2.0b1/src/strava_gear/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:05:07.830190 strava_gear-1.2.0b1/src/strava_gear/input/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 22:04:39.000000 strava_gear-1.2.0b1/src/strava_gear/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-13 22:04:39.000000 strava_gear-1.2.0b1/src/strava_gear/input/activities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-13 22:04:39.000000 strava_gear-1.2.0b1/src/strava_gear/input/date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5069 2024-05-13 22:04:39.000000 strava_gear-1.2.0b1/src/strava_gear/input/rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 22:04:39.000000 strava_gear-1.2.0b1/src/strava_gear/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-05-13 22:04:39.000000 strava_gear-1.2.0b1/src/strava_gear/report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:05:07.830190 strava_gear-1.2.0b1/src/strava_gear.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14995 2024-05-13 22:05:07.000000 strava_gear-1.2.0b1/src/strava_gear.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-13 22:05:07.000000 strava_gear-1.2.0b1/src/strava_gear.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 22:05:07.000000 strava_gear-1.2.0b1/src/strava_gear.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-13 22:05:07.000000 strava_gear-1.2.0b1/src/strava_gear.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-13 22:05:07.000000 strava_gear-1.2.0b1/src/strava_gear.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 22:05:07.000000 strava_gear-1.2.0b1/src/strava_gear.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:05:07.830190 strava_gear-1.2.0b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-05-13 22:04:39.000000 strava_gear-1.2.0b1/tests/csv.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      452 2024-05-13 22:04:39.000000 strava_gear-1.2.0b1/tests/include.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:05:07.830190 strava_gear-1.2.0b1/tests/readme/
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-13 22:04:39.000000 strava_gear-1.2.0b1/tests/readme/help.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-13 22:04:39.000000 strava_gear-1.2.0b1/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-13 22:04:39.000000 strava_gear-1.2.0b1/tests/test_input_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-05-13 22:04:39.000000 strava_gear-1.2.0b1/tests/test_input_rules.py
```

### Comparing `strava-gear-1.1.0a3/.github/workflows/check.yaml` & `strava_gear-1.2.0b1/.github/workflows/check.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -26,31 +26,31 @@
           - '3.11'
           - '3.12'
 
     steps:
       - uses: actions/checkout@v4
       - name: Set up Python ${{ matrix.python-version }}
         id: setup-python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
       - name: Get pip cache dir
         id: pip-cache
         run: |
           echo "dir=$(pip cache dir)" >> $GITHUB_OUTPUT
       - name: Persistent Github pip cache
-        uses: actions/cache@v3
+        uses: actions/cache@v4
         with:
           path: ${{ steps.pip-cache.outputs.dir }}
           key: pip-${{ runner.os }}-${{ matrix.python-version }}-${{ hashFiles('pyproject.toml', 'setup.cfg', 'setup.py', 'Makefile') }}
           restore-keys: |
             pip-${{ runner.os }}-${{ matrix.python-version }}-
             pip-${{ runner.os }}-
       - name: Persistent Github venv cache
-        uses: actions/cache@v3
+        uses: actions/cache@v4
         with:
           path: .venv/
           key: venv-${{ runner.os }}-${{ steps.setup-python.outputs.python-version }}-${{ hashFiles('pyproject.toml', 'setup.cfg', 'setup.py', 'Makefile') }}
       - name: Install dependencies
         run: make venv
       - name: flake8
         uses: liskin/gh-problem-matcher-wrap@v3
@@ -68,16 +68,16 @@
           linters: isort
           run: make lint-isort
       - name: pytest
         uses: liskin/gh-problem-matcher-wrap@v3
         with:
           linters: pytest
           run: make test-pytest
-      - name: cram, readme
-        run: make test-cram readme
+      - name: prysk, readme
+        run: make test-prysk readme
       - name: check-wheel
         run: make check-wheel
 
   check-distro:
     runs-on: ubuntu-latest
 
     strategy:
@@ -112,14 +112,31 @@
             | tr '\n' ' ' \
             | grep -o -P '\sdependencies-apt\s*=\s*\K\[.*?\]' \
             | grep -o -P '".*?"' \
             | tr -d '"')
           apt-cache --generate pkgnames \
             | grep --line-regexp --fixed-strings "$deps" \
             | xargs apt install -y
+      - name: Workaround for https://bugs.debian.org/cgi-bin/bugreport.cgi?bug=1057968
+        env:
+          DEBIAN_FRONTEND: noninteractive
+        shell: bash
+        run: |
+          set -ex
+          grep "Suites: noble" /etc/apt/sources.list.d/ubuntu.sources || exit 0
+          apt install -y debian-archive-keyring
+          ln -s /usr/share/keyrings/debian-archive-keyring.gpg /etc/apt/trusted.gpg.d/
+          python3_pycodestyle=$(dpkg-query --showformat='${Version}\n' --show python3-pycodestyle)
+          python3_flake8=$(dpkg-query --showformat='${Version}\n' --show python3-flake8)
+          if [[ $python3_pycodestyle == 2.11.* && $python3_flake8 == 5.* ]]; then
+            echo 'deb https://deb.debian.org/debian unstable main' >/etc/apt/sources.list.d/debian-unstable.list
+            echo 'APT::Default-Release "noble";' >/etc/apt/apt.conf.d/debian-release
+            apt update
+            apt install -t unstable -y python3-flake8
+          fi
       - name: Workaround for https://github.com/actions/checkout/pull/762 not persisting
         run: git config --global --add safe.directory "$PWD"
       - name: Install remaining dependencies
         run: make venv-system-site-packages
       - name: flake8
         uses: liskin/gh-problem-matcher-wrap@v3
         with:
@@ -136,21 +153,21 @@
           linters: isort
           run: make lint-isort
       - name: pytest
         uses: liskin/gh-problem-matcher-wrap@v3
         with:
           linters: pytest
           run: make test-pytest
-      - name: cram, readme
+      - name: prysk, readme
         run: make readme
       - name: check-wheel
         run: make check-wheel
 
   workflow-keepalive:
     if: github.event_name == 'schedule'
     runs-on: ubuntu-latest
+    permissions:
+      actions: write
     steps:
-      - name: Re-enable workflow
-        env:
+      - uses: liskin/gh-workflow-keepalive@v1
+        with:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
-        run: |
-          gh api -X PUT repos/${{ github.repository }}/actions/workflows/check.yaml/enable
```

### Comparing `strava-gear-1.1.0a3/.github/workflows/pypi.yaml` & `strava_gear-1.2.0b1/.github/workflows/pypi.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -13,25 +13,25 @@
     name: Build distribution 📦
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
         with:
           fetch-depth: 0  # needed for pre-releases
       - name: Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: '3.x'
       - name: Install dependencies
         run: |
           make venv
       - name: Build
         run: |
           make dist
       - name: Store artifacts
-        uses: actions/upload-artifact@v3
+        uses: actions/upload-artifact@v4
         with:
           name: dist
           path: dist/
 
   pypi:
     needs:
       - build
@@ -40,13 +40,13 @@
     environment:
       name: pypi
       url: https://pypi.org/p/strava-gear
     permissions:
       id-token: write
     steps:
       - name: Fetch artifacts
-        uses: actions/download-artifact@v3
+        uses: actions/download-artifact@v4
         with:
           name: dist
           path: dist/
       - name: Publish distribution 📦 to PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `strava-gear-1.1.0a3/LICENSE` & `strava_gear-1.2.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `strava-gear-1.1.0a3/Makefile` & `strava_gear-1.2.0b1/Makefile`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 VENV_USE_SYSTEM_SITE_PACKAGES = $(wildcard $(VENV_SYSTEM_SITE_PACKAGES))
 
 VENV_WHEEL = .venv-wheel
 VENV_WHEEL_PYTHON = $(VENV_WHEEL)/bin/python
 
 PACKAGE := $(shell sed -ne '/^name / { y/-/_/; s/^.*=\s*"\(.*\)"/\1/p }' pyproject.toml)
 
+TEMPLATES_DIR = $(HOME)/src
+TEMPLATE := $(shell realpath --relative-to=. $(TEMPLATES_DIR)/cookiecutter-python-cli)
+
 .PHONY: venv-system-site-packages
 venv-system-site-packages:
 	$(MAKE) VENV_USE_SYSTEM_SITE_PACKAGES=1 venv
 
 .PHONY: venv
 venv: $(VENV_DONE)
 
@@ -44,35 +47,35 @@
 	$(VENV_PYTHON) -m mypy --show-column-numbers $(LINT_SOURCES)
 
 .PHONY: lint-isort
 lint-isort: $(VENV_DONE)
 	$(VENV_PYTHON) -m isort --check $(LINT_SOURCES)
 
 .PHONY: test
-test: test-pytest test-cram
+test: test-pytest test-prysk
 
 .PHONY: test-pytest
 test-pytest: $(VENV_DONE)
 	$(VENV_PYTHON) -m pytest $(PYTEST_FLAGS) tests/
 
 .PHONY: readme
 readme: README.md
 	git diff --exit-code $^
 
-.PHONY: test-cram
-test-cram: CRAM_INTERACTIVE=$(shell [ -t 0 ] && echo --interactive)
-test-cram: $(VENV_DONE)
+.PHONY: test-prysk
+test-prysk: PRYSK_INTERACTIVE=$(shell [ -t 0 ] && echo --interactive)
+test-prysk: $(VENV_DONE)
 	PATH="$(CURDIR)/$(VENV)/bin:$$PATH" \
 	XDG_DATA_HOME=/home/user/.local/share \
 	XDG_CONFIG_HOME=/home/user/.config \
-	$(VENV_PYTHON) tests/cram-noescape.py --indent=4 --shell=/bin/bash $(CRAM_INTERACTIVE) \
+	$(VENV_PYTHON) -m prysk --indent=4 --shell=/bin/bash $(PRYSK_INTERACTIVE) \
 		$(wildcard tests/*.md tests/*/*.md tests/*/*/*.md)
 
 .PHONY: README.md
-README.md: test-cram
+README.md: test-prysk
 	tests/include.py < $@ > $@.tmp
 	mv -f $@.tmp $@
 
 .PHONY: dist
 dist: $(VENV_DONE)
 	rm -rf dist/
 	$(VENV_PYTHON) -m build --outdir dist
@@ -85,14 +88,22 @@
 ipython: $(VENV_DONE)
 	$(VENV_PYTHON) -m IPython
 
 .PHONY: clean
 clean:
 	git clean -ffdX
 
+.PHONY: template-update
+template-update:
+	$(TEMPLATE)/update.sh -t $(TEMPLATE) -p . -b template -i .cookiecutter.json
+
+.PHONY: template-merge
+template-merge: template-update
+	git merge template
+
 .PHONY: check-wheel
 check-wheel: dist
 	$(PYTHON) -m venv --clear --without-pip $(VENV_WHEEL)
 	cd $(VENV_WHEEL) && $(PYTHON) -m pip --isolated download pip
 	set -- $(VENV_WHEEL)/pip-*-py3-none-any.whl && $(VENV_WHEEL_PYTHON) $$1/pip install dist/$(PACKAGE)-*.whl
 	$(VENV_WHEEL_PYTHON) -m $(PACKAGE) --help
```

### Comparing `strava-gear-1.1.0a3/PKG-INFO` & `strava_gear-1.2.0b1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 Metadata-Version: 2.1
 Name: strava-gear
-Version: 1.1.0a3
+Version: 1.2.0b1
 Summary: Rule based tracker of gear and component wear primarily for Strava
 Author-email: Tomáš Janoušek <tomi@nomi.cz>
 License: MIT
 Project-URL: Homepage, https://github.com/liskin/strava-gear
-Classifier: Development Status :: 4 - Beta
+Project-URL: Release Notes, https://github.com/liskin/strava-gear/releases
+Project-URL: Issues, https://github.com/liskin/strava-gear/issues
+Project-URL: CI, https://github.com/liskin/strava-gear/actions
+Project-URL: Donations (GitHub), https://github.com/sponsors/liskin
+Project-URL: Donations (PayPal), https://www.paypal.me/lisknisi/10EUR
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -23,18 +28,18 @@
 Requires-Dist: importlib-metadata; python_version < "3.10"
 Requires-Dist: jsonschema
 Requires-Dist: platformdirs>=2.1
 Requires-Dist: python-dateutil>=2.7
 Requires-Dist: tabulate
 Provides-Extra: dev
 Requires-Dist: build>=0.7; extra == "dev"
-Requires-Dist: cram; extra == "dev"
 Requires-Dist: flake8>=3.7; extra == "dev"
 Requires-Dist: isort>=5.0; extra == "dev"
 Requires-Dist: mypy>=0.900; extra == "dev"
+Requires-Dist: prysk>=0.20.0; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: types-PyYAML; extra == "dev"
 Requires-Dist: types-python-dateutil; extra == "dev"
 Requires-Dist: types-tabulate; extra == "dev"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Provides-Extra: strava
@@ -331,15 +336,19 @@
                                       Type of report  [default: bikes]
       -f, --tablefmt TEXT             Table format, see <https://github.com/astanin/python-tabulate#table-format>.
                                       Additionally, "csv" is supported for CSV output.  [default: simple]
       --show-name / --hide-name       Show long component names  [default: show-name]
       --show-first-last / --hide-first-last
                                       Show first/last usage of components  [default: show-first-last]
       --show-vert / --hide-vert       Show vertical (elevation gain)  [default: hide-vert]
+      --show-retired / --hide-retired
+                                      Show retired bikes (on Strava)  [default: hide-retired]
       --units [metric|imperial]       Show data in metric or imperial  [default: metric]
+      --date-start ISO8601            Filter activities: start at or after the specified date(time)
+      --date-end ISO8601              Filter activities: start before the specified date(time)
       --help                          Show this message and exit.
 <!-- end include -->
 
 ## Donations (♥ = €)
 
 If you like this tool and wish to support its development and maintenance,
 please consider [a small donation](https://www.paypal.me/lisknisi/10EUR) or
```

### Comparing `strava-gear-1.1.0a3/README.md` & `strava_gear-1.2.0b1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -289,15 +289,19 @@
                                       Type of report  [default: bikes]
       -f, --tablefmt TEXT             Table format, see <https://github.com/astanin/python-tabulate#table-format>.
                                       Additionally, "csv" is supported for CSV output.  [default: simple]
       --show-name / --hide-name       Show long component names  [default: show-name]
       --show-first-last / --hide-first-last
                                       Show first/last usage of components  [default: show-first-last]
       --show-vert / --hide-vert       Show vertical (elevation gain)  [default: hide-vert]
+      --show-retired / --hide-retired
+                                      Show retired bikes (on Strava)  [default: hide-retired]
       --units [metric|imperial]       Show data in metric or imperial  [default: metric]
+      --date-start ISO8601            Filter activities: start at or after the specified date(time)
+      --date-end ISO8601              Filter activities: start before the specified date(time)
       --help                          Show this message and exit.
 <!-- end include -->
 
 ## Donations (♥ = €)
 
 If you like this tool and wish to support its development and maintenance,
 please consider [a small donation](https://www.paypal.me/lisknisi/10EUR) or
```

### Comparing `strava-gear-1.1.0a3/pyproject.toml` & `strava_gear-1.2.0b1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -9,68 +9,74 @@
 name = "strava-gear"
 description = "Rule based tracker of gear and component wear primarily for Strava"
 authors = [{name = "Tomáš Janoušek", email = "tomi@nomi.cz"}]
 license = {text = "MIT"}
 readme = {file="README.md", content-type="text/markdown"}
 dynamic = ["version"]
 classifiers = [ # https://pypi.org/classifiers/
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Utilities",
 ]
-urls = {Homepage = "https://github.com/liskin/strava-gear"}
 requires-python = "~= 3.8"
 dependencies = [
     "PyYAML",
     "click ~= 8.0",
     "importlib-metadata; python_version<'3.10'",
     "jsonschema",
     "platformdirs >= 2.1",
     "python-dateutil >= 2.7",
     "tabulate",
 ]
 
 [project.optional-dependencies]
 dev = [
     "build >= 0.7",
-    "cram",
     "flake8 >= 3.7",
     "isort >= 5.0",
     "mypy >= 0.900",
+    "prysk >= 0.20.0",
     "twine",
     "types-PyYAML",
     "types-python-dateutil",
     "types-tabulate",
 ]
 test = [
     "pytest",
 ]
 strava = [
     "strava-offline ~= 1.0",
 ]
 
+[project.urls]
+"Homepage" = "https://github.com/liskin/strava-gear"
+"Release Notes" = "https://github.com/liskin/strava-gear/releases"
+"Issues" = "https://github.com/liskin/strava-gear/issues"
+"CI" = "https://github.com/liskin/strava-gear/actions"
+"Donations (GitHub)" = "https://github.com/sponsors/liskin"
+"Donations (PayPal)" = "https://www.paypal.me/lisknisi/10EUR"
+
 [project.scripts]
 strava-gear = "strava_gear.cli:cli"
 strava-gear-sync = "strava_gear.cli_strava_offline:cli_sqlite [strava]"
 
 [tool.gha-check-distro]
 dependencies-apt = [
     "python3-bottle",
     "python3-build",
     "python3-click",
     "python3-click-option-group",
     "python3-configobj",
-    "python3-cram",
     "python3-dateutil",
     "python3-flake8",
     "python3-importlib-metadata",
     "python3-isort",
     "python3-jsonschema",
     "python3-mypy",
     "python3-pep517",
```

### Comparing `strava-gear-1.1.0a3/src/strava_gear/cli.py` & `strava_gear-1.2.0b1/src/strava_gear/cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,41 @@
+from datetime import datetime
 from pathlib import Path
+from typing import Dict
+from typing import List
 from typing import Optional
 from typing import TextIO
 
 import click
 import platformdirs
 
 from .core import apply_rules
 from .core import warn_unknown_bikes
 from .input.activities import essential_columns
 from .input.activities import read_input_csv
 from .input.activities import read_strava_offline
+from .input.date import parse_datetime
 from .input.rules import read_rules
 from .report import Units
 from .report import reports
 
 
+class DateTimeParam(click.ParamType):
+    name = "datetime"
+
+    def convert(self, value, _param, _ctx):
+        try:
+            return parse_datetime(value)
+        except ValueError as e:
+            self.fail(str(e) or "Could not parse datetime")
+
+    def get_metavar(self, _param):
+        return "ISO8601"
+
+
 @click.command(context_settings={'max_content_width': 120})
 @click.option(
     '--rules', 'rules_input', type=click.File('r'),
     default=platformdirs.user_config_path(appname=__package__) / 'rules.yaml',
     show_default=True,
     help="Rules configuration (bikes, components, ...)")
 @click.option(
@@ -51,37 +68,64 @@
 @click.option(
     '--show-first-last/--hide-first-last', default=True, show_default=True,
     help="Show first/last usage of components")
 @click.option(
     '--show-vert/--hide-vert', default=False, show_default=True,
     help="Show vertical (elevation gain)")
 @click.option(
+    '--show-retired/--hide-retired', default=False, show_default=True,
+    help="Show retired bikes (on Strava)")
+@click.option(
     '--units', type=click.Choice([u.name.lower() for u in Units]), default=Units.METRIC.name.lower(), show_default=True,
     callback=lambda _ctx, _param, v: Units[v.upper()],  # TODO: drop when Python 3.11 is the oldest supported
     help="Show data in metric or imperial")
+@click.option(
+    '--date-start', type=DateTimeParam(),
+    help="Filter activities: start at or after the specified date(time)")
+@click.option(
+    '--date-end', type=DateTimeParam(),
+    help="Filter activities: start before the specified date(time)")
 def cli(
     rules_input: TextIO,
     csv: Optional[TextIO],
     strava_database: Path,
     output: TextIO,
     report: str,
     tablefmt: str,
     show_name: bool,
     show_first_last: bool,
     show_vert: bool,
+    show_retired: bool,
     units: Units,
+    date_start: Optional[datetime],
+    date_end: Optional[datetime]
 ):
     if csv:
-        aliases, activities = read_input_csv(csv)
+        input = read_input_csv(csv)
     else:
-        aliases, activities = read_strava_offline(strava_database)
-    rules = read_rules(rules_input, aliases=aliases)
+        input = read_strava_offline(strava_database)
+    activities = activities_in_range(input.activities, date_start=date_start, date_end=date_end)
+    rules = read_rules(rules_input, aliases=input.aliases)
     res = apply_rules(rules, activities)
     reports[report](
         res,
         output=output, tablefmt=tablefmt,
         show_name=show_name,
         show_first_last=show_first_last,
         show_vert=show_vert,
+        show_bike=lambda b: show_retired or not input.bike_retired(b),
         units=units,
     )
     warn_unknown_bikes(rules, activities)
+
+
+def activities_in_range(
+    activities: List[Dict],
+    date_start: Optional[datetime],
+    date_end: Optional[datetime]
+) -> List[Dict]:
+    return [
+        a
+        for a in activities
+        if not date_start or a['start_date'] >= date_start
+        if not date_end or a['start_date'] < date_end
+    ]
```

### Comparing `strava-gear-1.1.0a3/src/strava_gear/core.py` & `strava_gear-1.2.0b1/src/strava_gear/core.py`

 * *Files identical despite different names*

### Comparing `strava-gear-1.1.0a3/src/strava_gear/data.py` & `strava_gear-1.2.0b1/src/strava_gear/data.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from dataclasses import dataclass
 from dataclasses import field
 from dataclasses import replace
 from datetime import datetime
 from datetime import timezone
 from functools import total_ordering
 from itertools import chain
+from typing import Callable
 from typing import Dict
 from typing import Iterable
 from typing import Iterator
 from typing import List
 from typing import NewType
 from typing import Optional
 from typing import Set
@@ -28,15 +29,21 @@
 HashTag = NewType('HashTag', str)
 
 Meters = NewType('Meters', float)
 Seconds = NewType('Seconds', float)
 
 ComponentMap = Dict[ComponentRole, ComponentId]
 Mapping = Dict[T, ComponentMap]
-ComponentAssignment = Tuple[BikeId, ComponentRole]
+
+
+@dataclass(frozen=True)
+class Input:
+    activities: List[Dict]
+    aliases: Dict[BikeName, BikeId] = field(default_factory=dict)
+    bike_retired: Callable[[BikeId], bool] = lambda _: False
 
 
 @total_ordering
 @dataclass(frozen=True)
 class FirstLast:
     _fl: Optional[Tuple[datetime, datetime]] = None
 
@@ -78,14 +85,20 @@
     def __str__(self) -> str:
         if self._fl is None:
             return "never"
         else:
             return f"{self.first.date()} … {self.last.date()}"
 
 
+@dataclass(order=True)
+class ComponentAssignment:
+    bike: BikeId
+    role: ComponentRole
+
+
 @dataclass(frozen=True)
 class Component:
     ident: ComponentId
     name: ComponentName
     distance: Meters = Meters(0.0)
     elevation_gain: Meters = Meters(0.0)
     time: Seconds = Seconds(0.0)
@@ -124,15 +137,15 @@
 
         other_components = {c for m in other.bikes.values() for c in m.values()}
         bikes = prune_mapping(update_mappings(filter_mapping(self.bikes, other_components), other.bikes))
         hashtags = prune_mapping(update_mappings(self.hashtags, other.hashtags))
         return replace(other, bikes=bikes, hashtags=hashtags)
 
     def component_assignments(self) -> Dict[ComponentId, ComponentAssignment]:
-        return {c: (b, t) for b, m in self.bikes.items() for t, c in m.items()}
+        return {c: ComponentAssignment(b, t) for b, m in self.bikes.items() for t, c in m.items()}
 
     def all_component_ids(self) -> Iterator[ComponentId]:
         """Return all component ids mentioned in this rule."""
         for m in chain(self.bikes.values(), self.hashtags.values()):
             for c in m.values():
                 if c is not None:
                     yield c
```

### Comparing `strava-gear-1.1.0a3/src/strava_gear/input/date.py` & `strava_gear-1.2.0b1/src/strava_gear/input/date.py`

 * *Files identical despite different names*

### Comparing `strava-gear-1.1.0a3/src/strava_gear/input/rules.py` & `strava_gear-1.2.0b1/src/strava_gear/input/rules.py`

 * *Files identical despite different names*

### Comparing `strava-gear-1.1.0a3/src/strava_gear/report.py` & `strava_gear-1.2.0b1/src/strava_gear/report.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from collections import defaultdict
 import csv
 from enum import Enum
 from enum import auto
 from functools import partial
+from typing import Callable
 from typing import Dict
 from typing import Final
 from typing import Iterator
 
 from tabulate import tabulate
 
 from .data import BikeId
@@ -27,14 +28,15 @@
     f,
     res: Result,
     output,
     tablefmt: str,
     show_name: bool,
     show_first_last: bool,
     show_vert: bool,
+    show_bike: Callable[[BikeId], bool],
     units: Units,
 ):
     def cols(d: Dict) -> Dict:
         if not show_name:
             del d["name"]
         if not show_first_last:
             del d["first … last"]
@@ -46,55 +48,59 @@
         else:
             del d["mi"]
             del d["vert ft"]
             if not show_vert:
                 del d["vert m"]
         return d
 
-    table = [cols(d) for d in f(res)]
+    table = [cols(d) for d in f(res, show_bike=show_bike)]
     if not table:
         return
 
     if tablefmt == 'csv':
         writer = csv.DictWriter(output, fieldnames=list(table[0].keys()), lineterminator='\n')
         writer.writeheader()
         writer.writerows(table)
     else:
         print(tabulate(table, headers="keys", floatfmt=".1f", tablefmt=tablefmt), file=output)
 
 
-def report_components(res: Result) -> Iterator[Dict]:
+def report_components(res: Result, **_kwargs) -> Iterator[Dict]:
     for c in sorted(res.components, key=lambda c: (c.firstlast, c.ident,)):
         yield {
             "id": c.ident,
             "name": c.name,
             "km": c.distance / 1000,
             "mi": c.distance / MILE_IN_METERS,
             "vert m": c.elevation_gain,
             "vert ft": c.elevation_gain / FOOT_IN_METERS,
             "hour": c.time / 3600,
             "first … last": c.firstlast,
         }
 
 
-def report_bikes(res: Result) -> Iterator[Dict]:
+def report_bikes(res: Result, show_bike: Callable[[BikeId], bool]) -> Iterator[Dict]:
     bikes_firstlasts = bikes_firstlast(res)
 
     def sort_key(c: Component):
         assert c.assignment
-        b, t = c.assignment
+        return bikes_firstlasts[c.assignment.bike], c.assignment
 
-        return bikes_firstlasts[b], b, t
-
-    for c in sorted((c for c in res.components if c.assignment), key=sort_key):
+    for c in sorted((
+            c
+            for c in res.components
+            if c.assignment
+            if show_bike(c.assignment.bike)
+        ),
+        key=sort_key
+    ):
         assert c.assignment
-        b, t = c.assignment
         yield {
-            "bike": res.bike_names.get(b, b),
-            "role": t,
+            "bike": res.bike_names.get(c.assignment.bike, c.assignment.bike),
+            "role": c.assignment.role,
             "id": c.ident,
             "name": c.name,
             "km": c.distance / 1000,
             "mi": c.distance / MILE_IN_METERS,
             "vert m": c.elevation_gain,
             "vert ft": c.elevation_gain / FOOT_IN_METERS,
             "hour": c.time / 3600,
@@ -102,16 +108,15 @@
         }
 
 
 def bikes_firstlast(res: Result) -> Dict[BikeId, FirstLast]:
     fl: Dict[BikeId, FirstLast] = defaultdict(FirstLast)
     for c in res.components:
         if c.assignment:
-            b, _ = c.assignment
-            fl[b] += c.firstlast
+            fl[c.assignment.bike] += c.firstlast
     return fl
 
 
 reports = {
     'components': partial(report, report_components),
     'bikes': partial(report, report_bikes),
 }
```

### Comparing `strava-gear-1.1.0a3/src/strava_gear.egg-info/PKG-INFO` & `strava_gear-1.2.0b1/src/strava_gear.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 Metadata-Version: 2.1
 Name: strava-gear
-Version: 1.1.0a3
+Version: 1.2.0b1
 Summary: Rule based tracker of gear and component wear primarily for Strava
 Author-email: Tomáš Janoušek <tomi@nomi.cz>
 License: MIT
 Project-URL: Homepage, https://github.com/liskin/strava-gear
-Classifier: Development Status :: 4 - Beta
+Project-URL: Release Notes, https://github.com/liskin/strava-gear/releases
+Project-URL: Issues, https://github.com/liskin/strava-gear/issues
+Project-URL: CI, https://github.com/liskin/strava-gear/actions
+Project-URL: Donations (GitHub), https://github.com/sponsors/liskin
+Project-URL: Donations (PayPal), https://www.paypal.me/lisknisi/10EUR
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -23,18 +28,18 @@
 Requires-Dist: importlib-metadata; python_version < "3.10"
 Requires-Dist: jsonschema
 Requires-Dist: platformdirs>=2.1
 Requires-Dist: python-dateutil>=2.7
 Requires-Dist: tabulate
 Provides-Extra: dev
 Requires-Dist: build>=0.7; extra == "dev"
-Requires-Dist: cram; extra == "dev"
 Requires-Dist: flake8>=3.7; extra == "dev"
 Requires-Dist: isort>=5.0; extra == "dev"
 Requires-Dist: mypy>=0.900; extra == "dev"
+Requires-Dist: prysk>=0.20.0; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: types-PyYAML; extra == "dev"
 Requires-Dist: types-python-dateutil; extra == "dev"
 Requires-Dist: types-tabulate; extra == "dev"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Provides-Extra: strava
@@ -331,15 +336,19 @@
                                       Type of report  [default: bikes]
       -f, --tablefmt TEXT             Table format, see <https://github.com/astanin/python-tabulate#table-format>.
                                       Additionally, "csv" is supported for CSV output.  [default: simple]
       --show-name / --hide-name       Show long component names  [default: show-name]
       --show-first-last / --hide-first-last
                                       Show first/last usage of components  [default: show-first-last]
       --show-vert / --hide-vert       Show vertical (elevation gain)  [default: hide-vert]
+      --show-retired / --hide-retired
+                                      Show retired bikes (on Strava)  [default: hide-retired]
       --units [metric|imperial]       Show data in metric or imperial  [default: metric]
+      --date-start ISO8601            Filter activities: start at or after the specified date(time)
+      --date-end ISO8601              Filter activities: start before the specified date(time)
       --help                          Show this message and exit.
 <!-- end include -->
 
 ## Donations (♥ = €)
 
 If you like this tool and wish to support its development and maintenance,
 please consider [a small donation](https://www.paypal.me/lisknisi/10EUR) or
```

### Comparing `strava-gear-1.1.0a3/src/strava_gear.egg-info/SOURCES.txt` & `strava_gear-1.2.0b1/src/strava_gear.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -22,14 +22,13 @@
 src/strava_gear.egg-info/entry_points.txt
 src/strava_gear.egg-info/requires.txt
 src/strava_gear.egg-info/top_level.txt
 src/strava_gear/input/__init__.py
 src/strava_gear/input/activities.py
 src/strava_gear/input/date.py
 src/strava_gear/input/rules.py
-tests/cram-noescape.py
 tests/csv.md
 tests/include.py
 tests/test_data.py
 tests/test_input_date.py
 tests/test_input_rules.py
 tests/readme/help.md
```

### Comparing `strava-gear-1.1.0a3/tests/csv.md` & `strava_gear-1.2.0b1/tests/csv.md`

 * *Files 15% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     > }
 
 Rules:
 
     $ cat >rules.yaml <<END
     > rules:
     >   - road:
+    >       frame: fr
     >       chain: c1
     >   - since: 2023-01-01
     >     road:
     >       chain: c2
     >   - since: 2024-01-01
     >     road:
     >       chain: c3
@@ -28,52 +29,72 @@
     > name,gear_id,start_date,moving_time,distance,total_elevation_gain
     > Ride 1,road,2022-01-01,3600,1000,10
     > Ride 2,road,2023-01-01,3600,1000,10
     > Ride 3,road,2023-02-01,3600,1000,10
     > END
     bike,role,id,name,km,hour,first … last
     road,chain,c3,c3,0.0,0.0,never
+    road,frame,fr,fr,3.0,3.0,2022-01-01 … 2023-02-01
 
 Components report:
 
-    $ strava-gear --report components <<END
+    $ strava-gear --report components <<END | grep -v ^fr,
     > name,gear_id,start_date,moving_time,distance,total_elevation_gain
     > Ride 1,road,2022-01-01,3600,1000,10
     > Ride 2,road,2023-01-01,3600,1000,10
     > Ride 3,road,2023-02-01,3600,1000,10
     > END
     id,name,km,hour,first … last
     c3,c3,0.0,0.0,never
     c5,c5,0.0,0.0,never
     c1,c1,1.0,1.0,2022-01-01 … 2022-01-01
     c2,c2,1.0,1.0,2023-01-01 … 2023-01-01
     c4,c4,1.0,1.0,2023-02-01 … 2023-02-01
 
 VirtualRide virtual hashtag:
 
-    $ strava-gear --report components <<END
+    $ strava-gear --report components <<END | grep -v ^fr,
     > name,gear_id,start_date,moving_time,distance,total_elevation_gain,type
     > Ride 1,road,2022-01-01,3600,1000,10,Ride
     > Ride 2,road,2023-01-01,3600,1000,10,Ride
     > Ride 4,road,2023-02-01,3600,1000,10,VirtualRide
     > END
     id,name,km,hour,first … last
     c3,c3,0.0,0.0,never
     c4,c4,0.0,0.0,never
     c1,c1,1.0,1.0,2022-01-01 … 2022-01-01
     c2,c2,1.0,1.0,2023-01-01 … 2023-01-01
     c5,c5,1.0,1.0,2023-02-01 … 2023-02-01
 
 Components report imperial:
 
-    $ strava-gear --report components --units imperial <<END
+    $ strava-gear --report components --units imperial <<END | grep -v ^fr,
     > name,gear_id,start_date,moving_time,distance,total_elevation_gain
     > Ride 1,road,2022-01-01,3600,1000,10
     > Ride 2,road,2023-01-01,3600,1000,10
     > Ride 3,road,2023-02-01,3600,1000,10
     > END
     id,name,mi,hour,first … last
     c3,c3,0.0,0.0,never
     c5,c5,0.0,0.0,never
     c1,c1,0.621371192237334,1.0,2022-01-01 … 2022-01-01
     c2,c2,0.621371192237334,1.0,2023-01-01 … 2023-01-01
     c4,c4,0.621371192237334,1.0,2023-02-01 … 2023-02-01
+
+Date range:
+
+    $ strava-gear --date-start 2023-01-01 <<END | grep frame
+    > name,gear_id,start_date,moving_time,distance,total_elevation_gain
+    > Ride 1,road,2022-01-01,3600,1000,10
+    > Ride 2,road,2023-01-01,3600,1000,10
+    > Ride 3,road,2023-02-01,3600,1000,10
+    > END
+    road,frame,fr,fr,2.0,2.0,2023-01-01 … 2023-02-01
+
+    $ strava-gear --date-end 2023-02-01 <<END | grep frame
+    > name,gear_id,start_date,moving_time,distance,total_elevation_gain
+    > Ride 1,road,2022-01-01,3600,1000,10
+    > Ride 2,road,2023-01-01,3600,1000,10
+    > Ride 3,road,2023-02-01,3600,1000,10
+    > END
+    road,frame,fr,fr,2.0,2.0,2022-01-01 … 2023-01-01
+
```

### Comparing `strava-gear-1.1.0a3/tests/readme/help.md` & `strava_gear-1.2.0b1/tests/readme/help.md`

 * *Files 14% similar despite different names*

```diff
@@ -17,9 +17,13 @@
                                       Type of report  [default: bikes]
       -f, --tablefmt TEXT             Table format, see <https://github.com/astanin/python-tabulate#table-format>.
                                       Additionally, "csv" is supported for CSV output.  [default: simple]
       --show-name / --hide-name       Show long component names  [default: show-name]
       --show-first-last / --hide-first-last
                                       Show first/last usage of components  [default: show-first-last]
       --show-vert / --hide-vert       Show vertical (elevation gain)  [default: hide-vert]
+      --show-retired / --hide-retired
+                                      Show retired bikes (on Strava)  [default: hide-retired]
       --units [metric|imperial]       Show data in metric or imperial  [default: metric]
+      --date-start ISO8601            Filter activities: start at or after the specified date(time)
+      --date-end ISO8601              Filter activities: start before the specified date(time)
       --help                          Show this message and exit.
```

### Comparing `strava-gear-1.1.0a3/tests/test_data.py` & `strava_gear-1.2.0b1/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `strava-gear-1.1.0a3/tests/test_input_date.py` & `strava_gear-1.2.0b1/tests/test_input_date.py`

 * *Files identical despite different names*

### Comparing `strava-gear-1.1.0a3/tests/test_input_rules.py` & `strava_gear-1.2.0b1/tests/test_input_rules.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
     assert rd("rules:\n - since: 2020-05-01T14:00")
     assert rd("rules:\n - since: 2020-05-01T14:00+02:00")
 
 
 def test_validation_fails():
     with pytest.raises(ValidationError) as e:
         rd("rules: []")
-    assert "[] is too short" in str(e.value)
+    assert "[] is too short" in str(e.value) or "[] should be non-empty" in str(e.value)
     assert list(e.value.absolute_path) == ['rules']
 
     with pytest.raises(ValidationError) as e:
         rd("xxx:")
     assert "unexpected" in str(e.value)
     assert list(e.value.absolute_path) == []
```

