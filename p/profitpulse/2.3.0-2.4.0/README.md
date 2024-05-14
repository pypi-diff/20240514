# Comparing `tmp/profitpulse-2.3.0.tar.gz` & `tmp/profitpulse-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "profitpulse-2.3.0.tar", max compression
+gzip compressed data, was "profitpulse-2.4.0.tar", max compression
```

## Comparing `profitpulse-2.3.0.tar` & `profitpulse-2.4.0.tar`

### file list

```diff
@@ -1,50 +1,52 @@
--rw-r--r--   0        0        0     1211 2024-04-27 17:48:38.569233 profitpulse-2.3.0/LICENSE
--rw-r--r--   0        0        0     1075 2024-05-04 13:05:41.429315 profitpulse-2.3.0/README.md
--rw-r--r--   0        0        0     1839 2024-05-13 10:22:15.599147 profitpulse-2.3.0/pyproject.toml
--rw-r--r--   0        0        0       69 2024-04-27 17:48:38.573607 profitpulse-2.3.0/src/profitpulse/__init__.py
--rw-r--r--   0        0        0        0 2024-05-04 13:54:47.669161 profitpulse-2.3.0/src/profitpulse/cli/__init__.py
--rw-r--r--   0        0        0     8064 2024-05-13 10:20:51.888363 profitpulse-2.3.0/src/profitpulse/cli/adapters.py
--rw-r--r--   0        0        0     5134 2024-05-13 10:20:51.533454 profitpulse-2.3.0/src/profitpulse/cli/main.py
--rw-r--r--   0        0        0        0 2024-04-27 17:48:38.580446 profitpulse-2.3.0/src/profitpulse/data/__init__.py
--rw-r--r--   0        0        0     3499 2024-05-13 06:35:10.855702 profitpulse-2.3.0/src/profitpulse/data/assets.py
--rw-r--r--   0        0        0     1982 2024-05-13 06:34:10.839383 profitpulse-2.3.0/src/profitpulse/data/assets_test.py
--rw-r--r--   0        0        0      360 2024-05-10 06:54:12.884114 profitpulse-2.3.0/src/profitpulse/data/data.py
--rw-r--r--   0        0        0     2532 2024-05-13 10:20:51.306545 profitpulse-2.3.0/src/profitpulse/data/expenses_view.py
--rw-r--r--   0        0        0     4459 2024-05-12 21:04:29.249063 profitpulse-2.3.0/src/profitpulse/data/expenses_view_test.py
--rw-r--r--   0        0        0     2149 2024-05-10 06:54:12.885295 profitpulse-2.3.0/src/profitpulse/data/pulse_view.py
--rw-r--r--   0        0        0     3057 2024-05-10 06:54:12.885866 profitpulse-2.3.0/src/profitpulse/data/pulse_view_test.py
--rw-r--r--   0        0        0     1417 2024-05-13 06:37:38.084914 profitpulse-2.3.0/src/profitpulse/data/views.py
--rw-r--r--   0        0        0     1029 2024-05-13 06:37:52.778193 profitpulse-2.3.0/src/profitpulse/data/views_test.py
--rw-r--r--   0        0        0      103 2024-04-27 17:48:38.577012 profitpulse-2.3.0/src/profitpulse/gateways/__init__.py
--rw-r--r--   0        0        0     3181 2024-05-12 20:03:01.452823 profitpulse-2.3.0/src/profitpulse/gateways/cgdfile.py
--rw-r--r--   0        0        0     2025 2024-05-12 20:00:26.624621 profitpulse-2.3.0/src/profitpulse/gateways/cgdfile_test.py
--rw-r--r--   0        0        0        0 2024-04-27 17:48:38.577797 profitpulse-2.3.0/src/profitpulse/infrastructure/__init__.py
--rw-r--r--   0        0        0      858 2024-04-27 17:48:38.578149 profitpulse-2.3.0/src/profitpulse/infrastructure/migrations.py
--rw-r--r--   0        0        0        0 2024-04-27 17:48:38.578381 profitpulse-2.3.0/src/profitpulse/lib/__init__.py
--rw-r--r--   0        0        0     1580 2024-05-13 06:32:18.799566 profitpulse-2.3.0/src/profitpulse/lib/asset.py
--rw-r--r--   0        0        0      541 2024-05-07 20:15:15.902011 profitpulse-2.3.0/src/profitpulse/lib/asset_name.py
--rw-r--r--   0        0        0      964 2024-05-10 06:54:12.889055 profitpulse-2.3.0/src/profitpulse/lib/money.py
--rw-r--r--   0        0        0      230 2024-05-12 19:58:55.502505 profitpulse-2.3.0/src/profitpulse/lib/transaction.py
--rw-r--r--   0        0        0      517 2024-05-13 06:30:19.972158 profitpulse-2.3.0/src/profitpulse/migrations/0001 - Initial.sql
--rw-r--r--   0        0        0        0 2024-05-04 09:13:33.128506 profitpulse-2.3.0/src/profitpulse/migrations/0002 - accounts.sql
--rw-r--r--   0        0        0        0 2024-05-04 09:13:33.128652 profitpulse-2.3.0/src/profitpulse/migrations/__init__.py
--rw-r--r--   0        0        0       77 2024-04-27 17:48:38.581726 profitpulse-2.3.0/src/profitpulse/services/__init__.py
--rw-r--r--   0        0        0     1468 2024-05-10 06:54:12.890186 profitpulse-2.3.0/src/profitpulse/services/acquire_asset.py
--rw-r--r--   0        0        0     1636 2024-05-10 06:54:12.891286 profitpulse-2.3.0/src/profitpulse/services/acquire_asset_test.py
--rw-r--r--   0        0        0     1298 2024-05-10 06:54:12.892139 profitpulse-2.3.0/src/profitpulse/services/delete_asset.py
--rw-r--r--   0        0        0     1475 2024-05-10 06:54:12.892714 profitpulse-2.3.0/src/profitpulse/services/delete_asset_test.py
--rw-r--r--   0        0        0     1684 2024-05-13 06:41:10.273093 profitpulse-2.3.0/src/profitpulse/services/deposit_into_asset.py
--rw-r--r--   0        0        0     2392 2024-05-13 06:41:20.391838 profitpulse-2.3.0/src/profitpulse/services/deposit_into_asset_test.py
--rw-r--r--   0        0        0     1428 2024-05-10 06:54:12.894591 profitpulse-2.3.0/src/profitpulse/services/divest_asset.py
--rw-r--r--   0        0        0     1611 2024-05-10 06:54:12.895330 profitpulse-2.3.0/src/profitpulse/services/divest_asset_test.py
--rw-r--r--   0        0        0      285 2024-05-07 20:15:15.913869 profitpulse-2.3.0/src/profitpulse/services/errors.py
--rw-r--r--   0        0        0     1487 2024-05-12 20:23:48.699613 profitpulse-2.3.0/src/profitpulse/services/import_transactions.py
--rw-r--r--   0        0        0     1609 2024-05-12 20:04:33.857117 profitpulse-2.3.0/src/profitpulse/services/revalue_asset.py
--rw-r--r--   0        0        0     1625 2024-05-10 06:54:12.897592 profitpulse-2.3.0/src/profitpulse/services/revalue_test.py
--rw-r--r--   0        0        0     1049 2024-05-10 06:54:12.898087 profitpulse-2.3.0/src/profitpulse/services/services.py
--rw-r--r--   0        0        0      288 2024-05-04 08:56:13.662438 profitpulse-2.3.0/src/profitpulse/testrig/__init__.py
--rw-r--r--   0        0        0      223 2024-05-03 15:10:38.942104 profitpulse-2.3.0/src/profitpulse/testrig/factory.py
--rw-r--r--   0        0        0     1639 2024-04-27 17:48:38.585921 profitpulse-2.3.0/src/profitpulse/testrig/fixtures.py
--rw-r--r--   0        0        0     4909 2024-05-13 10:20:51.647840 profitpulse-2.3.0/src/profitpulse/testrig/scenario.py
--rw-r--r--   0        0        0      330 2024-05-04 13:20:47.845916 profitpulse-2.3.0/src/profitpulse/turbofan.py
--rw-r--r--   0        0        0     2059 1970-01-01 00:00:00.000000 profitpulse-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-04-27 17:48:38.569233 profitpulse-2.4.0/LICENSE
+-rw-r--r--   0        0        0     1075 2024-05-04 13:05:41.429315 profitpulse-2.4.0/README.md
+-rw-r--r--   0        0        0     1855 2024-05-14 16:26:35.153080 profitpulse-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0       69 2024-04-27 17:48:38.573607 profitpulse-2.4.0/src/profitpulse/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-04 13:54:47.669161 profitpulse-2.4.0/src/profitpulse/cli/__init__.py
+-rw-r--r--   0        0        0     8070 2024-05-13 20:10:24.468388 profitpulse-2.4.0/src/profitpulse/cli/adapters.py
+-rw-r--r--   0        0        0     5100 2024-05-14 09:04:32.200516 profitpulse-2.4.0/src/profitpulse/cli/main.py
+-rw-r--r--   0        0        0        0 2024-04-27 17:48:38.580446 profitpulse-2.4.0/src/profitpulse/data/__init__.py
+-rw-r--r--   0        0        0     3499 2024-05-13 06:35:10.855702 profitpulse-2.4.0/src/profitpulse/data/assets.py
+-rw-r--r--   0        0        0     1982 2024-05-13 06:34:10.839383 profitpulse-2.4.0/src/profitpulse/data/assets_test.py
+-rw-r--r--   0        0        0     1417 2024-05-13 06:37:38.084914 profitpulse-2.4.0/src/profitpulse/data/assets_view.py
+-rw-r--r--   0        0        0     1035 2024-05-13 20:09:59.777422 profitpulse-2.4.0/src/profitpulse/data/assets_views_test.py
+-rw-r--r--   0        0        0      360 2024-05-10 06:54:12.884114 profitpulse-2.4.0/src/profitpulse/data/data.py
+-rw-r--r--   0        0        0     2578 2024-05-14 09:31:31.111362 profitpulse-2.4.0/src/profitpulse/data/expenses_view.py
+-rw-r--r--   0        0        0     4459 2024-05-12 21:04:29.249063 profitpulse-2.4.0/src/profitpulse/data/expenses_view_test.py
+-rw-r--r--   0        0        0     2149 2024-05-10 06:54:12.885295 profitpulse-2.4.0/src/profitpulse/data/pulse_view.py
+-rw-r--r--   0        0        0     3057 2024-05-10 06:54:12.885866 profitpulse-2.4.0/src/profitpulse/data/pulse_view_test.py
+-rw-r--r--   0        0        0      103 2024-04-27 17:48:38.577012 profitpulse-2.4.0/src/profitpulse/gateways/__init__.py
+-rw-r--r--   0        0        0     3209 2024-05-14 16:06:03.158753 profitpulse-2.4.0/src/profitpulse/gateways/cgdfile.py
+-rw-r--r--   0        0        0     1976 2024-05-14 16:05:06.945082 profitpulse-2.4.0/src/profitpulse/gateways/cgdfile_test.py
+-rw-r--r--   0        0        0        0 2024-05-14 06:50:39.333502 profitpulse-2.4.0/src/profitpulse/gui/__init__.py
+-rw-r--r--   0        0        0      618 2024-05-14 15:21:23.056783 profitpulse-2.4.0/src/profitpulse/gui/main.py
+-rw-r--r--   0        0        0        0 2024-04-27 17:48:38.577797 profitpulse-2.4.0/src/profitpulse/infrastructure/__init__.py
+-rw-r--r--   0        0        0      858 2024-04-27 17:48:38.578149 profitpulse-2.4.0/src/profitpulse/infrastructure/migrations.py
+-rw-r--r--   0        0        0        0 2024-04-27 17:48:38.578381 profitpulse-2.4.0/src/profitpulse/lib/__init__.py
+-rw-r--r--   0        0        0     1580 2024-05-13 06:32:18.799566 profitpulse-2.4.0/src/profitpulse/lib/asset.py
+-rw-r--r--   0        0        0      541 2024-05-07 20:15:15.902011 profitpulse-2.4.0/src/profitpulse/lib/asset_name.py
+-rw-r--r--   0        0        0      964 2024-05-10 06:54:12.889055 profitpulse-2.4.0/src/profitpulse/lib/money.py
+-rw-r--r--   0        0        0      230 2024-05-12 19:58:55.502505 profitpulse-2.4.0/src/profitpulse/lib/transaction.py
+-rw-r--r--   0        0        0      517 2024-05-13 06:30:19.972158 profitpulse-2.4.0/src/profitpulse/migrations/0001 - Initial.sql
+-rw-r--r--   0        0        0        0 2024-05-04 09:13:33.128506 profitpulse-2.4.0/src/profitpulse/migrations/0002 - accounts.sql
+-rw-r--r--   0        0        0        0 2024-05-04 09:13:33.128652 profitpulse-2.4.0/src/profitpulse/migrations/__init__.py
+-rw-r--r--   0        0        0       77 2024-04-27 17:48:38.581726 profitpulse-2.4.0/src/profitpulse/services/__init__.py
+-rw-r--r--   0        0        0     1468 2024-05-10 06:54:12.890186 profitpulse-2.4.0/src/profitpulse/services/acquire_asset.py
+-rw-r--r--   0        0        0     1636 2024-05-10 06:54:12.891286 profitpulse-2.4.0/src/profitpulse/services/acquire_asset_test.py
+-rw-r--r--   0        0        0     1298 2024-05-10 06:54:12.892139 profitpulse-2.4.0/src/profitpulse/services/delete_asset.py
+-rw-r--r--   0        0        0     1475 2024-05-10 06:54:12.892714 profitpulse-2.4.0/src/profitpulse/services/delete_asset_test.py
+-rw-r--r--   0        0        0     1684 2024-05-13 06:41:10.273093 profitpulse-2.4.0/src/profitpulse/services/deposit_into_asset.py
+-rw-r--r--   0        0        0     2392 2024-05-13 06:41:20.391838 profitpulse-2.4.0/src/profitpulse/services/deposit_into_asset_test.py
+-rw-r--r--   0        0        0     1428 2024-05-10 06:54:12.894591 profitpulse-2.4.0/src/profitpulse/services/divest_asset.py
+-rw-r--r--   0        0        0     1611 2024-05-10 06:54:12.895330 profitpulse-2.4.0/src/profitpulse/services/divest_asset_test.py
+-rw-r--r--   0        0        0      285 2024-05-07 20:15:15.913869 profitpulse-2.4.0/src/profitpulse/services/errors.py
+-rw-r--r--   0        0        0     2329 2024-05-14 16:06:43.025356 profitpulse-2.4.0/src/profitpulse/services/import_transactions.py
+-rw-r--r--   0        0        0     1609 2024-05-12 20:04:33.857117 profitpulse-2.4.0/src/profitpulse/services/revalue_asset.py
+-rw-r--r--   0        0        0     1625 2024-05-10 06:54:12.897592 profitpulse-2.4.0/src/profitpulse/services/revalue_test.py
+-rw-r--r--   0        0        0     1172 2024-05-14 16:06:05.081742 profitpulse-2.4.0/src/profitpulse/services/services.py
+-rw-r--r--   0        0        0      288 2024-05-04 08:56:13.662438 profitpulse-2.4.0/src/profitpulse/testrig/__init__.py
+-rw-r--r--   0        0        0      223 2024-05-03 15:10:38.942104 profitpulse-2.4.0/src/profitpulse/testrig/factory.py
+-rw-r--r--   0        0        0     1639 2024-04-27 17:48:38.585921 profitpulse-2.4.0/src/profitpulse/testrig/fixtures.py
+-rw-r--r--   0        0        0     4885 2024-05-14 09:03:35.585029 profitpulse-2.4.0/src/profitpulse/testrig/scenario.py
+-rw-r--r--   0        0        0      330 2024-05-04 13:20:47.845916 profitpulse-2.4.0/src/profitpulse/turbofan.py
+-rw-r--r--   0        0        0     2150 1970-01-01 00:00:00.000000 profitpulse-2.4.0/PKG-INFO
```

### Comparing `profitpulse-2.3.0/LICENSE` & `profitpulse-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `profitpulse-2.3.0/README.md` & `profitpulse-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `profitpulse-2.3.0/pyproject.toml` & `profitpulse-2.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.bandit]
 exclude_dirs = ["tests", "features"]
 
 [tool.poetry]
 name = "profitpulse"
-version = "2.3.0"
+version = "2.4.0"
 description = "Manage your personal finances"
 authors = ["Luís Miranda <luistm@gmail.com>"]
 maintainers = ["Luís Miranda <luistm@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/luistm/profitpulse"
 
@@ -40,26 +40,28 @@
 multi_line_output = 3
 
 [tool.black]
 max-line-length = 120
 target-version = ["py310","py311", "py312"]
 
 [tool.poetry.scripts]
-profitpulse = "profitpulse.cli.main:profitpulse_app"
-profit = "profitpulse.cli.main:profitpulse_app"
+profitpulse = "profitpulse.cli.main:cli"
+profit = "profitpulse.cli.main:cli"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-pendulum = "^3.0.0"
 rich = "^13.7.1"
 toml = "^0.10.2"
 turbofan = "^0.2.0"
 typer = "^0.12.3"
-gogotable = "0.1.0"
-pastperfect = "^0.1.0"
+gogotable = "^0.1.0"
+pastperfect = "^0.3.0"
+uvicorn = "^0.29.0"
+fastapi = "^0.111.0"
+jinja2 = "^3.1.4"
 
 [tool.pytest.ini_options]
 markers = ["integration: tags a test as integration tests"]
 
 [tool.poetry.dev-dependencies.bandit]
 extras = ["toml"]
 version = "^1.7.8"
```

### Comparing `profitpulse-2.3.0/src/profitpulse/cli/adapters.py` & `profitpulse-2.4.0/src/profitpulse/cli/adapters.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 from typing import Optional
 
 import pastperfect
 from gogotable import gogotable
 from turbofan.database import Database, Session
 
 from profitpulse.data.assets import Assets
+from profitpulse.data.assets_view import AssetsView
 from profitpulse.data.expenses_view import ExpensesView
 from profitpulse.data.pulse_view import PulseView
-from profitpulse.data.views import AssetsView
 from profitpulse.gateways.cgdfile import GatewayCGDFile  # type: ignore
 from profitpulse.lib.asset_name import AssetName
 from profitpulse.lib.money import Money
 from profitpulse.services.acquire_asset import (
     AcquireAssetService,
     AssetAlreadyExistsError,
     OpenAssetRequester,
```

### Comparing `profitpulse-2.3.0/src/profitpulse/cli/main.py` & `profitpulse-2.4.0/src/profitpulse/cli/main.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,63 +16,67 @@
     import_file,
     open_asset,
     pulse,
     report,
     reset,
     revalue,
 )
+from profitpulse.gui.main import start_server
 from profitpulse.infrastructure.migrations import migrate_database  # type: ignore
 
-profitpulse_app = typer.Typer(
+cli = typer.Typer(
     add_completion=False,
     help="Profitpulse helps you manage your personal finances.",
 )
 
-profitpulse_assets_app = typer.Typer()
-profitpulse_app.add_typer(
-    profitpulse_assets_app,
+assets = typer.Typer()
+cli.add_typer(
+    assets,
     name="assets",
     help="Handles assets",
 )
 
 
-@profitpulse_app.command(name="version", help="Shows the current profitpulse version")
+@cli.command(name="version", help="Shows the current profitpulse version")
 def version() -> None:
     migrate_database(database_path)
     typer.echo(get_version("profitpulse"))
 
 
-@profitpulse_app.command(name="pulse", help="Show's the health of your wealth")
+@cli.command(help="Opens the browser GUI of profitpulse")
+def gui() -> None:
+    start_server()
+
+
+@cli.command(name="pulse", help="Show's the health of your wealth")
 def pulse_() -> None:
     migrate_database(database_path)
     pulse()
 
 
-@profitpulse_app.command(
-    name="revalue", help="Revalues an asset to reflect it's current worth"
-)
+@cli.command(name="revalue", help="Revalues an asset to reflect it's current worth")
 def revalue_(
     cent_amount: int = typer.Argument(
         0, help="Amount to deposit in cents", metavar="AMOUNT"
     ),
     asset_name: str = typer.Argument(
         "", help="Name of the asset", metavar='"ASSET NAME"'
     ),
 ) -> None:
     migrate_database(database_path)
     revalue(cent_amount, asset_name)
 
 
-@profitpulse_app.command(name="import", help="Import transactions for expense tracking")
+@cli.command(name="import", help="Import transactions for expense tracking")
 def import_(file_path: Path) -> None:
     migrate_database(database_path)
     import_file(file_path)
 
 
-@profitpulse_app.command(name="report", help="Builds reports according to filter")
+@cli.command(name="report", help="Builds reports according to filter")
 def report_(
     seller: Optional[str] = typer.Option(
         default="", help="Filters report by Seller in description"
     ),
     group_seller: Optional[bool] = typer.Option(
         default=False, help="Groups report by the Seller description"
     ),
@@ -85,27 +89,27 @@
         help="Date until when the report must be shown (inclusive)",
     ),
 ) -> None:
     migrate_database(database_path)
     report(seller=seller, group_seller=group_seller, since=since, until=until)
 
 
-@profitpulse_app.command(name="reset", help="Deletes all information in profitpulse")
+@cli.command(name="reset", help="Deletes all information in profitpulse")
 def reset_() -> None:
     delete_information = typer.confirm(
         "Are you sure you want to delete all financial information ?"
     )
     migrate_database(database_path)
     if not delete_information:
         raise typer.Abort()
 
     reset()
 
 
-@profitpulse_app.command(name="deposit", help="Deposits money into an asset")
+@cli.command(name="deposit", help="Deposits money into an asset")
 def deposit_(
     cent_amount: int = typer.Argument(
         0, help="Amount to deposit in cents", metavar="AMOUNT"
     ),
     asset_name: str = typer.Argument(
         "", help="Name of the asset", metavar='"ASSET NAME"'
     ),
@@ -145,23 +149,23 @@
 
 # @profitpulse_assets_app.command(name="show", help="Shows existing assets")
 # def show() -> None:
 #     migrate_database(database_path)
 #     show_assets()
 
 
-@profitpulse_assets_app.command(name="open", help="Opens a new asset")
+@assets.command(name="open", help="Opens a new asset")
 def open_(
     name: str = typer.Argument("", help="Name of the asset", metavar='"ASSET NAME"'),
 ) -> None:
     migrate_database(database_path)
     open_asset(name)
 
 
-@profitpulse_assets_app.command(name="divest", help="Divests an asset")
+@assets.command(name="divest", help="Divests an asset")
 def divest_(
     name: str = typer.Argument("", help="Name of the asset", metavar='"ASSET NAME"'),
 ) -> None:
     migrate_database(database_path)
     divest_asset(name)
```

### Comparing `profitpulse-2.3.0/src/profitpulse/data/assets.py` & `profitpulse-2.4.0/src/profitpulse/data/assets.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.3.0/src/profitpulse/data/assets_test.py` & `profitpulse-2.4.0/src/profitpulse/data/assets_test.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.3.0/src/profitpulse/data/expenses_view.py` & `profitpulse-2.4.0/src/profitpulse/data/expenses_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,18 +25,18 @@
 
     @property
     def data(self) -> Any:  # noqa
         events = pastperfect.Events(self._session)
         if not len(events):
             return []
 
-        seller_value = {}
+        seller_value: typing.Dict[str, typing.Any] = {}
         results = []
 
-        def get_expenses_by_seller(evt: pastperfect.Event):
+        def get_expenses_by_seller(evt: pastperfect.Event) -> None:
             nonlocal seller_value
 
             if evt.name != EXPENSE_MADE:
                 return
 
             d = evt.data.get("description")
             if self._seller and self._seller not in d:
@@ -50,15 +50,15 @@
                 return
 
             try:
                 seller_value[d] = seller_value[d] + evt.data.get("value")
             except KeyError:
                 seller_value[d] = evt.data.get("value")
 
-        def get_expenses(evt: pastperfect.Event):
+        def get_expenses(evt: pastperfect.Event) -> None:
             nonlocal results
             if evt.name != EXPENSE_MADE:
                 return
 
             d = evt.data.get("description")
 
             if self._seller and self._seller not in d:
```

### Comparing `profitpulse-2.3.0/src/profitpulse/data/expenses_view_test.py` & `profitpulse-2.4.0/src/profitpulse/data/expenses_view_test.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.3.0/src/profitpulse/data/pulse_view.py` & `profitpulse-2.4.0/src/profitpulse/data/pulse_view.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.3.0/src/profitpulse/data/pulse_view_test.py` & `profitpulse-2.4.0/src/profitpulse/data/pulse_view_test.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.3.0/src/profitpulse/data/views.py` & `profitpulse-2.4.0/src/profitpulse/data/assets_view.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.3.0/src/profitpulse/data/views_test.py` & `profitpulse-2.4.0/src/profitpulse/data/assets_views_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pytest
 from turbofan.database import text
 
-from profitpulse.data.views import AssetsView
+from profitpulse.data.assets_view import AssetsView
 from profitpulse.lib.money import Money
 
 
 class TestAssetsView:
     @pytest.mark.integration
     def test_return_no_data_when_no_assets(self, tmp_db_session):
         assert AssetsView(tmp_db_session).data == []  # nosec
```

### Comparing `profitpulse-2.3.0/src/profitpulse/gateways/cgdfile.py` & `profitpulse-2.4.0/src/profitpulse/gateways/cgdfile.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # type: ignore
 import csv
 import pathlib
-
-import pendulum
+from datetime import datetime
 
 from profitpulse.lib.transaction import Transaction
 from profitpulse.services.import_transactions import ImportTransactionsTransactionGater
 
 
 class RowParser:
     """
@@ -54,15 +53,15 @@
         Get the date of the transaction.
         """
 
         raw_date = self.row[0]
         splited_date = raw_date.split("-")
         splited_date.reverse()
         joined_date = "-".join(splited_date)
-        return pendulum.parse(joined_date)
+        return datetime.strptime(joined_date, "%Y-%m-%d")
 
 
 class GatewayCGDFile(ImportTransactionsTransactionGater):
     """
     Example of a file:
         Consultar saldos e movimentos � ordem - 09-08-2022
```

### Comparing `profitpulse-2.3.0/src/profitpulse/gateways/cgdfile_test.py` & `profitpulse-2.4.0/src/profitpulse/gateways/cgdfile_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-import pendulum
+from datetime import datetime
+
 import pytest
 
 from profitpulse.gateways.cgdfile import RowParser
 
 
 class TestRowParser:
     """
@@ -72,9 +73,8 @@
             "",
             "COMPRAS C DEB FARMACI ",
             "",
             "2.115,69",
         ]
         row_parser = RowParser(row)
 
-        # TODO: Isolate logic to get a date object from a reversed date string
-        assert row_parser.date == pendulum.parse("2020-01-01")  # nosec
+        assert row_parser.date == datetime.strptime("2020-01-01", "%Y-%m-%d")  # nosec
```

### Comparing `profitpulse-2.3.0/src/profitpulse/infrastructure/migrations.py` & `profitpulse-2.4.0/src/profitpulse/infrastructure/migrations.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.3.0/src/profitpulse/lib/asset.py` & `profitpulse-2.4.0/src/profitpulse/lib/asset.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.3.0/src/profitpulse/lib/asset_name.py` & `profitpulse-2.4.0/src/profitpulse/lib/asset_name.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.3.0/src/profitpulse/lib/money.py` & `profitpulse-2.4.0/src/profitpulse/lib/money.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.3.0/src/profitpulse/migrations/0001 - Initial.sql` & `profitpulse-2.4.0/src/profitpulse/migrations/0001 - Initial.sql`

 * *Files identical despite different names*

### Comparing `profitpulse-2.3.0/src/profitpulse/services/acquire_asset.py` & `profitpulse-2.4.0/src/profitpulse/services/acquire_asset.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.3.0/src/profitpulse/services/acquire_asset_test.py` & `profitpulse-2.4.0/src/profitpulse/services/acquire_asset_test.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.3.0/src/profitpulse/services/delete_asset.py` & `profitpulse-2.4.0/src/profitpulse/services/delete_asset.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.3.0/src/profitpulse/services/delete_asset_test.py` & `profitpulse-2.4.0/src/profitpulse/services/delete_asset_test.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.3.0/src/profitpulse/services/deposit_into_asset.py` & `profitpulse-2.4.0/src/profitpulse/services/deposit_into_asset.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.3.0/src/profitpulse/services/deposit_into_asset_test.py` & `profitpulse-2.4.0/src/profitpulse/services/deposit_into_asset_test.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.3.0/src/profitpulse/services/divest_asset.py` & `profitpulse-2.4.0/src/profitpulse/services/divest_asset.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.3.0/src/profitpulse/services/divest_asset_test.py` & `profitpulse-2.4.0/src/profitpulse/services/divest_asset_test.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.3.0/src/profitpulse/services/revalue_asset.py` & `profitpulse-2.4.0/src/profitpulse/services/revalue_asset.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.3.0/src/profitpulse/services/revalue_test.py` & `profitpulse-2.4.0/src/profitpulse/services/revalue_test.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.3.0/src/profitpulse/services/services.py` & `profitpulse-2.4.0/src/profitpulse/services/services.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,16 +20,22 @@
         **___: typing.Dict[typing.Any, typing.Any],
     ) -> None:
         if event_log is None:
             raise Exception("'Event logged' service must have an event log")
         self._event_log = event_log
         self._event_name = event_name
 
-    def emit(self, **kwargs: dict[str, typing.Any]) -> None:
-        self._event_log.append(pastperfect.Event(name=self._event_name, data=kwargs))
+    def emit(
+        self, event_name: typing.Optional[str] = None, **kwargs: dict[str, typing.Any]
+    ) -> None:
+        en = self._event_name
+        if event_name:
+            en = event_name
+
+        self._event_log.append(pastperfect.Event(name=en, data=kwargs))
 
 
 # class StrEnum(str, Enum):
 #     # Once python3.9 and python.3.10 support is dropped, we can use
 #     # https://docs.python.org/3/library/enum.html#enum.StrEnum
 #     pass
 #
```

### Comparing `profitpulse-2.3.0/src/profitpulse/testrig/fixtures.py` & `profitpulse-2.4.0/src/profitpulse/testrig/fixtures.py`

 * *Files identical despite different names*

### Comparing `profitpulse-2.3.0/src/profitpulse/testrig/scenario.py` & `profitpulse-2.4.0/src/profitpulse/testrig/scenario.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # type: ignore
 from typing import Optional
 
 from typer.testing import CliRunner
 
-from profitpulse.cli.main import profitpulse_app
+from profitpulse.cli.main import cli
 
 runner = CliRunner(mix_stderr=False)
 
 
 class CLIScenario:
     """
     Builds scenarios up on the tests can be run and evaluates the result taking
     the context (CLI) into asset.
     """
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}"
 
     def __init__(self, *_, **__) -> None:
-        self._app = profitpulse_app
+        self._app = cli
 
     # Asset management -----------------------------------------------------------------------------------------------
 
     def show_assets(self):
         """
         Shows all the assets and their current balance.
         """
```

### Comparing `profitpulse-2.3.0/PKG-INFO` & `profitpulse-2.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 Metadata-Version: 2.1
 Name: profitpulse
-Version: 2.3.0
+Version: 2.4.0
 Summary: Manage your personal finances
 Home-page: https://github.com/luistm/profitpulse
 License: MIT
 Author: Luís Miranda
 Author-email: luistm@gmail.com
 Maintainer: Luís Miranda
 Maintainer-email: luistm@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: gogotable (==0.1.0)
-Requires-Dist: pastperfect (>=0.1.0,<0.2.0)
-Requires-Dist: pendulum (>=3.0.0,<4.0.0)
+Requires-Dist: fastapi (>=0.111.0,<0.112.0)
+Requires-Dist: gogotable (>=0.1.0,<0.2.0)
+Requires-Dist: jinja2 (>=3.1.4,<4.0.0)
+Requires-Dist: pastperfect (>=0.3.0,<0.4.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: turbofan (>=0.2.0,<0.3.0)
 Requires-Dist: typer (>=0.12.3,<0.13.0)
+Requires-Dist: uvicorn (>=0.29.0,<0.30.0)
 Project-URL: Repository, https://github.com/luistm/profitpulse
 Description-Content-Type: text/markdown
 
 # Profit Pulse
 
 [![PyPI version](https://badge.fury.io/py/profitpulse.svg)](https://badge.fury.io/py/profitpulse) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/profitpulse)
```

