# Comparing `tmp/tableau_migration-2.1.1.tar.gz` & `tmp/tableau_migration-3.0.0.tar.gz`

## Comparing `tableau_migration-2.1.1.tar` & `tableau_migration-3.0.0.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/requirements.txt
--rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/__init__.py
--rw-r--r--   0        0        0     8648 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/migration.py
--rw-r--r--   0        0        0    18376 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/migration_engine.py
--rw-r--r--   0        0        0     4275 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/migration_engine_hooks.py
--rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/migration_engine_hooks_filters.py
--rw-r--r--   0        0        0     3670 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/migration_engine_hooks_mappings.py
--rw-r--r--   0        0        0     3713 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/migration_engine_hooks_transformers.py
--rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/migration_engine_migrators.py
--rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/migration_engine_options.py
--rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/migration_logger.py
--rw-r--r--   0        0        0    19104 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Bcl.AsyncInterfaces.dll
--rw-r--r--   0        0        0    32432 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Bcl.TimeProvider.dll
--rw-r--r--   0        0        0    34848 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.AmbientMetadata.Application.dll
--rw-r--r--   0        0        0    40488 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Compliance.Abstractions.dll
--rw-r--r--   0        0        0    29448 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Configuration.Abstractions.dll
--rw-r--r--   0        0        0    44808 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Configuration.Binder.dll
--rw-r--r--   0        0        0    23312 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Configuration.EnvironmentVariables.dll
--rw-r--r--   0        0        0    45328 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Configuration.dll
--rw-r--r--   0        0        0    63264 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.DependencyInjection.Abstractions.dll
--rw-r--r--   0        0        0    34224 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.DependencyInjection.AutoActivation.dll
--rw-r--r--   0        0        0    93984 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.DependencyInjection.dll
--rw-r--r--   0        0        0    41376 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.DiagnosticAdapter.dll
--rw-r--r--   0        0        0    32008 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Diagnostics.Abstractions.dll
--rw-r--r--   0        0        0    31152 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Diagnostics.ExceptionSummarization.dll
--rw-r--r--   0        0        0    37144 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Diagnostics.dll
--rw-r--r--   0        0        0    23728 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.FileProviders.Abstractions.dll
--rw-r--r--   0        0        0    53000 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Hosting.Abstractions.dll
--rw-r--r--   0        0        0   115248 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Http.Diagnostics.dll
--rw-r--r--   0        0        0   129056 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Http.Resilience.dll
--rw-r--r--   0        0        0    89368 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Http.dll
--rw-r--r--   0        0        0    21680 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Localization.Abstractions.dll
--rw-r--r--   0        0        0    33968 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Localization.dll
--rw-r--r--   0        0        0    66336 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Logging.Abstractions.dll
--rw-r--r--   0        0        0    29968 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Logging.Configuration.dll
--rw-r--r--   0        0        0    52496 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Logging.dll
--rw-r--r--   0        0        0    25264 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.ObjectPool.dll
--rw-r--r--   0        0        0    24336 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Options.ConfigurationExtensions.dll
--rw-r--r--   0        0        0    66312 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Options.dll
--rw-r--r--   0        0        0    45336 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Primitives.dll
--rw-r--r--   0        0        0    37936 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Resilience.dll
--rw-r--r--   0        0        0    55344 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Telemetry.Abstractions.dll
--rw-r--r--   0        0        0   116768 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Telemetry.dll
--rw-r--r--   0        0        0    65568 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.IO.RecyclableMemoryStream.dll
--rw-r--r--   0        0        0   242976 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Polly.Core.dll
--rw-r--r--   0        0        0    56736 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Polly.Extensions.dll
--rw-r--r--   0        0        0    29600 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Polly.RateLimiting.dll
--rw-r--r--   0        0        0   247584 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/System.Collections.Immutable.dll
--rw-r--r--   0        0        0   164616 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/System.Diagnostics.DiagnosticSource.dll
--rw-r--r--   0        0        0     6656 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/System.IO.Abstractions.dll
--rw-r--r--   0        0        0    71440 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/System.Text.Encodings.Web.dll
--rw-r--r--   0        0        0   579848 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/System.Text.Json.dll
--rw-r--r--   0        0        0    70416 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/System.Threading.RateLimiting.dll
--rw-r--r--   0        0        0    37426 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Tableau.Migration.deps.json
--rw-r--r--   0        0        0   985600 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Tableau.Migration.dll
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Tableau.Migration.runtimeconfig.json
--rw-r--r--   0        0        0  1074636 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/Tableau.Migration.xml
--rw-r--r--   0        0        0    53248 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/TestableIO.System.IO.Abstractions.Wrappers.dll
--rw-r--r--   0        0        0    29184 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/TestableIO.System.IO.Abstractions.dll
--rw-r--r--   0        0        0    71448 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/src/tableau_migration/bin/runtimes/browser/lib/net6.0/System.Text.Encodings.Web.dll
--rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/.gitignore
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/LICENSE
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/README.md
--rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/pyproject.toml
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 tableau_migration-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/requirements.txt
+-rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/__init__.py
+-rw-r--r--   0        0        0     8648 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/migration.py
+-rw-r--r--   0        0        0    18376 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/migration_engine.py
+-rw-r--r--   0        0        0     4275 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/migration_engine_hooks.py
+-rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/migration_engine_hooks_filters.py
+-rw-r--r--   0        0        0     3670 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/migration_engine_hooks_mappings.py
+-rw-r--r--   0        0        0     3713 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/migration_engine_hooks_transformers.py
+-rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/migration_engine_migrators.py
+-rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/migration_engine_options.py
+-rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/migration_logger.py
+-rw-r--r--   0        0        0    19104 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Bcl.AsyncInterfaces.dll
+-rw-r--r--   0        0        0    32432 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Bcl.TimeProvider.dll
+-rw-r--r--   0        0        0    34848 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.AmbientMetadata.Application.dll
+-rw-r--r--   0        0        0    40488 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.Compliance.Abstractions.dll
+-rw-r--r--   0        0        0    29448 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.Configuration.Abstractions.dll
+-rw-r--r--   0        0        0    44808 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.Configuration.Binder.dll
+-rw-r--r--   0        0        0    23312 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.Configuration.EnvironmentVariables.dll
+-rw-r--r--   0        0        0    45328 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.Configuration.dll
+-rw-r--r--   0        0        0    63264 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.DependencyInjection.Abstractions.dll
+-rw-r--r--   0        0        0    34224 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.DependencyInjection.AutoActivation.dll
+-rw-r--r--   0        0        0    93984 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.DependencyInjection.dll
+-rw-r--r--   0        0        0    41376 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.DiagnosticAdapter.dll
+-rw-r--r--   0        0        0    32008 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.Diagnostics.Abstractions.dll
+-rw-r--r--   0        0        0    31152 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.Diagnostics.ExceptionSummarization.dll
+-rw-r--r--   0        0        0    37144 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.Diagnostics.dll
+-rw-r--r--   0        0        0    23728 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.FileProviders.Abstractions.dll
+-rw-r--r--   0        0        0    53000 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.Hosting.Abstractions.dll
+-rw-r--r--   0        0        0   115248 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.Http.Diagnostics.dll
+-rw-r--r--   0        0        0   129056 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.Http.Resilience.dll
+-rw-r--r--   0        0        0    89368 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.Http.dll
+-rw-r--r--   0        0        0    21680 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.Localization.Abstractions.dll
+-rw-r--r--   0        0        0    33968 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.Localization.dll
+-rw-r--r--   0        0        0    66336 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.Logging.Abstractions.dll
+-rw-r--r--   0        0        0    29968 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.Logging.Configuration.dll
+-rw-r--r--   0        0        0    52496 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.Logging.dll
+-rw-r--r--   0        0        0    25264 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.ObjectPool.dll
+-rw-r--r--   0        0        0    24336 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.Options.ConfigurationExtensions.dll
+-rw-r--r--   0        0        0    66312 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.Options.dll
+-rw-r--r--   0        0        0    45336 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.Primitives.dll
+-rw-r--r--   0        0        0    37936 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.Resilience.dll
+-rw-r--r--   0        0        0    55344 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.Telemetry.Abstractions.dll
+-rw-r--r--   0        0        0   116768 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.Telemetry.dll
+-rw-r--r--   0        0        0    65568 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.IO.RecyclableMemoryStream.dll
+-rw-r--r--   0        0        0   242976 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/bin/Polly.Core.dll
+-rw-r--r--   0        0        0    56736 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/bin/Polly.Extensions.dll
+-rw-r--r--   0        0        0    29600 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/bin/Polly.RateLimiting.dll
+-rw-r--r--   0        0        0   247584 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/bin/System.Collections.Immutable.dll
+-rw-r--r--   0        0        0   164616 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/bin/System.Diagnostics.DiagnosticSource.dll
+-rw-r--r--   0        0        0     6656 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/bin/System.IO.Abstractions.dll
+-rw-r--r--   0        0        0    71440 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/bin/System.Text.Encodings.Web.dll
+-rw-r--r--   0        0        0   579848 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/bin/System.Text.Json.dll
+-rw-r--r--   0        0        0    70416 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/bin/System.Threading.RateLimiting.dll
+-rw-r--r--   0        0        0    37426 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/bin/Tableau.Migration.deps.json
+-rw-r--r--   0        0        0  1008128 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/bin/Tableau.Migration.dll
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/bin/Tableau.Migration.runtimeconfig.json
+-rw-r--r--   0        0        0  1094499 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/bin/Tableau.Migration.xml
+-rw-r--r--   0        0        0    53248 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/bin/TestableIO.System.IO.Abstractions.Wrappers.dll
+-rw-r--r--   0        0        0    29184 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/bin/TestableIO.System.IO.Abstractions.dll
+-rw-r--r--   0        0        0    71448 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/src/tableau_migration/bin/runtimes/browser/lib/net6.0/System.Text.Encodings.Web.dll
+-rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/.gitignore
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/LICENSE
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/README.md
+-rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 tableau_migration-3.0.0/PKG-INFO
```

### Comparing `tableau_migration-2.1.1/src/tableau_migration/__init__.py` & `tableau_migration-3.0.0/src/tableau_migration/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2023, Salesforce, Inc.
+# Copyright (c) 2024, Salesforce, Inc.
 # SPDX-License-Identifier: Apache-2
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `tableau_migration-2.1.1/src/tableau_migration/migration.py` & `tableau_migration-3.0.0/src/tableau_migration/migration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2023, Salesforce, Inc.
+# Copyright (c) 2024, Salesforce, Inc.
 # SPDX-License-Identifier: Apache-2
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `tableau_migration-2.1.1/src/tableau_migration/migration_engine.py` & `tableau_migration-3.0.0/src/tableau_migration/migration_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2023, Salesforce, Inc.
+# Copyright (c) 2024, Salesforce, Inc.
 # SPDX-License-Identifier: Apache-2
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `tableau_migration-2.1.1/src/tableau_migration/migration_engine_hooks.py` & `tableau_migration-3.0.0/src/tableau_migration/migration_engine_hooks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2023, Salesforce, Inc.
+# Copyright (c) 2024, Salesforce, Inc.
 # SPDX-License-Identifier: Apache-2
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `tableau_migration-2.1.1/src/tableau_migration/migration_engine_hooks_filters.py` & `tableau_migration-3.0.0/src/tableau_migration/migration_engine_hooks_filters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2023, Salesforce, Inc.
+# Copyright (c) 2024, Salesforce, Inc.
 # SPDX-License-Identifier: Apache-2
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `tableau_migration-2.1.1/src/tableau_migration/migration_engine_hooks_mappings.py` & `tableau_migration-3.0.0/src/tableau_migration/migration_engine_hooks_mappings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2023, Salesforce, Inc.
+# Copyright (c) 2024, Salesforce, Inc.
 # SPDX-License-Identifier: Apache-2
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `tableau_migration-2.1.1/src/tableau_migration/migration_engine_hooks_transformers.py` & `tableau_migration-3.0.0/src/tableau_migration/migration_engine_hooks_transformers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2023, Salesforce, Inc.
+# Copyright (c) 2024, Salesforce, Inc.
 # SPDX-License-Identifier: Apache-2
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `tableau_migration-2.1.1/src/tableau_migration/migration_engine_migrators.py` & `tableau_migration-3.0.0/src/tableau_migration/migration_engine_migrators.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2023, Salesforce, Inc.
+# Copyright (c) 2024, Salesforce, Inc.
 # SPDX-License-Identifier: Apache-2
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `tableau_migration-2.1.1/src/tableau_migration/migration_engine_options.py` & `tableau_migration-3.0.0/src/tableau_migration/migration_engine_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2023, Salesforce, Inc.
+# Copyright (c) 2024, Salesforce, Inc.
 # SPDX-License-Identifier: Apache-2
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `tableau_migration-2.1.1/src/tableau_migration/migration_logger.py` & `tableau_migration-3.0.0/src/tableau_migration/migration_logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2023, Salesforce, Inc.
+# Copyright (c) 2024, Salesforce, Inc.
 # SPDX-License-Identifier: Apache-2
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Bcl.AsyncInterfaces.dll` & `tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Bcl.AsyncInterfaces.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Bcl.TimeProvider.dll` & `tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Bcl.TimeProvider.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.AmbientMetadata.Application.dll` & `tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.AmbientMetadata.Application.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Compliance.Abstractions.dll` & `tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.Compliance.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Configuration.Abstractions.dll` & `tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.Configuration.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Configuration.Binder.dll` & `tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.Configuration.Binder.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Configuration.EnvironmentVariables.dll` & `tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.Configuration.EnvironmentVariables.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Configuration.dll` & `tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.Configuration.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.DependencyInjection.Abstractions.dll` & `tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.DependencyInjection.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.DependencyInjection.AutoActivation.dll` & `tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.DependencyInjection.AutoActivation.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.DependencyInjection.dll` & `tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.DependencyInjection.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.DiagnosticAdapter.dll` & `tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.DiagnosticAdapter.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Diagnostics.Abstractions.dll` & `tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.Diagnostics.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Diagnostics.ExceptionSummarization.dll` & `tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.Diagnostics.ExceptionSummarization.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Diagnostics.dll` & `tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.Diagnostics.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.FileProviders.Abstractions.dll` & `tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.FileProviders.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Hosting.Abstractions.dll` & `tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.Hosting.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Http.Diagnostics.dll` & `tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.Http.Diagnostics.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Http.Resilience.dll` & `tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.Http.Resilience.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Http.dll` & `tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.Http.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Localization.Abstractions.dll` & `tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.Localization.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Localization.dll` & `tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.Localization.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Logging.Abstractions.dll` & `tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.Logging.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Logging.Configuration.dll` & `tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.Logging.Configuration.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Logging.dll` & `tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.Logging.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.ObjectPool.dll` & `tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.ObjectPool.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Options.ConfigurationExtensions.dll` & `tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.Options.ConfigurationExtensions.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Options.dll` & `tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.Options.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Primitives.dll` & `tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.Primitives.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Resilience.dll` & `tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.Resilience.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Telemetry.Abstractions.dll` & `tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.Telemetry.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.Extensions.Telemetry.dll` & `tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.Extensions.Telemetry.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.1/src/tableau_migration/bin/Microsoft.IO.RecyclableMemoryStream.dll` & `tableau_migration-3.0.0/src/tableau_migration/bin/Microsoft.IO.RecyclableMemoryStream.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.1/src/tableau_migration/bin/Polly.Core.dll` & `tableau_migration-3.0.0/src/tableau_migration/bin/Polly.Core.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.1/src/tableau_migration/bin/Polly.Extensions.dll` & `tableau_migration-3.0.0/src/tableau_migration/bin/Polly.Extensions.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.1/src/tableau_migration/bin/Polly.RateLimiting.dll` & `tableau_migration-3.0.0/src/tableau_migration/bin/Polly.RateLimiting.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.1/src/tableau_migration/bin/System.Collections.Immutable.dll` & `tableau_migration-3.0.0/src/tableau_migration/bin/System.Collections.Immutable.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.1/src/tableau_migration/bin/System.Diagnostics.DiagnosticSource.dll` & `tableau_migration-3.0.0/src/tableau_migration/bin/System.Diagnostics.DiagnosticSource.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.1/src/tableau_migration/bin/System.IO.Abstractions.dll` & `tableau_migration-3.0.0/src/tableau_migration/bin/System.IO.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.1/src/tableau_migration/bin/System.Text.Encodings.Web.dll` & `tableau_migration-3.0.0/src/tableau_migration/bin/System.Text.Encodings.Web.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.1/src/tableau_migration/bin/System.Text.Json.dll` & `tableau_migration-3.0.0/src/tableau_migration/bin/System.Text.Json.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.1/src/tableau_migration/bin/System.Threading.RateLimiting.dll` & `tableau_migration-3.0.0/src/tableau_migration/bin/System.Threading.RateLimiting.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.1/src/tableau_migration/bin/Tableau.Migration.deps.json` & `tableau_migration-3.0.0/src/tableau_migration/bin/Tableau.Migration.deps.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9921875%*

 * *Differences: {"'libraries'": "{'Tableau.Migration/3.0.0': OrderedDict([('type', 'project'), ('serviceable', "*

 * *                "False), ('sha512', '')]), delete: ['Tableau.Migration/2.1.1']}",*

 * * "'targets'": "{'.NETCoreApp,Version=v6.0': {'Tableau.Migration/3.0.0': "*

 * *              "OrderedDict([('dependencies', "*

 * *              "OrderedDict([('Microsoft.Extensions.Configuration.EnvironmentVariables', '8.0.0'), "*

 * *              "('Microsoft.Extensions.Http', '8.0.0'), ('Microsoft.Extensions.Http.Resilience', "*

 * *               […]*

```diff
@@ -305,15 +305,15 @@
         "System.Threading.RateLimiting/8.0.0": {
             "hashPath": "system.threading.ratelimiting.8.0.0.nupkg.sha512",
             "path": "system.threading.ratelimiting/8.0.0",
             "serviceable": true,
             "sha512": "sha512-7mu9v0QDv66ar3DpGSZHg9NuNcxDaaAcnMULuZlaTpP9+hwXhrxNGsF5GmLkSHxFdb5bBc1TzeujsRgTrPWi+Q==",
             "type": "package"
         },
-        "Tableau.Migration/2.1.1": {
+        "Tableau.Migration/3.0.0": {
             "serviceable": false,
             "sha512": "",
             "type": "project"
         },
         "TestableIO.System.IO.Abstractions.Wrappers/20.0.15": {
             "hashPath": "testableio.system.io.abstractions.wrappers.20.0.15.nupkg.sha512",
             "path": "testableio.system.io.abstractions.wrappers/20.0.15",
@@ -859,15 +859,15 @@
                 "runtime": {
                     "lib/net6.0/System.Threading.RateLimiting.dll": {
                         "assemblyVersion": "8.0.0.0",
                         "fileVersion": "8.0.23.53103"
                     }
                 }
             },
-            "Tableau.Migration/2.1.1": {
+            "Tableau.Migration/3.0.0": {
                 "dependencies": {
                     "Microsoft.Extensions.Configuration.EnvironmentVariables": "8.0.0",
                     "Microsoft.Extensions.Http": "8.0.0",
                     "Microsoft.Extensions.Http.Resilience": "8.2.0",
                     "Microsoft.Extensions.Localization": "8.0.2",
                     "Microsoft.Extensions.Options.ConfigurationExtensions": "8.0.0",
                     "Microsoft.IO.RecyclableMemoryStream": "3.0.0",
```

### Comparing `tableau_migration-2.1.1/src/tableau_migration/bin/Tableau.Migration.dll` & `tableau_migration-3.0.0/src/tableau_migration/bin/Tableau.Migration.dll`

 * *Files 22% similar despite different names*

#### pedump {}

```diff
@@ -1,146 +1,146 @@
 
 COFF Header:
 	                Machine: 0x014c
 	               Sections: 0x0003
-	             Time stamp: 0xe89acb94
+	             Time stamp: 0xd0c28832
 	Pointer to Symbol Table: 0x00000000
 	   	   Symbol Count: 0x00000000
 	   Optional Header Size: 0x00e0
 	   	Characteristics: 0x2022
 
 PE Header:
 	         Magic (0x010b): 0x010b
 	             LMajor (6): 0x30
 	             LMinor (0): 0x00
-	              Code Size: 0x000efa00
+	              Code Size: 0x000f5200
 	  Initialized Data Size: 0x00000e00
 	Uninitialized Data Size: 0x00000000
-	        Entry Point RVA: 0x000f19ca
+	        Entry Point RVA: 0x000f7156
 	 	  Code Base RVA: 0x00002000
-		  Data Base RVA: 0x000f2000
+		  Data Base RVA: 0x000f8000
 
 
 NT Header:
 	   Image Base (0x400000): 0x10000000
 	Section Alignment (8192): 0x00002000
 	   File Align (512/4096): 0x00000200
 	            OS Major (4): 0x0004
 	            OS Minor (0): 0x0000
 	  	  User Major (0): 0x0000
 	  	  User Minor (0): 0x0000
 	  	Subsys major (4): 0x0004
 	  	Subsys minor (0): 0x0000
 	 	       Reserverd: 0x00000000
-	 	      Image Size: 0x000f6000
+	 	      Image Size: 0x000fc000
 	 	     Header Size: 0x00000200
 	            Checksum (0): 0x00000000
 	               Subsystem: 0x0003
 	           DLL Flags (0): 0x8560
 	 Stack Reserve Size (1M): 0x00100000
 	Stack commit Size (4096): 0x00001000
 	  Heap Reserve Size (1M): 0x00100000
 	 Heap Commit Size (4096): 0x00001000
 	      Loader flags (0x1): 0x00000000
 	   Data Directories (16): 0x00000010
 
 Data directories:
 	     Export Table: 0x00000000 [0x00000000]
-	     Import Table: 0x000f1978 [0x0000004f]
-	   Resource Table: 0x000f2000 [0x00000a7c]
+	     Import Table: 0x000f7104 [0x0000004f]
+	   Resource Table: 0x000f8000 [0x00000a6c]
 	  Exception Table: 0x00000000 [0x00000000]
 	Certificate Table: 0x00000000 [0x00000000]
-	      Reloc Table: 0x000f4000 [0x0000000c]
-	            Debug: 0x000f1878 [0x00000054]
+	      Reloc Table: 0x000fa000 [0x0000000c]
+	            Debug: 0x000f7004 [0x00000054]
 	        Copyright: 0x00000000 [0x00000000]
 	       Global Ptr: 0x00000000 [0x00000000]
 	        TLS Table: 0x00000000 [0x00000000]
 	Load Config Table: 0x00000000 [0x00000000]
 	     Bound Import: 0x00000000 [0x00000000]
 	              IAT: 0x00002000 [0x00000008]
 	Delay Import Desc: 0x00000000 [0x00000000]
 	       CLI Header: 0x00002008 [0x00000048]
 
 	Name: .text
-	   Virtual Size: 0x000ef9d0
+	   Virtual Size: 0x000f515c
 	Virtual Address: 0x00002000
-	  Raw Data Size: 0x000efa00
+	  Raw Data Size: 0x000f5200
 	   Raw Data Ptr: 0x00000200
 	      Reloc Ptr: 0x00000000
 	     LineNo Ptr: 0x00000000
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
 	Flags: code, exec, read, 
 
 	Name: .rsrc
-	   Virtual Size: 0x00000a7c
-	Virtual Address: 0x000f2000
+	   Virtual Size: 0x00000a6c
+	Virtual Address: 0x000f8000
 	  Raw Data Size: 0x00000c00
-	   Raw Data Ptr: 0x000efc00
+	   Raw Data Ptr: 0x000f5400
 	      Reloc Ptr: 0x00000000
 	     LineNo Ptr: 0x00000000
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
 	Flags: data, read, 
 
 	Name: .reloc
 	   Virtual Size: 0x0000000c
-	Virtual Address: 0x000f4000
+	Virtual Address: 0x000fa000
 	  Raw Data Size: 0x00000200
-	   Raw Data Ptr: 0x000f0800
+	   Raw Data Ptr: 0x000f6000
 	      Reloc Ptr: 0x00000000
 	     LineNo Ptr: 0x00000000
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
 	Flags: data, discard, read, 
 
           CLI header size: 72
          Runtime required: 2.5
                     Flags: ilonly, 32/64, no-trackdebug, notsigned
-	         Metadata: 0x00043dbc [0x000abce4]
+	         Metadata: 0x0004597c [0x000af8b0]
 	Entry Point Token: 0x00000000
-	     Resources at: 0x000efaa0 [0x00001dd8]
+	     Resources at: 0x000f522c [0x00001dd8]
 	   Strong Name at: 0x00000000 [0x00000000]
 	  Code Manager at: 0x00000000 [0x00000000]
 	  VTableFixups at: 0x00000000 [0x00000000]
 	     EAT jumps at: 0x00000000 [0x00000000]
 
 Strong name: none
 
 Public key: none
 
 Metadata header:
            Version: 1.1
     Version string: v4.0.30319
 
 Metadata pointers:
-	Tables (#~): 0x0000006c - 0x000709a4 [461112 == 0x00070938]
-	    Strings: 0x000709a4 - 0x00088874 [98000 == 0x00017ed0]
-	       Blob: 0x0008e010 - 0x000abce4 [122068 == 0x0001dcd4]
-	User string: 0x00088874 - 0x0008e000 [22412 == 0x0000578c]
-	       GUID: 0x0008e000 - 0x0008e010 [16 == 0x00000010]
+	Tables (#~): 0x0000006c - 0x000738e4 [473208 == 0x00073878]
+	    Strings: 0x000738e4 - 0x0008ba04 [98592 == 0x00018120]
+	       Blob: 0x000911d4 - 0x000af8b0 [124636 == 0x0001e6dc]
+	User string: 0x0008ba04 - 0x000911c4 [22464 == 0x000057c0]
+	       GUID: 0x000911c4 - 0x000911d4 [16 == 0x00000010]
 Rows:
-Table Module: 1 records (12 bytes, at 420a4)
-Table TypeRef: 405 records (10 bytes, at 420b0)
-Table TypeDef: 1462 records (18 bytes, at 43082)
-Table Field: 4280 records (10 bytes, at 4974e)
-Table Method: 6118 records (18 bytes, at 53e7e)
-Table Param: 5469 records (8 bytes, at 6ecaa)
-Table InterfaceImpl: 1329 records (4 bytes, at 79792)
-Table MemberRef: 4529 records (10 bytes, at 7ac56)
-Table Constant: 420 records (8 bytes, at 85d40)
-Table CustomAttribute: 11187 records (10 bytes, at 86a60)
-Table StandaloneSig: 856 records (4 bytes, at a1f5e)
-Table EventMap: 2 records (4 bytes, at a2cbe)
-Table Event: 2 records (8 bytes, at a2cc6)
-Table PropertyMap: 483 records (4 bytes, at a2cd6)
-Table Property: 1526 records (10 bytes, at a3462)
-Table MethodSemantics: 2346 records (6 bytes, at a6ffe)
-Table MethodImpl: 705 records (6 bytes, at aa6fa)
-Table TypeSpec: 1662 records (4 bytes, at ab780)
-Table Assembly: 1 records (28 bytes, at ad178)
-Table AssemblyRef: 46 records (28 bytes, at ad194)
-Table ManifestResource: 3 records (14 bytes, at ad69c)
-Table NestedClass: 685 records (4 bytes, at ad6c6)
-Table GenericParam: 735 records (10 bytes, at ae17a)
-Table MethodSpec: 1527 records (6 bytes, at afe30)
-Table GenericParamConstraint: 473 records (4 bytes, at b21fa)
+Table Module: 1 records (12 bytes, at 43c64)
+Table TypeRef: 405 records (10 bytes, at 43c70)
+Table TypeDef: 1497 records (18 bytes, at 44c42)
+Table Field: 4415 records (10 bytes, at 4b584)
+Table Method: 6271 records (18 bytes, at 561fa)
+Table Param: 5584 records (8 bytes, at 71ae8)
+Table InterfaceImpl: 1429 records (4 bytes, at 7c968)
+Table MemberRef: 4591 records (10 bytes, at 7dfbc)
+Table Constant: 424 records (8 bytes, at 89312)
+Table CustomAttribute: 11543 records (10 bytes, at 8a052)
+Table StandaloneSig: 876 records (4 bytes, at a6338)
+Table EventMap: 2 records (4 bytes, at a70e8)
+Table Event: 2 records (8 bytes, at a70f0)
+Table PropertyMap: 497 records (4 bytes, at a7100)
+Table Property: 1581 records (10 bytes, at a78c4)
+Table MethodSemantics: 2431 records (6 bytes, at ab686)
+Table MethodImpl: 735 records (6 bytes, at aef80)
+Table TypeSpec: 1690 records (4 bytes, at b00ba)
+Table Assembly: 1 records (28 bytes, at b1b22)
+Table AssemblyRef: 46 records (28 bytes, at b1b3e)
+Table ManifestResource: 3 records (14 bytes, at b2046)
+Table NestedClass: 706 records (4 bytes, at b2070)
+Table GenericParam: 735 records (10 bytes, at b2b78)
+Table MethodSpec: 1570 records (6 bytes, at b482e)
+Table GenericParamConstraint: 473 records (4 bytes, at b6cfa)
```

### Comparing `tableau_migration-2.1.1/src/tableau_migration/bin/Tableau.Migration.xml` & `tableau_migration-3.0.0/src/tableau_migration/bin/Tableau.Migration.xml`

 * *Files 0% similar despite different names*

#### Comparing `tableau_migration-2.1.1/src/tableau_migration/bin/Tableau.Migration.xml` & `tableau_migration-3.0.0/src/tableau_migration/bin/Tableau.Migration.xml`

```diff
@@ -122,14 +122,42 @@
     </member>
     <member name="M:Tableau.Migration.Api.DataSourcesApiClient.GetConnectionsAsync(System.Guid,System.Threading.CancellationToken)">
       <inheritdoc/>
     </member>
     <member name="M:Tableau.Migration.Api.DataSourcesApiClient.UpdateConnectionAsync(System.Guid,System.Guid,Tableau.Migration.Api.Models.IUpdateConnectionOptions,System.Threading.CancellationToken)">
       <inheritdoc/>
     </member>
+    <member name="M:Tableau.Migration.Api.FlowsApiClient.GetAllFlowsAsync(System.Int32,System.Int32,System.Threading.CancellationToken)">
+      <summary>Gets all prep flows in the current site.</summary>
+      <param name="pageNumber">The 1-indexed page number.</param>
+      <param name="pageSize">The size of the page.</param>
+      <param name="cancel">A cancellation token to obey.</param>
+      <returns>A list of a page of prep flows in the current site.</returns>
+    </member>
+    <member name="M:Tableau.Migration.Api.FlowsApiClient.DownloadFlowAsync(System.Guid,System.Threading.CancellationToken)">
+      <summary>Downloads the prep flow file for the given ID.</summary>
+      <param name="flowId">The ID to download the flow file for.</param>
+      <param name="cancel">A cancellation token to obey.</param>
+      <returns>The file download result.</returns>
+    </member>
+    <member name="M:Tableau.Migration.Api.FlowsApiClient.PublishFlowAsync(Tableau.Migration.Api.Models.IPublishFlowOptions,System.Threading.CancellationToken)">
+      <inheritdoc/>
+    </member>
+    <member name="M:Tableau.Migration.Api.FlowsApiClient.GetPageAsync(System.Int32,System.Int32,System.Threading.CancellationToken)">
+      <inheritdoc/>
+    </member>
+    <member name="M:Tableau.Migration.Api.FlowsApiClient.GetPager(System.Int32)">
+      <inheritdoc/>
+    </member>
+    <member name="M:Tableau.Migration.Api.FlowsApiClient.PullAsync(Tableau.Migration.Content.IFlow,System.Threading.CancellationToken)">
+      <inheritdoc/>
+    </member>
+    <member name="M:Tableau.Migration.Api.FlowsApiClient.PublishAsync(Tableau.Migration.Content.IPublishableFlow,System.Threading.CancellationToken)">
+      <inheritdoc/>
+    </member>
     <member name="M:Tableau.Migration.Api.GroupsApiClient.CreateLocalGroupAsync(System.String,System.String,System.Threading.CancellationToken)">
       <inheritdoc/>
     </member>
     <member name="M:Tableau.Migration.Api.GroupsApiClient.GetAllGroupsAsync(System.Int32,System.Int32,System.Threading.CancellationToken)">
       <inheritdoc/>
     </member>
     <member name="M:Tableau.Migration.Api.GroupsApiClient.GetAllGroupsAsync(System.Int32,System.Int32,System.Collections.Generic.IEnumerable{Tableau.Migration.Net.Rest.Filtering.Filter},System.Threading.CancellationToken)">
@@ -376,14 +404,36 @@
       <param name="newProjectId">The LUID of a project to move the data source to, or null to not update the project.</param>
       <param name="newOwnerId">The LUID of a user to assign the data source to as owner, or null to not update the owner.</param>
       <param name="newIsCertified">Whether or not the data source is certified, or null to not update the flag.</param>
       <param name="newCertificationNote">The certification note, or null to not update the note.</param>
       <param name="newEncryptExtracts">Whether or not to encrypt extracts, or null to not update the option.</param>
       <returns>The update result.</returns>
     </member>
+    <member name="T:Tableau.Migration.Api.IFlowsApiClient">
+      <summary>Interface for API client prep flow operations.</summary>
+    </member>
+    <member name="M:Tableau.Migration.Api.IFlowsApiClient.GetAllFlowsAsync(System.Int32,System.Int32,System.Threading.CancellationToken)">
+      <summary>Gets all prep flows in the current site.</summary>
+      <param name="pageNumber">The 1-indexed page number.</param>
+      <param name="pageSize">The size of the page.</param>
+      <param name="cancel">A cancellation token to obey.</param>
+      <returns>A list of a page of prep flows in the current site.</returns>
+    </member>
+    <member name="M:Tableau.Migration.Api.IFlowsApiClient.DownloadFlowAsync(System.Guid,System.Threading.CancellationToken)">
+      <summary>Downloads the prep flow file for the given ID.</summary>
+      <param name="flowId">The ID to download the flow file for.</param>
+      <param name="cancel">A cancellation token to obey.</param>
+      <returns>The file download result.</returns>
+    </member>
+    <member name="M:Tableau.Migration.Api.IFlowsApiClient.PublishFlowAsync(Tableau.Migration.Api.Models.IPublishFlowOptions,System.Threading.CancellationToken)">
+      <summary>Uploads the input prep flow file.</summary>
+      <param name="options">The new prep flows's details.</param>
+      <param name="cancel">A cancellation token to obey.</param>
+      <returns>The published prep flow.</returns>
+    </member>
     <member name="T:Tableau.Migration.Api.IGroupsApiClient">
       <summary>Interface for API client group operations.</summary>
     </member>
     <member name="M:Tableau.Migration.Api.IGroupsApiClient.CreateLocalGroupAsync(System.String,System.String,System.Threading.CancellationToken)">
       <summary>Creates a local group</summary>
       <param name="name">The new group's name.</param>
       <param name="minimumSiteRole">The new group's minimum site role.</param>
@@ -658,14 +708,17 @@
     </member>
     <member name="P:Tableau.Migration.Api.ISitesApiClient.Workbooks">
       <summary>Gets the API client for workbook operations.</summary>
     </member>
     <member name="P:Tableau.Migration.Api.ISitesApiClient.Views">
       <summary>Gets the API client for views operations.</summary>
     </member>
+    <member name="P:Tableau.Migration.Api.ISitesApiClient.Flows">
+      <summary>Gets the API client for prep flow operations.</summary>
+    </member>
     <member name="M:Tableau.Migration.Api.ISitesApiClient.GetSiteAsync(System.Guid,System.Threading.CancellationToken)">
       <summary>Gets the site with the specified ID.</summary>
       <param name="siteId">The site's ID.</param>
       <param name="cancel">The cancellation token.</param>
       <returns>The site with the specified ID.</returns>
     </member>
     <member name="M:Tableau.Migration.Api.ISitesApiClient.GetSiteAsync(System.String,System.Threading.CancellationToken)">
@@ -1198,14 +1251,29 @@
     </member>
     <member name="P:Tableau.Migration.Api.Models.IPublishFileOptions.FileName">
       <summary>Gets the name of the file.</summary>
     </member>
     <member name="P:Tableau.Migration.Api.Models.IPublishFileOptions.FileType">
       <summary>Gets the type of the file.</summary>
     </member>
+    <member name="T:Tableau.Migration.Api.Models.IPublishFlowOptions">
+      <summary>Interface for API client prep flow publish options.</summary>
+    </member>
+    <member name="P:Tableau.Migration.Api.Models.IPublishFlowOptions.Name">
+      <summary>Gets the name of the prep flow.</summary>
+    </member>
+    <member name="P:Tableau.Migration.Api.Models.IPublishFlowOptions.Description">
+      <summary>Gets the description of the prep flow.</summary>
+    </member>
+    <member name="P:Tableau.Migration.Api.Models.IPublishFlowOptions.Overwrite">
+      <summary>Gets whether or not to overwrite any existing prep flow.</summary>
+    </member>
+    <member name="P:Tableau.Migration.Api.Models.IPublishFlowOptions.ProjectId">
+      <summary>Gets the ID of the project to publish to.</summary>
+    </member>
     <member name="T:Tableau.Migration.Api.Models.IPublishWorkbookOptions">
       <summary>Interface for API client workbook publish options.</summary>
     </member>
     <member name="P:Tableau.Migration.Api.Models.IPublishWorkbookOptions.Name">
       <summary>Gets the name of the workbook.</summary>
     </member>
     <member name="P:Tableau.Migration.Api.Models.IPublishWorkbookOptions.Description">
@@ -1531,14 +1599,51 @@
       <param name="dataSource">The publishable data source information.</param>
       <param name="file">
         The data source file as a
         <see cref="T:System.IO.Stream"/>
       </param>
       <param name="fileType">The type of data source file.</param>
     </member>
+    <member name="T:Tableau.Migration.Api.Models.PublishFlowOptions">
+      <summary>Class for API client prep flow publish options.</summary>
+    </member>
+    <member name="P:Tableau.Migration.Api.Models.PublishFlowOptions.Name">
+      <inheritdoc/>
+    </member>
+    <member name="P:Tableau.Migration.Api.Models.PublishFlowOptions.Description">
+      <inheritdoc/>
+    </member>
+    <member name="P:Tableau.Migration.Api.Models.PublishFlowOptions.Overwrite">
+      <inheritdoc/>
+    </member>
+    <member name="P:Tableau.Migration.Api.Models.PublishFlowOptions.ProjectId">
+      <inheritdoc/>
+    </member>
+    <member name="P:Tableau.Migration.Api.Models.PublishFlowOptions.File">
+      <inheritdoc/>
+    </member>
+    <member name="P:Tableau.Migration.Api.Models.PublishFlowOptions.FileName">
+      <inheritdoc/>
+    </member>
+    <member name="P:Tableau.Migration.Api.Models.PublishFlowOptions.FileType">
+      <inheritdoc/>
+    </member>
+    <member name="M:Tableau.Migration.Api.Models.PublishFlowOptions.#ctor(Tableau.Migration.Content.IPublishableFlow,System.IO.Stream,System.String)">
+      <summary>
+        Creates a new
+        <see cref="T:Tableau.Migration.Api.Models.PublishFlowOptions"/>
+        instance.
+      </summary>
+      <param name="flow">The publishable prep flow information.</param>
+      <param name="file">
+        The prep flow file as a
+        <see cref="T:System.IO.Stream"/>
+      </param>
+      <param name="fileType">The type of prep flow file.</param>
+    </member>
     <member name="T:Tableau.Migration.Api.Models.PublishWorkbookOptions">
       <summary>Class for API client workbook publish options.</summary>
     </member>
     <member name="P:Tableau.Migration.Api.Models.PublishWorkbookOptions.Name">
       <inheritdoc/>
     </member>
     <member name="P:Tableau.Migration.Api.Models.PublishWorkbookOptions.Description">
@@ -2032,14 +2137,17 @@
       <summary>Interface for file publisher classes.</summary>
     </member>
     <member name="M:Tableau.Migration.Api.Publishing.IFilePublisher`2.PublishAsync(`0,System.Threading.CancellationToken)">
       <summary>Publishes the file with the specified options.</summary>
       <param name="options">The publish options</param>
       <param name="cancel">A cancellation token to obey.</param>
     </member>
+    <member name="T:Tableau.Migration.Api.Publishing.IFlowPublisher">
+      <summary>Interface for prep flow publisher classes.</summary>
+    </member>
     <member name="T:Tableau.Migration.Api.Publishing.IWorkbookPublisher">
       <summary>Interface for workbook publisher classes.</summary>
     </member>
     <member name="T:Tableau.Migration.Api.RefreshAuthenticationTokenDelegate">
       <summary>Delegate for refreshing an authentication token.</summary>
       <param name="cancel">The cancellation token to obey.</param>
       <returns>The result of the token refresh operation.</returns>
@@ -2226,14 +2334,32 @@
     </member>
     <member name="P:Tableau.Migration.Api.Rest.Models.IDataSourceType.UseRemoteQueryAgent">
       <summary>Gets whether or not the data source uses a remote query agent for the response.</summary>
     </member>
     <member name="P:Tableau.Migration.Api.Rest.Models.IDataSourceType.WebpageUrl">
       <summary>Gets the data source webpage URL for the response.</summary>
     </member>
+    <member name="T:Tableau.Migration.Api.Rest.Models.IFlowType">
+      <summary>Interface for a prep flow REST response.</summary>
+    </member>
+    <member name="P:Tableau.Migration.Api.Rest.Models.IFlowType.Description">
+      <summary>Gets the description for the response.</summary>
+    </member>
+    <member name="P:Tableau.Migration.Api.Rest.Models.IFlowType.CreatedAt">
+      <summary>Gets the created timestamp for the response.</summary>
+    </member>
+    <member name="P:Tableau.Migration.Api.Rest.Models.IFlowType.UpdatedAt">
+      <summary>Gets the updated timestamp for the response.</summary>
+    </member>
+    <member name="P:Tableau.Migration.Api.Rest.Models.IFlowType.WebpageUrl">
+      <summary>Gets the data source webpage URL for the response.</summary>
+    </member>
+    <member name="P:Tableau.Migration.Api.Rest.Models.IFlowType.FileType">
+      <summary>Gets the file type for the response.</summary>
+    </member>
     <member name="T:Tableau.Migration.Api.Rest.Models.ILocationType">
       <summary>Class representing an XML element for the location of a content item that has a name.</summary>
     </member>
     <member name="P:Tableau.Migration.Api.Rest.Models.ILocationType.Type">
       <summary>Gets or sets the type for the response.</summary>
     </member>
     <member name="T:Tableau.Migration.Api.Rest.Models.IOwnerType">
@@ -2737,14 +2863,56 @@
     </member>
     <member name="T:Tableau.Migration.Api.Rest.Models.Requests.CommitDataSourcePublishRequest.DataSourceType.ProjectType">
       <summary>The project type in the API request body.</summary>
     </member>
     <member name="P:Tableau.Migration.Api.Rest.Models.Requests.CommitDataSourcePublishRequest.DataSourceType.ProjectType.Id">
       <summary>Gets or sets the ID for the request's project.</summary>
     </member>
+    <member name="T:Tableau.Migration.Api.Rest.Models.Requests.CommitFlowPublishRequest">
+      <summary>
+        <para>Class representing an commit prep flow request.</para>
+        <para>
+          See
+          <see href="https://help.tableau.com/current/api/rest_api/en-us/REST/rest_api_ref_flow.htm#publish_flow">Tableau API Reference</see>
+          for documentation.
+        </para>
+      </summary>
+    </member>
+    <member name="M:Tableau.Migration.Api.Rest.Models.Requests.CommitFlowPublishRequest.#ctor">
+      <summary>The default parameterless constructor.</summary>
+    </member>
+    <member name="M:Tableau.Migration.Api.Rest.Models.Requests.CommitFlowPublishRequest.#ctor(Tableau.Migration.Api.Models.IPublishFlowOptions)">
+      <summary>
+        Creates a new
+        <see cref="T:Tableau.Migration.Api.Rest.Models.Requests.CommitFlowPublishRequest"/>
+        object.
+      </summary>
+      <param name="options">The publish options.</param>
+    </member>
+    <member name="P:Tableau.Migration.Api.Rest.Models.Requests.CommitFlowPublishRequest.Flow">
+      <summary>Gets or sets the prep flow for the request.</summary>
+    </member>
+    <member name="T:Tableau.Migration.Api.Rest.Models.Requests.CommitFlowPublishRequest.FlowType">
+      <summary>The prep flow type in the API request body.</summary>
+    </member>
+    <member name="P:Tableau.Migration.Api.Rest.Models.Requests.CommitFlowPublishRequest.FlowType.Name">
+      <summary>Gets or sets the name for the prep flow.</summary>
+    </member>
+    <member name="P:Tableau.Migration.Api.Rest.Models.Requests.CommitFlowPublishRequest.FlowType.Description">
+      <summary>Gets or sets the description for the prep flow.</summary>
+    </member>
+    <member name="P:Tableau.Migration.Api.Rest.Models.Requests.CommitFlowPublishRequest.FlowType.Project">
+      <summary>Gets or sets the prep flow's project for the request.</summary>
+    </member>
+    <member name="T:Tableau.Migration.Api.Rest.Models.Requests.CommitFlowPublishRequest.FlowType.ProjectType">
+      <summary>The project type in the API request body.</summary>
+    </member>
+    <member name="P:Tableau.Migration.Api.Rest.Models.Requests.CommitFlowPublishRequest.FlowType.ProjectType.Id">
+      <summary>Gets or sets the ID for the request's project.</summary>
+    </member>
     <member name="T:Tableau.Migration.Api.Rest.Models.Requests.CommitWorkbookPublishRequest">
       <summary>
         <para>Class representing an commit workbook request.</para>
         <para>
           See
           <see href="https://help.tableau.com/current/api/rest_api/en-us/REST/rest_api_ref_publishing.htm#publish_workbook">Tableau API Reference</see>
           for documentation.
@@ -4284,14 +4452,95 @@
         Creates a new
         <see cref="T:Tableau.Migration.Api.Rest.Models.Responses.FileUploadResponse.FileUploadType"/>
         instance.
       </summary>
       <param name="uploadSessionId">The server's generated session ID.</param>
       <param name="fileSize">The server's product version.</param>
     </member>
+    <member name="T:Tableau.Migration.Api.Rest.Models.Responses.FlowResponse">
+      <summary>
+        Class representing a prep flow response.
+        <see href="https://help.tableau.com/current/api/rest_api/en-us/REST/rest_api_ref_flow.htm#publish_flow">Tableau API Reference</see>
+        for documentation.
+      </summary>
+    </member>
+    <member name="P:Tableau.Migration.Api.Rest.Models.Responses.FlowResponse.Item">
+      <summary>Gets or sets the prep flow for the response.</summary>
+    </member>
+    <member name="T:Tableau.Migration.Api.Rest.Models.Responses.FlowResponse.FlowType">
+      <summary>Class representing a site response.</summary>
+    </member>
+    <member name="P:Tableau.Migration.Api.Rest.Models.Responses.FlowResponse.FlowType.Id">
+      <summary>Gets or sets the ID for the response.</summary>
+    </member>
+    <member name="P:Tableau.Migration.Api.Rest.Models.Responses.FlowResponse.FlowType.Name">
+      <summary>Gets or sets the name for the response.</summary>
+    </member>
+    <member name="P:Tableau.Migration.Api.Rest.Models.Responses.FlowResponse.FlowType.Description">
+      <summary>Gets or sets the description for the response.</summary>
+    </member>
+    <member name="P:Tableau.Migration.Api.Rest.Models.Responses.FlowResponse.FlowType.WebpageUrl">
+      <summary>Gets or sets the webpage URL for the response.</summary>
+    </member>
+    <member name="P:Tableau.Migration.Api.Rest.Models.Responses.FlowResponse.FlowType.FileType">
+      <summary>Gets or sets the file type for the response.</summary>
+    </member>
+    <member name="P:Tableau.Migration.Api.Rest.Models.Responses.FlowResponse.FlowType.CreatedAt">
+      <summary>Gets or sets the created timestamp for the response.</summary>
+    </member>
+    <member name="P:Tableau.Migration.Api.Rest.Models.Responses.FlowResponse.FlowType.UpdatedAt">
+      <summary>Gets or sets the updated timestamp for the response.</summary>
+    </member>
+    <member name="P:Tableau.Migration.Api.Rest.Models.Responses.FlowResponse.FlowType.Project">
+      <summary>Gets or sets the project for the response.</summary>
+    </member>
+    <member name="P:Tableau.Migration.Api.Rest.Models.Responses.FlowResponse.FlowType.Owner">
+      <summary>Gets or sets the owner for the response.</summary>
+    </member>
+    <member name="P:Tableau.Migration.Api.Rest.Models.Responses.FlowResponse.FlowType.Tags">
+      <summary>Gets or sets the tags for the response.</summary>
+    </member>
+    <member name="T:Tableau.Migration.Api.Rest.Models.Responses.FlowResponse.FlowType.ProjectType">
+      <summary>Class representing a REST API project response.</summary>
+    </member>
+    <member name="P:Tableau.Migration.Api.Rest.Models.Responses.FlowResponse.FlowType.ProjectType.Id">
+      <summary>Gets or sets the ID for the response.</summary>
+    </member>
+    <member name="P:Tableau.Migration.Api.Rest.Models.Responses.FlowResponse.FlowType.ProjectType.Name">
+      <summary>Gets or sets the name for the response.</summary>
+    </member>
+    <member name="T:Tableau.Migration.Api.Rest.Models.Responses.FlowResponse.FlowType.OwnerType">
+      <summary>Class representing a REST API user response.</summary>
+    </member>
+    <member name="P:Tableau.Migration.Api.Rest.Models.Responses.FlowResponse.FlowType.OwnerType.Id">
+      <summary>Gets or sets the ID for the response.</summary>
+    </member>
+    <member name="P:Tableau.Migration.Api.Rest.Models.Responses.FlowResponse.FlowType.OwnerType.Name">
+      <summary>Gets or sets the name for the response.</summary>
+    </member>
+    <member name="T:Tableau.Migration.Api.Rest.Models.Responses.FlowResponse.FlowType.TagType">
+      <summary>Class representing a REST API tag response.</summary>
+    </member>
+    <member name="P:Tableau.Migration.Api.Rest.Models.Responses.FlowResponse.FlowType.TagType.Label">
+      <summary>Gets or sets the label for the response.</summary>
+    </member>
+    <member name="M:Tableau.Migration.Api.Rest.Models.Responses.FlowResponse.FlowType.TagType.#ctor">
+      <summary>The default parameterless constructor.</summary>
+    </member>
+    <member name="M:Tableau.Migration.Api.Rest.Models.Responses.FlowResponse.FlowType.TagType.#ctor(Tableau.Migration.Api.Rest.Models.ITagType)">
+      <summary>
+        Constructor to build from
+        <see cref="T:Tableau.Migration.Api.Rest.Models.ITagType"/>
+      </summary>
+      <param name="tag">
+        The
+        <see cref="T:Tableau.Migration.Api.Rest.Models.ITagType"/>
+        object.
+      </param>
+    </member>
     <member name="T:Tableau.Migration.Api.Rest.Models.Responses.FlowsResponse">
       <summary>Class representing a flow response.
             
             This is incomplete, there are more attributes than we're saving</summary>
     </member>
     <member name="P:Tableau.Migration.Api.Rest.Models.Responses.FlowsResponse.Items">
       <summary>Gets or sets the groups for the response.</summary>
@@ -4307,14 +4556,17 @@
     </member>
     <member name="P:Tableau.Migration.Api.Rest.Models.Responses.FlowsResponse.FlowType.Description">
       <summary>Gets or sets the description for the response.</summary>
     </member>
     <member name="P:Tableau.Migration.Api.Rest.Models.Responses.FlowsResponse.FlowType.WebpageUrl">
       <summary>Gets or sets the webpage URL for the response.</summary>
     </member>
+    <member name="P:Tableau.Migration.Api.Rest.Models.Responses.FlowsResponse.FlowType.FileType">
+      <summary>Gets or sets the file type for the response.</summary>
+    </member>
     <member name="P:Tableau.Migration.Api.Rest.Models.Responses.FlowsResponse.FlowType.CreatedAt">
       <summary>Gets or sets the created timestamp for the response.</summary>
     </member>
     <member name="P:Tableau.Migration.Api.Rest.Models.Responses.FlowsResponse.FlowType.UpdatedAt">
       <summary>Gets or sets the updated timestamp for the response.</summary>
     </member>
     <member name="P:Tableau.Migration.Api.Rest.Models.Responses.FlowsResponse.FlowType.Project">
@@ -4331,29 +4583,43 @@
     </member>
     <member name="P:Tableau.Migration.Api.Rest.Models.Responses.FlowsResponse.FlowType.ProjectType.Id">
       <summary>Gets or sets the ID for the response.</summary>
     </member>
     <member name="P:Tableau.Migration.Api.Rest.Models.Responses.FlowsResponse.FlowType.ProjectType.Name">
       <summary>Gets or sets the name for the response.</summary>
     </member>
-    <member name="T:Tableau.Migration.Api.Rest.Models.Responses.FlowsResponse.FlowType.UserType">
+    <member name="T:Tableau.Migration.Api.Rest.Models.Responses.FlowsResponse.FlowType.OwnerType">
       <summary>Class representing a REST API user response.</summary>
     </member>
-    <member name="P:Tableau.Migration.Api.Rest.Models.Responses.FlowsResponse.FlowType.UserType.Id">
+    <member name="P:Tableau.Migration.Api.Rest.Models.Responses.FlowsResponse.FlowType.OwnerType.Id">
       <summary>Gets or sets the ID for the response.</summary>
     </member>
-    <member name="P:Tableau.Migration.Api.Rest.Models.Responses.FlowsResponse.FlowType.UserType.Name">
+    <member name="P:Tableau.Migration.Api.Rest.Models.Responses.FlowsResponse.FlowType.OwnerType.Name">
       <summary>Gets or sets the name for the response.</summary>
     </member>
     <member name="T:Tableau.Migration.Api.Rest.Models.Responses.FlowsResponse.FlowType.TagType">
       <summary>Class representing a REST API tag response.</summary>
     </member>
     <member name="P:Tableau.Migration.Api.Rest.Models.Responses.FlowsResponse.FlowType.TagType.Label">
       <summary>Gets or sets the label for the response.</summary>
     </member>
+    <member name="M:Tableau.Migration.Api.Rest.Models.Responses.FlowsResponse.FlowType.TagType.#ctor">
+      <summary>The default parameterless constructor.</summary>
+    </member>
+    <member name="M:Tableau.Migration.Api.Rest.Models.Responses.FlowsResponse.FlowType.TagType.#ctor(Tableau.Migration.Api.Rest.Models.ITagType)">
+      <summary>
+        Constructor to build from
+        <see cref="T:Tableau.Migration.Api.Rest.Models.ITagType"/>
+      </summary>
+      <param name="tag">
+        The
+        <see cref="T:Tableau.Migration.Api.Rest.Models.ITagType"/>
+        object.
+      </param>
+    </member>
     <member name="T:Tableau.Migration.Api.Rest.Models.Responses.GroupResponse">
       <summary>Class representing a group response.</summary>
     </member>
     <member name="P:Tableau.Migration.Api.Rest.Models.Responses.GroupResponse.Item">
       <summary>Gets or sets the group for the response.</summary>
     </member>
     <member name="T:Tableau.Migration.Api.Rest.Models.Responses.GroupResponse.GroupType">
@@ -6200,14 +6466,30 @@
     </member>
     <member name="F:Tableau.Migration.Api.Rest.Models.Types.DataSourceFileTypes.Tdsx">
       <summary>Gets the name of the Tdsx data source file type.</summary>
     </member>
     <member name="F:Tableau.Migration.Api.Rest.Models.Types.DataSourceFileTypes.Tde">
       <summary>Gets the name of the Tde data source file type.</summary>
     </member>
+    <member name="T:Tableau.Migration.Api.Rest.Models.Types.FlowFileTypes">
+      <summary>
+        <para>Class containing prep flow file type constants.</para>
+        <para>
+          See
+          <see href="https://help.tableau.com/current/api/rest_api/en-us/REST/rest_api_ref_flow.htm#publish_flow">Tableau API Reference</see>
+          for documentation.
+        </para>
+      </summary>
+    </member>
+    <member name="F:Tableau.Migration.Api.Rest.Models.Types.FlowFileTypes.Tfl">
+      <summary>Gets the name of the TFL prep flow file type.</summary>
+    </member>
+    <member name="F:Tableau.Migration.Api.Rest.Models.Types.FlowFileTypes.Tflx">
+      <summary>Gets the name of the TFLX prep flow file type.</summary>
+    </member>
     <member name="T:Tableau.Migration.Api.Rest.Models.Types.GranteeCapabilityType">
       <summary>Class that defines the Grantee Capability element for the Tableau REST API XML response.</summary>
     </member>
     <member name="M:Tableau.Migration.Api.Rest.Models.Types.GranteeCapabilityType.#ctor(Tableau.Migration.Content.Permissions.IGranteeCapability)">
       <summary>
         Constructor to build from
         <see cref="T:Tableau.Migration.Content.Permissions.IGranteeCapability"/>
@@ -6287,32 +6569,36 @@
     </member>
     <member name="F:Tableau.Migration.Api.Rest.Models.Types.WorkbookFileTypes.Twbx">
       <summary>Gets the name of the twbx workbook file type.</summary>
     </member>
     <member name="T:Tableau.Migration.Api.Rest.RestException">
       <summary>Class representing an error from a Tableau REST API</summary>
     </member>
+    <member name="F:Tableau.Migration.Api.Rest.RestException.HttpMethod">
+      <summary>Gets the request URI from Tableau API.</summary>
+    </member>
     <member name="F:Tableau.Migration.Api.Rest.RestException.RequestUri">
       <summary>Gets the request URI from Tableau API.</summary>
     </member>
     <member name="F:Tableau.Migration.Api.Rest.RestException.Code">
       <summary>Gets the error code from Tableau API.</summary>
     </member>
     <member name="F:Tableau.Migration.Api.Rest.RestException.Detail">
       <summary>Gets the error detail from Tableau API.</summary>
     </member>
     <member name="F:Tableau.Migration.Api.Rest.RestException.Summary">
       <summary>Gets the error summary from Tableau API.</summary>
     </member>
-    <member name="M:Tableau.Migration.Api.Rest.RestException.#ctor(System.Uri,Tableau.Migration.Api.Rest.Models.Error,Tableau.Migration.Resources.ISharedResourcesLocalizer)">
+    <member name="M:Tableau.Migration.Api.Rest.RestException.#ctor(System.Net.Http.HttpMethod,System.Uri,Tableau.Migration.Api.Rest.Models.Error,Tableau.Migration.Resources.ISharedResourcesLocalizer)">
       <summary>
         Creates a new
         <see cref="T:Tableau.Migration.Api.Rest.RestException"/>
         instance.
       </summary>
+      <param name="httpMethod">The http method that generated the current error.</param>
       <param name="requestUri">The request URI that generated the current error.</param>
       <param name="error">
         The
         <see cref="T:Tableau.Migration.Api.Rest.Models.Error"/>
         returned from the Tableau API.
       </param>
       <param name="sharedResourcesLocalizer">A string localizer.</param>
@@ -7124,14 +7410,17 @@
     </member>
     <member name="P:Tableau.Migration.Api.SitesApiClient.Workbooks">
       <inheritdoc/>
     </member>
     <member name="P:Tableau.Migration.Api.SitesApiClient.Views">
       <inheritdoc/>
     </member>
+    <member name="P:Tableau.Migration.Api.SitesApiClient.Flows">
+      <inheritdoc/>
+    </member>
     <member name="M:Tableau.Migration.Api.SitesApiClient.GetReadApiClient``1">
       <inheritdoc/>
     </member>
     <member name="M:Tableau.Migration.Api.SitesApiClient.GetListApiClient``1">
       <inheritdoc/>
     </member>
     <member name="M:Tableau.Migration.Api.SitesApiClient.GetPullApiClient``2">
@@ -8858,14 +9147,32 @@
         has an FFS prefix.
             All comparisons are case insensitive.
       </summary>
       <param name="xmlName">The (possibly FFS prefixed) name to test.</param>
       <param name="matchName">The XML name to match to - should not contain any FFS prefix.</param>
       <returns>True if the name matches given FFS considerations, otherwise false.</returns>
     </member>
+    <member name="P:Tableau.Migration.Content.Flow.Description">
+      <inheritdoc/>
+    </member>
+    <member name="P:Tableau.Migration.Content.Flow.CreatedAt">
+      <inheritdoc/>
+    </member>
+    <member name="P:Tableau.Migration.Content.Flow.UpdatedAt">
+      <inheritdoc/>
+    </member>
+    <member name="P:Tableau.Migration.Content.Flow.WebpageUrl">
+      <inheritdoc/>
+    </member>
+    <member name="P:Tableau.Migration.Content.Flow.FileType">
+      <inheritdoc/>
+    </member>
+    <member name="P:Tableau.Migration.Content.Flow.Tags">
+      <inheritdoc/>
+    </member>
     <member name="P:Tableau.Migration.Content.GroupUser.User">
       <inheritdoc/>
     </member>
     <member name="T:Tableau.Migration.Content.IChildPermissionsContent">
       <summary>Interface to be inherited by content items that have permissions.</summary>
     </member>
     <member name="P:Tableau.Migration.Content.IChildPermissionsContent.ChildType">
@@ -8946,14 +9253,20 @@
     </member>
     <member name="T:Tableau.Migration.Content.IFileContent">
       <summary>Interface for content items that publish via file upload.</summary>
     </member>
     <member name="P:Tableau.Migration.Content.IFileContent.File">
       <summary>Gets or sets the file to publish for the content item.</summary>
     </member>
+    <member name="T:Tableau.Migration.Content.IFlow">
+      <summary>Interface for a prep flow content item.</summary>
+    </member>
+    <member name="P:Tableau.Migration.Content.IFlow.FileType">
+      <summary>Get or sets the prep flow file type.</summary>
+    </member>
     <member name="T:Tableau.Migration.Content.IGroup">
       <summary>Interface for a group content item.</summary>
     </member>
     <member name="P:Tableau.Migration.Content.IGroup.GrantLicenseMode">
       <summary>Gets the grant license mode of the group.</summary>
     </member>
     <member name="P:Tableau.Migration.Content.IGroup.SiteRole">
@@ -9042,14 +9355,22 @@
       <summary>
         Interface for a
         <see cref="T:Tableau.Migration.Content.IDataSource"/>
         that has been downloaded
             and has full information necessary for re-publishing.
       </summary>
     </member>
+    <member name="T:Tableau.Migration.Content.IPublishableFlow">
+      <summary>
+        Interface for a
+        <see cref="T:Tableau.Migration.Content.IFlow"/>
+        that has been downloaded
+            and has full information necessary for re-publishing.
+      </summary>
+    </member>
     <member name="T:Tableau.Migration.Content.IPublishableGroup">
       <summary>Interface for a group content item with users.</summary>
     </member>
     <member name="P:Tableau.Migration.Content.IPublishableGroup.Users">
       <summary>Gets or sets the users assigned to the group.</summary>
     </member>
     <member name="T:Tableau.Migration.Content.IPublishableWorkbook">
@@ -9514,14 +9835,22 @@
       <inheritdoc/>
     </member>
     <member name="M:Tableau.Migration.Content.PublishableDataSource.DisposeAsync">
       <summary>Performs application-defined tasks associated with freeing, releasing, or resetting
             unmanaged resources asynchronously.</summary>
       <returns>A task that represents the asynchronous dispose operation.</returns>
     </member>
+    <member name="P:Tableau.Migration.Content.PublishableFlow.File">
+      <inheritdoc/>
+    </member>
+    <member name="M:Tableau.Migration.Content.PublishableFlow.DisposeAsync">
+      <summary>Performs application-defined tasks associated with freeing, releasing, or resetting
+            unmanaged resources asynchronously.</summary>
+      <returns>A task that represents the asynchronous dispose operation.</returns>
+    </member>
     <member name="P:Tableau.Migration.Content.PublishableGroup.Users">
       <inheritdoc/>
     </member>
     <member name="P:Tableau.Migration.Content.PublishableWorkbook.ThumbnailsUserId">
       <inheritdoc/>
     </member>
     <member name="P:Tableau.Migration.Content.PublishableWorkbook.File">
```

### Comparing `tableau_migration-2.1.1/src/tableau_migration/bin/TestableIO.System.IO.Abstractions.Wrappers.dll` & `tableau_migration-3.0.0/src/tableau_migration/bin/TestableIO.System.IO.Abstractions.Wrappers.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.1/src/tableau_migration/bin/TestableIO.System.IO.Abstractions.dll` & `tableau_migration-3.0.0/src/tableau_migration/bin/TestableIO.System.IO.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.1/src/tableau_migration/bin/runtimes/browser/lib/net6.0/System.Text.Encodings.Web.dll` & `tableau_migration-3.0.0/src/tableau_migration/bin/runtimes/browser/lib/net6.0/System.Text.Encodings.Web.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.1/.gitignore` & `tableau_migration-3.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.1.1/pyproject.toml` & `tableau_migration-3.0.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "tableau_migration"
 dynamic = ["version"]
 
 authors = [
-  { name="Tableau a Salesforce Product" },
+  { name="Salesforce, Inc." },
 ]
 description = "Tableau Migration SDK"
 readme = "README.md"
 # https://devguide.python.org/versions/
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `tableau_migration-2.1.1/PKG-INFO` & `tableau_migration-3.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.3
 Name: tableau_migration
-Version: 2.1.1
+Version: 3.0.0
 Summary: Tableau Migration SDK
 Project-URL: Homepage, http://www.tableau.com
 Project-URL: Bug Tracker, http://www.tableau.com
 Project-URL: Repository, https://github.com/tableau/tableau-migration-sdk
-Author: Tableau a Salesforce Product
+Author: Salesforce, Inc.
 License-File: LICENSE
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: cffi==1.16.0
 Requires-Dist: clr-loader==0.2.6
 Requires-Dist: pycparser==2.21
```

