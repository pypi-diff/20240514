# Comparing `tmp/jupyterlab_new_launcher-0.2.3.tar.gz` & `tmp/jupyterlab_new_launcher-0.3.0.tar.gz`

## Comparing `jupyterlab_new_launcher-0.2.3.tar` & `jupyterlab_new_launcher-0.3.0.tar`

### file list

```diff
@@ -1,61 +1,64 @@
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/.copier-answers.yml
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/.prettierignore
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/.yarnrc.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/CHANGELOG.md
--rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/babel.config.js
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/install.json
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/jest.config.js
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/junit.xml
--rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/setup.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/tsconfig.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/tsconfig.test.json
--rw-r--r--   0        0        0   376569 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/yarn.lock
--rw-r--r--   0        0        0    54951 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/docs/images/dialog.png
--rw-r--r--   0        0        0    58321 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/docs/images/launcher.png
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/jupyterlab_new_launcher/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/jupyterlab_new_launcher/_version.py
--rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/jupyterlab_new_launcher/labextension/package.json
--rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/package.json.orig
--rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/plugin.json
--rw-r--r--   0        0        0    24938 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/jupyterlab_new_launcher/labextension/static/239.a28bc3eddd733aecbd06.js
--rw-r--r--   0        0        0     9025 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/jupyterlab_new_launcher/labextension/static/728.fa379db84cb7d3fbc55e.js
--rw-r--r--   0        0        0     7174 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/jupyterlab_new_launcher/labextension/static/remoteEntry.beb3c4798d84f1b62e25.js
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/jupyterlab_new_launcher/labextension/static/style.js
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/jupyterlab_new_launcher/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/schema/plugin.json
--rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/src/commands.ts
--rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/src/database.ts
--rw-r--r--   0        0        0     9470 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/src/dialogs.tsx
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/src/icons.ts
--rw-r--r--   0        0        0     5562 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/src/index.ts
--rw-r--r--   0        0        0     4729 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/src/item.ts
--rw-r--r--   0        0        0    10196 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/src/launcher.tsx
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/src/svg.d.ts
--rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/src/types.ts
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/src/__tests__/jupyterlab_new_launcher.spec.ts
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/src/components/card.tsx
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/src/components/section.tsx
--rw-r--r--   0        0        0    11435 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/src/components/table.tsx
--rw-r--r--   0        0        0     4897 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/style/index.js
--rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/style/icons/code-server.svg
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/style/icons/md/LICENSE
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/style/icons/md/file.svg
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/style/icons/md/star.svg
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/ui-tests/README.md
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/ui-tests/playwright.config.js
--rw-r--r--   0        0        0   148126 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/ui-tests/yarn.lock
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/ui-tests/tests/jupyterlab_new_launcher.spec.ts
--rw-r--r--   0        0        0    26996 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-linux.png
--rw-r--r--   0        0        0    27431 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-search-in-individual-linux.png
--rw-r--r--   0        0        0    33351 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-with-starred-linux.png
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/.gitignore
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/LICENSE
--rw-r--r--   0        0        0     3441 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/README.md
--rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     6392 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/.copier-answers.yml
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/.prettierignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/babel.config.js
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/install.json
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/jest.config.js
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/junit.xml
+-rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/setup.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/tsconfig.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/tsconfig.test.json
+-rw-r--r--   0        0        0   376569 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/yarn.lock
+-rw-r--r--   0        0        0    54951 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/docs/images/dialog.png
+-rw-r--r--   0        0        0    58321 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/docs/images/launcher.png
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/jupyterlab_new_launcher/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/jupyterlab_new_launcher/_version.py
+-rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/jupyterlab_new_launcher/labextension/package.json
+-rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/package.json.orig
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/plugin.json
+-rw-r--r--   0        0        0    11071 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/jupyterlab_new_launcher/labextension/static/728.5be4ee0b94a07decd5f8.js
+-rw-r--r--   0        0        0    28571 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/jupyterlab_new_launcher/labextension/static/787.d3e306a9eb8983db2644.js
+-rw-r--r--   0        0        0     7174 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/jupyterlab_new_launcher/labextension/static/remoteEntry.697e41989e560bf8e1db.js
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/jupyterlab_new_launcher/labextension/static/style.js
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/jupyterlab_new_launcher/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/schema/plugin.json
+-rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/src/commands.ts
+-rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/src/database.ts
+-rw-r--r--   0        0        0     9601 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/src/dialogs.tsx
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/src/icons.ts
+-rw-r--r--   0        0        0     6052 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/src/index.ts
+-rw-r--r--   0        0        0     4729 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/src/item.ts
+-rw-r--r--   0        0        0    10204 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/src/launcher.tsx
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/src/svg.d.ts
+-rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/src/types.ts
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/src/typings.d.ts
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/src/__tests__/jupyterlab_new_launcher.spec.ts
+-rw-r--r--   0        0        0     6346 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/src/components/base-table.tsx
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/src/components/card.tsx
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/src/components/section.tsx
+-rw-r--r--   0        0        0    12213 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/src/components/table.tsx
+-rw-r--r--   0        0        0     6844 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/style/index.js
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/style/webkit.raw.css
+-rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/style/icons/code-server.svg
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/style/icons/md/LICENSE
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/style/icons/md/file.svg
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/style/icons/md/star.svg
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/ui-tests/README.md
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0   148126 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/ui-tests/yarn.lock
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/ui-tests/tests/jupyterlab_new_launcher.spec.ts
+-rw-r--r--   0        0        0    27608 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-linux.png
+-rw-r--r--   0        0        0    28063 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-search-in-individual-linux.png
+-rw-r--r--   0        0        0    33928 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-with-starred-linux.png
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3441 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/README.md
+-rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6392 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.0/PKG-INFO
```

### Comparing `jupyterlab_new_launcher-0.2.3/.copier-answers.yml` & `jupyterlab_new_launcher-0.3.0/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.3/RELEASE.md` & `jupyterlab_new_launcher-0.3.0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.3/jest.config.js` & `jupyterlab_new_launcher-0.3.0/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.3/package.json` & `jupyterlab_new_launcher-0.3.0/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'0.3.0'"}*

```diff
@@ -195,9 +195,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.2.3"
+    "version": "0.3.0"
 }
```

### Comparing `jupyterlab_new_launcher-0.2.3/tsconfig.json` & `jupyterlab_new_launcher-0.3.0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.3/yarn.lock` & `jupyterlab_new_launcher-0.3.0/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.3/docs/images/dialog.png` & `jupyterlab_new_launcher-0.3.0/docs/images/dialog.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.3/docs/images/launcher.png` & `jupyterlab_new_launcher-0.3.0/docs/images/launcher.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.3/jupyterlab_new_launcher/__init__.py` & `jupyterlab_new_launcher-0.3.0/jupyterlab_new_launcher/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.3/jupyterlab_new_launcher/labextension/package.json` & `jupyterlab_new_launcher-0.3.0/jupyterlab_new_launcher/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9788194444444445%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.697e41989e560bf8e1db.js'}}",*

 * * "'version'": "'0.3.0'"}*

```diff
@@ -108,15 +108,15 @@
         "src/**/*.{ts,tsx}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/nebari-dev/jupyterlab-new-launcher",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.beb3c4798d84f1b62e25.js",
+            "load": "static/remoteEntry.697e41989e560bf8e1db.js",
             "style": "./style"
         },
         "disabledExtensions": [
             "@jupyterlab/launcher-extension",
             "@jupyterlab/apputils-extension:sessionDialogs"
         ],
         "extension": true,
@@ -200,9 +200,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.2.3"
+    "version": "0.3.0"
 }
```

### Comparing `jupyterlab_new_launcher-0.2.3/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/package.json.orig` & `jupyterlab_new_launcher-0.3.0/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'0.3.0'"}*

```diff
@@ -195,9 +195,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.2.3"
+    "version": "0.3.0"
 }
```

### Comparing `jupyterlab_new_launcher-0.2.3/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/plugin.json` & `jupyterlab_new_launcher-0.3.0/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/plugin.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996527777777777%*

 * *Differences: {"'properties'": "{'hiddenColumns': {'default': {'conda_language': 'hidden', "*

 * *                 "'conda_is_base_environment': 'hidden', 'conda_is_currently_running': 'hidden'}}}"}*

```diff
@@ -56,14 +56,17 @@
                     "visible",
                     "hidden"
                 ],
                 "type": "string"
             },
             "default": {
                 "conda_env_path": "hidden",
+                "conda_is_base_environment": "hidden",
+                "conda_is_currently_running": "hidden",
+                "conda_language": "hidden",
                 "conda_raw_kernel_name": "hidden"
             },
             "title": "Hidden columns",
             "type": "object"
         },
         "searchAllSections": {
             "default": true,
```

### Comparing `jupyterlab_new_launcher-0.2.3/jupyterlab_new_launcher/labextension/static/239.a28bc3eddd733aecbd06.js` & `jupyterlab_new_launcher-0.3.0/jupyterlab_new_launcher/labextension/static/787.d3e306a9eb8983db2644.js`

 * *Files 13% similar despite different names*

#### js-beautify {}

```diff
@@ -1,40 +1,41 @@
 "use strict";
 (self.webpackChunkjupyterlab_new_launcher = self.webpackChunkjupyterlab_new_launcher || []).push([
-    [239], {
-        239: (e, t, n) => {
+    [787], {
+        787: (e, t, n) => {
             n.r(t), n.d(t, {
-                default: () => F
+                default: () => V
             });
             var a = n(626),
                 s = n(923),
                 o = n(670),
                 r = n(260),
                 l = n(825),
                 c = n(265),
                 i = n(527),
                 d = n(53),
-                m = n(345);
-            const u = new i.LabIcon({
+                m = n(345),
+                u = n.n(m);
+            const h = new i.LabIcon({
                     name: "jupyterlab-new-launcher:star",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">\n  <path class="jp-icon3 jp-star-filled" fill="rgb(97,97,97)" d="M12 17.27L18.18 21l-1.64-7.03L22 9.24l-7.19-.61L12 2 9.19 8.63 2 9.24l5.46 4.73L5.82 21z" />\n  <path class="jp-icon3 jp-star-border" fill="rgb(97,97,97)" d="M22 9.24l-7.19-.62L12 2 9.19 8.63 2 9.24l5.46 4.73L5.82 21 12 17.27 18.18 21l-1.63-7.03L22 9.24zM12 15.4l-3.76 2.27 1-4.28-3.32-2.88 4.38-.38L12 6.1l1.71 4.04 4.38.38-3.32 2.88 1 4.28L12 15.4z" />\n</svg>\n'
                 }),
-                h = new i.LabIcon({
+                p = new i.LabIcon({
                     name: "jupyterlab-new-launcher:file",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">\n  <path class="jp-icon3" fill="rgb(97,97,97)" d="M13.81 22H6C4.89 22 4 21.11 4 20V4C4 2.9 4.89 2 6 2H14L20 8V13.09C19.67 13.04 19.34 13 19 13S18.33 13.04 18 13.09V9H13V4H6V20H13.09C13.21 20.72 13.46 21.39 13.81 22M23 18H20V15H18V18H15V20H18V23H20V20H23V18Z" />\n</svg>'
                 }),
-                p = new i.LabIcon({
+                g = new i.LabIcon({
                     name: "jupyterlab-new-launcher:code-server",
                     svgstr: '<svg width="64" viewBox="0 0 2250 2250" version="1.1" xmlns="http://www.w3.org/2000/svg" style="fill-rule:evenodd;clip-rule:evenodd;stroke-linejoin:round;stroke-miterlimit:2;">\n<g class="jp-icon0" fill="#000" style="fill-rule:nonzero;">\n  <path d="M1991.66,1034.72c-38.493,0 -64.144,-22.57 -64.144,-68.897l-0,-266.084c-0,-169.867 -69.982,-263.709 -250.762,-263.709l-83.976,0l-0,179.368l25.661,0c71.144,0 104.967,39.201 104.967,109.285l0,235.201c0,102.156 30.324,143.733 96.806,165.114c-66.482,20.196 -96.806,62.958 -96.806,165.114l0,174.621c0,48.7 0,96.216 -12.829,144.917c-12.829,45.141 -33.823,87.903 -62.98,124.726c-16.329,21.386 -34.991,39.202 -55.981,55.835l-0,23.755l83.971,-0c180.781,-0 250.763,-93.843 250.763,-263.709l-0,-266.084c-0,-47.516 24.485,-68.897 64.144,-68.897l47.822,-0l-0,-179.37l-46.656,-0l0,-1.186Z"/>\n  <path d="M1420.16,706.904l-258.923,0c-5.833,0 -10.495,-4.752 -10.495,-10.691l-0,-20.192c-0,-5.941 4.662,-10.692 10.495,-10.692l260.089,0c5.83,0 10.495,4.751 10.495,10.692l0,20.192c0,5.939 -5.833,10.691 -11.661,10.691Z" />\n  <path d="M1464.48,963.474l-188.942,0c-5.833,0 -10.501,-4.754 -10.501,-10.693l0,-20.192c0,-5.938 4.668,-10.691 10.501,-10.691l188.942,-0c5.833,-0 10.495,4.753 10.495,10.691l-0,20.192c-0,4.754 -4.662,10.693 -10.495,10.693Z"/>\n  <path d="M1539.12,835.188l-377.885,0c-5.833,0 -10.495,-4.75 -10.495,-10.689l-0,-20.196c-0,-5.939 4.662,-10.69 10.495,-10.69l376.719,0c5.833,0 10.499,4.751 10.499,10.69l-0,20.196c-0,4.75 -3.5,10.689 -9.333,10.689Z"/>\n  <path d="M861.493,765.074c25.658,0 51.319,2.376 75.811,8.316l0,-48.705c0,-68.897 34.989,-109.285 104.971,-109.285l25.658,0l-0,-179.368l-83.977,0c-180.781,0 -250.758,93.842 -250.758,263.709l0,87.901c40.819,-14.252 83.977,-22.568 128.295,-22.568Z"/>\n  <path d="M1618.44,1411.25c-18.662,-150.861 -132.962,-276.776 -279.919,-305.285c-40.818,-8.314 -81.642,-9.504 -121.295,-2.376c-1.166,-0 -1.166,-1.189 -2.332,-1.189c-64.148,-136.605 -201.772,-226.884 -351.063,-226.884c-149.289,-0 -285.747,87.905 -351.062,224.51c-1.166,-0 -1.166,1.188 -2.332,1.188c-41.987,-4.753 -83.975,-2.379 -125.963,8.314c-144.623,35.634 -254.257,159.175 -274.085,308.847c-2.332,15.441 -3.499,30.883 -3.499,45.141c0,45.136 30.325,86.713 74.645,92.652c54.817,8.317 102.636,-34.448 101.469,-89.089c0,-8.317 0,-17.821 1.167,-26.134c9.331,-76.025 66.48,-140.168 141.123,-157.99c23.328,-5.939 46.654,-7.124 68.814,-3.559c71.146,9.502 141.124,-27.324 171.449,-91.467c22.162,-47.516 57.151,-89.094 103.804,-111.664c51.314,-24.946 109.633,-28.506 163.286,-9.499c55.979,20.192 97.966,62.954 123.627,116.409c26.824,52.27 39.653,89.093 96.805,96.221c23.325,3.559 88.639,2.374 113.132,1.185c47.82,0 95.64,16.631 129.463,51.079c22.156,23.757 38.485,53.455 45.486,86.715c10.495,53.455 -2.334,106.908 -33.825,147.296c-22.162,28.509 -52.485,49.89 -86.308,59.394c-16.329,4.754 -32.657,5.939 -48.986,5.939l-257.757,0c-51.314,0 -92.138,-41.573 -92.138,-93.842l0,-348.049c0,-14.251 -11.661,-26.13 -25.658,-26.13l-36.156,0c-71.148,1.185 -128.295,81.964 -128.295,167.488l-0,312.415c-0,92.652 73.476,167.488 164.451,167.488c0,0 404.714,-1.19 410.544,-1.19c93.304,-9.503 179.614,-58.204 237.927,-133.04c58.319,-72.46 85.142,-167.492 73.481,-264.894Z"/>\n</g></svg>'
                 });
-            var g = n(602);
-            class v {
+            var v = n(602);
+            class f {
                 constructor(e) {
                     var t, n, a, s, o;
-                    this._options = e, this._refreshLastUsed = new g.Signal(this), this._refreshClock = null, this._lastUsed = null;
+                    this._options = e, this._refreshLastUsed = new v.Signal(this), this._refreshClock = null, this._lastUsed = null;
                     const {
                         item: r,
                         commands: l,
                         lastUsedDatabase: c,
                         favoritesDatabase: i,
                         cwd: d
                     } = e, m = {
@@ -46,22 +47,22 @@
                     if (u) {
                         const e = (null !== (a = u.conda_env_name) && void 0 !== a ? a : "").match(/(?<namespace>.+)-(?<duplicate>\1)-(?<environment>.+)/);
                         if (e && this.metadata) {
                             const t = e.groups;
                             this.label = null !== (s = u.conda_language) && void 0 !== s ? s : t.environment, this.metadata = {
                                 ...this.metadata,
                                 kernel: {
-                                    ...u,
+                                    Namespace: t.namespace,
                                     conda_env_name: t.environment,
-                                    Namespace: t.namespace
+                                    ...u
                                 }
                             }
                         }
                     }
-                    "server-proxy:open" === this.command && (null === (o = this.kernelIconUrl) || void 0 === o ? void 0 : o.endsWith("/vscode")) && (this.icon = p)
+                    "server-proxy:open" === this.command && (null === (o = this.kernelIconUrl) || void 0 === o ? void 0 : o.endsWith("/vscode")) && (this.icon = g)
                 }
                 get lastUsed() {
                     return this._lastUsed
                 }
                 set lastUsed(e) {
                     this._lastUsed = e, this._setRefreshClock()
                 }
@@ -96,26 +97,144 @@
                     const t = Date.now() - e.getTime(),
                         n = t < 6e4 ? 1e4 : t < 36e5 ? 6e4 : 36e5;
                     this._refreshClock = window.setTimeout((() => {
                         this._refreshLastUsed.emit(), this._setRefreshClock()
                     }), n)
                 }
             }
-            var f = n(702),
-                _ = n(262);
-            const b = "jupyterlab-new-launcher:plugin";
-            var w;
+            var b = n(702);
+            const _ = "jp-sortable-table";
+
+            function w(e) {
+                const [t, n] = (0, m.useState)({
+                    sortKey: e.sortKey,
+                    sortDirection: e.sortDirection || 1
+                });
+                let a = e.rows;
+                const s = e.columns.filter((e => e.id === t.sortKey))[0];
+                if (s) {
+                    const n = s.sort.bind(s);
+                    a = e.rows.sort(((e, a) => {
+                        var s;
+                        return (null !== (s = n(e.data, a.data)) && void 0 !== s ? s : 0) * t.sortDirection
+                    }))
+                }
+                const o = e.columns.filter((e => (!e.isAvailable || e.isAvailable()) && !e.isHidden)),
+                    [r, l] = u().useState({}),
+                    c = a.map((t => {
+                        const n = o.map((e => u().createElement("td", {
+                            key: e.id + "-" + t.key,
+                            className: r[e.id] ? "jp-mod-col-resized" : ""
+                        }, e.renderCell(t.data))));
+                        return u().createElement("tr", {
+                            key: t.key,
+                            "data-key": t.key,
+                            onClick: e.onRowClick,
+                            className: "jp-sortable-table-tr"
+                        }, n)
+                    })),
+                    i = o.map((e => u().createElement(y, {
+                        label: e.label,
+                        id: e.id,
+                        state: t,
+                        key: e.id,
+                        onSort: () => {
+                            var a;
+                            (a = e.id) === t.sortKey ? n({
+                                sortKey: a,
+                                sortDirection: -1 * t.sortDirection
+                            }) : n({
+                                sortKey: a,
+                                sortDirection: 1
+                            })
+                        },
+                        onResize: () => {
+                            l({
+                                ...r,
+                                [e.id]: !0
+                            })
+                        },
+                        minWidth: e.minWidth
+                    })));
+                return u().createElement("table", {
+                    className: _
+                }, u().createElement("thead", null, u().createElement("tr", {
+                    className: "jp-sortable-table-tr"
+                }, i)), u().createElement("tbody", null, c))
+            }
+
+            function y(e) {
+                var t;
+                const n = e.id === e.state.sortKey,
+                    a = n && 1 !== e.state.sortDirection ? i.caretDownIcon : i.caretUpIcon,
+                    [s, o] = u().useState(null),
+                    r = u().useRef(null),
+                    [l, c] = u().useState(!1),
+                    [d, h] = (0, m.useState)(null);
+                requestAnimationFrame((() => {
+                    if (r.current) {
+                        const {
+                            left: e
+                        } = r.current.getBoundingClientRect();
+                        h(e)
+                    }
+                })), u().useEffect((() => {
+                    const t = t => {
+                            if (l) {
+                                let n;
+                                if (null === d) {
+                                    if (!r.current) throw Error("Cannot resize: no reference to the current table");
+                                    console.warn("Resize cache for column was not available"), n = r.current.getBoundingClientRect().left
+                                } else n = d;
+                                o(t.clientX - n), e.onResize()
+                            }
+                        },
+                        n = e => {
+                            l && (document.body.classList.remove(v), c(!1), e.stopImmediatePropagation())
+                        };
+                    return document.body.addEventListener("pointermove", t), document.body.addEventListener("pointerup", n), () => {
+                        document.body.removeEventListener("pointermove", t), document.body.removeEventListener("pointerup", n)
+                    }
+                }));
+                const p = [];
+                n && p.push("jp-sorted-header"), l && p.push("jp-header-resizing");
+                const g = "jp-sortable-table-resize-handle",
+                    v = "jp-mod-resize-table";
+                return u().createElement("th", {
+                    key: e.id,
+                    ref: r,
+                    onClick: () => e.onSort(),
+                    className: p.join(" "),
+                    "data-id": e.id,
+                    style: {
+                        width: null !== s ? `${Math.max(null!==(t=e.minWidth)&&void 0!==t?t:50,s)}px` : ""
+                    },
+                    onPointerDown: e => {
+                        e.target instanceof HTMLElement && e.target.className === g && (document.body.classList.add(v), c(!0))
+                    }
+                }, u().createElement("div", {
+                    className: "jp-sortable-table-th-wrapper"
+                }, u().createElement("label", null, e.label), u().createElement(a.react, {
+                    tag: "span",
+                    className: "jp-sort-icon"
+                })), u().createElement("div", {
+                    className: g
+                }))
+            }
+            var C = n(262);
+            const k = "jupyterlab-new-launcher:plugin";
+            var E;
             ! function(e) {
                 e.create = "launcher:create", e.moveColumn = "new-launcher:table-move-column", e.toggleColumn = "new-launcher:table-toggle-column"
-            }(w || (w = {}));
-            const y = new _.Token("jupyterlab-new-launcher:ILauncherDatabase", "Databases for new launcher."),
-                C = "jp-starIconButton",
-                k = "jp-TableKernelItem";
+            }(E || (E = {}));
+            const j = new C.Token("jupyterlab-new-launcher:ILauncherDatabase", "Databases for new launcher."),
+                D = "jp-starIconButton",
+                L = "jp-TableKernelItem";
 
-            function L(e) {
+            function N(e) {
                 if (0 === e.length) return "(empty)";
                 switch (e) {
                     case "conda_env_name":
                         return "Environment";
                     case "conda_env_path":
                         return "Environment path";
                     case "conda_language":
@@ -126,37 +245,48 @@
                         return "Base?";
                     case "conda_is_currently_running":
                         return "Running?"
                 }
                 return e[0].toUpperCase() + e.substring(1)
             }
 
-            function D(e) {
+            function S(e) {
+                return m.createElement("div", {
+                    className: "jp-ellipsis-wrapper",
+                    title: e.title
+                }, m.createElement("div", {
+                    className: "jp-ellipsis"
+                }, e.children))
+            }
+
+            function I(e) {
                 var t, n, a, s;
                 const {
                     trans: o
                 } = e;
                 let r, l;
                 const [c, d] = m.useState("");
                 e.showSearchBox ? (r = c, l = d) : r = e.query;
-                const [, h] = m.useReducer((e => e + 1), 0), p = new Set;
+                const [, u] = m.useReducer((e => e + 1), 0), p = new Set;
                 for (const n of e.items) {
                     const e = null === (t = n.metadata) || void 0 === t ? void 0 : t.kernel;
                     if (e)
                         for (const t of Object.keys(e)) p.add(t)
                 }
                 const g = [...p].map((e => ({
                     id: e,
-                    label: L(e),
+                    label: N(e),
                     renderCell: t => {
                         var n;
                         const a = null === (n = t.metadata) || void 0 === n ? void 0 : n.kernel;
-                        if (!a) return "-";
-                        const s = a[e];
-                        return "string" == typeof s ? s : JSON.stringify(s)
+                        return m.createElement(S, null, (() => {
+                            if (!a) return "-";
+                            const t = a[e];
+                            return "string" == typeof t ? t : JSON.stringify(t)
+                        })())
                     },
                     sort: (t, n) => {
                         var a, s;
                         const o = null === (a = t.metadata) || void 0 === a ? void 0 : a.kernel,
                             r = null === (s = n.metadata) || void 0 === s ? void 0 : s.kernel,
                             l = o ? o[e] : void 0,
                             c = r ? r[e] : void 0;
@@ -168,76 +298,78 @@
                     label: o.__("Type"),
                     renderCell: e => e.command.split(":")[0],
                     sort: (e, t) => e.command.localeCompare(t.command)
                 });
                 const v = [{
                         id: "kernel",
                         label: o.__("Kernel"),
-                        renderCell: t => m.createElement(m.Fragment, null, m.createElement("span", {
+                        renderCell: t => m.createElement(S, null, m.createElement("span", {
+                            className: L,
+                            onClick: n => {
+                                e.onClick(t), n.stopPropagation()
+                            },
+                            onKeyDown: e => {
+                                "Enter" === e.key && t.execute()
+                            },
+                            tabIndex: 0
+                        }, m.createElement("span", {
                             className: "jp-LauncherCard-icon",
                             onClick: () => e.onClick(t)
                         }, t.kernelIconUrl ? m.createElement("img", {
                             src: t.kernelIconUrl,
                             className: "jp-Launcher-kernelIcon",
                             alt: t.label
                         }) : m.createElement("div", {
                             className: "jp-LauncherCard-noKernelIcon"
                         }, t.label[0].toUpperCase())), m.createElement("span", {
-                            className: k,
-                            onClick: n => {
-                                e.onClick(t), n.stopPropagation()
-                            },
-                            onKeyDown: e => {
-                                "Enter" === e.key && t.execute()
-                            },
-                            tabIndex: 0
-                        }, t.label)),
+                            className: "jp-TableKernelItem-label"
+                        }, t.label))),
                         sort: (e, t) => e.label.localeCompare(t.label)
                     }, ...g, {
                         id: "last-used",
                         label: o.__("Last Used"),
                         renderCell: e => m.createElement(i.UseSignal, {
                             signal: e.refreshLastUsed
-                        }, (() => e.lastUsed ? m.createElement("span", {
-                            title: f.Time.format(e.lastUsed)
-                        }, f.Time.formatHuman(e.lastUsed)) : o.__("Never"))),
+                        }, (() => m.createElement(S, {
+                            title: e.lastUsed ? b.Time.format(e.lastUsed) : o.__("No information about last use of this kernel is available in the layout database")
+                        }, e.lastUsed ? b.Time.formatHuman(e.lastUsed) : o.__("Never")))),
                         sort: (e, t) => e.lastUsed === t.lastUsed ? 0 : e.lastUsed ? t.lastUsed && e.lastUsed > t.lastUsed ? 1 : -1 : 1
                     }, {
                         id: "star",
                         label: "",
                         renderCell: e => {
                             const t = e.starred,
                                 n = t ? o.__("Click to add this kernel to favourites") : o.__("Click to remove the kernel from favourites");
                             return m.createElement("button", {
-                                className: t ? `${C} jp-mod-starred` : C,
+                                className: t ? `${D} jp-mod-starred` : D,
                                 title: n,
                                 onClick: t => {
-                                    e.toggleStar(), h(), t.stopPropagation()
+                                    e.toggleStar(), u(), t.stopPropagation()
                                 }
-                            }, m.createElement(u.react, {
+                            }, m.createElement(h.react, {
                                 className: "jp-starIcon"
                             }))
                         },
                         sort: (e, t) => Number(e.starred) - Number(t.starred)
                     }],
-                    _ = null !== (n = e.hideColumns) && void 0 !== n ? n : [],
-                    b = v.filter((e => !_.includes(e.id))),
-                    [y, D] = m.useState(null !== (a = e.settings.composite.hiddenColumns) && void 0 !== a ? a : {}),
-                    S = b.map((e => e.id)),
-                    [E, I] = m.useState(null !== (s = e.settings.composite.columnOrder) && void 0 !== s ? s : S),
-                    j = i.Table,
-                    N = () => {
+                    f = null !== (n = e.hideColumns) && void 0 !== n ? n : [],
+                    _ = v.filter((e => !f.includes(e.id))),
+                    [y, C] = m.useState(null !== (a = e.settings.composite.hiddenColumns) && void 0 !== a ? a : {}),
+                    k = _.map((e => e.id)),
+                    [j, I] = m.useState(null !== (s = e.settings.composite.columnOrder) && void 0 !== s ? s : k),
+                    U = w,
+                    x = () => {
                         var t, n;
                         const a = null !== (t = e.settings.composite.hiddenColumns) && void 0 !== t ? t : {};
-                        y !== a && D(a);
-                        const s = null !== (n = e.settings.composite.columnOrder) && void 0 !== n ? n : S;
-                        E !== s && I(s)
+                        y !== a && C(a);
+                        const s = null !== (n = e.settings.composite.columnOrder) && void 0 !== n ? n : k;
+                        j !== s && I(s)
                     };
-                return m.useEffect((() => (e.settings.changed.connect(N), () => {
-                    e.settings.changed.disconnect(N)
+                return m.useEffect((() => (e.settings.changed.connect(x), () => {
+                    e.settings.changed.disconnect(x)
                 }))), m.createElement("div", {
                     className: "jp-NewLauncher-table"
                 }, e.showSearchBox ? m.createElement("div", {
                     className: "jp-Launcher-searchBox"
                 }, m.createElement(i.FilterBox, {
                     placeholder: o.__("Filter kernels"),
                     updateFilter: (e, t) => {
@@ -252,69 +384,69 @@
                         t.preventDefault();
                         const a = new i.MenuSvg({
                                 commands: e.commands
                             }),
                             s = new i.MenuSvg({
                                 commands: e.commands
                             });
-                        for (const e of b) s.addItem({
-                            command: w.toggleColumn,
+                        for (const e of _) s.addItem({
+                            command: E.toggleColumn,
                             args: {
                                 id: e.id,
                                 label: e.label
                             }
                         });
                         s.title.label = o.__("Visible Columns"), a.addItem({
                             type: "submenu",
                             submenu: s
                         });
                         const r = null === (n = t.target.closest("th[data-id]")) || void 0 === n ? void 0 : n.dataset.id;
                         r && (a.addItem({
-                            command: w.moveColumn,
+                            command: E.moveColumn,
                             args: {
                                 direction: "left",
-                                order: E,
+                                order: j,
                                 id: r
                             }
                         }), a.addItem({
-                            command: w.moveColumn,
+                            command: E.moveColumn,
                             args: {
                                 direction: "right",
-                                order: E,
+                                order: j,
                                 id: r
                             }
                         })), a.open(t.clientX, t.clientY)
                     }
-                }, m.createElement(j, {
+                }, m.createElement(U, {
                     rows: e.items.filter((e => -1 !== e.label.toLowerCase().indexOf(r.toLowerCase()))).map((e => ({
                         data: e,
                         key: e.command + JSON.stringify(e.args)
                     }))),
                     blankIndicator: () => m.createElement("div", null, o.__("No entries")),
                     sortKey: "kernel",
                     onRowClick: e => {
                         const t = e.target,
                             n = t.closest("tr");
                         if (!n) return;
                         const a = t.closest("td"),
-                            s = null == a ? void 0 : a.querySelector(`.${C}`);
+                            s = null == a ? void 0 : a.querySelector(`.${D}`);
                         if (s) return s.click();
-                        n.querySelector(`.${k}`).click()
+                        n.querySelector(`.${L}`).click()
                     },
-                    columns: b.filter((e => "hidden" !== y[e.id])).map((e => {
+                    columns: _.filter((e => "hidden" !== y[e.id])).map((e => {
                         var t;
                         return {
                             ...e,
-                            rank: null !== (t = E.indexOf(e.id)) && void 0 !== t ? t : 10
+                            rank: null !== (t = j.indexOf(e.id)) && void 0 !== t ? t : 10
                         }
                     })).sort(((e, t) => e.rank - t.rank))
                 })))
             }
 
-            function S(e) {
+            function U(e) {
                 const [t, n] = m.useState(e.open);
                 return m.createElement("details", {
                     onToggle: t => {
                         n(t.currentTarget.open), e.onToggled && e.onToggled(t.currentTarget.open)
                     },
                     className: (0, i.classes)(e.className, "jp-CollapsibleSection"),
                     open: t
@@ -329,15 +461,15 @@
                 }), m.createElement("h3", {
                     className: "jp-CollapsibleSection-Title"
                 }, e.title)), m.createElement("div", {
                     className: "jp-Launcher-CardGroup jp-Launcher-cardContainer"
                 }, e.children))
             }
 
-            function E(e) {
+            function x(e) {
                 const {
                     item: t
                 } = e;
                 return m.createElement("div", {
                     onClick: () => t.execute(),
                     className: "jp-Launcher-TypeCard jp-LauncherCard",
                     title: t.caption,
@@ -348,120 +480,120 @@
                     icon: t.icon,
                     iconClass: (0, i.classes)(t.iconClass, "jp-Icon-cover")
                 })), m.createElement("div", {
                     className: "jp-LauncherCard-label"
                 }, m.createElement("p", null, t.label)))
             }
 
-            function I(e) {
+            function B(e) {
                 var t;
                 const {
                     trans: n,
                     cwd: a,
                     typeItems: s,
                     otherItems: o,
                     favouritesChanged: r
-                } = e, [l, c] = m.useState(""), [, d] = m.useReducer((e => e + 1), 0), [p, g] = m.useState(e.settings.composite.starredSection), [v, f] = m.useState(e.settings.composite.searchAllSections), _ = () => {
+                } = e, [l, c] = m.useState(""), [, d] = m.useReducer((e => e + 1), 0), [u, g] = m.useState(e.settings.composite.starredSection), [v, f] = m.useState(e.settings.composite.searchAllSections), b = () => {
                     const t = e.settings.composite.starredSection;
-                    p !== t && g(t);
+                    u !== t && g(t);
                     const n = e.settings.composite.searchAllSections;
                     v !== n && f(n)
                 };
-                if (m.useEffect((() => (e.settings.changed.connect(_), () => {
-                        e.settings.changed.disconnect(_)
+                if (m.useEffect((() => (e.settings.changed.connect(b), () => {
+                        e.settings.changed.disconnect(b)
                     }))), r) {
                     const e = () => {
-                        p && d()
+                        u && d()
                     };
                     m.useEffect((() => (r.connect(e), () => {
                         r.disconnect(e)
                     })))
                 }
-                const b = new Set;
+                const _ = new Set;
                 for (const n of e.notebookItems) {
                     const e = null === (t = n.metadata) || void 0 === t ? void 0 : t.kernel;
                     if (e)
-                        for (const t of Object.keys(e)) b.add(t)
+                        for (const t of Object.keys(e)) _.add(t)
                 }
                 const w = [...e.notebookItems, ...e.consoleItems].filter((e => e.starred)),
                     y = e.settings.composite.collapsedSections;
                 return m.createElement("div", {
                     className: "jp-LauncherBody"
                 }, m.createElement("div", {
                     className: "jp-NewLauncher-TopBar"
                 }, m.createElement("div", {
                     className: "jp-Launcher-cwd"
                 }, m.createElement("h3", null, n.__("Current folder:"), " ", m.createElement("code", null, a || "/"))), m.createElement("div", {
                     className: "jp-NewLauncher-OtherItems"
-                }, o.map((e => m.createElement(E, {
+                }, o.map((e => m.createElement(x, {
                     item: e,
                     trans: n
                 }))))), v ? m.createElement("div", {
                     className: "jp-Launcher-searchBox"
                 }, m.createElement(i.FilterBox, {
                     placeholder: n.__("Filter"),
                     updateFilter: (e, t) => {
                         c(null != t ? t : "")
                     },
                     initialQuery: "",
                     useFuzzyFilter: !1
-                })) : null, m.createElement(S, {
+                })) : null, m.createElement(U, {
                     className: "jp-Launcher-openByType",
                     title: n.__("Create Empty"),
-                    icon: h,
+                    icon: p,
                     open: "collapsed" !== y["create-empty"]
-                }, s.filter((e => !l || -1 !== e.label.toLowerCase().indexOf(l.toLowerCase()))).map((e => m.createElement(E, {
+                }, s.filter((e => !l || -1 !== e.label.toLowerCase().indexOf(l.toLowerCase()))).map((e => m.createElement(x, {
                     item: e,
                     trans: n
-                })))), p ? m.createElement(S, {
+                })))), u ? m.createElement(U, {
                     className: "jp-Launcher-openByKernel",
                     title: n.__("Starred"),
-                    icon: u,
+                    icon: h,
                     open: "collapsed" !== y.starred
-                }, w.length > 0 ? m.createElement(D, {
+                }, w.length > 0 ? m.createElement(I, {
                     items: w,
                     commands: e.commands,
                     showSearchBox: !v,
                     showWidgetType: !0,
                     query: l,
                     settings: e.settings,
                     trans: n,
                     onClick: e => e.execute()
-                }) : "No starred items") : null, m.createElement(S, {
+                }) : "No starred items") : null, m.createElement(U, {
                     className: "jp-Launcher-openByKernel jp-Launcher-launchNotebook",
-                    title: n.__("Launch Notebook"),
+                    title: n.__("Launch New Notebook"),
                     icon: i.notebookIcon,
                     open: "collapsed" !== y["launch-notebook"]
-                }, m.createElement(D, {
+                }, m.createElement(I, {
                     items: e.notebookItems,
                     commands: e.commands,
                     showSearchBox: !v,
                     query: l,
                     settings: e.settings,
                     trans: n,
                     onClick: e => e.execute()
-                })), m.createElement(S, {
+                })), m.createElement(U, {
                     className: "jp-Launcher-openByKernel jp-Launcher-launchConsole",
-                    title: n.__("Launch Console"),
+                    title: n.__("Launch New Console"),
                     icon: i.consoleIcon,
                     open: "collapsed" !== y["launch-console"]
-                }, m.createElement(D, {
+                }, m.createElement(I, {
                     items: e.consoleItems,
                     commands: e.commands,
                     showSearchBox: !v,
                     query: l,
                     settings: e.settings,
                     trans: n,
                     onClick: e => e.execute()
                 })))
             }
-            const j = "server-proxy:open";
-            class N extends r.Launcher {
+            const K = "server-proxy:open";
+            class T extends r.Launcher {
                 constructor(e) {
-                    super(e), this.renderCommand = e => new v({
+                    super(e), this.renderCommand = e => new f({
                         item: e,
                         cwd: this.cwd,
                         commands: this.commands,
                         lastUsedDatabase: this._lastUsedDatabase,
                         favoritesDatabase: this._favoritesDatabase
                     }), this.renderKernelCommand = e => this.renderCommand(e), this.commands = e.commands, this.trans = this.translator.load("jupyterlab-new-launcher"), this._lastUsedDatabase = e.lastUsedDatabase, this._favoritesDatabase = e.favoritesDatabase, this._settings = e.settings
                 }
@@ -470,15 +602,15 @@
                     const e = this.trans,
                         t = [...this.model.items()],
                         n = e.__("Notebook"),
                         a = e.__("Console"),
                         s = [n, a],
                         o = this._settings.composite.utilityCommands,
                         r = t.filter((e => o.includes(e.command))).map(this.renderCommand),
-                        l = t.filter((e => (!e.category || !s.includes(e.category)) && !o.includes(e.command) || e.command === j)),
+                        l = t.filter((e => (!e.category || !s.includes(e.category)) && !o.includes(e.command) || e.command === K)),
                         c = {
                             "terminal:create-new": 3,
                             "fileeditor:create-new": 6,
                             "fileeditor:create-new-markdown-file": 5
                         };
                     for (const e of l) e.command in c && (e.rank = c[e.command]);
                     const i = [{
@@ -487,31 +619,31 @@
                         }, {
                             command: "console:create",
                             rank: 4
                         }, ...l].sort(((e, t) => {
                             var n, a;
                             return (null !== (n = null == e ? void 0 : e.rank) && void 0 !== n ? n : 0) - (null !== (a = null == t ? void 0 : t.rank) && void 0 !== a ? a : 0)
                         })),
-                        d = t.filter((e => e.category && e.category === n && e.command !== j)).map(this.renderKernelCommand),
-                        u = t.filter((e => e.category && e.category === a && e.command !== j)).map(this.renderKernelCommand),
+                        d = t.filter((e => e.category && e.category === n && e.command !== K)).map(this.renderKernelCommand),
+                        u = t.filter((e => e.category && e.category === a && e.command !== K)).map(this.renderKernelCommand),
                         h = i.map(this.renderCommand);
-                    return m.createElement(I, {
+                    return m.createElement(B, {
                         trans: this.trans,
                         cwd: this.cwd,
                         commands: this.commands,
                         typeItems: h,
                         notebookItems: d,
                         consoleItems: u,
                         otherItems: r,
                         settings: this._settings,
                         favouritesChanged: this._favoritesDatabase.changed
                     })
                 }
             }
-            class U extends s.SessionContextDialogs {
+            class A extends s.SessionContextDialogs {
                 constructor(e) {
                     var t;
                     super(e), this.options = e;
                     const n = null !== (t = e.translator) && void 0 !== t ? t : c.nullTranslator;
                     this.trans = n.load("jupyterlab")
                 }
                 async selectKernel(e) {
@@ -524,23 +656,24 @@
                         }), s.Dialog.okButton({
                             label: t.__("Select"),
                             ariaLabel: t.__("Select Kernel"),
                             className: "jp-KernelSelector-SelectButton"
                         })],
                         o = e.kernelPreference.autoStartDefault,
                         r = "boolean" == typeof o,
-                        l = await this.options.settingRegistry.load(b),
+                        l = await this.options.settingRegistry.load(k),
                         c = new s.Dialog({
                             title: t.__("Select Kernel"),
-                            body: new B({
+                            body: new R({
                                 data: {
                                     specs: e.specsManager.specs,
                                     sessions: e.sessionManager.running(),
                                     preference: e.kernelPreference
                                 },
+                                name: e.name,
                                 commands: this.options.commands,
                                 favoritesDatabase: this.options.database.favorites,
                                 lastUsedDatabase: this.options.database.lastUsed,
                                 settings: l,
                                 trans: t,
                                 acceptDialog: () => {
                                     c.resolve(1)
@@ -561,36 +694,36 @@
                         autoStartDefault: i.isChecked
                     });
                     const d = i.value;
                     if (null === d && !e.hasNoKernel) return e.shutdown();
                     d && await e.changeKernel(d)
                 }
             }
-            const x = {
+            const M = {
                 id: "jupyterlab-new-launcher:dialogs",
                 description: "Session dialogs for redesigned JupyterLab launcher",
                 provides: s.ISessionContextDialogs,
                 autoStart: !0,
-                requires: [c.ITranslator, y, l.ISettingRegistry],
-                activate: (e, t, n, a) => new U({
+                requires: [c.ITranslator, j, l.ISettingRegistry],
+                activate: (e, t, n, a) => new A({
                     translator: t,
                     database: n,
                     commands: e.commands,
                     settingRegistry: a
                 })
             };
-            class B extends s.ReactWidget {
+            class R extends s.ReactWidget {
                 constructor(e) {
-                    super(), this.options = e, this.renderKernelCommand = e => new v({
+                    super(), this.options = e, this.renderKernelCommand = e => new f({
                         item: e,
                         cwd: "",
                         commands: this.commands,
                         lastUsedDatabase: this._lastUsedDatabase,
                         favoritesDatabase: this._favoritesDatabase
-                    }), this._selection = null, this.commands = e.commands, this._lastUsedDatabase = e.lastUsedDatabase, this._favoritesDatabase = e.favoritesDatabase, this._settings = e.settings, this.trans = e.trans
+                    }), this._selection = null, this.commands = e.commands, this._lastUsedDatabase = e.lastUsedDatabase, this._favoritesDatabase = e.favoritesDatabase, this._settings = e.settings, this._name = e.name, this.trans = e.trans
                 }
                 onBeforeAttach(e) {
                     super.onBeforeAttach(e), this.node.style.minWidth = "", this.node.style.minHeight = ""
                 }
                 onAfterAttach(e) {
                     super.onAfterAttach(e), requestAnimationFrame((() => {
                         const e = this.node.getBoundingClientRect();
@@ -608,15 +741,15 @@
                             command: "notebook:create-new",
                             args: {
                                 isLauncher: !0,
                                 kernelName: e.name
                             },
                             kernelIconUrl: n,
                             metadata: {
-                                kernel: _.JSONExt.deepCopy(e.metadata || {})
+                                kernel: C.JSONExt.deepCopy(e.metadata || {})
                             }
                         })
                     }
                     const a = [];
                     for (const t of this.options.data.sessions) {
                         const s = t.kernel;
                         if (!s) continue;
@@ -627,39 +760,39 @@
                             args: {
                                 isLauncher: !0,
                                 kernelName: o.name
                             },
                             kernelIconUrl: r,
                             metadata: {
                                 kernel: {
-                                    ..._.JSONExt.deepCopy(o.metadata || {}),
+                                    ...C.JSONExt.deepCopy(o.metadata || {}),
                                     state: null !== (e = s.execution_state) && void 0 !== e ? e : "running",
                                     "used by": t.name
                                 },
                                 model: s
                             }
                         })
                     }
                     const s = t.map(this.renderKernelCommand),
                         o = a.map(this.renderKernelCommand);
                     return m.createElement(m.Fragment, null, m.createElement("h3", {
                         className: "jp-KernelSelector-Section"
-                    }, this.trans.__("Start a new kernel")), m.createElement(D, {
+                    }, this.trans.__('Start a new kernel for "%1"', this._name)), m.createElement(I, {
                         trans: this.trans,
                         commands: this.commands,
                         items: s,
                         settings: this._settings,
                         query: "",
                         showSearchBox: !0,
                         onClick: e => {
                             this._selection = e, this.options.acceptDialog()
                         }
                     }), o.length > 0 ? m.createElement(m.Fragment, null, m.createElement("h3", {
                         className: "jp-KernelSelector-Section"
-                    }, this.trans.__("Connect to a running kernel")), m.createElement(D, {
+                    }, this.trans.__("Connect to a running kernel")), m.createElement(I, {
                         trans: this.trans,
                         commands: this.commands,
                         items: o,
                         settings: this._settings,
                         query: "",
                         showSearchBox: !1,
                         onClick: e => {
@@ -671,100 +804,107 @@
                 getValue() {
                     var e;
                     return this._selection ? (null === (e = this._selection.metadata) || void 0 === e ? void 0 : e.model) ? this._selection.metadata.model : {
                         name: this._selection.args.kernelName
                     } : null
                 }
             }
-            var K = n(101);
-            class T {
+            var O = n(101);
+            class z {
                 constructor(e) {
                     this._updateDB = async () => {
                         const e = await this._fetch();
                         this._db = e
                     }, this._db = null, this._stateDB = e.stateDB;
-                    const t = new _.PromiseDelegate;
+                    const t = new C.PromiseDelegate;
                     this.ready = t.promise, this._updateDB().then((() => t.resolve())), window.setInterval(this._updateDB, e.fetchInterval)
                 }
                 _get(e) {
                     return this._db ? this._db[this._itemKey(e)] : (console.error("Database is not ready!"), null)
                 }
                 async _set(e, t) {
                     const n = await this._fetch();
                     this._db = n, n[this._itemKey(e)] = t, await this._stateDB.save(this._stateDBKey, n)
                 }
                 async _fetch() {
                     let e = await this._stateDB.fetch(this._stateDBKey);
                     return void 0 === e && (e = await this._stateDB.fetch(this._stateDBKey)), void 0 === e ? {} : e
                 }
             }
-            class M extends T {
+            class H extends z {
                 _itemKey(e) {
                     return e.command + "_" + JSON.stringify(e.args)
                 }
             }
-            class A extends M {
+            class F extends H {
                 constructor() {
                     super(...arguments), this._stateDBKey = "new-launcher:last-used"
                 }
                 get(e) {
                     const t = super._get(e);
                     return t ? new Date(t) : null
                 }
                 async recordAsUsedNow(e) {
                     this._set(e, (new Date).toUTCString())
                 }
             }
-            class R extends M {
+            class q extends H {
                 constructor() {
-                    super(...arguments), this._stateDBKey = "new-launcher:favorites", this._changed = new g.Signal(this)
+                    super(...arguments), this._stateDBKey = "new-launcher:favorites", this._changed = new v.Signal(this)
                 }
                 get(e) {
                     var t;
                     return null !== (t = super._get(e)) && void 0 !== t ? t : null
                 }
                 async set(e, t) {
                     this._set(e, t), this._changed.emit()
                 }
                 get changed() {
                     return this._changed
                 }
             }
-            const O = {
+            const P = {
                     id: "jupyterlab-new-launcher:database",
                     description: "A redesigned JupyterLab launcher databases",
-                    provides: y,
+                    provides: j,
                     autoStart: !0,
-                    requires: [K.IStateDB],
+                    requires: [O.IStateDB],
                     activate: (e, t) => {
                         const n = {
                             stateDB: t,
                             fetchInterval: 1e4
                         };
                         return {
-                            lastUsed: new A(n),
-                            favorites: new R(n)
+                            lastUsed: new F(n),
+                            favorites: new q(n)
                         }
                     }
                 },
-                F = [{
-                    id: b,
+                V = [{
+                    id: k,
                     description: "A redesigned JupyterLab launcher",
                     provides: r.ILauncher,
                     autoStart: !0,
-                    requires: [c.ITranslator, l.ISettingRegistry, y],
+                    requires: [c.ITranslator, l.ISettingRegistry, j],
                     optional: [a.ILabShell, s.ICommandPalette, o.IDefaultFileBrowser],
                     activate: function(e, t, n, a, o, l, c) {
                         const {
                             commands: m,
                             shell: u
                         } = e, h = t.load("jupyterlab-new-launcher"), p = new r.LauncherModel;
-                        return n.load(b).then((t => {
+                        if (-1 !== navigator.userAgent.indexOf("AppleWebKit") && -1 === navigator.userAgent.indexOf("Chrome")) {
+                            const e = function(e) {
+                                const t = document.createElement("style");
+                                return t.setAttribute("type", "text/css"), t.appendChild(document.createTextNode(".jp-starIconButton {\n  /* do not rotate on webkit as the result is off when zoomed in see https://bugs.webkit.org/show_bug.cgi?id=194903 */\n  --jp-transition-transform: rotate(0deg);\n}\n\n.jp-starIcon .jp-star-filled,\n.jp-starIcon .jp-star-border {\n  /* disable animation on webkit */\n  transition-property: none;\n}\n")), t
+                            }();
+                            document.body.appendChild(e)
+                        }
+                        return n.load(k).then((t => {
                             ! function(e, t, n) {
-                                e.commands.addCommand(w.toggleColumn, {
+                                e.commands.addCommand(E.toggleColumn, {
                                     label: e => {
                                         if (e.label) return e.label;
                                         if (e.id) {
                                             const t = e.id;
                                             return t[0].toLocaleUpperCase() + t.substring(1)
                                         }
                                         return t.__("Toggle given column")
@@ -778,85 +918,85 @@
                                     },
                                     isToggleable: !0,
                                     isToggled: e => {
                                         var t;
                                         const a = e.id;
                                         return a ? "hidden" !== (null !== (t = n.user.hiddenColumns) && void 0 !== t ? t : {})[a] : (console.error("Column ID missing for checking if toggled"), !1)
                                     }
-                                }), e.commands.addCommand(w.moveColumn, {
+                                }), e.commands.addCommand(E.moveColumn, {
                                     label: e => "left" === e.direction ? t.__("Move Column Left") : "right" === e.direction ? t.__("Move Column Right") : t.__("Move column left or right"),
                                     execute: async e => {
                                         const t = e.order,
                                             a = e.id,
                                             s = t.indexOf(a),
                                             o = s + ("left" === e.direction ? -1 : 1);
                                         if (o < 0 || o >= t.length) return void console.log("Cannot move the column any further");
                                         const r = t[o];
                                         t[o] = a, t[s] = r, await n.set("columnOrder", t)
                                     }
                                 })
                             }(e, h, t)
-                        })), m.addCommand(w.create, {
+                        })), m.addCommand(E.create, {
                             label: h.__("New Launcher"),
                             icon: e => e.toolbar ? i.addIcon : void 0,
                             execute: async e => {
                                 var r, l;
                                 const g = null !== (l = null !== (r = e.cwd) && void 0 !== r ? r : null == c ? void 0 : c.model.path) && void 0 !== l ? l : "",
-                                    v = "launcher-" + H.id++,
-                                    f = await n.load(b);
+                                    v = "launcher-" + W.id++,
+                                    f = await n.load(k);
                                 await Promise.all([a.lastUsed.ready, a.favorites.ready]);
-                                const _ = new N({
+                                const b = new T({
                                     model: p,
                                     cwd: g,
                                     callback: e => {
                                         (0, d.find)(u.widgets("main"), (t => t === e)) && (u.add(e, "main", {
                                             ref: v
-                                        }), _.dispose())
+                                        }), b.dispose())
                                     },
                                     commands: m,
                                     translator: t,
                                     lastUsedDatabase: a.lastUsed,
                                     favoritesDatabase: a.favorites,
                                     settings: f
                                 });
-                                _.model = p, _.title.icon = i.launcherIcon, _.title.label = h.__("Launcher");
-                                const w = new s.MainAreaWidget({
-                                    content: _
+                                b.model = p, b.title.icon = i.launcherIcon, b.title.label = h.__("Launcher");
+                                const _ = new s.MainAreaWidget({
+                                    content: b
                                 });
-                                if (w.title.closable = !!Array.from(u.widgets("main")).length, w.id = v, u.add(w, "main", {
+                                if (_.title.closable = !!Array.from(u.widgets("main")).length, _.id = v, u.add(_, "main", {
                                         activate: e.activate,
                                         ref: e.ref
                                     }), o && o.layoutModified.connect((() => {
-                                        w.title.closable = Array.from(o.widgets("main")).length > 1
-                                    }), w), c) {
+                                        _.title.closable = Array.from(o.widgets("main")).length > 1
+                                    }), _), c) {
                                     const e = e => {
-                                        _.cwd = e.path
+                                        b.cwd = e.path
                                     };
-                                    c.model.pathChanged.connect(e), _.disposed.connect((() => {
+                                    c.model.pathChanged.connect(e), b.disposed.connect((() => {
                                         c.model.pathChanged.disconnect(e)
                                     }))
                                 }
-                                return w
+                                return _
                             }
                         }), o && Promise.all([e.restored, null == c ? void 0 : c.model.restored]).then((() => {
                             o.layoutModified.connect((() => {
-                                o.isEmpty("main") && m.execute(w.create)
+                                o.isEmpty("main") && m.execute(E.create)
                             }))
                         })), l && l.addItem({
-                            command: w.create,
+                            command: E.create,
                             category: h.__("Launcher")
                         }), o && (o.addButtonEnabled = !0, o.addRequested.connect(((e, t) => {
                             var n;
                             const a = (null === (n = t.currentTitle) || void 0 === n ? void 0 : n.owner.id) || t.titles[t.titles.length - 1].owner.id;
-                            return m.execute(w.create, {
+                            return m.execute(E.create, {
                                 ref: a
                             })
                         }))), p
                     }
-                }, x, O];
-            var H;
+                }, M, P];
+            var W;
             ! function(e) {
                 e.id = 0
-            }(H || (H = {}))
+            }(W || (W = {}))
         }
     }
 ]);
```

### Comparing `jupyterlab_new_launcher-0.2.3/jupyterlab_new_launcher/labextension/static/728.fa379db84cb7d3fbc55e.js` & `jupyterlab_new_launcher-0.3.0/jupyterlab_new_launcher/labextension/static/728.5be4ee0b94a07decd5f8.js`

 * *Files 15% similar despite different names*

#### js-beautify {}

```diff
@@ -5,15 +5,15 @@
             t.d(e, {
                 A: () => p
             });
             var r = t(601),
                 a = t.n(r),
                 o = t(314),
                 i = t.n(o)()(a());
-            i.push([n.id, ".jp-Launcher-CardGroup {\n  justify-content: center;\n}\n\n.jp-CollapsibleSection {\n  --jp-animation-depth: 10px;\n  --jp-animation-time: 150ms;\n  --jp-title-height: 24px;\n\n  padding: var(--jp-animation-depth);\n  padding-left: 0;\n  padding-right: 0;\n}\n\n.jp-Launcher-cwd > h3 {\n  font-size: var(--jp-ui-font-size1);\n  margin: 0;\n}\n\n.jp-NewLauncher-OtherItems {\n  display: flex;\n  gap: 4px;\n}\n\n.jp-NewLauncher-OtherItems .jp-LauncherCard-label {\n  display: none;\n}\n\n.jp-NewLauncher-OtherItems .jp-Launcher-TypeCard {\n  width: unset;\n  min-height: unset;\n  flex-direction: row;\n  margin: 0;\n  box-shadow: none;\n  border-color: var(--jp-border-color0);\n}\n\n.jp-NewLauncher-OtherItems .jp-LauncherCard-icon {\n  height: 24px;\n}\n\n.jp-NewLauncher-OtherItems .jp-Launcher-TypeCard > .jp-LauncherCard-icon svg {\n  width: 24px;\n  height: 16px;\n}\n\n.jp-NewLauncher-TopBar {\n  display: flex;\n  justify-content: space-between;\n  align-items: center;\n  padding: 8px 0;\n}\n\n.jp-Launcher-searchBox input {\n  /* (no longer needed in lab 4.2+) */\n  box-shadow: none;\n}\n\n.jp-Launcher-searchBox input,\n.jp-Launcher-searchBox jp-search::part(root) {\n  border: var(--jp-border-width) solid var(--jp-border-color1);\n}\n\n.jp-Launcher-searchBox .jp-FilterBox {\n  width: 100%;\n}\n\n.jp-CollapsibleSection > summary {\n  cursor: pointer;\n  transition: margin var(--jp-animation-time) ease-out;\n  list-style: none;\n  display: inline-block; /* contain the clickable area */\n  padding-right: 12px; /* but extend it a little */\n  min-width: 185px;\n}\n\n.jp-CollapsibleSection > summary:hover {\n  background-color: var(--jp-layout-color2);\n}\n\n.jp-CollapsibleSection[open] > summary {\n  margin-bottom: var(--jp-animation-depth);\n}\n\n.jp-CollapsibleSection-CollapserIcon > svg {\n  transition: transform var(--jp-animation-time) ease-out;\n  width: var(--jp-title-height);\n  height: var(--jp-title-height);\n}\n\n.jp-CollapsibleSection[open] .jp-CollapsibleSection-CollapserIcon > svg {\n  transform: rotate(90deg);\n}\n\n.jp-CollapsibleSection-CollapserIconWrapper {\n  display: inline-block;\n}\n\n.jp-CollapsibleSection-CategoryIcon > svg {\n  width: 24px;\n  height: 24px;\n  margin-left: 4px;\n  margin-right: 8px;\n}\n\n.jp-CollapsibleSection-Title {\n  display: inline-block;\n  line-height: var(--jp-title-height);\n  vertical-align: top;\n  margin: 0;\n  user-select: none;\n  font-weight: normal;\n}\n\n.jp-LauncherBody {\n  padding: 0 24px;\n  height: 100%;\n  overflow-y: auto;\n}\n\n.jp-NewLauncher-table {\n  --jp-icon-size: 16px;\n\n  display: flex;\n  flex-direction: column;\n  overflow: hidden;\n}\n\n.jp-NewLauncher-table .jp-sortable-table {\n  border: var(--jp-border-width) solid var(--jp-border-color2);\n  border-top: 0;\n}\n\n.jp-NewLauncher-table .jp-Launcher-kernelIcon {\n  width: var(--jp-icon-size);\n  height: var(--jp-icon-size);\n}\n\n.jp-NewLauncher-table .jp-LauncherCard-noKernelIcon {\n  font-size: var(--jp-icon-size);\n  line-height: var(--jp-icon-size);\n}\n\n.jp-NewLauncher-table .jp-LauncherCard-icon {\n  height: var(--jp-icon-size);\n  width: var(--jp-icon-size);\n  display: inline-block;\n}\n\n.jp-TableKernelItem {\n  display: inline-block;\n  line-height: var(--jp-icon-size);\n  vertical-align: top;\n  padding-left: 4px;\n}\n\n.jp-NewLauncher-table th[data-id='icon'],\n.jp-NewLauncher-table th[data-id='star'] {\n  width: var(--jp-icon-size);\n}\n\n.jp-NewLauncher-table .jp-starIcon {\n  width: var(--jp-icon-size);\n  height: var(--jp-icon-size);\n}\n\n.jp-starIconButton:hover > .jp-starIcon {\n  border-radius: 50%;\n  box-shadow: 0 0 0 2px var(--jp-layout-color3);\n  background: var(--jp-layout-color1);\n}\n\n.jp-NewLauncher-table-scroller {\n  overflow: auto;\n  margin-top: 4px;\n}\n\n.jp-starIconButton {\n  --jp-transition-transform: rotate(72deg);\n\n  border: 0;\n  margin: 0;\n  padding: 0 6px;\n  background: transparent;\n  cursor: pointer;\n}\n\n.jp-starIcon .jp-star-filled {\n  opacity: 0;\n}\n\n.jp-starIcon .jp-star-filled,\n.jp-starIcon .jp-star-border {\n  transition-property: opacity, transform;\n  transition-duration: 0.2s;\n  transition-timing-function: ease-out;\n  transform-origin: center;\n}\n\n.jp-starIconButton.jp-mod-starred .jp-star-filled {\n  opacity: 1;\n  transform: var(--jp-transition-transform);\n}\n\n.jp-starIconButton.jp-mod-starred .jp-star-border {\n  opacity: 0;\n  transform: var(--jp-transition-transform);\n}\n\n.jp-KernelSelector-Dialog > .jp-Dialog-content {\n  max-height: 80%;\n  max-width: unset;\n}\n\n.jp-KernelSelector-Dialog > .jp-Dialog-content > .jp-Dialog-header {\n  display: none;\n}\n\n.jp-KernelSelector-SelectButton {\n  display: none;\n}\n\n.jp-KernelSelector-Dialog .jp-NewLauncher-table {\n  margin-bottom: 8px;\n}\n\n.jp-KernelSelector-Section {\n  margin: 0;\n  margin-bottom: 4px;\n}\n\n/* Styles for scenario where full row is clickable  */\n\n.jp-NewLauncher-table tr {\n  cursor: pointer;\n}\n\n.jp-Launcher-TypeCard {\n  user-select: none;\n}\n\n.jp-Launcher-TypeCard > .jp-LauncherCard-icon svg {\n  align-items: center;\n  display: flex;\n  height: 52px;\n  width: 52px;\n}\n", ""]);
+            i.push([n.id, ".jp-Launcher-CardGroup {\n  justify-content: center;\n}\n\n.jp-CollapsibleSection {\n  --jp-animation-depth: 10px;\n  --jp-animation-time: 150ms;\n  --jp-title-height: 24px;\n\n  padding: var(--jp-animation-depth);\n  padding-left: 0;\n  padding-right: 0;\n}\n\n.jp-Launcher-cwd > h3 {\n  font-size: var(--jp-ui-font-size1);\n  margin: 0;\n}\n\n.jp-NewLauncher-OtherItems {\n  display: flex;\n  gap: 4px;\n}\n\n.jp-NewLauncher-OtherItems .jp-LauncherCard-label {\n  display: none;\n}\n\n.jp-NewLauncher-OtherItems .jp-Launcher-TypeCard {\n  width: unset;\n  min-height: unset;\n  flex-direction: row;\n  margin: 0;\n  box-shadow: none;\n  border-color: var(--jp-border-color0);\n}\n\n.jp-NewLauncher-OtherItems .jp-LauncherCard-icon {\n  height: 24px;\n}\n\n.jp-NewLauncher-OtherItems .jp-Launcher-TypeCard > .jp-LauncherCard-icon svg {\n  width: 24px;\n  height: 16px;\n}\n\n.jp-NewLauncher-TopBar {\n  display: flex;\n  justify-content: space-between;\n  align-items: center;\n  padding: 8px 0;\n}\n\n.jp-Launcher-searchBox input {\n  /* (no longer needed in lab 4.2+) */\n  box-shadow: none;\n}\n\n.jp-Launcher-searchBox input,\n.jp-Launcher-searchBox jp-search::part(root) {\n  border: var(--jp-border-width) solid var(--jp-border-color1);\n}\n\n.jp-Launcher-searchBox .jp-FilterBox {\n  width: 100%;\n}\n\n.jp-CollapsibleSection > summary {\n  cursor: pointer;\n  transition: margin var(--jp-animation-time) ease-out;\n  list-style: none;\n  display: inline-block; /* contain the clickable area */\n  padding-right: 12px; /* but extend it a little */\n  min-width: 185px;\n}\n\n.jp-CollapsibleSection > summary:hover {\n  background-color: var(--jp-layout-color2);\n}\n\n.jp-CollapsibleSection[open] > summary {\n  margin-bottom: var(--jp-animation-depth);\n}\n\n.jp-CollapsibleSection-CollapserIcon > svg {\n  transition: transform var(--jp-animation-time) ease-out;\n  width: var(--jp-title-height);\n  height: var(--jp-title-height);\n}\n\n.jp-CollapsibleSection[open] .jp-CollapsibleSection-CollapserIcon > svg {\n  transform: rotate(90deg);\n}\n\n.jp-CollapsibleSection-CollapserIconWrapper {\n  display: inline-block;\n}\n\n.jp-CollapsibleSection-CategoryIcon > svg {\n  width: 24px;\n  height: 24px;\n  margin-left: 4px;\n  margin-right: 8px;\n}\n\n.jp-CollapsibleSection-Title {\n  display: inline-block;\n  line-height: var(--jp-title-height);\n  vertical-align: top;\n  margin: 0;\n  user-select: none;\n  font-weight: normal;\n}\n\n.jp-LauncherBody {\n  padding: 0 24px;\n  height: 100%;\n  overflow-y: auto;\n}\n\n.jp-NewLauncher-table {\n  --jp-icon-size: 16px;\n\n  display: flex;\n  flex-direction: column;\n  overflow: hidden;\n}\n\n.jp-NewLauncher-table .jp-sortable-table {\n  border: var(--jp-border-width) solid var(--jp-border-color2);\n  border-top: 0;\n}\n\n.jp-NewLauncher-table .jp-Launcher-kernelIcon {\n  width: var(--jp-icon-size);\n  height: var(--jp-icon-size);\n}\n\n.jp-NewLauncher-table .jp-LauncherCard-noKernelIcon {\n  font-size: var(--jp-icon-size);\n  line-height: var(--jp-icon-size);\n}\n\n.jp-NewLauncher-table .jp-LauncherCard-icon {\n  height: var(--jp-icon-size);\n  width: var(--jp-icon-size);\n  display: inline-block;\n}\n\n.jp-TableKernelItem {\n  line-height: var(--jp-icon-size);\n}\n\n.jp-TableKernelItem > .jp-LauncherCard-icon {\n  margin-right: 4px;\n  vertical-align: top;\n  height: var(--jp-icon-size);\n}\n\n.jp-TableKernelItem-label {\n  vertical-align: top;\n}\n\n.jp-NewLauncher-table th[data-id='icon'],\n.jp-NewLauncher-table th[data-id='star'] {\n  width: var(--jp-icon-size);\n}\n\n.jp-NewLauncher-table .jp-starIcon {\n  width: var(--jp-icon-size);\n  height: var(--jp-icon-size);\n}\n\n.jp-starIconButton:hover > .jp-starIcon {\n  border-radius: 50%;\n  box-shadow: 0 0 0 2px var(--jp-layout-color3);\n  background: var(--jp-layout-color1);\n}\n\n.jp-NewLauncher-table-scroller {\n  overflow: auto;\n  margin-top: 4px;\n}\n\n.jp-starIconButton {\n  --jp-transition-transform: rotate(72deg);\n\n  border: 0;\n  margin: 0;\n  padding: 0 6px;\n  background: transparent;\n  cursor: pointer;\n}\n\n.jp-starIcon .jp-star-filled {\n  opacity: 0;\n}\n\n.jp-starIcon .jp-star-filled,\n.jp-starIcon .jp-star-border {\n  transition-property: opacity, transform;\n  transition-duration: 0.2s;\n  transition-timing-function: ease-out;\n  transform-origin: center;\n}\n\n.jp-starIconButton.jp-mod-starred .jp-star-filled {\n  opacity: 1;\n  transform: var(--jp-transition-transform);\n}\n\n.jp-starIconButton.jp-mod-starred .jp-star-border {\n  opacity: 0;\n  transform: var(--jp-transition-transform);\n}\n\n.jp-KernelSelector-Dialog > .jp-Dialog-content {\n  max-height: 80%;\n  max-width: unset;\n}\n\n.jp-KernelSelector-Dialog > .jp-Dialog-content > .jp-Dialog-header {\n  display: none;\n}\n\n.jp-KernelSelector-SelectButton {\n  display: none;\n}\n\n.jp-KernelSelector-Dialog .jp-NewLauncher-table {\n  margin-bottom: 8px;\n}\n\n.jp-KernelSelector-Section {\n  margin: 0;\n  margin-bottom: 4px;\n}\n\n/* Styles for scenario where full row is clickable  */\n\n.jp-NewLauncher-table tr {\n  cursor: pointer;\n}\n\n.jp-Launcher-TypeCard {\n  user-select: none;\n}\n\n.jp-Launcher-TypeCard > .jp-LauncherCard-icon svg {\n  align-items: center;\n  display: flex;\n  height: 52px;\n  width: 52px;\n}\n\n.jp-NewLauncher-table .jp-sortable-table-tr > td {\n  white-space: nowrap;\n}\n\n.jp-sortable-table-tr > td.jp-mod-col-resized > .jp-ellipsis-wrapper {\n  white-space: nowrap;\n  position: absolute;\n  inset: 0;\n}\n\n.jp-sortable-table-tr\n  > td.jp-mod-col-resized\n  > .jp-ellipsis-wrapper\n  > .jp-ellipsis {\n  white-space: nowrap;\n  overflow: hidden;\n  text-overflow: ellipsis;\n\n  /* TODO share values for padding and height from `.jp-sortable-table-tr > td` via variable; not top padding is a sum of bottom and top in plain td to align text. */\n  padding: 5px 12px 1px;\n}\n\n.jp-sortable-table-tr > td > .jp-starIconButton {\n  white-space: nowrap;\n}\n\n.jp-sortable-table-tr > th,\n.jp-sortable-table-tr > td {\n  padding: 3px 12px;\n}\n\ntd > .jp-starIconButton {\n  position: relative;\n  top: 1px;\n}\n\n/* To contribute upstream  */\n\n.jp-sortable-table-resize-handle {\n  width: 4px;\n  position: absolute;\n  right: 0;\n  top: 0;\n  height: 100%;\n  cursor: ew-resize;\n}\n\n.jp-sortable-table-tr > th {\n  overflow: hidden;\n  box-sizing: border-box;\n  height: 24px;\n  padding: 0;\n  -webkit-user-select: none;\n}\n\n.jp-sortable-table-resize-handle:hover {\n  background: var(--jp-layout-color3);\n}\n\n.jp-header-resizing > .jp-sortable-table-resize-handle {\n  background: var(--jp-brand-color1) !important;\n}\n\nbody.jp-mod-resize-table * {\n  cursor: ew-resize;\n}\n\nbody.jp-mod-resize-table .jp-sortable-table {\n  pointer-events: none;\n}\n\n/*\nThis will likely be needed upstream when no ellipsis wrapping is used.\n.jp-sortable-table-tr > td > * {\n  white-space: normal;\n}\n*/\n\n.jp-sortable-table-th-wrapper > label {\n  overflow: hidden;\n  font-weight: 500;\n}\n\n.jp-sortable-table-th-wrapper {\n  width: inherit;\n  box-sizing: border-box;\n  padding: 4px 12px 2px;\n\n  /* fill-available is only needed when heading does not collapse\n  /* min-width: -webkit-fill-available; */\n}\n", ""]);
             const p = i
         },
         314: n => {
             n.exports = function(n) {
                 var e = [];
                 return e.toString = function() {
                     return this.map((function(e) {
@@ -24,20 +24,20 @@
                 }, e.i = function(n, t, r, a, o) {
                     "string" == typeof n && (n = [
                         [null, n, void 0]
                     ]);
                     var i = {};
                     if (r)
                         for (var p = 0; p < this.length; p++) {
-                            var c = this[p][0];
-                            null != c && (i[c] = !0)
+                            var l = this[p][0];
+                            null != l && (i[l] = !0)
                         }
-                    for (var l = 0; l < n.length; l++) {
-                        var s = [].concat(n[l]);
-                        r && i[s[0]] || (void 0 !== o && (void 0 === s[5] || (s[1] = "@layer".concat(s[5].length > 0 ? " ".concat(s[5]) : "", " {").concat(s[1], "}")), s[5] = o), t && (s[2] ? (s[1] = "@media ".concat(s[2], " {").concat(s[1], "}"), s[2] = t) : s[2] = t), a && (s[4] ? (s[1] = "@supports (".concat(s[4], ") {").concat(s[1], "}"), s[4] = a) : s[4] = "".concat(a)), e.push(s))
+                    for (var s = 0; s < n.length; s++) {
+                        var c = [].concat(n[s]);
+                        r && i[c[0]] || (void 0 !== o && (void 0 === c[5] || (c[1] = "@layer".concat(c[5].length > 0 ? " ".concat(c[5]) : "", " {").concat(c[1], "}")), c[5] = o), t && (c[2] ? (c[1] = "@media ".concat(c[2], " {").concat(c[1], "}"), c[2] = t) : c[2] = t), a && (c[4] ? (c[1] = "@supports (".concat(c[4], ") {").concat(c[1], "}"), c[4] = a) : c[4] = "".concat(a)), e.push(c))
                     }
                 }, e
             }
         },
         601: n => {
             n.exports = function(n) {
                 return n[1]
@@ -52,37 +52,37 @@
                         t = r;
                         break
                     } return t
             }
 
             function r(n, r) {
                 for (var o = {}, i = [], p = 0; p < n.length; p++) {
-                    var c = n[p],
-                        l = r.base ? c[0] + r.base : c[0],
-                        s = o[l] || 0,
-                        u = "".concat(l, " ").concat(s);
-                    o[l] = s + 1;
-                    var d = t(u),
-                        h = {
-                            css: c[1],
-                            media: c[2],
-                            sourceMap: c[3],
-                            supports: c[4],
-                            layer: c[5]
+                    var l = n[p],
+                        s = r.base ? l[0] + r.base : l[0],
+                        c = o[s] || 0,
+                        d = "".concat(s, " ").concat(c);
+                    o[s] = c + 1;
+                    var h = t(d),
+                        u = {
+                            css: l[1],
+                            media: l[2],
+                            sourceMap: l[3],
+                            supports: l[4],
+                            layer: l[5]
                         };
-                    if (-1 !== d) e[d].references++, e[d].updater(h);
+                    if (-1 !== h) e[h].references++, e[h].updater(u);
                     else {
-                        var j = a(h, r);
+                        var j = a(u, r);
                         r.byIndex = p, e.splice(p, 0, {
-                            identifier: u,
+                            identifier: d,
                             updater: j,
                             references: 1
                         })
                     }
-                    i.push(u)
+                    i.push(d)
                 }
                 return i
             }
 
             function a(n, e) {
                 var t = e.domAPI(e);
                 return t.update(n),
@@ -97,19 +97,19 @@
                 var o = r(n = n || [], a = a || {});
                 return function(n) {
                     n = n || [];
                     for (var i = 0; i < o.length; i++) {
                         var p = t(o[i]);
                         e[p].references--
                     }
-                    for (var c = r(n, a), l = 0; l < o.length; l++) {
-                        var s = t(o[l]);
-                        0 === e[s].references && (e[s].updater(), e.splice(s, 1))
+                    for (var l = r(n, a), s = 0; s < o.length; s++) {
+                        var c = t(o[s]);
+                        0 === e[c].references && (e[c].updater(), e.splice(c, 1))
                     }
-                    o = c
+                    o = l
                 }
             }
         },
         659: n => {
             var e = {};
             n.exports = function(n, t) {
                 var r = function(n) {
@@ -179,20 +179,20 @@
         728: (n, e, t) => {
             t.r(e);
             var r = t(72),
                 a = t.n(r),
                 o = t(206),
                 i = t.n(o),
                 p = t(659),
-                c = t.n(p),
-                l = t(56),
-                s = t.n(l),
-                u = t(540),
-                d = t.n(u),
-                h = t(113),
-                j = t.n(h),
-                f = t(475),
+                l = t.n(p),
+                s = t(56),
+                c = t.n(s),
+                d = t(540),
+                h = t.n(d),
+                u = t(113),
+                j = t.n(u),
+                b = t(475),
                 m = {};
-            m.styleTagTransform = j(), m.setAttributes = s(), m.insert = c().bind(null, "head"), m.domAPI = i(), m.insertStyleElement = d(), a()(f.A, m), f.A && f.A.locals && f.A.locals
+            m.styleTagTransform = j(), m.setAttributes = c(), m.insert = l().bind(null, "head"), m.domAPI = i(), m.insertStyleElement = h(), a()(b.A, m), b.A && b.A.locals && b.A.locals
         }
     }
 ]);
```

### Comparing `jupyterlab_new_launcher-0.2.3/jupyterlab_new_launcher/labextension/static/remoteEntry.beb3c4798d84f1b62e25.js` & `jupyterlab_new_launcher-0.3.0/jupyterlab_new_launcher/labextension/static/remoteEntry.697e41989e560bf8e1db.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, a, o, i, u, l, f, d, s, p, c, h, v, b, g = {
+    var e, r, t, n, a, o, i, u, l, f, s, d, p, c, h, v, b, g = {
             795: (e, r, t) => {
                 var n = {
-                        "./index": () => t.e(239).then((() => () => t(239))),
-                        "./extension": () => t.e(239).then((() => () => t(239))),
+                        "./index": () => t.e(787).then((() => () => t(787))),
+                        "./extension": () => t.e(787).then((() => () => t(787))),
                         "./style": () => t.e(728).then((() => () => t(728)))
                     },
                     a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     o = (e, r) => {
                         if (t.S) {
@@ -43,49 +43,49 @@
         }), r
     }, m.d = (e, r) => {
         for (var t in r) m.o(r, t) && !m.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, m.f = {}, m.e = e => Promise.all(Object.keys(m.f).reduce(((r, t) => (m.f[t](e, r), r)), [])), m.u = e => e + "." + {
-        239: "a28bc3eddd733aecbd06",
-        728: "fa379db84cb7d3fbc55e"
+        728: "5be4ee0b94a07decd5f8",
+        787: "d3e306a9eb8983db2644"
     } [e] + ".js?v=" + {
-        239: "a28bc3eddd733aecbd06",
-        728: "fa379db84cb7d3fbc55e"
+        728: "5be4ee0b94a07decd5f8",
+        787: "d3e306a9eb8983db2644"
     } [e], m.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), m.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "jupyterlab-new-launcher:", m.l = (t, n, a, o) => {
         if (e[t]) e[t].push(n);
         else {
             var i, u;
             if (void 0 !== a)
                 for (var l = document.getElementsByTagName("script"), f = 0; f < l.length; f++) {
-                    var d = l[f];
-                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + a) {
-                        i = d;
+                    var s = l[f];
+                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + a) {
+                        i = s;
                         break
                     }
                 }
             i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, m.nc && i.setAttribute("nonce", m.nc), i.setAttribute("data-webpack", r + a), i.src = t), e[t] = [n];
-            var s = (r, n) => {
+            var d = (r, n) => {
                     i.onerror = i.onload = null, clearTimeout(p);
                     var a = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), a && a.forEach((e => e(n))), r) return r(n)
                 },
-                p = setTimeout(s.bind(null, void 0, {
+                p = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = s.bind(null, i.onerror), i.onload = s.bind(null, i.onload), u && document.head.appendChild(i)
+            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), u && document.head.appendChild(i)
         }
     }, m.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -102,19 +102,19 @@
                 var o = m.S[t],
                     i = "jupyterlab-new-launcher",
                     u = [];
                 return "default" === t && ((e, r, t, n) => {
                     var a = o[e] = o[e] || {},
                         u = a[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (a[r] = {
-                        get: () => m.e(239).then((() => () => m(239))),
+                        get: () => m.e(787).then((() => () => m(787))),
                         from: i,
                         eager: !1
                     })
-                })("jupyterlab-new-launcher", "0.2.3"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("jupyterlab-new-launcher", "0.3.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         m.g.importScripts && (e = m.g.location + "");
         var r = m.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -164,33 +164,33 @@
     }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 a = n < 0;
             a && (n = -n - 1);
             for (var i = 0, u = 1, l = !0;; u++, i++) {
-                var f, d, s = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (d = (typeof(f = r[i]))[0])) return !l || ("u" == s ? u > n && !a : "" == s != a);
-                if ("u" == d) {
-                    if (!l || "u" != s) return !1
+                var f, s, d = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (s = (typeof(f = r[i]))[0])) return !l || ("u" == d ? u > n && !a : "" == d != a);
+                if ("u" == s) {
+                    if (!l || "u" != d) return !1
                 } else if (l)
-                    if (s == d)
+                    if (d == s)
                         if (u <= n) {
                             if (f != e[u]) return !1
                         } else {
                             if (a ? f > e[u] : f < e[u]) return !1;
                             f != e[u] && (l = !1)
                         }
-                else if ("s" != s && "n" != s) {
+                else if ("s" != d && "n" != d) {
                     if (a || u <= n) return !1;
                     l = !1, u--
                 } else {
-                    if (u <= n || d < s != a) return !1;
+                    if (u <= n || s < d != a) return !1;
                     l = !1
-                } else "s" != s && "n" != s && (l = !1, u--)
+                } else "s" != d && "n" != d && (l = !1, u--)
             }
         }
         var p = [],
             c = p.pop.bind(p);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
             p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? o(h, r) : !c())
@@ -201,18 +201,18 @@
         if (!t || !m.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
     }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", f = (e, r, t, n) => {
         var a = u(e, t);
-        return o(n, a) || d(l(e, t, a, n)), s(e[t][a])
-    }, d = e => {
+        return o(n, a) || s(l(e, t, a, n)), d(e[t][a])
+    }, s = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, s = e => (e.loaded = 1, e.get()), p = (e => function(r, t, n, a) {
+    }, d = e => (e.loaded = 1, e.get()), p = (e => function(r, t, n, a) {
         var o = m.I(r);
         return o && o.then ? o.then(e.bind(e, r, m.S[r], t, n, a)) : e(r, m.S[r], t, n)
     })(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), c = {}, h = {
         53: () => p("default", "@lumino/algorithm", [1, 2, 0, 0]),
         101: () => p("default", "@jupyterlab/statedb", [1, 4, 2, 0]),
         260: () => p("default", "@jupyterlab/launcher", [1, 4, 2, 0]),
         262: () => p("default", "@lumino/coreutils", [1, 2, 0, 0]),
@@ -222,15 +222,15 @@
         602: () => p("default", "@lumino/signaling", [1, 2, 0, 0]),
         626: () => p("default", "@jupyterlab/application", [1, 4, 2, 0]),
         670: () => p("default", "@jupyterlab/filebrowser", [1, 4, 2, 0]),
         702: () => p("default", "@jupyterlab/coreutils", [1, 6, 2, 0]),
         825: () => p("default", "@jupyterlab/settingregistry", [1, 4, 2, 0]),
         923: () => p("default", "@jupyterlab/apputils", [1, 4, 3, 0])
     }, v = {
-        239: [53, 101, 260, 262, 265, 345, 527, 602, 626, 670, 702, 825, 923]
+        787: [53, 101, 260, 262, 265, 345, 527, 602, 626, 670, 702, 825, 923]
     }, b = {}, m.f.consumes = (e, r) => {
         m.o(v, e) && v[e].forEach((e => {
             if (m.o(c, e)) return r.push(c[e]);
             if (!b[e]) {
                 var t = r => {
                     c[e] = 0, m.m[e] = t => {
                         delete m.c[e], t.exports = r()
```

### Comparing `jupyterlab_new_launcher-0.2.3/jupyterlab_new_launcher/labextension/static/third-party-licenses.json` & `jupyterlab_new_launcher-0.3.0/jupyterlab_new_launcher/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.3/schema/plugin.json` & `jupyterlab_new_launcher-0.3.0/schema/plugin.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996527777777777%*

 * *Differences: {"'properties'": "{'hiddenColumns': {'default': {'conda_language': 'hidden', "*

 * *                 "'conda_is_base_environment': 'hidden', 'conda_is_currently_running': 'hidden'}}}"}*

```diff
@@ -56,14 +56,17 @@
                     "visible",
                     "hidden"
                 ],
                 "type": "string"
             },
             "default": {
                 "conda_env_path": "hidden",
+                "conda_is_base_environment": "hidden",
+                "conda_is_currently_running": "hidden",
+                "conda_language": "hidden",
                 "conda_raw_kernel_name": "hidden"
             },
             "title": "Hidden columns",
             "type": "object"
         },
         "searchAllSections": {
             "default": true,
```

### Comparing `jupyterlab_new_launcher-0.2.3/src/commands.ts` & `jupyterlab_new_launcher-0.3.0/src/commands.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.3/src/database.ts` & `jupyterlab_new_launcher-0.3.0/src/database.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.3/src/dialogs.tsx` & `jupyterlab_new_launcher-0.3.0/src/dialogs.tsx`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,15 @@
       title: trans.__('Select Kernel'),
       body: new KernelSelector({
         data: {
           specs: sessionContext.specsManager.specs,
           sessions: sessionContext.sessionManager.running(),
           preference: sessionContext.kernelPreference
         },
+        name: sessionContext.name,
         commands: this.options.commands,
         favoritesDatabase: this.options.database.favorites,
         lastUsedDatabase: this.options.database.lastUsed,
         settings,
         trans,
         acceptDialog: () => {
           dialog.resolve(1);
@@ -160,18 +161,18 @@
 export class KernelSelector extends ReactWidget {
   constructor(protected options: KernelSelector.IOptions) {
     super();
     this.commands = options.commands;
     this._lastUsedDatabase = options.lastUsedDatabase;
     this._favoritesDatabase = options.favoritesDatabase;
     this._settings = options.settings;
+    this._name = options.name;
     this.trans = options.trans;
   }
-  private _lastUsedDatabase: ILastUsedDatabase;
-  private _favoritesDatabase: IFavoritesDatabase;
+
   trans: TranslationBundle;
 
   renderKernelCommand = (item: ILauncher.IItemOptions): IItem => {
     return new Item({
       item,
       cwd: '',
       commands: this.commands,
@@ -250,15 +251,15 @@
     }
     const notebookItems = items.map(this.renderKernelCommand);
     const runningKernelsItems = runningItems.map(this.renderKernelCommand);
 
     return (
       <>
         <h3 className="jp-KernelSelector-Section">
-          {this.trans.__('Start a new kernel')}
+          {this.trans.__('Start a new kernel for "%1"', this._name)}
         </h3>
         <KernelTable
           trans={this.trans}
           commands={this.commands}
           items={notebookItems}
           settings={this._settings}
           query=""
@@ -301,20 +302,24 @@
     }
     return { name: this._selection.args!.kernelName as string };
   }
 
   protected commands: CommandRegistry;
   private _settings: ISettingRegistry.ISettings;
   private _selection: IKernelItem | null = null;
+  private _lastUsedDatabase: ILastUsedDatabase;
+  private _favoritesDatabase: IFavoritesDatabase;
+  private _name: string;
 }
 
 export namespace KernelSelector {
   export interface IOptions {
     lastUsedDatabase: ILastUsedDatabase;
     favoritesDatabase: IFavoritesDatabase;
     settings: ISettingRegistry.ISettings;
     commands: CommandRegistry;
     trans: TranslationBundle;
     data: SessionContext.IKernelSearch;
     acceptDialog: () => void;
+    name: string;
   }
 }
```

### Comparing `jupyterlab_new_launcher-0.2.3/src/icons.ts` & `jupyterlab_new_launcher-0.3.0/src/icons.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.3/src/index.ts` & `jupyterlab_new_launcher-0.3.0/src/index.ts`

 * *Files 7% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import { ReadonlyPartialJSONObject } from '@lumino/coreutils';
 import { DockPanel, TabBar, Widget } from '@lumino/widgets';
 import { NewLauncher as Launcher } from './launcher';
 import { CommandIDs, ILauncherDatabase, MAIN_PLUGIN_ID } from './types';
 import { addCommands } from './commands';
 import { sessionDialogsPlugin } from './dialogs';
 import { databasePlugin } from './database';
+import webkitCSSPatch from '../style/webkit.raw.css';
 
 /**
  * Initialization data for the jupyterlab-new-launcher extension.
  */
 const launcherPlugin: JupyterFrontEndPlugin<ILauncher> = {
   id: MAIN_PLUGIN_ID,
   description: 'A redesigned JupyterLab launcher',
@@ -31,14 +32,21 @@
   requires: [ITranslator, ISettingRegistry, ILauncherDatabase],
   optional: [ILabShell, ICommandPalette, IDefaultFileBrowser],
   activate
 };
 
 export default [launcherPlugin, sessionDialogsPlugin, databasePlugin];
 
+function createStyleSheet(text: string): HTMLStyleElement {
+  const style = document.createElement('style');
+  style.setAttribute('type', 'text/css');
+  style.appendChild(document.createTextNode(text));
+  return style;
+}
+
 /**
  * Activate the launcher.
  */
 function activate(
   app: JupyterFrontEnd,
   translator: ITranslator,
   settingRegistry: ISettingRegistry,
@@ -47,14 +55,22 @@
   palette: ICommandPalette | null,
   defaultBrowser: IDefaultFileBrowser | null
 ): ILauncher {
   const { commands, shell } = app;
   const trans = translator.load('jupyterlab-new-launcher');
   const model = new LauncherModel();
 
+  if (
+    navigator.userAgent.indexOf('AppleWebKit') !== -1 &&
+    navigator.userAgent.indexOf('Chrome') === -1
+  ) {
+    const style = createStyleSheet(webkitCSSPatch);
+    document.body.appendChild(style);
+  }
+
   settingRegistry.load(MAIN_PLUGIN_ID).then(settings => {
     addCommands(app, trans, settings);
   });
 
   commands.addCommand(CommandIDs.create, {
     label: trans.__('New Launcher'),
     icon: args => (args.toolbar ? addIcon : undefined),
```

### Comparing `jupyterlab_new_launcher-0.2.3/src/item.ts` & `jupyterlab_new_launcher-0.3.0/src/item.ts`

 * *Files 1% similar despite different names*

```diff
@@ -60,17 +60,17 @@
         const groups = condaStoreMatch.groups!;
         this.label =
           (kernel['conda_language'] as string | undefined) ??
           groups.environment;
         this.metadata = {
           ...this.metadata,
           kernel: {
-            ...kernel,
+            Namespace: groups.namespace,
             conda_env_name: groups.environment,
-            Namespace: groups.namespace
+            ...kernel
           }
         };
       }
     }
     // set the code-server icon to support dark theme properly
     if (
       this.command === 'server-proxy:open' &&
```

### Comparing `jupyterlab_new_launcher-0.2.3/src/launcher.tsx` & `jupyterlab_new_launcher-0.3.0/src/launcher.tsx`

 * *Files 2% similar despite different names*

```diff
@@ -166,15 +166,15 @@
           ) : (
             'No starred items'
           )}
         </CollapsibleSection>
       ) : null}
       <CollapsibleSection
         className="jp-Launcher-openByKernel jp-Launcher-launchNotebook"
-        title={trans.__('Launch Notebook')}
+        title={trans.__('Launch New Notebook')}
         icon={notebookIcon}
         open={startCollapsed['launch-notebook'] !== 'collapsed'}
       >
         <KernelTable
           items={props.notebookItems}
           commands={props.commands}
           showSearchBox={!searchAll}
@@ -182,15 +182,15 @@
           settings={props.settings}
           trans={trans}
           onClick={item => item.execute()}
         />
       </CollapsibleSection>
       <CollapsibleSection
         className="jp-Launcher-openByKernel jp-Launcher-launchConsole"
-        title={trans.__('Launch Console')}
+        title={trans.__('Launch New Console')}
         icon={consoleIcon}
         open={startCollapsed['launch-console'] !== 'collapsed'}
       >
         <KernelTable
           items={props.consoleItems}
           commands={props.commands}
           showSearchBox={!searchAll}
```

### Comparing `jupyterlab_new_launcher-0.2.3/src/types.ts` & `jupyterlab_new_launcher-0.3.0/src/types.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.3/src/components/card.tsx` & `jupyterlab_new_launcher-0.3.0/src/components/card.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.3/src/components/section.tsx` & `jupyterlab_new_launcher-0.3.0/src/components/section.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.3/src/components/table.tsx` & `jupyterlab_new_launcher-0.3.0/src/components/table.tsx`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 // Copyright (c) Nebari Development Team.
 // Distributed under the terms of the Modified BSD License.
 import type { CommandRegistry } from '@lumino/commands';
 import { ReadonlyJSONObject } from '@lumino/coreutils';
 import { Time } from '@jupyterlab/coreutils';
 import { ISettingRegistry } from '@jupyterlab/settingregistry';
 import { TranslationBundle } from '@jupyterlab/translation';
-import {
-  FilterBox,
-  Table,
-  UseSignal,
-  MenuSvg
-} from '@jupyterlab/ui-components';
+import { FilterBox, UseSignal, MenuSvg } from '@jupyterlab/ui-components';
+import { Table } from './base-table';
 import * as React from 'react';
 import { ISettingsLayout, CommandIDs, IKernelItem } from '../types';
 import { starIcon } from '../icons';
 
 const STAR_BUTTON_CLASS = 'jp-starIconButton';
 const KERNEL_ITEM_CLASS = 'jp-TableKernelItem';
 
@@ -37,14 +33,22 @@
       return 'Base?';
     case 'conda_is_currently_running':
       return 'Running?';
   }
   return key[0].toUpperCase() + key.substring(1);
 }
 
+function EllipsedCell(props: React.PropsWithChildren<{ title?: string }>) {
+  return (
+    <div className="jp-ellipsis-wrapper" title={props.title}>
+      <div className="jp-ellipsis">{props.children}</div>
+    </div>
+  );
+}
+
 export function KernelTable(props: {
   trans: TranslationBundle;
   items: IKernelItem[];
   commands: CommandRegistry;
   settings: ISettingRegistry.ISettings;
   showSearchBox: boolean;
   query: string;
@@ -83,22 +87,25 @@
       return {
         id: metadataKey,
         label: columnLabelFromKey(metadataKey),
         renderCell: (item: IKernelItem) => {
           const kernelMeta = item.metadata?.kernel as
             | ReadonlyJSONObject
             | undefined;
-          if (!kernelMeta) {
-            return '-';
-          }
-          const value = kernelMeta[metadataKey];
-          if (typeof value === 'string') {
-            return value;
-          }
-          return JSON.stringify(value);
+          const render = () => {
+            if (!kernelMeta) {
+              return '-';
+            }
+            const value = kernelMeta[metadataKey];
+            if (typeof value === 'string') {
+              return value;
+            }
+            return JSON.stringify(value);
+          };
+          return <EllipsedCell>{render()}</EllipsedCell>;
         },
         sort: (a: IKernelItem, b: IKernelItem) => {
           const aKernelMeta = a.metadata?.kernel as
             | ReadonlyJSONObject
             | undefined;
           const bKernelMeta = b.metadata?.kernel as
             | ReadonlyJSONObject
@@ -136,65 +143,73 @@
   }
 
   const availableColumns: Table.IColumn<IKernelItem>[] = [
     {
       id: 'kernel',
       label: trans.__('Kernel'),
       renderCell: (row: IKernelItem) => (
-        <>
-          <span
-            className="jp-LauncherCard-icon"
-            onClick={() => props.onClick(row)}
-          >
-            {row.kernelIconUrl ? (
-              <img
-                src={row.kernelIconUrl}
-                className="jp-Launcher-kernelIcon"
-                alt={row.label}
-              />
-            ) : (
-              <div className="jp-LauncherCard-noKernelIcon">
-                {row.label[0].toUpperCase()}
-              </div>
-            )}
-          </span>
+        <EllipsedCell>
           <span
             className={KERNEL_ITEM_CLASS}
             onClick={event => {
               props.onClick(row);
               event.stopPropagation();
             }}
             onKeyDown={event => {
               // TODO memoize func defs for perf
               if (event.key === 'Enter') {
                 row.execute();
               }
             }}
             tabIndex={0}
           >
-            {row.label}
+            <span
+              className="jp-LauncherCard-icon"
+              onClick={() => props.onClick(row)}
+            >
+              {row.kernelIconUrl ? (
+                <img
+                  src={row.kernelIconUrl}
+                  className="jp-Launcher-kernelIcon"
+                  alt={row.label}
+                />
+              ) : (
+                <div className="jp-LauncherCard-noKernelIcon">
+                  {row.label[0].toUpperCase()}
+                </div>
+              )}
+            </span>
+            <span className="jp-TableKernelItem-label">{row.label}</span>
           </span>
-        </>
+        </EllipsedCell>
       ),
       sort: (a: IKernelItem, b: IKernelItem) => a.label.localeCompare(b.label)
     },
     ...extraColumns,
     {
       id: 'last-used',
       label: trans.__('Last Used'),
       renderCell: (row: IKernelItem) => {
         return (
           <UseSignal signal={row.refreshLastUsed}>
             {() => {
-              return row.lastUsed ? (
-                <span title={Time.format(row.lastUsed)}>
-                  {Time.formatHuman(row.lastUsed)}
-                </span>
-              ) : (
-                trans.__('Never')
+              return (
+                <EllipsedCell
+                  title={
+                    row.lastUsed
+                      ? Time.format(row.lastUsed)
+                      : trans.__(
+                          'No information about last use of this kernel is available in the layout database'
+                        )
+                  }
+                >
+                  {row.lastUsed
+                    ? Time.formatHuman(row.lastUsed)
+                    : trans.__('Never')}
+                </EllipsedCell>
               );
             }}
           </UseSignal>
         );
       },
       sort: (a: IKernelItem, b: IKernelItem) => {
         if (a.lastUsed === b.lastUsed) {
```

### Comparing `jupyterlab_new_launcher-0.2.3/style/icons/code-server.svg` & `jupyterlab_new_launcher-0.3.0/style/icons/code-server.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.3/style/icons/md/LICENSE` & `jupyterlab_new_launcher-0.3.0/style/icons/md/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.3/ui-tests/README.md` & `jupyterlab_new_launcher-0.3.0/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.3/ui-tests/yarn.lock` & `jupyterlab_new_launcher-0.3.0/ui-tests/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.3/ui-tests/tests/jupyterlab_new_launcher.spec.ts` & `jupyterlab_new_launcher-0.3.0/ui-tests/tests/jupyterlab_new_launcher.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.3/.gitignore` & `jupyterlab_new_launcher-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.3/LICENSE` & `jupyterlab_new_launcher-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.3/README.md` & `jupyterlab_new_launcher-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.3/pyproject.toml` & `jupyterlab_new_launcher-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.2.3/PKG-INFO` & `jupyterlab_new_launcher-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jupyterlab-new-launcher
-Version: 0.2.3
+Version: 0.3.0
 Dynamic: Keywords
 Summary: A redesigned JupyterLab launcher
 Project-URL: Homepage, https://github.com/nebari-dev/jupyterlab-new-launcher
 Project-URL: Bug Tracker, https://github.com/nebari-dev/jupyterlab-new-launcher/issues
 Project-URL: Repository, https://github.com/nebari-dev/jupyterlab-new-launcher.git
 Author-email: Nebari development team <internal-it@quansight.com>
 License: BSD 3-Clause License
```

