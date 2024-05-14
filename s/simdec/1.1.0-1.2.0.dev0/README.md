# Comparing `tmp/simdec-1.1.0.tar.gz` & `tmp/simdec-1.2.0.dev0.tar.gz`

## Comparing `simdec-1.1.0.tar` & `simdec-1.2.0.dev0.tar`

### file list

```diff
@@ -1,14 +1,12 @@
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 simdec-1.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     5698 2020-02-02 00:00:00.000000 simdec-1.1.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 simdec-1.1.0/Dockerfile
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 simdec-1.1.0/Makefile
--rw-r--r--   0        0        0     9626 2020-02-02 00:00:00.000000 simdec-1.1.0/app.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 simdec-1.1.0/src/simdec/__init__.py
--rw-r--r--   0        0        0     5286 2020-02-02 00:00:00.000000 simdec-1.1.0/src/simdec/decomposition.py
--rw-r--r--   0        0        0     5619 2020-02-02 00:00:00.000000 simdec-1.1.0/src/simdec/sensitivity_indices.py
--rw-r--r--   0        0        0     5194 2020-02-02 00:00:00.000000 simdec-1.1.0/src/simdec/visualization.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 simdec-1.1.0/.gitignore
--rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 simdec-1.1.0/LICENSE.txt
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 simdec-1.1.0/README.md
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 simdec-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 simdec-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 simdec-1.2.0.dev0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     6600 2020-02-02 00:00:00.000000 simdec-1.2.0.dev0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 simdec-1.2.0.dev0/src/simdec/__init__.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 simdec-1.2.0.dev0/src/simdec/auth.py
+-rw-r--r--   0        0        0     5834 2020-02-02 00:00:00.000000 simdec-1.2.0.dev0/src/simdec/decomposition.py
+-rw-r--r--   0        0        0     5619 2020-02-02 00:00:00.000000 simdec-1.2.0.dev0/src/simdec/sensitivity_indices.py
+-rw-r--r--   0        0        0     7379 2020-02-02 00:00:00.000000 simdec-1.2.0.dev0/src/simdec/visualization.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 simdec-1.2.0.dev0/.gitignore
+-rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 simdec-1.2.0.dev0/LICENSE.txt
+-rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 simdec-1.2.0.dev0/README.md
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 simdec-1.2.0.dev0/pyproject.toml
+-rw-r--r--   0        0        0     4346 2020-02-02 00:00:00.000000 simdec-1.2.0.dev0/PKG-INFO
```

### Comparing `simdec-1.1.0/CONTRIBUTING.md` & `simdec-1.2.0.dev0/CONTRIBUTING.md`

 * *Files 12% similar despite different names*

```diff
@@ -157,7 +157,43 @@
 1. Update the version in the main `pyproject.toml`.
 2. Build locally using `hatch build`, and verify the content of the artifacts
 3. Submit PR, wait for tests to pass, and merge release into `main`
 4. Tag release with version number and push to the repo
 5. Check that release has been deployed to PyPI
 6. Check documentation is built and deployed to readthedocs
 7. Check that auto-generated PR is auto-merged on the conda-forge feedstock repo
+
+## Dashboard
+A live dashboard is available at:
+
+https://simdec.io
+
+The DNS records are available on CPanel and the rest is hosted on Google Cloud
+Platform.
+
+Developing locally requires the installation of GCP CLI and Docker engine.
+
+A few helper commands are provided in the Makefile.
+
+### Local use
+
+The dashboard can be run locally using:
+
+    make serve-dev
+
+If you want to test OAuth, you need to export the following env variables:
+
+    export PANEL_OAUTH_REDIRECT_URI=http://localhost:5006/app
+    export PANEL_OAUTH_KEY=[VALUE IN GCP Secret Manager]
+    export PANEL_OAUTH_SECRET=[VALUE IN GCP Secret Manager]
+    export PANEL_OAUTH_ENCRYPTION=[VALUE IN GCP Secret Manager]
+
+Use the CLI tool `direnv` for convenience. Then you can serve with
+OAuth support:
+
+    make serve-oauth
+
+### Deployment
+
+New version can either be deployed from the CI with `cloudbuild` or locally:
+
+    make production
```

### Comparing `simdec-1.1.0/src/simdec/decomposition.py` & `simdec-1.2.0.dev0/src/simdec/decomposition.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,69 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
+from hashlib import blake2b
 from typing import Literal
 
 import numpy as np
 import pandas as pd
 from scipy import stats
 
 
 __all__ = ["decomposition", "states_expansion"]
 
 
 def states_expansion(states: list[int], inputs: pd.DataFrame) -> list[list[str]]:
     """Expand states list to fully represent all scenarios."""
     inputs = pd.DataFrame(inputs)
-    for i, state in enumerate(states):
+    expanded_states = []
+    for state in states:
         if isinstance(state, int):
-            states: list
             if state == 2:
-                states[i] = ["low", "high"]
+                expanded_states.append(["low", "high"])
             elif state == 3:
-                states[i] = ["low", "medium", "high"]
+                expanded_states.append(["low", "medium", "high"])
+        else:
+            expanded_states.append(state)
 
     # categorical for a given variable
     cat_cols = inputs.select_dtypes(exclude=["number"])
     cat_cols_idx = []
     states_cats_ = []
     for cat_col in cat_cols:
         _, cats = pd.factorize(inputs[cat_col])
         cat_cols_idx.append(inputs.columns.get_loc(cat_col))
         states_cats_.append(cats)
 
     for i, states_cat_ in zip(cat_cols_idx, states_cats_):
         n_unique = np.unique(inputs.iloc[:, i]).size
-        states[i] = list(states_cat_) if n_unique < 5 else states[i]
+        expanded_states[i] = list(states_cat_) if n_unique < 5 else expanded_states[i]
 
-    return states
+    return expanded_states
 
 
 @dataclass
 class DecompositionResult:
     var_names: list[str]
     statistic: np.ndarray
     bins: pd.DataFrame
     states: list[int]
     bin_edges: np.ndarray
 
+    def __reduce__(self):
+        h = blake2b(key=b"result hashing", digest_size=20)
+
+        h.update(str(self.var_names).encode())
+        h.update(str(self.statistic).encode())
+        h.update(str(self.bins).encode())
+        h.update(str(self.states).encode())
+        h.update(str(self.bin_edges).encode())
+
+        return [h.hexdigest()]
+
 
 def decomposition(
     inputs: pd.DataFrame,
     output: pd.DataFrame,
     *,
     sensitivity_indices: np.ndarray,
     dec_limit: float = 1,
@@ -105,17 +119,21 @@
     output = output.to_numpy()
 
     # 1. variables for decomposition
     var_order = np.argsort(sensitivity_indices)[::-1]
 
     # only keep the explained variance corresponding to `dec_limit`
     sensitivity_indices = sensitivity_indices[var_order]
-    n_var_dec = np.where(np.cumsum(sensitivity_indices) < dec_limit)[0].size
-    n_var_dec = max(1, n_var_dec)  # keep at least one variable
-    n_var_dec = min(5, n_var_dec)  # use at most 5 variables
+
+    if auto_ordering:
+        n_var_dec = np.where(np.cumsum(sensitivity_indices) < dec_limit)[0].size
+        n_var_dec = max(1, n_var_dec)  # keep at least one variable
+        n_var_dec = min(5, n_var_dec)  # use at most 5 variables
+    else:
+        n_var_dec = inputs.shape[1]
 
     # 2. states formation
     if states is None:
         states = 3 if n_var_dec < 3 else 2
         states = [states] * n_var_dec
 
         # categorical for a given variable
```

### Comparing `simdec-1.1.0/src/simdec/sensitivity_indices.py` & `simdec-1.2.0.dev0/src/simdec/sensitivity_indices.py`

 * *Files identical despite different names*

### Comparing `simdec-1.1.0/LICENSE.txt` & `simdec-1.2.0.dev0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `simdec-1.1.0/README.md` & `simdec-1.2.0.dev0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -23,51 +23,25 @@
 [discord community](https://discord.gg/54SFcNsZS4).
 
 ## Python API
 The library is distributed on PyPi and can be installed with:
 
     pip install simdec
 
-To install the development version, download the source and from the root of
-the repository:
-
-    pip install -e .[dev]
-
 ## Dashboard
 A live dashboard is available at:
 
 https://simdec.io
 
-### Local use
-
-The dashboard can be run locally using:
-
-    make serve
-
-### Deployment
-
-The live version of the dashboard is hosted on GCP. To deploy a new version:
-
-    PANEL_TOKEN=... make production
-
-###
-
 ## Citations
 
 The algorithms and visualizations used in this package came primarily out of
 research at LUT University, Lappeenranta, Finland, and Stanford University,
 California, U.S., supported with grants from Business Finland, Wihuri
 Foundation, and Finnish Foundation for Economic Education.
 
 If you use SimDec in your research we would appreciate a citation to the
 following publications:
 
-- Kozlova, M., & Yeomans, J. S. (2022). Monte Carlo Enhancement via Simulation
-  Decomposition: A “Must-Have” Inclusion for Many Disciplines. _INFORMS
-  Transactions on Education, 22_(3), 147-159. DOI:10.1287/ited.2019.0240.
-- Kozlova, M., Moss, R. J., Yeomans, J. S., & Caers, J. (forthcoming).
-  Uncovering Heterogeneous Effects in Computational Models for Sustainable
-  Decision-making. _Environmental Modelling & Software_.
-- Kozlova, M., Moss, R. J., Roy, P., Alam, A., & Yeomans, J. S. (forthcoming).
-  SimDec algorithm. In M. Kozlova & J. S. Yeomans (Eds.), _Sensitivity Analysis
-  for Business, Technology, and Policymaking Made Easy with Simulation
-  Decomposition_. Routledge.
+- Kozlova, M., & Yeomans, J. S. (2022). Monte Carlo Enhancement via Simulation Decomposition: A “Must-Have” Inclusion for Many Disciplines. _INFORMS Transactions on Education, 22_(3), 147-159. [Available here](https://pubsonline.informs.org/doi/10.1287/ited.2019.0240).
+- Kozlova, M., Moss, R. J., Yeomans, J. S., & Caers, J. (2024). Uncovering Heterogeneous Effects in Computational Models for Sustainable Decision-making. _Environmental Modelling & Software_, 171, 105898. [https://doi.org/10.1016/j.envsoft.2023.105898](https://doi.org/10.1016/j.envsoft.2023.105898)
+- Kozlova, M., Moss, R. J., Roy, P., Alam, A., & Yeomans, J. S. (forthcoming). SimDec algorithm and guidelines for its usage and interpretation. In M. Kozlova & J. S. Yeomans (Eds.), _Sensitivity Analysis for Business, Technology, and Policymaking. Made Easy with Simulation Decomposition_. Routledge.
```

### Comparing `simdec-1.1.0/pyproject.toml` & `simdec-1.2.0.dev0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = ["hatchling>=1.14.0"]
 build-backend = "hatchling.build"
 
 [project]
 name = "simdec"
-version = "1.1.0"
+version = "1.2.0dev0"
 description = "Sensitivity analysis using simulation decomposition"
 readme = "README.md"
-requires-python = ">=3.9"
+requires-python = ">=3.10"
 license = "BSD-3-Clause"
 authors = [
     { name = "Pamphile Roy" },
 ]
 maintainers = [
     { name = "simdec contributors" },
 ]
@@ -19,65 +19,72 @@
     "Intended Audience :: End Users/Desktop",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: BSD License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
 ]
 
 dependencies = [
     "numpy",
     "pandas",
     "SALib",
     "seaborn",
-    "typer[all]",
-    "panel",
 ]
 
 [project.optional-dependencies]
+dashboard = [
+    "panel>=1.3.8",
+    "cryptography",
+]
+
 test = [
     "pytest",
     "pytest-cov",
 ]
 
 doc = [
     "sphinx",
     "pydata-sphinx-theme",
     "accessible-pygments",
     "numpydoc",
 ]
 
 dev = [
-    "simdec[doc,test]",
+    "simdec[doc,test,dashboard]",
     "pre-commit",
     "hatch",
 ]
 
-[project.scripts]
-simdec = "simdec.workflow:app"
-
 [project.urls]
 homepage = "https://www.simdec.fi/"
 documentation = "https://simdec.readthedocs.io"
 source = "https://github.com/Simulation-Decomposition/simdec-python"
 
 [tool.hatch]
+build.targets.wheel.packages = ["src/simdec"]
 build.targets.sdist.exclude = [
   ".github",
   "docs",
+  "panel",
   "tests",
   "*.rst",
   "*.yml",
   ".*",
+  "Makefile",
+  "Dockerfile",
 ]
 
+[project.entry-points."panel.auth"]
+custom_google = "simdec.auth:CustomGoogleLoginHandler"
+
 [tool.pytest.ini_options]
 addopts = "--durations 10"
 testpaths = [
     "tests",
 ]
 
 [tool.ruff.per-file-ignores]
```

### Comparing `simdec-1.1.0/PKG-INFO` & `simdec-1.2.0.dev0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: simdec
-Version: 1.1.0
+Version: 1.2.0.dev0
 Summary: Sensitivity analysis using simulation decomposition
 Project-URL: homepage, https://www.simdec.fi/
 Project-URL: documentation, https://simdec.readthedocs.io
 Project-URL: source, https://github.com/Simulation-Decomposition/simdec-python
 Author: Pamphile Roy
 Maintainer: simdec contributors
 License-Expression: BSD-3-Clause
@@ -12,28 +12,36 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.9
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.10
 Requires-Dist: numpy
 Requires-Dist: pandas
-Requires-Dist: panel
 Requires-Dist: salib
 Requires-Dist: seaborn
-Requires-Dist: typer[all]
+Provides-Extra: dashboard
+Requires-Dist: cryptography; extra == 'dashboard'
+Requires-Dist: panel>=1.3.8; extra == 'dashboard'
 Provides-Extra: dev
+Requires-Dist: accessible-pygments; extra == 'dev'
+Requires-Dist: cryptography; extra == 'dev'
 Requires-Dist: hatch; extra == 'dev'
+Requires-Dist: numpydoc; extra == 'dev'
+Requires-Dist: panel>=1.3.8; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
-Requires-Dist: simdec[doc,test]; extra == 'dev'
+Requires-Dist: pydata-sphinx-theme; extra == 'dev'
+Requires-Dist: pytest; extra == 'dev'
+Requires-Dist: pytest-cov; extra == 'dev'
+Requires-Dist: sphinx; extra == 'dev'
 Provides-Extra: doc
 Requires-Dist: accessible-pygments; extra == 'doc'
 Requires-Dist: numpydoc; extra == 'doc'
 Requires-Dist: pydata-sphinx-theme; extra == 'doc'
 Requires-Dist: sphinx; extra == 'doc'
 Provides-Extra: test
 Requires-Dist: pytest; extra == 'test'
@@ -65,51 +73,25 @@
 [discord community](https://discord.gg/54SFcNsZS4).
 
 ## Python API
 The library is distributed on PyPi and can be installed with:
 
     pip install simdec
 
-To install the development version, download the source and from the root of
-the repository:
-
-    pip install -e .[dev]
-
 ## Dashboard
 A live dashboard is available at:
 
 https://simdec.io
 
-### Local use
-
-The dashboard can be run locally using:
-
-    make serve
-
-### Deployment
-
-The live version of the dashboard is hosted on GCP. To deploy a new version:
-
-    PANEL_TOKEN=... make production
-
-###
-
 ## Citations
 
 The algorithms and visualizations used in this package came primarily out of
 research at LUT University, Lappeenranta, Finland, and Stanford University,
 California, U.S., supported with grants from Business Finland, Wihuri
 Foundation, and Finnish Foundation for Economic Education.
 
 If you use SimDec in your research we would appreciate a citation to the
 following publications:
 
-- Kozlova, M., & Yeomans, J. S. (2022). Monte Carlo Enhancement via Simulation
-  Decomposition: A “Must-Have” Inclusion for Many Disciplines. _INFORMS
-  Transactions on Education, 22_(3), 147-159. DOI:10.1287/ited.2019.0240.
-- Kozlova, M., Moss, R. J., Yeomans, J. S., & Caers, J. (forthcoming).
-  Uncovering Heterogeneous Effects in Computational Models for Sustainable
-  Decision-making. _Environmental Modelling & Software_.
-- Kozlova, M., Moss, R. J., Roy, P., Alam, A., & Yeomans, J. S. (forthcoming).
-  SimDec algorithm. In M. Kozlova & J. S. Yeomans (Eds.), _Sensitivity Analysis
-  for Business, Technology, and Policymaking Made Easy with Simulation
-  Decomposition_. Routledge.
+- Kozlova, M., & Yeomans, J. S. (2022). Monte Carlo Enhancement via Simulation Decomposition: A “Must-Have” Inclusion for Many Disciplines. _INFORMS Transactions on Education, 22_(3), 147-159. [Available here](https://pubsonline.informs.org/doi/10.1287/ited.2019.0240).
+- Kozlova, M., Moss, R. J., Yeomans, J. S., & Caers, J. (2024). Uncovering Heterogeneous Effects in Computational Models for Sustainable Decision-making. _Environmental Modelling & Software_, 171, 105898. [https://doi.org/10.1016/j.envsoft.2023.105898](https://doi.org/10.1016/j.envsoft.2023.105898)
+- Kozlova, M., Moss, R. J., Roy, P., Alam, A., & Yeomans, J. S. (forthcoming). SimDec algorithm and guidelines for its usage and interpretation. In M. Kozlova & J. S. Yeomans (Eds.), _Sensitivity Analysis for Business, Technology, and Policymaking. Made Easy with Simulation Decomposition_. Routledge.
```

