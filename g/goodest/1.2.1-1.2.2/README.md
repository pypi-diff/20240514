# Comparing `tmp/goodest-1.2.1.tar.gz` & `tmp/goodest-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goodest-1.2.1.tar", max compression
+gzip compressed data, was "goodest-1.2.2.tar", max compression
```

## Comparing `goodest-1.2.1.tar` & `goodest-1.2.2.tar`

### file list

```diff
@@ -1,1452 +1,1507 @@
--rwxr-xr-x   0        0        0     1299 2024-05-14 01:26:46.907128 goodest-1.2.1/pyproject.toml
--rwxr-xr-x   0        0        0     2804 2024-05-13 23:04:12.647856 goodest-1.2.1/venue.S.HTML
--rwxr-xr-x   0        0        0      105 2024-04-27 16:44:17.965844 goodest-1.2.1/venue_journal.S.HTML
--rwxr-xr-x   0        0        0      397 2024-05-13 23:21:53.823261 goodest-1.2.1/venue_monetary.S.HTML
--rwxr-xr-x   0        0        0      405 2024-04-17 03:33:22.073284 goodest-1.2.1/venues/stages/goodest/[__objectives]/book/Vitamin B.S.HTML
--rwxr-xr-x   0        0        0       63 2024-04-17 03:33:22.073284 goodest-1.2.1/venues/stages/goodest/[__objectives]/book/Vitamin K.S.HTML
--rwxr-xr-x   0        0        0      201 2024-04-28 20:53:16.850555 goodest-1.2.1/venues/stages/goodest/[__objectives]/objectives - elliptic.S.HTML
--rwxr-xr-x   0        0        0     1729 2024-05-13 00:59:01.377145 goodest-1.2.1/venues/stages/goodest/[__objectives]/objectives.S.HTML
--rwxr-xr-x   0        0        0      533 2024-05-13 00:59:01.385145 goodest-1.2.1/venues/stages/goodest/[_license]/license.s.HTML
--rwxr-xr-x   0        0        0      116 2024-05-13 00:59:01.385145 goodest-1.2.1/venues/stages/goodest/[_license]/list/goodest.s.HTML
--rwxr-xr-x   0        0        0    37279 2024-04-17 03:33:22.077284 goodest-1.2.1/venues/stages/goodest/[_license]/list/gpl-3.0-standalone.html
--rwxr-xr-x   0        0        0      131 2024-04-28 20:54:59.933399 goodest-1.2.1/venues/stages/goodest/[_license]/list/non-commercial.S.HTML
--rwxr-xr-x   0        0        0     1776 2024-05-13 01:42:44.905899 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves/exports/goodest_inventory/certifications/goodest_inventory.certifications.1.JSON
--rwxr-xr-x   0        0        0   985917 2024-05-13 01:42:46.309870 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves/exports/goodest_inventory/food/goodest_inventory.food.1.JSON
--rwxr-xr-x   0        0        0   985917 2024-05-13 23:22:03.551180 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves/exports/goodest_inventory/food/goodest_inventory.food.2.JSON
--rwxr-xr-x   0        0        0   726299 2024-05-13 01:42:46.301870 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves/exports/goodest_inventory/supp/goodest_inventory.supp.1.JSON
--rwxr-xr-x   0        0        0   726299 2024-05-13 23:22:03.771178 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves/exports/goodest_inventory/supp/goodest_inventory.supp.2.JSON
--rwxr-xr-x   0        0        0      118 2024-05-09 02:02:40.749714 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves/exports/goodest_tract/cautionary_ingredients/goodest_tract.cautionary_ingredients.1.JSON
--rwxr-xr-x   0        0        0      118 2024-05-13 23:22:03.975176 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves/exports/goodest_tract/cautionary_ingredients/goodest_tract.cautionary_ingredients.2.JSON
--rwxr-xr-x   0        0        0        0 2024-05-09 02:02:41.749703 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves/exports/goodest_tract/certifications/goodest_tract.certifications.1.JSON
--rwxr-xr-x   0        0        0        0 2024-05-13 23:22:04.959168 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves/exports/goodest_tract/certifications/goodest_tract.certifications.2.JSON
--rwxr-xr-x   0        0        0     5140 2024-05-09 02:02:40.997712 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves/exports/goodest_tract/essential_nutrients/goodest_tract.essential_nutrients.1.JSON
--rwxr-xr-x   0        0        0     5140 2024-05-13 23:22:04.239174 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves/exports/goodest_tract/essential_nutrients/goodest_tract.essential_nutrients.2.JSON
--rwxr-xr-x   0        0        0        0 2024-05-09 02:02:41.245709 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves/exports/goodest_tract/glossary/goodest_tract.glossary.1.JSON
--rwxr-xr-x   0        0        0        0 2024-05-13 23:22:04.451172 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves/exports/goodest_tract/glossary/goodest_tract.glossary.2.JSON
--rwxr-xr-x   0        0        0     5771 2024-05-09 02:02:41.509706 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves/exports/goodest_tract/goals/goodest_tract.goals.1.JSON
--rwxr-xr-x   0        0        0     5782 2024-05-13 23:22:04.739170 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves/exports/goodest_tract/goals/goodest_tract.goals.2.JSON
--rwxr-xr-x   0        0        0      118 2024-04-17 03:33:22.117283 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v1/exports/goodest_tract/cautionary_ingredients/1.JSON
--rwxr-xr-x   0        0        0      118 2024-04-23 22:05:34.538523 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v1/exports/goodest_tract/cautionary_ingredients/2.JSON
--rwxr-xr-x   0        0        0      118 2024-04-23 22:07:10.673303 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v1/exports/goodest_tract/cautionary_ingredients/3.JSON
--rwxr-xr-x   0        0        0      118 2024-04-27 17:35:00.336394 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v1/exports/goodest_tract/cautionary_ingredients/4.JSON
--rwxr-xr-x   0        0        0      118 2024-04-28 19:02:50.497975 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v1/exports/goodest_tract/cautionary_ingredients/5.JSON
--rwxr-xr-x   0        0        0      118 2024-04-28 19:04:10.818025 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v1/exports/goodest_tract/cautionary_ingredients/6.JSON
--rwxr-xr-x   0        0        0     5140 2024-04-17 03:33:22.117283 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v1/exports/goodest_tract/essential_nutrients/1.JSON
--rwxr-xr-x   0        0        0     5140 2024-04-23 22:05:35.566512 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v1/exports/goodest_tract/essential_nutrients/2.JSON
--rwxr-xr-x   0        0        0     5140 2024-04-23 22:07:11.713281 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v1/exports/goodest_tract/essential_nutrients/3.JSON
--rwxr-xr-x   0        0        0     5140 2024-04-27 17:35:01.316362 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v1/exports/goodest_tract/essential_nutrients/4.JSON
--rwxr-xr-x   0        0        0     5140 2024-04-28 19:02:51.533976 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v1/exports/goodest_tract/essential_nutrients/5.JSON
--rwxr-xr-x   0        0        0     5140 2024-04-28 19:04:11.850026 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v1/exports/goodest_tract/essential_nutrients/6.JSON
--rwxr-xr-x   0        0        0        0 2024-04-23 22:05:36.562502 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v1/exports/goodest_tract/glossary/2.JSON
--rwxr-xr-x   0        0        0        0 2024-04-23 22:07:12.697261 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v1/exports/goodest_tract/glossary/3.JSON
--rwxr-xr-x   0        0        0        0 2024-04-27 17:35:02.312330 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v1/exports/goodest_tract/glossary/4.JSON
--rwxr-xr-x   0        0        0        0 2024-04-28 19:02:52.497976 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v1/exports/goodest_tract/glossary/5.JSON
--rwxr-xr-x   0        0        0        0 2024-04-28 19:04:12.822027 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v1/exports/goodest_tract/glossary/6.JSON
--rwxr-xr-x   0        0        0     5771 2024-04-28 19:04:04.554021 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v1/exports/goodest_tract/goals/5.JSON
--rwxr-xr-x   0        0        0     5771 2024-04-28 19:04:13.826027 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v1/exports/goodest_tract/goals/6.JSON
--rwxr-xr-x   0        0        0      667 2024-05-02 03:16:33.983190 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v1/saves.S.HTML
--rwxr-xr-x   0        0        0      416 2024-05-09 02:31:06.501585 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v2/dumps/goodest_tract/cautionary_ingredients/goodest_tract.cautionary_ingredients.1.dump.gzip
--rwxr-xr-x   0        0        0     1708 2024-05-09 02:31:06.761583 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v2/dumps/goodest_tract/essential_nutrients/goodest_tract.essential_nutrients.1.dump.gzip
--rwxr-xr-x   0        0        0     1799 2024-05-09 02:31:07.257579 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v2/dumps/goodest_tract/goals/goodest_tract.goals.1.dump.gzip
--rwxr-xr-x   0        0        0        0 2024-05-09 01:42:50.087325 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v2/exports/goodest_inventory/food/goodest_inventory.foods.1.JSON
--rwxr-xr-x   0        0        0        0 2024-05-09 02:02:14.490013 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v2/exports/goodest_inventory/food/goodest_inventory.foods.2.JSON
--rwxr-xr-x   0        0        0        0 2024-05-09 02:02:40.217721 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v2/exports/goodest_inventory/food/goodest_inventory.foods.3.JSON
--rwxr-xr-x   0        0        0        0 2024-05-09 01:42:51.099313 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v2/exports/goodest_inventory/supp/goodest_inventory.supps.1.JSON
--rwxr-xr-x   0        0        0        0 2024-05-09 02:02:15.518002 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v2/exports/goodest_inventory/supp/goodest_inventory.supps.2.JSON
--rwxr-xr-x   0        0        0        0 2024-05-09 02:02:40.489717 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v2/exports/goodest_inventory/supp/goodest_inventory.supps.3.JSON
--rwxr-xr-x   0        0        0      118 2024-05-09 01:42:52.135301 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v2/exports/goodest_tract/cautionary_ingredients/goodest_tract.cautionary_ingredients.1.JSON
--rwxr-xr-x   0        0        0      118 2024-05-09 02:02:16.521990 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v2/exports/goodest_tract/cautionary_ingredients/goodest_tract.cautionary_ingredients.2.JSON
--rwxr-xr-x   0        0        0      118 2024-05-09 02:02:40.749714 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v2/exports/goodest_tract/cautionary_ingredients/goodest_tract.cautionary_ingredients.3.JSON
--rwxr-xr-x   0        0        0        0 2024-05-09 01:42:56.123255 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v2/exports/goodest_tract/certifications/goodest_tract.certifications.1.JSON
--rwxr-xr-x   0        0        0        0 2024-05-09 02:02:20.505945 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v2/exports/goodest_tract/certifications/goodest_tract.certifications.2.JSON
--rwxr-xr-x   0        0        0        0 2024-05-09 02:02:41.749703 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v2/exports/goodest_tract/certifications/goodest_tract.certifications.3.JSON
--rwxr-xr-x   0        0        0     5140 2024-05-09 01:42:53.139290 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v2/exports/goodest_tract/essential_nutrients/goodest_tract.essential_nutrients.1.JSON
--rwxr-xr-x   0        0        0     5140 2024-05-09 02:02:17.505979 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v2/exports/goodest_tract/essential_nutrients/goodest_tract.essential_nutrients.2.JSON
--rwxr-xr-x   0        0        0     5140 2024-05-09 02:02:40.997712 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v2/exports/goodest_tract/essential_nutrients/goodest_tract.essential_nutrients.3.JSON
--rwxr-xr-x   0        0        0        0 2024-05-09 01:42:54.127278 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v2/exports/goodest_tract/glossary/goodest_tract.glossary.1.JSON
--rwxr-xr-x   0        0        0        0 2024-05-09 02:02:18.517968 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v2/exports/goodest_tract/glossary/goodest_tract.glossary.2.JSON
--rwxr-xr-x   0        0        0        0 2024-05-09 02:02:41.245709 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v2/exports/goodest_tract/glossary/goodest_tract.glossary.3.JSON
--rwxr-xr-x   0        0        0     5771 2024-05-09 01:42:55.151266 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v2/exports/goodest_tract/goals/goodest_tract.goals.1.JSON
--rwxr-xr-x   0        0        0     5771 2024-05-09 02:02:19.509956 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v2/exports/goodest_tract/goals/goodest_tract.goals.2.JSON
--rwxr-xr-x   0        0        0     5771 2024-05-09 02:02:41.509706 goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v2/exports/goodest_tract/goals/goodest_tract.goals.3.JSON
--rwxr-xr-x   0        0        0      378 2024-05-13 00:59:57.244563 goodest-1.2.1/venues/stages/goodest/__dictionary/goodest_1
--rwxr-xr-x   0        0        0      429 2024-05-13 00:59:01.377145 goodest-1.2.1/venues/stages/goodest/__init__.py
--rwxr-xr-x   0        0        0   128501 2024-05-14 00:56:03.406178 goodest-1.2.1/venues/stages/goodest/__status/API/DB/records.json
--rwxr-xr-x   0        0        0     2100 2024-05-13 00:59:57.292563 goodest-1.2.1/venues/stages/goodest/__status/API/status.proc.py
--rwxr-xr-x   0        0        0     1172 2024-04-17 03:33:22.077284 goodest-1.2.1/venues/stages/goodest/__status/__pycache__/status_API.proc.cpython-310.pyc
--rwxr-xr-x   0        0        0       11 2024-04-23 21:56:29.284154 goodest-1.2.1/venues/stages/goodest/__status/main/.gitignore
--rwxr-xr-x   0        0        0 14150440 2024-05-14 01:27:59.758315 goodest-1.2.1/venues/stages/goodest/__status/main/DB/records.json
--rwxr-xr-x   0        0        0    41183 2024-04-25 01:22:42.760494 goodest-1.2.1/venues/stages/goodest/__status/main/output.json
--rwxr-xr-x   0        0        0     2121 2024-05-13 00:59:58.016555 goodest-1.2.1/venues/stages/goodest/__status/main/status.proc.py
--rwxr-xr-x   0        0        0     1561 2024-05-13 01:04:39.489623 goodest-1.2.1/venues/stages/goodest/_controls/__pycache__/_clique.cpython-310.pyc
--rwxr-xr-x   0        0        0      738 2024-04-23 19:31:08.382022 goodest-1.2.1/venues/stages/goodest/_controls/__pycache__/off.cpython-310.pyc
--rwxr-xr-x   0        0        0      756 2024-04-23 19:30:52.306199 goodest-1.2.1/venues/stages/goodest/_controls/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0      544 2024-04-23 19:31:08.382022 goodest-1.2.1/venues/stages/goodest/_controls/__pycache__/refresh.cpython-310.pyc
--rwxr-xr-x   0        0        0      781 2024-04-23 19:31:08.382022 goodest-1.2.1/venues/stages/goodest/_controls/__pycache__/status.cpython-310.pyc
--rwxr-xr-x   0        0        0     1643 2024-05-13 00:59:57.240563 goodest-1.2.1/venues/stages/goodest/_controls/_clique.py
--rwxr-xr-x   0        0        0     1145 2024-05-13 00:59:57.240563 goodest-1.2.1/venues/stages/goodest/_essence/__init__.py
--rwxr-xr-x   0        0        0      986 2024-05-13 01:04:39.493623 goodest-1.2.1/venues/stages/goodest/_essence/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2438 2024-05-13 00:59:57.240563 goodest-1.2.1/venues/stages/goodest/_essence/activate_alert--/__init__.py
--rwxr-xr-x   0        0        0     1802 2024-05-02 23:21:54.655013 goodest-1.2.1/venues/stages/goodest/_essence/activate_alert--/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      790 2024-05-02 23:21:54.655013 goodest-1.2.1/venues/stages/goodest/_essence/activate_alert--/__pycache__/parse_exception.cpython-310.pyc
--rwxr-xr-x   0        0        0      505 2024-05-13 00:59:57.240563 goodest-1.2.1/venues/stages/goodest/_essence/activate_alert--/parse_exception.py
--rwxr-xr-x   0        0        0      202 2024-04-27 16:49:31.955662 goodest-1.2.1/venues/stages/goodest/_essence/essence.S.HTML
--rwxr-xr-x   0        0        0     3322 2024-05-13 01:45:50.158347 goodest-1.2.1/venues/stages/goodest/_essence/merge/__init__.py
--rwxr-xr-x   0        0        0     1986 2024-05-13 01:47:00.241135 goodest-1.2.1/venues/stages/goodest/_essence/merge/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      719 2024-05-02 02:39:12.702510 goodest-1.2.1/venues/stages/goodest/_essence/scan/__init__.py
--rwxr-xr-x   0        0        0      842 2024-05-02 22:19:11.125002 goodest-1.2.1/venues/stages/goodest/_essence/scan/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      754 2024-05-02 22:19:56.188529 goodest-1.2.1/venues/stages/goodest/_essence/seek/__init__.py
--rwxr-xr-x   0        0        0      770 2024-05-02 22:20:00.192486 goodest-1.2.1/venues/stages/goodest/_essence/seek/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      735 2024-05-10 19:20:27.044506 goodest-1.2.1/venues/stages/goodest/adventures/DNS/counsellor.S.HTML
--rwxr-xr-x   0        0        0      590 2024-05-13 00:59:57.240563 goodest-1.2.1/venues/stages/goodest/adventures/HTTPS_Certs/HTTPS_Certs.S.HTML
--rwxr-xr-x   0        0        0     1538 2024-05-13 01:04:39.489623 goodest-1.2.1/venues/stages/goodest/adventures/_ops/__pycache__/_clique.cpython-310.pyc
--rwxr-xr-x   0        0        0      882 2024-05-13 01:04:39.757620 goodest-1.2.1/venues/stages/goodest/adventures/_ops/__pycache__/off.cpython-310.pyc
--rwxr-xr-x   0        0        0      912 2024-05-13 01:04:39.489623 goodest-1.2.1/venues/stages/goodest/adventures/_ops/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0      583 2024-05-13 01:04:39.757620 goodest-1.2.1/venues/stages/goodest/adventures/_ops/__pycache__/refresh.cpython-310.pyc
--rwxr-xr-x   0        0        0     1111 2024-05-13 01:04:39.757620 goodest-1.2.1/venues/stages/goodest/adventures/_ops/__pycache__/status.cpython-310.pyc
--rwxr-xr-x   0        0        0      861 2024-05-13 00:59:57.232563 goodest-1.2.1/venues/stages/goodest/adventures/_ops/_clique.py
--rwxr-xr-x   0        0        0      794 2024-04-23 19:52:04.387492 goodest-1.2.1/venues/stages/goodest/adventures/_ops/monitor.py
--rwxr-xr-x   0        0        0      763 2024-05-13 00:59:57.232563 goodest-1.2.1/venues/stages/goodest/adventures/_ops/off.py
--rwxr-xr-x   0        0        0      804 2024-05-13 00:59:57.232563 goodest-1.2.1/venues/stages/goodest/adventures/_ops/on.py
--rwxr-xr-x   0        0        0      434 2024-05-13 00:59:57.232563 goodest-1.2.1/venues/stages/goodest/adventures/_ops/refresh.py
--rwxr-xr-x   0        0        0     1028 2024-05-13 00:59:57.232563 goodest-1.2.1/venues/stages/goodest/adventures/_ops/status.py
--rwxr-xr-x   0        0        0      780 2024-05-10 19:21:14.303955 goodest-1.2.1/venues/stages/goodest/adventures/adventures.S.HTML
--rwxr-xr-x   0        0        0     2491 2024-05-13 18:53:48.503003 goodest-1.2.1/venues/stages/goodest/adventures/alerting/__init__.py
--rwxr-xr-x   0        0        0     1851 2024-05-13 18:54:07.598756 goodest-1.2.1/venues/stages/goodest/adventures/alerting/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      788 2024-05-13 01:04:39.753620 goodest-1.2.1/venues/stages/goodest/adventures/alerting/__pycache__/parse_exception.cpython-310.pyc
--rwxr-xr-x   0        0        0      505 2024-05-13 00:59:57.232563 goodest-1.2.1/venues/stages/goodest/adventures/alerting/parse_exception.py
--rwxr-xr-x   0        0        0      794 2024-05-13 00:59:57.240563 goodest-1.2.1/venues/stages/goodest/adventures/cloud_flares/cloud_flares.S.HTML
--rwxr-xr-x   0        0        0      160 2024-05-09 04:34:51.673638 goodest-1.2.1/venues/stages/goodest/adventures/customs/__init__.py
--rwxr-xr-x   0        0        0      630 2024-05-09 04:34:54.301616 goodest-1.2.1/venues/stages/goodest/adventures/customs/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      926 2024-04-17 03:33:22.113283 goodest-1.2.1/venues/stages/goodest/adventures/customs/__pycache__/clique.cpython-310.pyc
--rwxr-xr-x   0        0        0      245 2024-04-17 03:33:22.113283 goodest-1.2.1/venues/stages/goodest/adventures/customs/__pycache__/off.cpython-310.pyc
--rwxr-xr-x   0        0        0      345 2024-04-17 03:33:22.113283 goodest-1.2.1/venues/stages/goodest/adventures/customs/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0      251 2024-04-17 03:33:22.113283 goodest-1.2.1/venues/stages/goodest/adventures/customs/__pycache__/status.cpython-310.pyc
--rwxr-xr-x   0        0        0      948 2024-05-13 01:04:39.761620 goodest-1.2.1/venues/stages/goodest/adventures/customs/_ops/__pycache__/_clique.cpython-310.pyc
--rwxr-xr-x   0        0        0      579 2024-05-13 00:59:57.240563 goodest-1.2.1/venues/stages/goodest/adventures/customs/_ops/_clique.py
--rwxr-xr-x   0        0        0        2 2024-05-09 04:35:38.109250 goodest-1.2.1/venues/stages/goodest/adventures/customs/_ops/off.py
--rwxr-xr-x   0        0        0      662 2024-05-09 04:39:09.399469 goodest-1.2.1/venues/stages/goodest/adventures/customs/_ops/on.py
--rwxr-xr-x   0        0        0        2 2024-04-27 23:15:34.237762 goodest-1.2.1/venues/stages/goodest/adventures/customs/_ops/status.py
--rwxr-xr-x   0        0        0      285 2024-05-09 04:40:07.774973 goodest-1.2.1/venues/stages/goodest/adventures/customs/configs_school/embargo.NFT
--rwxr-xr-x   0        0        0      145 2024-04-27 23:16:20.801181 goodest-1.2.1/venues/stages/goodest/adventures/customs/customs.S.HTML
--rwxr-xr-x   0        0        0     1327 2024-01-25 05:00:54.191593 goodest-1.2.1/venues/stages/goodest/adventures/demux_hap/HA.s.HTML
--rwxr-xr-x   0        0        0      238 2023-12-02 04:53:31.462384 goodest-1.2.1/venues/stages/goodest/adventures/demux_hap/SSL/SSL.r.HTML
--rwxr-xr-x   0        0        0      985 2023-12-14 02:01:36.217926 goodest-1.2.1/venues/stages/goodest/adventures/demux_hap/SSL/__init__.py
--rwxr-xr-x   0        0        0     1086 2024-05-10 01:30:13.387176 goodest-1.2.1/venues/stages/goodest/adventures/demux_hap/SSL/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1872 2023-12-14 02:01:38.764897 goodest-1.2.1/venues/stages/goodest/adventures/demux_hap/SSL/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1757 2023-12-01 23:15:16.435121 goodest-1.2.1/venues/stages/goodest/adventures/demux_hap/SSL/certificate.pem
--rwxr-xr-x   0        0        0     3272 2023-12-01 23:15:16.430121 goodest-1.2.1/venues/stages/goodest/adventures/demux_hap/SSL/certificate.pem.key
--rwxr-xr-x   0        0        0      346 2023-12-01 18:00:33.471576 goodest-1.2.1/venues/stages/goodest/adventures/demux_hap/__init__.py
--rwxr-xr-x   0        0        0      576 2024-05-10 01:29:49.491477 goodest-1.2.1/venues/stages/goodest/adventures/demux_hap/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      737 2024-05-12 19:04:34.064153 goodest-1.2.1/venues/stages/goodest/adventures/demux_hap/_controls/__pycache__/_clique.cpython-310.pyc
--rwxr-xr-x   0        0        0      617 2024-05-13 01:04:39.761620 goodest-1.2.1/venues/stages/goodest/adventures/demux_hap/_controls/__pycache__/build.cpython-310.pyc
--rwxr-xr-x   0        0        0      328 2024-05-10 01:44:25.794256 goodest-1.2.1/venues/stages/goodest/adventures/demux_hap/_controls/__pycache__/off.cpython-310.pyc
--rwxr-xr-x   0        0        0      924 2024-05-13 01:04:39.757620 goodest-1.2.1/venues/stages/goodest/adventures/demux_hap/_controls/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0      345 2024-05-12 16:13:33.336331 goodest-1.2.1/venues/stages/goodest/adventures/demux_hap/_controls/_clique.py
--rwxr-xr-x   0        0        0      312 2024-05-13 00:59:57.232563 goodest-1.2.1/venues/stages/goodest/adventures/demux_hap/_controls/build.py
--rwxr-xr-x   0        0        0       77 2024-05-10 01:44:23.514282 goodest-1.2.1/venues/stages/goodest/adventures/demux_hap/_controls/off.py
--rwxr-xr-x   0        0        0      901 2024-05-13 00:59:57.232563 goodest-1.2.1/venues/stages/goodest/adventures/demux_hap/_controls/on.py
--rwxr-xr-x   0        0        0     1295 2023-12-02 01:06:44.630336 goodest-1.2.1/venues/stages/goodest/adventures/demux_hap/configs/HTTPS_to_HTTP/1.py
--rwxr-xr-x   0        0        0      567 2023-12-04 23:16:04.198925 goodest-1.2.1/venues/stages/goodest/adventures/demux_hap/configs/HTTPS_to_HTTP/HTTPS_to_HTTP.s.HTML
--rwxr-xr-x   0        0        0     1892 2024-05-13 00:59:57.232563 goodest-1.2.1/venues/stages/goodest/adventures/demux_hap/configs/HTTPS_to_HTTP/__init__.py
--rwxr-xr-x   0        0        0     1921 2024-05-13 01:04:39.757620 goodest-1.2.1/venues/stages/goodest/adventures/demux_hap/configs/HTTPS_to_HTTP/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2832 2023-12-14 04:27:42.320026 goodest-1.2.1/venues/stages/goodest/adventures/demux_hap/configs/HTTPS_to_HTTP/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1296 2023-12-01 22:31:43.018311 goodest-1.2.1/venues/stages/goodest/adventures/demux_hap/configs/HTTP_balancer/__init__.py
--rwxr-xr-x   0        0        0     1774 2023-12-01 22:50:16.802479 goodest-1.2.1/venues/stages/goodest/adventures/demux_hap/configs/HTTP_balancer/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      277 2023-12-01 21:44:47.102165 goodest-1.2.1/venues/stages/goodest/adventures/demux_hap/configs/HTTP_balancer/examples/example_1.cfg
--rwxr-xr-x   0        0        0     1652 2023-12-01 18:07:24.317812 goodest-1.2.1/venues/stages/goodest/adventures/demux_hap/configs/__pycache__/HTTP_balancer.cpython-311.pyc
--rwxr-xr-x   0        0        0     3286 2023-12-01 18:05:41.851249 goodest-1.2.1/venues/stages/goodest/adventures/demux_hap/configs/examples/haproxy.cfg
--rwxr-xr-x   0        0        0     2457 2023-12-01 21:46:11.432916 goodest-1.2.1/venues/stages/goodest/adventures/demux_hap/configs/examples/haproxy_2.cfg
--rwxr-xr-x   0        0        0     2191 2024-01-25 05:03:52.719628 goodest-1.2.1/venues/stages/goodest/adventures/demux_hap/configs/external_reverse/__init__.py
--rwxr-xr-x   0        0        0      217 2024-05-10 00:51:31.625387 goodest-1.2.1/venues/stages/goodest/adventures/demux_hap/demux.S.HTML
--rwxr-xr-x   0        0        0      229 2023-12-02 01:03:02.539647 goodest-1.2.1/venues/stages/goodest/adventures/demux_hap/journalctl/journalctl.r.HTML
--rwxr-xr-x   0        0        0      227 2023-12-02 01:02:28.789164 goodest-1.2.1/venues/stages/goodest/adventures/demux_hap/systemctl/systemctl.S.HTML
--rwxr-xr-x   0        0        0       14 2024-04-24 01:06:32.184393 goodest-1.2.1/venues/stages/goodest/adventures/monetary/.gitignore
--rwxr-xr-x   0        0        0      856 2024-05-13 01:04:39.753620 goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_inventory/__pycache__/connect.cpython-310.pyc
--rwxr-xr-x   0        0        0     1266 2024-05-13 01:04:39.753620 goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_inventory/_treasures/_indexes/__pycache__/drop_and_create.cpython-310.pyc
--rwxr-xr-x   0        0        0     1034 2024-05-13 00:59:57.240563 goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_inventory/_treasures/_indexes/drop_and_create.py
--rwxr-xr-x   0        0        0      905 2024-05-13 00:59:57.240563 goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_inventory/connect.py
--rwxr-xr-x   0        0        0     1041 2024-05-10 02:47:15.578725 goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_inventory/foods/_indexes/__pycache__/drop_and_create.cpython-310.pyc
--rwxr-xr-x   0        0        0     1370 2024-05-13 01:08:31.375266 goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_inventory/foods/document/__pycache__/find.cpython-310.pyc
--rwxr-xr-x   0        0        0     2028 2024-05-13 04:19:23.390074 goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_inventory/foods/document/__pycache__/insert.cpython-310.pyc
--rwxr-xr-x   0        0        0     1210 2024-05-13 00:59:57.236563 goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_inventory/foods/document/find.py
--rwxr-xr-x   0        0        0     2182 2024-05-13 04:18:05.491009 goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_inventory/foods/document/insert.py
--rwxr-xr-x   0        0        0      132 2024-05-13 00:59:57.240563 goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_inventory/goodest_inventory.S.HTML
--rwxr-xr-x   0        0        0     1327 2024-05-13 01:08:31.375266 goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_inventory/supps/document/__pycache__/find.cpython-310.pyc
--rwxr-xr-x   0        0        0     1981 2024-05-12 23:53:44.710441 goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_inventory/supps/document/__pycache__/insert.cpython-310.pyc
--rwxr-xr-x   0        0        0     1156 2024-05-13 00:59:57.236563 goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_inventory/supps/document/find.py
--rwxr-xr-x   0        0        0     2108 2024-05-13 04:18:36.698634 goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_inventory/supps/document/insert.py
--rwxr-xr-x   0        0        0       17 2024-04-17 03:33:22.117283 goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_tract/.gitignore
--rwxr-xr-x   0        0        0      454 2024-04-17 03:33:22.117283 goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_tract/__itinerary/itinerary.S.HTML
--rwxr-xr-x   0        0        0     1820 2024-04-17 03:33:22.117283 goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_tract/__pycache__/clique.cpython-310.pyc
--rwxr-xr-x   0        0        0      832 2024-05-13 01:08:31.263266 goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_tract/__pycache__/connect.cpython-310.pyc
--rwxr-xr-x   0        0        0      799 2024-05-13 01:08:31.359266 goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_tract/_land/__pycache__/find_name.cpython-310.pyc
--rwxr-xr-x   0        0        0        4 2024-04-28 00:13:51.336698 goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_tract/_land/__pycache__/insert_document.cpython-310.pyc
--rwxr-xr-x   0        0        0      811 2024-05-13 01:08:31.263266 goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_tract/_land/__pycache__/retrieve_every.cpython-310.pyc
--rwxr-xr-x   0        0        0      196 2024-04-24 22:53:29.564774 goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_tract/_land/_land.S.HTML
--rwxr-xr-x   0        0        0      712 2024-05-13 00:59:57.236563 goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_tract/_land/find_name.py
--rwxr-xr-x   0        0        0      934 2024-05-13 00:59:57.236563 goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_tract/_land/insert_document.py
--rwxr-xr-x   0        0        0      613 2024-05-13 00:59:57.236563 goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_tract/_land/retrieve_every.py
--rwxr-xr-x   0        0        0      170 2024-04-17 03:33:22.117283 goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_tract/cautionary_ingredients/cautionary_ingredients.S.HTML
--rwxr-xr-x   0        0        0     1172 2024-05-13 00:59:57.236563 goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_tract/connect.py
--rwxr-xr-x   0        0        0      721 2024-04-24 23:09:34.366674 goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_tract/essential_nutrients/essential_nutrients.S.HTML
--rwxr-xr-x   0        0        0      401 2024-04-24 23:06:14.224847 goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_tract/glossary/glossary.S.HTML
--rwxr-xr-x   0        0        0     1824 2024-05-14 00:11:11.229872 goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_tract/goals/__pycache__/find_ingredient.cpython-310.pyc
--rwxr-xr-x   0        0        0     1257 2024-05-13 02:41:11.683142 goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_tract/goals/__pycache__/insert.cpython-310.pyc
--rwxr-xr-x   0        0        0      732 2024-05-13 02:42:37.938213 goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_tract/goals/__pycache__/retrieve.cpython-310.pyc
--rwxr-xr-x   0        0        0      725 2024-05-13 21:38:26.763908 goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_tract/goals/__pycache__/retrieve_one.cpython-310.pyc
--rwxr-xr-x   0        0        0      860 2024-04-28 02:43:34.943005 goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_tract/goals/_indexes/__pycache__/create.cpython-310.pyc
--rwxr-xr-x   0        0        0     1071 2024-05-02 22:26:24.276333 goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_tract/goals/_indexes/__pycache__/drop_and_create.cpython-310.pyc
--rwxr-xr-x   0        0        0      840 2024-05-13 00:59:57.236563 goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_tract/goals/_indexes/drop_and_create.py
--rwxr-xr-x   0        0        0     1843 2024-05-14 00:11:06.453950 goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_tract/goals/find_ingredient.py
--rwxr-xr-x   0        0        0      117 2024-04-28 02:07:02.567921 goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_tract/goals/goals.S.HTML
--rwxr-xr-x   0        0        0     1376 2024-05-13 02:41:09.559165 goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_tract/goals/insert.py
--rwxr-xr-x   0        0        0      653 2024-05-13 02:42:27.038331 goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_tract/goals/retrieve.py
--rwxr-xr-x   0        0        0      622 2024-05-13 19:28:44.851419 goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_tract/goals/retrieve_one.py
--rwxr-xr-x   0        0        0     1489 2024-05-13 00:59:57.236563 goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_tract/ingredients.S.HTML
--rwxr-xr-x   0        0        0        0 2024-04-17 03:33:22.113283 goodest-1.2.1/venues/stages/goodest/adventures/monetary/__init__.py
--rwxr-xr-x   0        0        0      150 2024-04-17 03:36:48.047066 goodest-1.2.1/venues/stages/goodest/adventures/monetary/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1687 2024-04-17 03:33:22.113283 goodest-1.2.1/venues/stages/goodest/adventures/monetary/__pycache__/clique.cpython-310.pyc
--rwxr-xr-x   0        0        0      680 2024-04-17 03:33:22.113283 goodest-1.2.1/venues/stages/goodest/adventures/monetary/__pycache__/connect.cpython-310.pyc
--rwxr-xr-x   0        0        0      857 2024-04-17 03:33:22.113283 goodest-1.2.1/venues/stages/goodest/adventures/monetary/__pycache__/off.cpython-310.pyc
--rwxr-xr-x   0        0        0     1904 2024-04-17 03:33:22.113283 goodest-1.2.1/venues/stages/goodest/adventures/monetary/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0     1610 2024-04-23 19:31:08.342022 goodest-1.2.1/venues/stages/goodest/adventures/monetary/__pycache__/status.cpython-310.pyc
--rwxr-xr-x   0        0        0     1451 2024-05-13 01:04:39.757620 goodest-1.2.1/venues/stages/goodest/adventures/monetary/_ops/__pycache__/_clique.cpython-310.pyc
--rwxr-xr-x   0        0        0      879 2024-05-13 01:04:39.757620 goodest-1.2.1/venues/stages/goodest/adventures/monetary/_ops/__pycache__/off.cpython-310.pyc
--rwxr-xr-x   0        0        0     2209 2024-05-13 01:04:39.713620 goodest-1.2.1/venues/stages/goodest/adventures/monetary/_ops/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0     1659 2024-05-13 01:04:39.713620 goodest-1.2.1/venues/stages/goodest/adventures/monetary/_ops/__pycache__/status.cpython-310.pyc
--rwxr-xr-x   0        0        0     1087 2024-05-13 00:59:57.232563 goodest-1.2.1/venues/stages/goodest/adventures/monetary/_ops/_clique.py
--rwxr-xr-x   0        0        0      875 2024-05-13 00:59:57.232563 goodest-1.2.1/venues/stages/goodest/adventures/monetary/_ops/off.py
--rwxr-xr-x   0        0        0     2712 2024-05-13 00:59:57.232563 goodest-1.2.1/venues/stages/goodest/adventures/monetary/_ops/on.py
--rwxr-xr-x   0        0        0     1913 2024-05-13 01:04:39.761620 goodest-1.2.1/venues/stages/goodest/adventures/monetary/_ops/saves/__pycache__/_clique.cpython-310.pyc
--rwxr-xr-x   0        0        0     2152 2024-04-17 03:33:22.117283 goodest-1.2.1/venues/stages/goodest/adventures/monetary/_ops/saves/__pycache__/clique.cpython-310.pyc
--rwxr-xr-x   0        0        0     1651 2024-05-13 00:59:57.232563 goodest-1.2.1/venues/stages/goodest/adventures/monetary/_ops/saves/_clique.py
--rwxr-xr-x   0        0        0     1442 2024-05-13 01:04:39.761620 goodest-1.2.1/venues/stages/goodest/adventures/monetary/_ops/saves/dumps/__pycache__/dump.cpython-310.pyc
--rwxr-xr-x   0        0        0     1428 2024-05-13 01:04:39.761620 goodest-1.2.1/venues/stages/goodest/adventures/monetary/_ops/saves/dumps/__pycache__/restore.cpython-310.pyc
--rwxr-xr-x   0        0        0     1580 2024-05-13 00:59:57.232563 goodest-1.2.1/venues/stages/goodest/adventures/monetary/_ops/saves/dumps/dump.py
--rwxr-xr-x   0        0        0     1508 2024-05-13 00:59:57.232563 goodest-1.2.1/venues/stages/goodest/adventures/monetary/_ops/saves/dumps/restore.py
--rwxr-xr-x   0        0        0     1407 2024-05-13 01:04:39.761620 goodest-1.2.1/venues/stages/goodest/adventures/monetary/_ops/saves/exports/__pycache__/monetary_export.cpython-310.pyc
--rwxr-xr-x   0        0        0     1398 2024-05-13 01:04:39.761620 goodest-1.2.1/venues/stages/goodest/adventures/monetary/_ops/saves/exports/__pycache__/monetary_import.cpython-310.pyc
--rwxr-xr-x   0        0        0     1463 2024-05-13 00:59:57.232563 goodest-1.2.1/venues/stages/goodest/adventures/monetary/_ops/saves/exports/monetary_export.py
--rwxr-xr-x   0        0        0     1420 2024-05-13 00:59:57.232563 goodest-1.2.1/venues/stages/goodest/adventures/monetary/_ops/saves/exports/monetary_import.py
--rwxr-xr-x   0        0        0      390 2024-04-23 20:10:51.728325 goodest-1.2.1/venues/stages/goodest/adventures/monetary/_ops/saves/memories.S.HTML
--rwxr-xr-x   0        0        0     1797 2024-05-13 00:59:57.232563 goodest-1.2.1/venues/stages/goodest/adventures/monetary/_ops/status.py
--rwxr-xr-x   0        0        0      459 2024-05-13 00:59:57.240563 goodest-1.2.1/venues/stages/goodest/adventures/monetary/monetary.S.HTML
--rwxr-xr-x   0        0        0      631 2024-05-13 01:04:39.713620 goodest-1.2.1/venues/stages/goodest/adventures/monetary/moves/URL/__pycache__/retrieve.cpython-310.pyc
--rwxr-xr-x   0        0        0      482 2024-05-13 00:59:57.232563 goodest-1.2.1/venues/stages/goodest/adventures/monetary/moves/URL/retrieve.py
--rwxr-xr-x   0        0        0     1014 2024-05-13 00:59:57.236563 goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/__init__.py
--rwxr-xr-x   0        0        0     1108 2024-05-13 01:08:31.375266 goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2093 2024-01-20 22:08:03.263097 goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1416 2024-01-18 21:56:05.761257 goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/scan_3.s.HTML
--rwxr-xr-x   0        0        0      764 2024-05-13 00:41:57.767791 goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/__pycache__/limits.cpython-310.pyc
--rwxr-xr-x   0        0        0     1242 2024-01-17 21:00:52.050922 goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/__pycache__/limits.cpython-311.pyc
--rwxr-xr-x   0        0        0     3355 2024-01-18 01:45:49.087517 goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/__pycache__/stats.cpython-311.pyc
--rwxr-xr-x   0        0        0      578 2024-05-13 00:17:13.283304 goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/limits.py
--rwxr-xr-x   0        0        0     5944 2024-05-13 02:50:49.488923 goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/__init__.py
--rwxr-xr-x   0        0        0     4822 2024-05-13 02:50:52.584894 goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     7791 2024-01-20 22:06:11.831292 goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      560 2024-02-05 15:21:50.027143 goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/affirm/__pycache__/direction.cpython-310.pyc
--rwxr-xr-x   0        0        0      770 2024-01-19 00:57:06.516080 goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/affirm/__pycache__/direction.cpython-311.pyc
--rwxr-xr-x   0        0        0     1079 2024-01-19 21:24:23.060989 goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/affirm/__pycache__/filters.cpython-311.pyc
--rwxr-xr-x   0        0        0      386 2024-01-19 00:13:41.687885 goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/affirm/direction.py
--rwxr-xr-x   0        0        0      693 2024-02-05 15:21:50.035142 goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/__pycache__/before_and_after.cpython-310.pyc
--rwxr-xr-x   0        0        0      842 2024-01-19 00:57:36.578735 goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/__pycache__/before_and_after.cpython-311.pyc
--rwxr-xr-x   0        0        0      470 2024-02-05 15:21:50.031142 goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/__pycache__/check_fields.cpython-310.pyc
--rwxr-xr-x   0        0        0      540 2024-01-19 00:57:36.577735 goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/__pycache__/check_fields.cpython-311.pyc
--rwxr-xr-x   0        0        0      461 2024-02-05 15:21:50.031142 goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/__pycache__/lower_case_name.cpython-310.pyc
--rwxr-xr-x   0        0        0      511 2024-01-19 00:57:36.578735 goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/__pycache__/lower_case_name.cpython-311.pyc
--rwxr-xr-x   0        0        0      509 2024-02-05 15:21:50.031142 goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/__pycache__/sort_name_emblem.cpython-310.pyc
--rwxr-xr-x   0        0        0      587 2024-01-19 00:57:36.578735 goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/__pycache__/sort_name_emblem.cpython-311.pyc
--rwxr-xr-x   0        0        0      671 2024-02-05 15:21:50.031142 goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/__pycache__/unionize.cpython-310.pyc
--rwxr-xr-x   0        0        0      847 2024-01-19 00:57:06.516080 goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/__pycache__/unionize.cpython-311.pyc
--rwxr-xr-x   0        0        0      848 2024-01-19 00:29:46.750852 goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/before_and_after.py
--rwxr-xr-x   0        0        0      170 2024-01-18 22:27:33.009237 goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/check_fields.py
--rwxr-xr-x   0        0        0      514 2024-02-05 15:21:50.035142 goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/filters/__pycache__/limit.cpython-310.pyc
--rwxr-xr-x   0        0        0      564 2024-01-19 01:20:04.182165 goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/filters/__pycache__/limit.cpython-311.pyc
--rwxr-xr-x   0        0        0      524 2024-02-05 15:21:50.035142 goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/filters/__pycache__/scan_string.cpython-310.pyc
--rwxr-xr-x   0        0        0      683 2024-01-19 00:57:36.578735 goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/filters/__pycache__/scan_string.cpython-311.pyc
--rwxr-xr-x   0        0        0      683 2024-02-05 15:21:50.035142 goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/filters/__pycache__/vector_name.cpython-310.pyc
--rwxr-xr-x   0        0        0      795 2024-01-19 00:57:36.579735 goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/filters/__pycache__/vector_name.cpython-311.pyc
--rwxr-xr-x   0        0        0      939 2024-02-05 15:21:50.035142 goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/filters/__pycache__/vector_name_and_emblem.cpython-310.pyc
--rwxr-xr-x   0        0        0     1143 2024-01-19 21:47:13.310446 goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/filters/__pycache__/vector_name_and_emblem.cpython-311.pyc
--rwxr-xr-x   0        0        0      618 2024-01-19 00:53:26.187609 goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/filters/filters.s.HTML
--rwxr-xr-x   0        0        0      290 2024-01-19 01:19:36.215470 goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/filters/limit.py
--rwxr-xr-x   0        0        0      238 2024-01-18 22:32:50.168704 goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/filters/scan_string.py
--rwxr-xr-x   0        0        0     1208 2024-01-19 00:52:38.678154 goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/filters/vector_name.py
--rwxr-xr-x   0        0        0     1977 2024-01-19 21:47:09.259509 goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/filters/vector_name_and_emblem.py
--rwxr-xr-x   0        0        0      617 2024-02-15 00:15:32.679560 goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/formats/__pycache__/format_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      658 2024-01-20 22:07:26.051496 goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/formats/__pycache__/format_1.cpython-311.pyc
--rwxr-xr-x   0        0        0      290 2024-02-15 00:15:31.703573 goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/formats/format_1.py
--rwxr-xr-x   0        0        0      121 2024-01-18 22:29:05.056212 goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/lower_case_name.py
--rwxr-xr-x   0        0        0      379 2024-01-19 00:29:48.264835 goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/sort_name_emblem.py
--rwxr-xr-x   0        0        0      591 2024-01-19 00:29:46.767852 goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/unionize.py
--rwxr-xr-x   0        0        0      665 2024-02-05 15:21:50.027143 goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/spruce/__pycache__/filters.cpython-310.pyc
--rwxr-xr-x   0        0        0     1169 2024-01-19 21:33:44.004002 goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/spruce/__pycache__/filters.cpython-311.pyc
--rwxr-xr-x   0        0        0      528 2024-01-19 21:33:42.836021 goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/spruce/filters.py
--rwxr-xr-x   0        0        0     1304 2024-05-13 00:45:24.741643 goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/stats/__init__.py
--rwxr-xr-x   0        0        0      972 2024-05-13 00:45:27.617613 goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/stats/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1100 2024-01-19 19:16:29.681719 goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/stats/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     3148 2024-01-19 00:55:25.534239 goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/stats/__pycache__/union.cpython-311.pyc
--rwxr-xr-x   0        0        0     3461 2024-05-13 00:59:57.236563 goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/stats/union.py
--rwxr-xr-x   0        0        0     1343 2024-04-23 22:34:43.485503 goodest-1.2.1/venues/stages/goodest/adventures/redis_mix/_ops/__pycache__/off.cpython-310.pyc
--rwxr-xr-x   0        0        0     1759 2024-04-23 22:34:42.625513 goodest-1.2.1/venues/stages/goodest/adventures/redis_mix/_ops/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0     1288 2024-04-23 22:34:43.489503 goodest-1.2.1/venues/stages/goodest/adventures/redis_mix/_ops/__pycache__/refresh.cpython-310.pyc
--rwxr-xr-x   0        0        0     1311 2024-04-23 22:34:42.629513 goodest-1.2.1/venues/stages/goodest/adventures/redis_mix/_ops/__pycache__/status.cpython-310.pyc
--rwxr-xr-x   0        0        0      802 2024-05-13 00:59:57.240563 goodest-1.2.1/venues/stages/goodest/adventures/redis_mix/_ops/_clique.py
--rwxr-xr-x   0        0        0      332 2024-05-13 00:59:57.240563 goodest-1.2.1/venues/stages/goodest/adventures/redis_mix/_ops/off.py
--rwxr-xr-x   0        0        0      329 2024-05-13 00:59:57.240563 goodest-1.2.1/venues/stages/goodest/adventures/redis_mix/_ops/on.py
--rwxr-xr-x   0        0        0      334 2024-05-13 00:59:57.240563 goodest-1.2.1/venues/stages/goodest/adventures/redis_mix/_ops/refresh.py
--rwxr-xr-x   0        0        0      343 2024-05-13 00:59:57.240563 goodest-1.2.1/venues/stages/goodest/adventures/redis_mix/_ops/status.py
--rwxr-xr-x   0        0        0      130 2024-04-24 18:57:58.564669 goodest-1.2.1/venues/stages/goodest/adventures/redis_mix/redis_mix.S.HTML
--rwxr-xr-x   0        0        0      730 2024-05-12 20:01:09.578795 goodest-1.2.1/venues/stages/goodest/adventures/sanique/[objectives]/objectives.S.HTML
--rwxr-xr-x   0        0        0      188 2024-04-17 03:33:22.117283 goodest-1.2.1/venues/stages/goodest/adventures/sanique/__init__.py
--rwxr-xr-x   0        0        0      598 2024-04-17 17:46:30.800270 goodest-1.2.1/venues/stages/goodest/adventures/sanique/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1415 2024-05-13 01:04:39.757620 goodest-1.2.1/venues/stages/goodest/adventures/sanique/_ops/__pycache__/off.cpython-310.pyc
--rwxr-xr-x   0        0        0     1920 2024-05-13 01:04:39.489623 goodest-1.2.1/venues/stages/goodest/adventures/sanique/_ops/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0     1362 2024-05-13 01:04:39.757620 goodest-1.2.1/venues/stages/goodest/adventures/sanique/_ops/__pycache__/refresh.cpython-310.pyc
--rwxr-xr-x   0        0        0     1330 2024-05-13 17:13:10.736946 goodest-1.2.1/venues/stages/goodest/adventures/sanique/_ops/__pycache__/status.cpython-310.pyc
--rwxr-xr-x   0        0        0     1467 2024-05-13 00:59:01.401145 goodest-1.2.1/venues/stages/goodest/adventures/sanique/_ops/off.py
--rwxr-xr-x   0        0        0     1990 2024-05-13 00:59:01.401145 goodest-1.2.1/venues/stages/goodest/adventures/sanique/_ops/on.py
--rwxr-xr-x   0        0        0     1235 2024-05-13 00:59:01.401145 goodest-1.2.1/venues/stages/goodest/adventures/sanique/_ops/refresh.py
--rwxr-xr-x   0        0        0     1303 2024-05-13 17:13:01.173055 goodest-1.2.1/venues/stages/goodest/adventures/sanique/_ops/status.py
--rwxr-xr-x   0        0        0     1064 2024-05-13 00:59:01.405145 goodest-1.2.1/venues/stages/goodest/adventures/sanique/_status/API_status_besties__food_USDA__nature_v2__FDC_ID_1.py
--rwxr-xr-x   0        0        0     1199 2024-05-13 01:14:34.821033 goodest-1.2.1/venues/stages/goodest/adventures/sanique/_status/__pycache__/API_status_besties__food_USDA__nature_v2__FDC_ID_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      791 2024-05-13 00:59:01.401145 goodest-1.2.1/venues/stages/goodest/adventures/sanique/clique.py
--rwxr-xr-x   0        0        0     4380 2024-05-13 23:54:27.255294 goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/__init__.py
--rwxr-xr-x   0        0        0     3170 2024-05-13 23:54:41.334864 goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     3636 2024-05-13 23:56:30.107741 goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/addresses/guest/__init__.py
--rwxr-xr-x   0        0        0     3506 2024-05-13 23:56:33.579646 goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/addresses/guest/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     3002 2024-05-14 01:19:21.344071 goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/addresses/guest/vue/__init__.py
--rw-r--r--   0        0        0     2359 2024-05-14 01:19:23.656046 goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/addresses/guest/vue/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     3335 2024-01-21 04:18:08.256227 goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/addresses/guest/vue/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      561 2024-05-08 21:23:06.200098 goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/addresses/guest/vue/caching.S.HTML
--rwxr-xr-x   0        0        0     1658 2024-05-13 01:10:51.450510 goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/addresses/guest_bits/__init__.py
--rwxr-xr-x   0        0        0     1187 2024-05-13 01:11:00.310457 goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/addresses/guest_bits/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      168 2024-05-12 20:24:56.030964 goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/addresses/guest_bits/bits.S.HTML
--rwxr-xr-x   0        0        0     3242 2024-05-13 02:52:14.056108 goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/addresses/guest_goodest_inventory/foods/__init__.py
--rwxr-xr-x   0        0        0     2485 2024-05-13 02:52:19.484055 goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/addresses/guest_goodest_inventory/foods/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      696 2024-05-13 00:59:01.405145 goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/addresses/guest_goodest_inventory/recipes/__init__.py
--rwxr-xr-x   0        0        0      907 2024-05-13 01:11:00.310457 goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/addresses/guest_goodest_inventory/recipes/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      687 2024-05-13 00:59:01.405145 goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/addresses/guest_goodest_inventory/supps/__init__.py
--rwxr-xr-x   0        0        0      892 2024-05-13 01:11:00.310457 goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/addresses/guest_goodest_inventory/supps/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     3101 2024-05-13 23:36:01.872117 goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/addresses/staff/__init__.py
--rwxr-xr-x   0        0        0     2834 2024-05-13 23:47:08.646472 goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/addresses/staff/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1608 2024-05-13 22:57:24.026758 goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/addresses/staff/__pycache__/besties__food_USDA__nature_v2__FDC_ID.cpython-310.pyc
--rwxr-xr-x   0        0        0     1573 2024-05-13 22:57:24.026758 goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/addresses/staff/__pycache__/besties__supp_NIH__nature_v2__DSLD_ID.cpython-310.pyc
--rwxr-xr-x   0        0        0     1722 2024-05-13 22:56:54.814945 goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/addresses/staff/besties__food_USDA__nature_v2__FDC_ID.py
--rwxr-xr-x   0        0        0     1480 2024-05-13 22:56:59.294916 goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/addresses/staff/besties__supp_NIH__nature_v2__DSLD_ID.py
--rwxr-xr-x   0        0        0      283 2024-05-08 23:22:18.957260 goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/addresses/staff/protected.S.HTML
--rwxr-xr-x   0        0        0     1734 2024-05-14 00:13:46.691384 goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/addresses/staff_goodest_inventory/foods/__init__.py
--rwxr-xr-x   0        0        0     2011 2024-05-14 00:16:09.005179 goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/addresses/staff_goodest_inventory/foods/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      837 2024-05-13 23:36:20.623959 goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/addresses/staff_goodest_inventory/recipes/__init__.py
--rwxr-xr-x   0        0        0     1107 2024-05-13 23:47:08.746471 goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/addresses/staff_goodest_inventory/recipes/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1416 2024-05-14 00:14:11.990987 goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/addresses/staff_goodest_inventory/supps/__init__.py
--rwxr-xr-x   0        0        0     1590 2024-05-14 00:16:09.009179 goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/addresses/staff_goodest_inventory/supps/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      425 2024-05-13 00:59:01.401145 goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/sockets_guest/__init__.py
--rwxr-xr-x   0        0        0      726 2024-05-13 01:08:31.003267 goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/sockets_guest/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1008 2024-05-12 22:50:40.664451 goodest-1.2.1/venues/stages/goodest/adventures/sanique/quests_guests/__pycache__/find_food.cpython-310.pyc
--rwxr-xr-x   0        0        0     1374 2024-05-13 22:06:23.071845 goodest-1.2.1/venues/stages/goodest/adventures/sanique/quests_guests/__pycache__/retrieve_food.cpython-310.pyc
--rwxr-xr-x   0        0        0      625 2024-05-13 02:35:09.679038 goodest-1.2.1/venues/stages/goodest/adventures/sanique/quests_guests/__pycache__/retrieve_goals.cpython-310.pyc
--rwxr-xr-x   0        0        0     1191 2024-05-13 03:57:04.720471 goodest-1.2.1/venues/stages/goodest/adventures/sanique/quests_guests/__pycache__/retrieve_recipe.cpython-310.pyc
--rwxr-xr-x   0        0        0     1167 2024-05-13 22:16:56.062569 goodest-1.2.1/venues/stages/goodest/adventures/sanique/quests_guests/__pycache__/retrieve_supp.cpython-310.pyc
--rwxr-xr-x   0        0        0     1908 2024-05-13 02:00:30.545915 goodest-1.2.1/venues/stages/goodest/adventures/sanique/quests_guests/__pycache__/search_goods.cpython-310.pyc
--rwxr-xr-x   0        0        0     1922 2024-05-13 22:06:05.327965 goodest-1.2.1/venues/stages/goodest/adventures/sanique/quests_guests/retrieve_food.py
--rwxr-xr-x   0        0        0      373 2024-05-13 02:29:10.122901 goodest-1.2.1/venues/stages/goodest/adventures/sanique/quests_guests/retrieve_goal.py
--rwxr-xr-x   0        0        0      405 2024-05-13 02:35:06.463072 goodest-1.2.1/venues/stages/goodest/adventures/sanique/quests_guests/retrieve_goals.py
--rwxr-xr-x   0        0        0     1103 2024-05-13 03:57:01.616503 goodest-1.2.1/venues/stages/goodest/adventures/sanique/quests_guests/retrieve_recipe.py
--rwxr-xr-x   0        0        0     1500 2024-05-13 22:16:53.362595 goodest-1.2.1/venues/stages/goodest/adventures/sanique/quests_guests/retrieve_supp.py
--rwxr-xr-x   0        0        0     2488 2024-05-13 02:00:26.473964 goodest-1.2.1/venues/stages/goodest/adventures/sanique/quests_guests/search_goods.py
--rwxr-xr-x   0        0        0      530 2024-05-13 00:59:01.405145 goodest-1.2.1/venues/stages/goodest/adventures/sanique/sanique.S.HTML
--rwxr-xr-x   0        0        0     1200 2024-05-09 23:05:53.524539 goodest-1.2.1/venues/stages/goodest/adventures/sanique/utilities/__pycache__/generate_inventory_paths.cpython-310.pyc
--rwxr-xr-x   0        0        0      388 2024-04-17 03:36:47.855070 goodest-1.2.1/venues/stages/goodest/adventures/sanique/utilities/__pycache__/has_sanic_check.cpython-310.pyc
--rwxr-xr-x   0        0        0      533 2024-05-13 01:14:35.297030 goodest-1.2.1/venues/stages/goodest/adventures/sanique/utilities/__pycache__/retrieve_sanique_URL.cpython-310.pyc
--rwxr-xr-x   0        0        0      539 2024-05-13 00:59:01.401145 goodest-1.2.1/venues/stages/goodest/adventures/sanique/utilities/check_key/__init__.py
--rwxr-xr-x   0        0        0      786 2024-05-13 01:08:31.259266 goodest-1.2.1/venues/stages/goodest/adventures/sanique/utilities/check_key/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1538 2024-05-09 23:04:59.513271 goodest-1.2.1/venues/stages/goodest/adventures/sanique/utilities/generate_inventory_paths.py
--rwxr-xr-x   0        0        0      167 2024-04-17 03:33:22.117283 goodest-1.2.1/venues/stages/goodest/adventures/sanique/utilities/has_sanic_check.py
--rwxr-xr-x   0        0        0      296 2024-05-13 00:59:01.401145 goodest-1.2.1/venues/stages/goodest/adventures/sanique/utilities/retrieve_sanique_URL.py
--rwxr-xr-x   0        0        0      127 2024-05-08 19:30:19.000000 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/.eslintrc.js--
--rwxr-xr-x   0        0        0       94 2024-05-08 19:30:19.000000 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/.gitignore
--rwxr-xr-x   0        0        0       26 2024-05-08 19:30:19.000000 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/.npmrc
--rwxr-xr-x   0        0        0      939 2024-05-08 19:30:19.000000 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/README.md
--rwxr-xr-x   0        0        0     1285 2024-05-08 20:46:06.699827 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/__objectives/objectives -- possibilities.S.HTML
--rwxr-xr-x   0        0        0       27 2024-05-08 20:45:59.995896 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/__objectives/objectives.S.HTML
--rwxr-xr-x   0        0        0        2 2024-05-08 21:03:01.449010 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/_controls/off.py
--rwxr-xr-x   0        0        0        0 2024-05-08 21:06:04.803018 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/_controls/on.py
--rwxr-xr-x   0        0        0      127 2024-05-08 19:30:19.000000 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/school/.eslintrc.cjs
--rwxr-xr-x   0        0        0      353 2024-05-09 21:32:18.768121 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/school/index.html
--rwxr-xr-x   0        0        0      370 2024-05-10 02:14:54.482607 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/school/package.json
--rwxr-xr-x   0        0        0     1435 2024-05-08 19:30:19.000000 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/school/public/typescript.svg
--rwxr-xr-x   0        0        0     1497 2024-05-08 19:30:19.000000 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/school/public/vite.svg
--rwxr-xr-x   0        0        0       23 2024-05-09 21:32:59.207717 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/school/src/main.js
--rwxr-xr-x   0        0        0       75 2024-05-08 19:30:19.000000 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/school/tsconfig.json--
--rwxr-xr-x   0        0        0      365 2024-05-10 02:14:10.075052 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/school/vite.config.js
--rwxr-xr-x   0        0        0      127 2024-05-08 19:30:19.000000 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/staff/.eslintrc.cjs
--rwxr-xr-x   0        0        0      363 2024-05-09 21:34:48.778605 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/staff/index.html
--rwxr-xr-x   0        0        0      397 2024-05-10 02:10:36.785101 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/staff/package.json
--rwxr-xr-x   0        0        0     1435 2024-05-08 19:30:19.000000 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/staff/public/typescript.svg
--rwxr-xr-x   0        0        0     1497 2024-05-08 19:30:19.000000 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/staff/public/vite.svg
--rwxr-xr-x   0        0        0        1 2024-05-09 21:33:50.275202 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/staff/src/main.js
--rwxr-xr-x   0        0        0      367 2024-05-10 02:08:38.618156 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/staff/vite.config.js
--rwxr-xr-x   0        0        0      127 2024-05-08 19:30:19.000000 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/.eslintrc.cjs--
--rwxr-xr-x   0        0        0      556 2024-05-08 22:05:09.904886 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/.eslintrc.json
--rwxr-xr-x   0        0        0     1156 2024-05-14 00:06:31.058668 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/index.html
--rwxr-xr-x   0        0        0     2241 2024-05-10 02:12:54.363797 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/package.json
--rwxr-xr-x   0        0        0     2369 2024-05-12 21:40:53.463627 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/Earth/app.js
--rwxr-xr-x   0        0        0     1704 2024-05-14 00:16:03.101269 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/Earth/logistics/guests/index.js
--rwxr-xr-x   0        0        0      800 2024-05-11 00:47:10.035262 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/Earth/logistics/index.js
--rwxr-xr-x   0        0        0       27 2023-12-08 17:29:39.919713 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/Earth/logistics/logistics.s.HTML
--rwxr-xr-x   0        0        0      205 2024-05-11 00:47:10.019262 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/Earth/logistics/staff/index.js
--rwxr-xr-x   0        0        0      893 2024-05-11 00:12:34.448880 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/Earth/logistics/status/index.js
--rwxr-xr-x   0        0        0      229 2024-02-02 20:25:55.023588 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/Earth/logistics/workshop/index.js
--rwxr-xr-x   0        0        0      286 2024-03-06 23:00:24.198272 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/Earth/scenery/planet/components/local_storage_flip/decor.js
--rwxr-xr-x   0        0        0      335 2024-03-06 23:20:10.831615 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/Earth/scenery/planet/components/local_storage_flip/decor.vue
--rwxr-xr-x   0        0        0     2544 2024-05-09 19:36:44.871475 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/Earth/scenery/planet/field.js
--rwxr-xr-x   0        0        0     2442 2024-03-25 23:22:40.575764 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/Earth/scenery/planet/field.vue
--rwxr-xr-x   0        0        0     1202 2024-03-21 19:29:12.760368 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/Earth/warehouses/layout/index.js
--rwxr-xr-x   0        0        0       26 2024-02-18 21:37:35.527677 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/apps.S.HTML
--rwxr-xr-x   0        0        0     1455 2024-03-31 04:39:51.030367 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/fields/app/index.js
--rwxr-xr-x   0        0        0     1590 2024-03-31 04:39:16.990772 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/fields/append.js
--rwxr-xr-x   0        0        0      811 2024-02-19 01:14:44.725717 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/fields/boundary/embellishments.js
--rwxr-xr-x   0        0        0     3144 2024-02-19 03:39:47.599945 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/fields/boundary/embellishments.vue
--rwxr-xr-x   0        0        0      716 2024-05-09 19:36:44.871475 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/fields/fields.S.HTML
--rwxr-xr-x   0        0        0     2024 2024-02-20 02:24:26.825728 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/fields/hacienda/eco.js
--rwxr-xr-x   0        0        0      762 2024-03-30 03:27:25.126133 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/fields/hacienda/eco.vue
--rwxr-xr-x   0        0        0     1215 2024-02-19 03:34:56.055049 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/fields/hacienda/methods/fn/keypress.js
--rwxr-xr-x   0        0        0     1950 2024-02-19 03:11:56.242621 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/fields/hacienda/methods/index.js
--rwxr-xr-x   0        0        0      330 2023-12-13 05:57:32.245095 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/fields/moves/build_field_element.js
--rwxr-xr-x   0        0        0      208 2023-12-13 05:58:02.416723 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/fields/moves/get_next_coordinate.js
--rwxr-xr-x   0        0        0      153 2023-12-13 05:44:37.428631 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/fields/moves/variables.js
--rwxr-xr-x   0        0        0      739 2024-03-30 19:18:20.469563 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/fields/remove.js
--rwxr-xr-x   0        0        0     2015 2023-08-08 03:01:34.460945 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/assets/base--.css
--rwxr-xr-x   0        0        0      276 2023-08-08 02:05:29.442900 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/assets/logo.svg
--rwxr-xr-x   0        0        0      373 2023-11-14 00:07:17.821680 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/assets/main.css
--rwxr-xr-x   0        0        0      107 2024-05-10 22:52:00.937025 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/constants/index.js
--rwxr-xr-x   0        0        0     1248 2024-05-13 00:59:57.080565 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/fleet/ask/get.js
--rwxr-xr-x   0        0        0      218 2024-05-12 22:34:30.027372 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/fleet/fleet.s.HTML
--rwxr-xr-x   0        0        0      744 2024-05-13 03:57:29.508215 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/fleet/goodest_DB/essential_nutrients/recipe/index.js
--rwxr-xr-x   0        0        0      628 2024-05-13 17:41:19.302286 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/fleet/goodest_DB/food/retrieve/index.js
--rwxr-xr-x   0        0        0      602 2024-05-13 17:41:43.085996 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/fleet/goodest_DB/supp/retrieve/index.js
--rwxr-xr-x   0        0        0      596 2024-05-13 00:59:57.080565 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/fleet/goodest_DB/treasures/search/index.js
--rwxr-xr-x   0        0        0      389 2024-05-13 02:27:50.727752 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/fleet/nutrition_meadow/goals/scan.js
--rwxr-xr-x   0        0        0      397 2024-05-13 02:27:55.755698 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/fleet/nutrition_meadow/goals/scan_emblem.js
--rwxr-xr-x   0        0        0     1115 2024-05-13 00:49:31.551077 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/fleet/syllabus/lap/index.js
--rwxr-xr-x   0        0        0      131 2024-02-13 05:37:01.717416 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/fleet/syllabus/lap/index.s.HTML
--rwxr-xr-x   0        0        0      881 2023-12-08 23:49:09.502834 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/Fraction/to_float.ST.js
--rwxr-xr-x   0        0        0      702 2023-12-12 01:06:28.803271 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/Fraction/to_float.js
--rwxr-xr-x   0        0        0      204 2023-09-13 18:17:19.482855 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/PERCENTIZE/FRACTION.ST.js
--rwxr-xr-x   0        0        0      159 2023-11-07 02:46:35.479079 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/PERCENTIZE/FRACTION.js
--rwxr-xr-x   0        0        0      497 2024-02-13 05:22:20.703032 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/PERSIST/index.js
--rwxr-xr-x   0        0        0      212 2023-12-08 02:24:16.484912 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/assert/equal.js
--rwxr-xr-x   0        0        0      348 2023-11-02 01:04:18.515660 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/circuit/index.js
--rwxr-xr-x   0        0        0      373 2024-02-05 20:27:55.449652 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/document_title/document_title.s.HTML
--rwxr-xr-x   0        0        0      273 2024-02-12 00:35:32.740011 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/element-tree/element-tree.s.HTML
--rwxr-xr-x   0        0        0     1090 2024-02-02 19:24:05.871600 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/food/FIND_ENERGY_PER_GRAM.js
--rwxr-xr-x   0        0        0      227 2024-02-02 19:24:05.914600 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/food/FIND_TEAM.js
--rwxr-xr-x   0        0        0      208 2023-11-02 01:35:32.692959 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/food/find_name.js
--rwxr-xr-x   0        0        0      198 2024-02-02 19:24:05.892600 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/food/find_stats_link.js
--rwxr-xr-x   0        0        0      174 2023-11-02 01:36:19.736289 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/food/food.r.html
--rwxr-xr-x   0        0        0      841 2024-02-12 01:38:07.918853 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/furnish/array.js
--rwxr-xr-x   0        0        0      676 2024-02-12 01:38:26.850644 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/furnish/array.status.js
--rwxr-xr-x   0        0        0      994 2024-02-12 01:39:02.930246 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/furnish/index.js
--rwxr-xr-x   0        0        0      407 2023-11-07 01:16:23.318853 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/furnish/index.status.js
--rwxr-xr-x   0        0        0      828 2024-02-12 01:39:31.409932 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/furnish/string.js
--rwxr-xr-x   0        0        0      753 2023-11-02 01:53:09.683957 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/furnish/string.status.js
--rwxr-xr-x   0        0        0     1443 2023-11-01 23:25:43.495916 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/monitors/focus.js
--rwxr-xr-x   0        0        0      307 2023-12-16 01:10:42.413067 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/brand/name.js
--rwxr-xr-x   0        0        0    19575 2023-12-08 22:35:11.870201 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/essential_nutrients/grove/calc_linear_grove/grove-1.js
--rwxr-xr-x   0        0        0      986 2023-12-08 22:47:39.547348 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/essential_nutrients/grove/calc_linear_grove/index.ST.js
--rwxr-xr-x   0        0        0     1098 2024-03-29 22:13:21.370645 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/essential_nutrients/grove/calc_linear_grove/index.js
--rwxr-xr-x   0        0        0      534 2023-12-17 02:09:13.722149 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/essential_nutrients/grove/ingredient/biological_activity.js
--rwxr-xr-x   0        0        0      451 2023-12-09 01:07:30.680541 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/essential_nutrients/grove/ingredient/mass_plus_mass_eq.js
--rwxr-xr-x   0        0        0      307 2023-12-16 01:00:27.201226 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/essential_nutrients/grove/ingredient/name_0.js
--rwxr-xr-x   0        0        0    19583 2023-12-09 00:19:43.841136 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/essential_nutrients/grove/sort/cryo/grove-1.js
--rwxr-xr-x   0        0        0     1033 2023-12-09 00:47:16.810756 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/essential_nutrients/grove/sort/index.2.ST.js
--rwxr-xr-x   0        0        0      762 2024-03-29 21:09:30.234921 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/essential_nutrients/grove/sort/index.ST.js
--rwxr-xr-x   0        0        0     2893 2024-03-29 21:07:07.864628 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/essential_nutrients/grove/sort/index.js
--rwxr-xr-x   0        0        0      318 2023-12-16 01:07:05.372883 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/identity/name.js
--rwxr-xr-x   0        0        0      321 2023-12-08 17:26:20.969221 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/product/find_brand_name.js
--rwxr-xr-x   0        0        0      370 2023-11-02 03:41:07.550130 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/product/find_name.js
--rwxr-xr-x   0        0        0      333 2023-12-08 17:22:41.038887 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/product/find_product_name.js
--rwxr-xr-x   0        0        0      367 2023-11-02 03:39:40.191371 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/product/find_stats_link.js
--rwxr-xr-x   0        0        0      522 2023-11-02 02:34:36.978741 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/product/is.js
--rwxr-xr-x   0        0        0      281 2023-11-15 03:58:43.852449 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/product/kind.ST.js
--rwxr-xr-x   0        0        0      291 2023-11-15 03:59:01.299303 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/product/kind.js
--rwxr-xr-x   0        0        0        0 2023-11-13 20:01:59.479392 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/product/mass/index.js
--rwxr-xr-x   0        0        0      375 2023-11-13 21:26:12.604024 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/product/quantified_grove/sort.ST.js
--rwxr-xr-x   0        0        0     1921 2023-12-08 04:04:27.829816 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/product/quantified_grove/sort.js
--rwxr-xr-x   0        0        0     3116 2024-02-02 20:18:47.275475 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nutrients--/sort/index.ST.js
--rwxr-xr-x   0        0        0     1456 2023-09-13 19:07:48.507970 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nutrients--/sort/index.js
--rwxr-xr-x   0        0        0      196 2023-11-07 01:47:24.334036 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/object/has_field.js
--rwxr-xr-x   0        0        0        9 2023-09-22 19:27:47.727905 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/processor/index.js
--rwxr-xr-x   0        0        0        8 2023-09-22 19:27:42.190982 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/queue/index.js
--rwxr-xr-x   0        0        0      882 2023-12-08 23:08:26.437630 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/round_quantity/index.ST.js
--rwxr-xr-x   0        0        0      645 2023-12-09 04:44:44.573476 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/round_quantity/index.js
--rwxr-xr-x   0        0        0     2106 2023-11-13 20:35:06.226320 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/struct_2/ingredient/mass.ST.js
--rwxr-xr-x   0        0        0     1463 2023-11-13 20:35:15.278220 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/struct_2/ingredient/mass.js
--rwxr-xr-x   0        0        0      349 2023-11-02 03:40:22.158775 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/struct_2/product/find_brand_name.js
--rwxr-xr-x   0        0        0      370 2023-11-02 03:41:07.550130 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/struct_2/product/find_name.js
--rwxr-xr-x   0        0        0      363 2023-11-02 03:49:19.294141 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/struct_2/product/find_product_name.js
--rwxr-xr-x   0        0        0      367 2023-11-02 03:39:40.191371 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/struct_2/product/find_stats_link.js
--rwxr-xr-x   0        0        0      522 2023-11-02 02:34:36.978741 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/struct_2/product/is.js
--rwxr-xr-x   0        0        0      281 2023-11-15 03:58:43.852449 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/struct_2/product/kind.ST.js
--rwxr-xr-x   0        0        0      291 2023-11-15 03:59:01.299303 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/struct_2/product/kind.js
--rwxr-xr-x   0        0        0        0 2023-11-13 20:01:59.479392 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/struct_2/product/mass/index.js
--rwxr-xr-x   0        0        0      375 2023-11-13 21:26:12.604024 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/struct_2/product/quantified_grove/sort.ST.js
--rwxr-xr-x   0        0        0     1920 2023-12-08 23:49:54.502496 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/struct_2/product/quantified_grove/sort.js
--rwxr-xr-x   0        0        0      205 2024-02-02 20:05:48.697210 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/wait_for.js
--rwxr-xr-x   0        0        0       59 2024-02-11 19:01:30.792959 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/main.js
--rwxr-xr-x   0        0        0      282 2024-02-02 20:07:26.009544 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/_template/field.js
--rwxr-xr-x   0        0        0      165 2023-12-13 00:55:20.087280 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/_template/field.vue
--rwxr-xr-x   0        0        0       85 2024-03-21 19:09:31.608077 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/about/about.S.HTML
--rwxr-xr-x   0        0        0      564 2024-01-19 23:32:34.020141 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/about/decor.js
--rwxr-xr-x   0        0        0     2922 2024-05-13 00:59:57.100565 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/about/decor.vue
--rwxr-xr-x   0        0        0      253 2024-03-30 19:18:20.557562 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/about/open.js
--rwxr-xr-x   0        0        0      897 2024-05-11 00:16:05.358492 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/controls/decor/custom/decor.vue
--rwxr-xr-x   0        0        0     2338 2024-05-11 00:16:31.550197 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/controls/decor/generic/decor.vue
--rwxr-xr-x   0        0        0      676 2023-11-10 00:33:31.498239 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/controls/decor/references/decor.vue
--rwxr-xr-x   0        0        0      915 2024-05-10 22:56:04.106070 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/controls/decor.js
--rwxr-xr-x   0        0        0      474 2024-05-11 00:40:59.670388 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/controls/decor.s.HTML
--rwxr-xr-x   0        0        0     1043 2024-05-10 21:22:09.919119 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/controls/decor.vue
--rwxr-xr-x   0        0        0     1119 2023-09-21 01:20:42.255138 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/controls/notes/ARIA/roles.r.html
--rwxr-xr-x   0        0        0      303 2023-11-26 17:48:20.650243 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/controls/notes/Windows/notes.r.html
--rwxr-xr-x   0        0        0       82 2023-09-27 22:36:56.542685 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/controls/notes/linux/NOTES.HTML
--rwxr-xr-x   0        0        0     1050 2023-11-26 17:48:20.630243 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/controls/notes/notes.r.html
--rwxr-xr-x   0        0        0     1148 2024-03-30 03:28:33.537352 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/controls/priorities/possibilities.s.HTML
--rwxr-xr-x   0        0        0      620 2024-03-30 19:18:20.553562 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/empty_cart/field.js
--rwxr-xr-x   0        0        0      650 2023-12-13 06:11:58.148410 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/empty_cart/field.vue
--rwxr-xr-x   0        0        0      501 2024-03-15 03:09:43.926060 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/goal/features.js
--rwxr-xr-x   0        0        0      300 2024-03-15 00:08:58.070241 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/goal/features.vue
--rwxr-xr-x   0        0        0      249 2024-03-30 19:18:20.553562 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/goal/open.js
--rwxr-xr-x   0        0        0       55 2024-03-31 04:40:52.717638 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/ingredient/feature.js
--rwxr-xr-x   0        0        0      569 2024-03-31 04:42:03.016814 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/ingredient/feature.vue
--rwxr-xr-x   0        0        0      380 2024-03-31 04:39:06.150901 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/ingredient/open.js
--rwxr-xr-x   0        0        0     2738 2024-02-12 01:43:57.151144 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/navigation-lab/field.js
--rwxr-xr-x   0        0        0     2257 2024-02-11 23:57:55.473669 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/navigation-lab/field.vue
--rwxr-xr-x   0        0        0      179 2024-05-10 22:53:28.043951 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/parcels.s.HTML
--rwxr-xr-x   0        0        0     1852 2024-05-09 19:36:44.919475 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/physics/field.js
--rwxr-xr-x   0        0        0     1259 2024-03-21 17:53:56.773315 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/physics/field.vue
--rwxr-xr-x   0        0        0      261 2024-05-09 19:36:44.919475 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/physics/open.js
--rwxr-xr-x   0        0        0      864 2024-05-14 00:40:55.296193 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/scan_filter_by/field.js
--rwxr-xr-x   0        0        0      866 2024-05-14 00:41:11.672024 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/scan_filter_by/field.vue
--rwxr-xr-x   0        0        0      321 2024-03-30 19:18:20.549562 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/scan_filter_by/open.js
--rwxr-xr-x   0        0        0      286 2024-02-18 23:10:18.011339 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/scan_sort_by/field.js
--rwxr-xr-x   0        0        0      350 2024-02-11 23:57:55.657667 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/scan_sort_by/field.vue
--rwxr-xr-x   0        0        0      309 2024-03-30 19:18:20.549562 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/scan_sort_by/open.js
--rwxr-xr-x   0        0        0       29 2024-02-05 20:30:45.897227 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/search filter/field.js
--rwxr-xr-x   0        0        0      352 2024-02-11 23:57:55.825665 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/search filter/field.vue
--rwxr-xr-x   0        0        0     1475 2024-05-09 01:16:32.527415 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/sink-filter/field.js
--rwxr-xr-x   0        0        0     6354 2024-05-09 01:02:12.873953 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/sink-filter/field.vue
--rwxr-xr-x   0        0        0      302 2024-03-30 19:18:20.553562 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/sink-filter/open.js
--rwxr-xr-x   0        0        0       44 2024-02-19 04:49:00.682527 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/sink-filter/slides/slide-1/scenery.vue
--rwxr-xr-x   0        0        0     1042 2024-05-13 00:59:57.100565 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/sink-filter/steps.S.HTML
--rwxr-xr-x   0        0        0     1112 2024-02-16 03:50:07.925341 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/sink-filter/steps_v1.S.HTML
--rwxr-xr-x   0        0        0     1072 2024-05-13 00:59:57.100565 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/sink-filter/steps_v2.S.HTML
--rwxr-xr-x   0        0        0      240 2024-03-30 19:18:20.541562 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/unit_systems/decor/system_international_with_food_calories_and_IU/field.js
--rwxr-xr-x   0        0        0     2352 2024-02-05 20:31:31.369067 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/unit_systems/decor/system_international_with_food_calories_and_IU/field.vue
--rwxr-xr-x   0        0        0      418 2024-03-30 19:18:20.541562 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/unit_systems/field.js
--rwxr-xr-x   0        0        0      384 2024-03-30 19:18:20.537562 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/unit_systems/field.vue
--rwxr-xr-x   0        0        0       25 2024-02-05 20:32:55.188729 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/unreported/field.js
--rwxr-xr-x   0        0        0      725 2024-02-11 23:57:55.953664 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/unreported/field.vue
--rwxr-xr-x   0        0        0     1392 2024-03-30 19:18:20.497563 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/__shows_d3/decor.vue
--rwxr-xr-x   0        0        0      159 2023-11-07 02:31:40.330665 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/__shows_d3/theatrics/ERROR.vue
--rwxr-xr-x   0        0        0     1165 2024-03-30 19:18:20.493563 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/__shows_d3/theatrics/NETWORK_2/field.js
--rwxr-xr-x   0        0        0      135 2024-03-30 19:18:20.489563 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/__shows_d3/theatrics/NETWORK_2/field.vue
--rwxr-xr-x   0        0        0     5571 2023-10-16 00:06:58.093758 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/__shows_d3/theatrics/NETWORK_D3_2/PHYSICAL/index.js
--rwxr-xr-x   0        0        0     1923 2024-03-30 19:18:20.493563 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/__shows_d3/theatrics/NETWORK_D3_2/field.js
--rwxr-xr-x   0        0        0      251 2024-03-30 19:18:20.493563 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/__shows_d3/theatrics/NETWORK_D3_2/field.vue
--rwxr-xr-x   0        0        0     2649 2024-03-30 19:18:20.497563 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/__shows_d3/theatrics/NETWORK_D3_3/field.js
--rwxr-xr-x   0        0        0      341 2024-03-30 19:18:20.497563 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/__shows_d3/theatrics/NETWORK_D3_3/field.vue
--rwxr-xr-x   0        0        0      262 2023-10-16 00:43:32.202900 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/__shows_d3/theatrics/NETWORK_D3_3/methods/FIND_STRUCTURE.js
--rwxr-xr-x   0        0        0     6029 2023-11-09 01:36:29.097181 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/__shows_d3/theatrics/NETWORK_D3_3/methods/PHYSICAL/index.js
--rwxr-xr-x   0        0        0     1802 2023-11-09 01:35:18.334938 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/__shows_d3/theatrics/NETWORK_D3_3/methods/reinvigorate.js
--rwxr-xr-x   0        0        0        2 2023-11-09 02:22:38.537393 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/__shows_d3/theatrics/intro/show.js
--rwxr-xr-x   0        0        0      792 2023-11-09 02:23:32.503812 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/__shows_d3/theatrics/intro/show.vue
--rwxr-xr-x   0        0        0     4310 2023-11-09 01:27:57.103654 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/__shows_d3/theatrics/net/field.js
--rwxr-xr-x   0        0        0      135 2023-11-09 01:26:19.886675 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/__shows_d3/theatrics/net/field.vue
--rwxr-xr-x   0        0        0      172 2024-05-13 00:59:57.092565 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/bests/decor.vue
--rwxr-xr-x   0        0        0     2053 2024-05-13 04:20:41.973139 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/cart/decor.js
--rwxr-xr-x   0        0        0     2540 2024-03-22 00:08:58.862157 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/cart/decor.vue
--rwxr-xr-x   0        0        0        0 2023-09-01 01:58:11.319246 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/comparisons/region.js
--rwxr-xr-x   0        0        0       38 2023-09-01 02:02:20.555211 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/comparisons/region.vue
--rwxr-xr-x   0        0        0       14 2024-03-07 01:00:36.002731 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/customer.s.HTML
--rwxr-xr-x   0        0        0      105 2023-11-16 17:27:03.728124 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/emblem/decor.js
--rwxr-xr-x   0        0        0       99 2023-11-16 17:27:21.384926 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/emblem/decor.vue
--rwxr-xr-x   0        0        0      395 2023-12-08 17:28:03.400445 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor/brands/decor.js
--rwxr-xr-x   0        0        0      318 2024-02-12 02:52:00.985418 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor/brands/decor.vue
--rwxr-xr-x   0        0        0      342 2024-02-02 19:55:15.353779 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor/comments.vue
--rwxr-xr-x   0        0        0      888 2024-03-11 02:46:39.110041 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor/composition/decor.js
--rwxr-xr-x   0        0        0     1039 2024-03-11 02:46:15.522334 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor/composition/decor.vue
--rwxr-xr-x   0        0        0      294 2023-11-02 04:14:07.392983 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor/composition--/composition.r.html
--rwxr-xr-x   0        0        0      935 2023-11-12 23:41:04.957885 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor/composition--/field.js
--rwxr-xr-x   0        0        0      887 2024-02-02 19:55:38.510667 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor/composition--/field.vue
--rwxr-xr-x   0        0        0      396 2023-12-17 02:24:04.194955 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor/ingredients_unmeasured/decor.vue
--rwxr-xr-x   0        0        0      135 2024-02-12 02:50:10.018607 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor/kind.vue
--rwxr-xr-x   0        0        0      995 2024-03-31 22:51:44.207173 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor/product/decor.js
--rwxr-xr-x   0        0        0     1148 2024-03-31 22:53:25.562095 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor/product/decor.vue
--rwxr-xr-x   0        0        0      211 2023-11-14 00:45:18.997484 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor/quantity/decor.vue
--rwxr-xr-x   0        0        0        0 2023-11-02 04:09:32.993886 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor/recommendations/decor.js
--rwxr-xr-x   0        0        0     1226 2024-02-02 19:55:57.099620 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor/recommendations/decor.vue
--rwxr-xr-x   0        0        0     1055 2023-12-17 02:27:33.154567 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor/references/decor.vue
--rwxr-xr-x   0        0        0      371 2024-02-12 02:50:42.554259 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor/warnings.vue
--rwxr-xr-x   0        0        0      106 2024-02-02 19:28:46.031884 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor/zone.vue
--rwxr-xr-x   0        0        0     1727 2024-03-31 22:35:01.749748 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor.js
--rwxr-xr-x   0        0        0     4080 2024-05-13 04:23:09.363403 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor.vue
--rwxr-xr-x   0        0        0      921 2024-05-13 00:59:57.092565 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/methods/index.js
--rwxr-xr-x   0        0        0     1375 2024-03-12 20:01:19.748652 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/goal/room.js
--rwxr-xr-x   0        0        0     1810 2024-03-22 01:23:27.394386 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/goal/room.vue
--rwxr-xr-x   0        0        0     2762 2024-03-09 19:36:31.563195 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/goal/room_v1.vue
--rwxr-xr-x   0        0        0     3219 2024-05-13 00:59:57.096565 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/goods/cycles/methods.js
--rwxr-xr-x   0        0        0      805 2024-05-09 19:36:44.887475 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/goods/decor/food--/decor.js
--rwxr-xr-x   0        0        0     1241 2024-03-06 23:29:46.725085 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/goods/decor/food--/decor.vue
--rwxr-xr-x   0        0        0     2074 2024-03-21 23:11:47.526494 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/goods/decor/search_controls/decor.vue
--rwxr-xr-x   0        0        0      702 2024-05-09 19:36:44.887475 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/goods/decor/supplement/decor.js
--rwxr-xr-x   0        0        0     1110 2024-02-05 20:44:18.272696 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/goods/decor/supplement/decor.vue
--rwxr-xr-x   0        0        0     1193 2024-05-10 22:58:59.788002 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/goods/decor.js
--rwxr-xr-x   0        0        0       84 2024-05-10 22:57:41.412919 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/goods/decor.s.HTML
--rwxr-xr-x   0        0        0     4097 2024-05-10 23:00:15.635121 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/goods/decor.vue
--rwxr-xr-x   0        0        0       52 2024-05-09 19:36:44.887475 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/goods/physics/index.js
--rwxr-xr-x   0        0        0     2110 2024-05-13 00:59:57.096565 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/habitat/decor.js
--rwxr-xr-x   0        0        0      307 2024-05-13 19:42:04.890785 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/habitat/decor.vue
--rwxr-xr-x   0        0        0      273 2024-02-03 01:10:33.156562 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/habitat/panels/image_styles.js
--rwxr-xr-x   0        0        0     2750 2024-05-13 17:24:05.206246 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/habitat/panels/panel_1.vue
--rwxr-xr-x   0        0        0     3186 2024-05-13 00:59:57.096565 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/habitat/panels/panel_goodness.vue
--rwxr-xr-x   0        0        0     3610 2024-05-13 19:56:47.025810 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/habitat/panels/panel_health.vue
--rwxr-xr-x   0        0        0     4052 2024-05-13 19:45:58.980254 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/habitat/panels/panel_moon.vue
--rwxr-xr-x   0        0        0     3129 2024-05-13 19:14:53.224302 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/habitat/panels/panel_organic_crop_farming.vue
--rwxr-xr-x   0        0        0     3763 2024-05-13 20:39:28.652548 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/habitat/panels/panel_physics.vue
--rwxr-xr-x   0        0        0     3245 2024-05-13 02:14:33.692290 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/habitat/panels/panel_sink.vue
--rwxr-xr-x   0        0        0     2478 2024-05-13 00:59:57.096565 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/habitat/panels/panel_sink_caution.vue
--rwxr-xr-x   0        0        0     2317 2024-05-09 01:10:44.396492 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/habitat/panels/panel_sloop.vue
--rwxr-xr-x   0        0        0     3309 2024-05-13 19:47:52.367028 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/habitat/panels/panel_tech.vue
--rwxr-xr-x   0        0        0     1242 2024-02-12 02:21:47.246129 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/map/decor.js
--rwxr-xr-x   0        0        0      869 2024-02-12 02:21:30.222335 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/map/decor.vue
--rwxr-xr-x   0        0        0       64 2024-03-21 19:37:18.810900 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/recipes/decor.vue
--rwxr-xr-x   0        0        0      493 2024-03-07 01:00:36.426725 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor/brands/decor.js
--rwxr-xr-x   0        0        0      316 2023-12-16 01:11:08.924844 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor/brands/decor.vue
--rwxr-xr-x   0        0        0      344 2024-02-02 19:55:46.154059 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor/comments.vue
--rwxr-xr-x   0        0        0      938 2023-11-12 17:32:45.874714 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor/composition--/field.js
--rwxr-xr-x   0        0        0      916 2023-11-12 17:31:30.962525 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor/composition--/field.vue
--rwxr-xr-x   0        0        0       79 2023-09-20 21:35:51.996726 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor/films/field.vue
--rwxr-xr-x   0        0        0      148 2023-11-09 21:59:10.425347 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor/kind.vue
--rwxr-xr-x   0        0        0     2408 2024-03-11 02:24:13.877519 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor/measured_ingredients/fountains.js
--rwxr-xr-x   0        0        0     3341 2024-03-11 02:27:03.199709 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor/measured_ingredients/fountains.vue
--rwxr-xr-x   0        0        0     1095 2024-03-31 23:39:17.593025 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor/product/decor.js
--rwxr-xr-x   0        0        0     1575 2024-04-01 02:00:57.182789 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor/product/decor.vue
--rwxr-xr-x   0        0        0     1096 2023-12-20 19:19:58.798510 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor/references/decor.vue
--rwxr-xr-x   0        0        0       68 2023-09-18 16:29:02.330860 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor/stat.vue
--rwxr-xr-x   0        0        0      304 2023-12-16 03:54:22.787318 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor/statements/decor.js
--rwxr-xr-x   0        0        0      807 2023-12-16 03:54:15.119382 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor/statements/decor.vue
--rwxr-xr-x   0        0        0       77 2023-12-16 04:08:24.127308 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor/unmeasured_ingredients/fountain.js
--rwxr-xr-x   0        0        0      393 2023-12-16 04:10:08.207440 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor/unmeasured_ingredients/fountain.vue
--rwxr-xr-x   0        0        0     1663 2023-11-13 18:59:31.232825 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor/warnings.vue
--rwxr-xr-x   0        0        0       58 2023-11-09 22:29:37.646696 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor/zone.vue
--rwxr-xr-x   0        0        0     1663 2024-03-31 22:55:12.260954 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor.js
--rwxr-xr-x   0        0        0     4316 2024-05-13 04:23:06.535436 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor.vue
--rwxr-xr-x   0        0        0      934 2024-05-13 00:59:57.096565 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/methods/index.js
--rwxr-xr-x   0        0        0       69 2023-11-10 19:36:19.034821 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/variables/index.js
--rwxr-xr-x   0        0        0      188 2023-12-17 02:39:17.775516 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/not_found.vue
--rwxr-xr-x   0        0        0      146 2024-04-01 00:02:44.025380 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/regions.s.HTML
--rwxr-xr-x   0        0        0       62 2023-11-15 01:52:25.248899 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/staff/food/decor.vue
--rwxr-xr-x   0        0        0       40 2024-05-11 00:47:10.035262 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/staff/habitat/decor.vue
--rwxr-xr-x   0        0        0       69 2024-03-07 02:39:01.545825 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/staff/supplement/decor.vue
--rwxr-xr-x   0        0        0      137 2024-02-02 20:39:47.327551 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/status/DAC/region.js
--rwxr-xr-x   0        0        0      123 2024-02-02 20:40:09.375901 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/status/DAC/region.vue
--rwxr-xr-x   0        0        0      420 2023-12-16 01:38:10.714287 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/status/index/scenery.vue
--rwxr-xr-x   0        0        0      138 2024-02-02 20:36:54.688872 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/status/waterfall/region.js
--rwxr-xr-x   0        0        0      284 2024-02-02 20:24:03.258300 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/status/waterfall/region.vue
--rwxr-xr-x   0        0        0      401 2024-03-10 04:32:12.206055 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/workshop/scenery/region.js
--rwxr-xr-x   0        0        0      455 2024-03-10 04:32:42.525826 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/workshop/scenery/region.vue
--rwxr-xr-x   0        0        0      374 2023-12-16 01:26:20.040221 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/_example/_status/_example.status.js
--rwxr-xr-x   0        0        0       44 2024-02-02 20:31:12.955078 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/_example/_status/region.vue
--rwxr-xr-x   0        0        0       38 2023-12-16 01:24:25.483179 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/_example/example.vue
--rwxr-xr-x   0        0        0      402 2024-02-12 00:41:59.519874 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/_status_Se/region.vue
--rwxr-xr-x   0        0        0       52 2024-01-20 23:13:27.680787 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/alerts/decor.js
--rwxr-xr-x   0        0        0      300 2024-01-20 23:16:22.966890 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/alerts/decor.vue
--rwxr-xr-x   0        0        0     2109 2024-05-09 19:36:44.767476 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/browser_storage/component.vue
--rwxr-xr-x   0        0        0      365 2024-02-12 01:41:42.400514 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/button/_status/button.status.js
--rwxr-xr-x   0        0        0      772 2024-05-13 17:30:41.938573 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/button/decor.js
--rwxr-xr-x   0        0        0     1027 2024-05-13 21:20:48.464951 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/button/decor.vue
--rwxr-xr-x   0        0        0      365 2024-02-12 01:41:42.400514 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/button_3D/_status/button.status.js
--rwxr-xr-x   0        0        0     3177 2024-03-16 01:40:22.479063 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/button_3D/decor--.js
--rwxr-xr-x   0        0        0     1640 2024-05-12 21:48:37.116802 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/button_3D/decor--.vue
--rwxr-xr-x   0        0        0      716 2024-05-11 00:12:32.840898 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/button_3D/decor.js
--rwxr-xr-x   0        0        0      982 2024-05-12 21:48:30.780836 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/button_3D/decor.vue
--rwxr-xr-x   0        0        0      478 2024-05-10 22:58:52.960081 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/canvases/canvases.S.HTML
--rwxr-xr-x   0        0        0    89476 2024-05-13 00:59:57.064565 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/caution-sign/goodestSink-export.svg
--rwxr-xr-x   0        0        0    88829 2024-05-13 00:59:57.064565 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/caution-sign/scenery.vue
--rwxr-xr-x   0        0        0      654 2024-02-02 15:30:27.876924 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/change_indicator/indicators/spinner/indicator.js
--rwxr-xr-x   0        0        0     1421 2023-12-12 22:09:16.041899 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/change_indicator/indicators/spinner/indicator.vue
--rwxr-xr-x   0        0        0      341 2024-01-12 03:15:22.087200 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/change_indicator/scenery.js
--rwxr-xr-x   0        0        0     1775 2024-01-12 03:42:31.305006 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/change_indicator/scenery.vue
--rwxr-xr-x   0        0        0     2650 2024-02-02 20:38:35.056936 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/charts/composition_DAC/chart.js
--rwxr-xr-x   0        0        0      437 2024-02-02 20:38:42.538683 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/charts/composition_DAC/chart.vue
--rwxr-xr-x   0        0        0      262 2023-10-16 00:43:32.202900 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/charts/composition_DAC/methods/FIND_STRUCTURE.js
--rwxr-xr-x   0        0        0     6029 2023-11-09 01:36:29.097181 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/charts/composition_DAC/methods/PHYSICAL/index.js
--rwxr-xr-x   0        0        0     1802 2023-11-09 01:35:18.334938 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/charts/composition_DAC/methods/reinvigorate.js
--rwxr-xr-x   0        0        0     3390 2024-02-11 21:15:24.477394 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/charts/composition_waterfall/chart.js
--rwxr-xr-x   0        0        0      332 2024-05-09 19:36:44.855476 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/charts/composition_waterfall/chart.vue
--rwxr-xr-x   0        0        0      484 2023-08-25 23:43:27.103848 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/charts/composition_waterfall/data.js
--rwxr-xr-x   0        0        0      195 2023-12-11 23:36:26.510190 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/charts/pie/_status/pie.status.js
--rwxr-xr-x   0        0        0     1182 2024-02-11 19:38:54.408096 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/charts/pie/make/build/data.js
--rwxr-xr-x   0        0        0     1208 2024-02-11 19:41:21.790449 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/charts/pie/make/build/options.js
--rwxr-xr-x   0        0        0     1131 2023-12-12 04:00:52.936450 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/charts/pie/make/build/plugins.js
--rwxr-xr-x   0        0        0      660 2024-02-12 00:52:23.817062 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/charts/pie/make/index.js
--rwxr-xr-x   0        0        0      945 2024-02-11 23:52:07.861502 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/charts/pie/make/utilities/--find_value.js
--rwxr-xr-x   0        0        0      570 2024-02-11 19:34:33.475199 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/charts/pie/make/utilities/find_name.js
--rwxr-xr-x   0        0        0       55 2024-02-11 19:37:20.529181 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/charts/pie/model.Se.vue
--rwxr-xr-x   0        0        0     2827 2024-02-12 01:03:07.501975 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/charts/pie/veranda.js
--rwxr-xr-x   0        0        0      298 2023-12-12 01:13:33.273737 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/charts/pie/veranda.vue
--rwxr-xr-x   0        0        0     1180 2024-05-13 22:39:05.317211 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/checkbox/decor.js
--rwxr-xr-x   0        0        0     1372 2024-05-13 22:38:54.385324 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/checkbox/decor.vue
--rwxr-xr-x   0        0        0     1100 2024-02-12 01:03:31.757707 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/curtain/decor.js
--rwxr-xr-x   0        0        0     1095 2024-05-12 19:46:18.226920 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/curtain/decor.vue
--rwxr-xr-x   0        0        0      988 2024-02-11 19:09:26.348094 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/example/_status/decor.ST.js
--rwxr-xr-x   0        0        0      267 2023-10-29 02:14:14.575679 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/example/_status/palette.js
--rwxr-xr-x   0        0        0      383 2024-02-12 01:43:33.199389 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/example/decor.js
--rwxr-xr-x   0        0        0      235 2023-10-29 02:35:27.283997 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/example/decor.vue
--rwxr-xr-x   0        0        0      335 2024-02-12 00:39:43.917336 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/example_two/decor.vue
--rwxr-xr-x   0        0        0      711 2024-02-02 19:24:25.841602 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/exception/field.vue
--rwxr-xr-x   0        0        0     1135 2024-03-06 22:37:09.225730 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/flip/decor--.js
--rwxr-xr-x   0        0        0      329 2024-03-06 23:06:49.208941 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/flip/decor.js
--rwxr-xr-x   0        0        0     1270 2024-05-09 19:36:44.771476 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/flip/decor.vue
--rwxr-xr-x   0        0        0      213 2023-11-02 00:22:56.985169 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/focusable/decor.vue
--rwxr-xr-x   0        0        0      921 2024-03-06 23:58:15.605648 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/food_or_supp_summary/decor.js
--rwxr-xr-x   0        0        0     2064 2024-03-09 19:22:16.538125 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/food_or_supp_summary/decor.vue
--rwxr-xr-x   0        0        0        2 2024-02-18 23:29:05.402268 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/foundations/eagle/scene.js
--rwxr-xr-x   0        0        0     1473 2024-05-09 01:10:44.432492 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/foundations/eagle/scene.vue
--rwxr-xr-x   0        0        0      112 2024-02-12 00:38:00.794440 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/gesture/gesture.s.HTML
--rwxr-xr-x   0        0        0      791 2024-03-21 18:05:53.908624 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/goal/components/goal_amount.vue
--rwxr-xr-x   0        0        0       84 2024-03-12 19:53:20.149662 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/goal/components/include.vue
--rwxr-xr-x   0        0        0     1713 2024-03-14 23:56:32.550876 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/goal/decor.js
--rwxr-xr-x   0        0        0     3387 2024-03-15 00:06:57.047615 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/goal/decor.vue
--rwxr-xr-x   0        0        0     1799 2024-03-09 21:58:48.378771 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/goal/decor_1.vue
--rwxr-xr-x   0        0        0        0 2023-10-29 19:45:47.360285 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/hw_button/decor.js
--rwxr-xr-x   0        0        0      767 2024-05-10 23:57:45.139416 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/hw_button/decor.vue
--rwxr-xr-x   0        0        0      771 2024-05-10 23:53:11.467027 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/hw_button/decor_v1.vue
--rwxr-xr-x   0        0        0     1121 2024-05-13 22:25:07.653778 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/icons/book/field.vue
--rwxr-xr-x   0        0        0       67 2024-03-30 03:59:23.274857 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/icons/icons.S.HTML
--rwxr-xr-x   0        0        0        0 2023-11-01 23:46:29.107176 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/input/_status/decor.status.js
--rwxr-xr-x   0        0        0     1331 2024-01-15 22:18:55.662581 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/input/decor.js
--rwxr-xr-x   0        0        0     2461 2024-05-13 22:31:58.481608 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/input/decor.vue
--rwxr-xr-x   0        0        0      451 2024-02-11 23:57:56.457658 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/line/decor.vue
--rwxr-xr-x   0        0        0     1064 2024-05-14 00:04:16.069185 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/link/outer/decor.vue
--rwxr-xr-x   0        0        0     1596 2024-05-12 21:50:04.432303 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/lounge/decor.js
--rwxr-xr-x   0        0        0      693 2024-02-13 06:25:25.937282 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/lounge/decor.s.HTML
--rwxr-xr-x   0        0        0      291 2024-05-09 19:36:44.771476 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/lounge/decor.vue
--rwxr-xr-x   0        0        0    22053 2024-01-21 01:14:15.300256 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/mascot/craft.vue
--rwxr-xr-x   0        0        0    11002 2024-01-17 17:58:07.993655 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/mascot/craft_v1.vue
--rwxr-xr-x   0        0        0    11973 2024-01-17 17:46:49.047355 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/mascot/mascot-1.svg
--rwxr-xr-x   0        0        0   199059 2024-01-21 00:48:09.525250 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/mascot/mascot.svg
--rwxr-xr-x   0        0        0     3653 2023-12-20 18:33:55.488744 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/name/_assets/Rugged Vegan.svg
--rwxr-xr-x   0        0        0   523296 2024-05-13 00:59:57.032565 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/name/_assets/Vegan Lantern - Export.svg
--rwxr-xr-x   0        0        0   724519 2024-05-13 00:59:57.004566 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/name/_assets/goodest sloop - mural - v1.svg
--rwxr-xr-x   0        0        0   724643 2024-05-13 00:59:57.028566 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/name/_assets/goodest sloop - mural - v2.svg
--rwxr-xr-x   0        0        0   724823 2024-05-13 00:59:57.060565 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/name/_assets/goodest sloop - mural - v3.svg
--rwxr-xr-x   0        0        0   724891 2024-05-13 00:59:57.004566 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/name/mural.vue
--rwxr-xr-x   0        0        0    61548 2023-12-13 03:15:36.204804 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/name/mural_v1.vue
--rwxr-xr-x   0        0        0     3557 2024-01-15 21:06:50.292544 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/name/mural_v2.vue
--rwxr-xr-x   0        0        0     4104 2024-01-16 02:07:39.029898 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/name/mural_v3.vue
--rwxr-xr-x   0        0        0     3987 2024-02-02 05:33:49.728771 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/name/mural_v4.vue
--rwxr-xr-x   0        0        0   523241 2024-05-13 00:59:57.000566 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/name/mural_v5.vue
--rwxr-xr-x   0        0        0     2761 2023-12-16 18:51:32.031662 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nature_cautionary_ingredients/shack.js
--rwxr-xr-x   0        0        0     2233 2024-03-30 02:18:06.952972 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nature_cautionary_ingredients/shack.vue
--rwxr-xr-x   0        0        0       30 2024-02-11 19:32:07.085089 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nature_essentials_nutrients/model.vue
--rwxr-xr-x   0        0        0     2980 2024-03-30 02:07:54.200279 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nature_essentials_nutrients/shack.js
--rwxr-xr-x   0        0        0     3919 2024-03-30 02:18:12.832902 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nature_essentials_nutrients/shack.vue
--rwxr-xr-x   0        0        0       51 2023-12-16 01:51:11.241801 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nature_ingredients_table/_status/region.vue
--rwxr-xr-x   0        0        0      367 2024-03-30 00:57:37.706848 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nature_ingredients_table/components/mass.vue
--rwxr-xr-x   0        0        0      873 2024-03-30 03:42:25.810936 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nature_ingredients_table/components/name.vue
--rwxr-xr-x   0        0        0      360 2024-03-30 03:33:49.781346 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nature_ingredients_table/components/the_percent.vue
--rwxr-xr-x   0        0        0     2805 2024-05-13 22:08:50.078779 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nature_ingredients_table/fields/methods.js
--rwxr-xr-x   0        0        0     5724 2024-05-11 00:12:32.852898 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nature_ingredients_table/fields/methods_/prepare_columns.js
--rwxr-xr-x   0        0        0     1793 2024-03-30 03:23:07.753064 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nature_ingredients_table/fields/methods_/prepare_rows.js
--rwxr-xr-x   0        0        0     2131 2024-05-11 00:12:32.864898 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nature_ingredients_table/fountains.js
--rwxr-xr-x   0        0        0      346 2024-03-31 04:02:30.811735 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nature_ingredients_table/fountains.vue
--rwxr-xr-x   0        0        0       51 2023-12-16 01:51:11.241801 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nature_ingredients_table_v1/_status/region.vue
--rwxr-xr-x   0        0        0     3842 2024-05-11 00:12:32.868898 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nature_ingredients_table_v1/fountains.js
--rwxr-xr-x   0        0        0     3125 2024-03-26 02:31:39.534326 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nature_ingredients_table_v1/fountains.vue
--rwxr-xr-x   0        0        0      495 2024-05-09 19:36:44.863475 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nav_1/decor.js
--rwxr-xr-x   0        0        0     1550 2024-05-13 17:23:17.158703 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nav_1/decor.vue
--rwxr-xr-x   0        0        0      654 2024-02-12 01:42:45.279877 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nav_1/navs/mobile_top/field.js
--rwxr-xr-x   0        0        0      631 2024-01-21 03:51:57.002319 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nav_1/navs/mobile_top/field.vue
--rwxr-xr-x   0        0        0     1705 2024-05-10 22:52:19.472795 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nav_1/navs/top/field.js
--rwxr-xr-x   0        0        0     2402 2024-05-14 00:15:30.677767 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nav_1/navs/top/field.vue
--rwxr-xr-x   0        0        0      595 2024-05-09 19:36:44.767476 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nav_2/decor.js
--rwxr-xr-x   0        0        0     1175 2024-05-14 00:15:45.821534 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nav_2/decor.vue
--rwxr-xr-x   0        0        0     1009 2024-02-12 01:27:50.397664 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/navigation infrastructure/methods/awareness/keydown.js
--rwxr-xr-x   0        0        0      278 2024-02-12 01:25:04.639492 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/navigation infrastructure/methods/awareness/keys.s.HTML
--rwxr-xr-x   0        0        0      237 2024-02-12 01:28:10.421443 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/navigation infrastructure/methods/find_element_index.js
--rwxr-xr-x   0        0        0     1493 2024-02-12 01:28:47.309037 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/navigation infrastructure/methods/focus_land_mark.js
--rwxr-xr-x   0        0        0      237 2024-02-12 01:28:20.997327 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/navigation infrastructure/methods/index.js
--rwxr-xr-x   0        0        0       29 2023-11-26 17:48:20.457245 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/navigation infrastructure/notes/notes.html
--rwxr-xr-x   0        0        0      362 2023-11-10 01:55:44.853516 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/navigation infrastructure/priorities.s.HTML
--rwxr-xr-x   0        0        0      914 2024-03-18 23:29:59.338994 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/navigation infrastructure/structure.js
--rwxr-xr-x   0        0        0     1774 2024-03-18 23:32:06.137547 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/navigation infrastructure/structure.vue
--rwxr-xr-x   0        0        0        0 2023-10-29 19:36:27.733924 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/panel/decor.js
--rwxr-xr-x   0        0        0     1537 2024-05-11 00:10:56.545996 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/panel/decor.vue
--rwxr-xr-x   0        0        0       19 2024-02-02 19:21:05.508081 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/paragraph/scenery.js
--rwxr-xr-x   0        0        0      245 2024-02-02 19:22:31.236941 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/paragraph/scenery.vue
--rwxr-xr-x   0        0        0     2516 2024-03-07 00:24:06.697068 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/quantity_chooser/decor.js
--rwxr-xr-x   0        0        0      993 2024-03-21 23:12:03.846331 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/quantity_chooser/decor.vue
--rwxr-xr-x   0        0        0      197 2023-12-09 04:41:31.507002 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/router_link/_status/1.status.js
--rwxr-xr-x   0        0        0      934 2024-01-15 21:55:41.717670 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/router_link/decor.js
--rwxr-xr-x   0        0        0     1632 2024-05-13 21:30:16.487247 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/router_link/decor.vue
--rwxr-xr-x   0        0        0      223 2024-03-16 01:03:10.281823 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/scenery.s.HTML
--rwxr-xr-x   0        0        0     1010 2024-03-06 21:32:00.501591 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/select/decor.js
--rwxr-xr-x   0        0        0      590 2024-02-05 21:07:41.006147 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/select/decor.status.js
--rwxr-xr-x   0        0        0     1476 2024-05-13 22:19:54.176871 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/select/decor.vue
--rwxr-xr-x   0        0        0      331 2023-11-09 01:39:06.154492 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/select/show.vue
--rwxr-xr-x   0        0        0       76 2023-11-29 19:31:03.919410 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/service/error/scenery.vue
--rwxr-xr-x   0        0        0       57 2023-11-29 19:30:41.590672 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/service/not_found/scenery.vue
--rwxr-xr-x   0        0        0       78 2024-02-19 04:56:48.625281 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/slides/scenery.js
--rwxr-xr-x   0        0        0      288 2024-02-19 04:47:31.307536 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/slides/scenery.vue
--rwxr-xr-x   0        0        0     1281 2023-12-08 04:01:35.070938 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/struct_2/composition/decor.js
--rwxr-xr-x   0        0        0     1023 2023-11-18 05:08:17.333020 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/struct_2/composition/decor.vue
--rwxr-xr-x   0        0        0      823 2023-12-08 21:43:22.157591 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/struct_2/composition/furniture/mass_of_quantified_ingredients.vue
--rwxr-xr-x   0        0        0      404 2023-11-07 02:46:35.565079 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/struct_2/quantified_grove/decor/mass.vue
--rwxr-xr-x   0        0        0     2254 2024-03-30 19:18:20.305565 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/struct_2/quantified_grove/fields/methods.js
--rwxr-xr-x   0        0        0      609 2024-03-30 19:18:20.305565 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/struct_2/quantified_grove/table.js
--rwxr-xr-x   0        0        0     2953 2024-02-11 23:57:56.641656 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/struct_2/quantified_grove/table.vue
--rwxr-xr-x   0        0        0       72 2023-11-07 00:13:33.997933 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/table/decor.js
--rwxr-xr-x   0        0        0     2260 2024-03-14 22:09:35.613243 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/table/decor.vue
--rwxr-xr-x   0        0        0       96 2023-11-07 00:14:30.745330 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/table/status/check_1.se.js
--rwxr-xr-x   0        0        0        2 2024-03-14 21:55:36.298300 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/table/table.S.HTML
--rwxr-xr-x   0        0        0     1048 2024-05-14 00:05:03.588280 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/treasure/affiliates/decor.vue
--rwxr-xr-x   0        0        0     1512 2024-03-31 22:53:45.469882 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/treasure/goodness_certifications/money.vue
--rwxr-xr-x   0        0        0       15 2019-02-15 21:43:43.000000 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/.gitignore
--rwxr-xr-x   0        0        0     1078 2019-02-15 21:43:43.000000 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/LICENSE.md
--rwxr-xr-x   0        0        0     1097 2019-02-15 21:43:43.000000 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/README.md
--rwxr-xr-x   0        0        0      463 2019-02-15 21:43:43.000000 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/bower.json
--rwxr-xr-x   0        0        0     5389 2019-02-15 21:43:43.000000 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/index.html
--rwxr-xr-x   0        0        0     4712 2019-02-15 21:43:43.000000 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/site-assets/images/download-btn.png
--rwxr-xr-x   0        0        0     3733 2019-02-15 21:43:43.000000 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/site-assets/images/tweet-btn.png
--rwxr-xr-x   0        0        0     1347 2019-02-15 21:43:43.000000 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/svg-loaders/audio.svg
--rwxr-xr-x   0        0        0     1926 2019-02-15 21:43:43.000000 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/svg-loaders/ball-triangle.svg
--rwxr-xr-x   0        0        0     2319 2019-02-15 21:43:43.000000 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/svg-loaders/bars.svg
--rwxr-xr-x   0        0        0     1923 2019-02-15 21:43:43.000000 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/svg-loaders/circles.svg
--rwxr-xr-x   0        0        0     2048 2019-02-15 21:43:43.000000 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/svg-loaders/grid.svg
--rwxr-xr-x   0        0        0     1357 2019-02-15 21:43:43.000000 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/svg-loaders/hearts.svg
--rwxr-xr-x   0        0        0      694 2019-02-15 21:43:43.000000 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/svg-loaders/oval.svg
--rwxr-xr-x   0        0        0     1460 2019-02-15 21:43:43.000000 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/svg-loaders/puff.svg
--rwxr-xr-x   0        0        0     1784 2019-02-15 21:43:43.000000 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/svg-loaders/rings.svg
--rwxr-xr-x   0        0        0     2782 2019-02-15 21:43:43.000000 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/svg-loaders/spinning-circles.svg
--rwxr-xr-x   0        0        0     1309 2019-02-15 21:43:43.000000 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/svg-loaders/tail-spin.svg
--rwxr-xr-x   0        0        0     1510 2019-02-15 21:43:43.000000 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/svg-loaders/three-dots.svg
--rwxr-xr-x   0        0        0        1 2024-01-12 03:13:03.137742 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/scenery/action/drawing.svg
--rwxr-xr-x   0        0        0      655 2024-01-12 03:23:52.078508 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/scenery/action/scenery.js
--rwxr-xr-x   0        0        0    12705 2024-02-02 15:29:43.493436 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/scenery/action/scenery.vue
--rwxr-xr-x   0        0        0    12243 2024-01-12 03:25:38.748314 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/scenery/action/scenery_v1.vue
--rwxr-xr-x   0        0        0     1371 2024-02-11 23:56:32.126588 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/_research/observables.js
--rwxr-xr-x   0        0        0     1701 2024-03-07 00:24:06.801066 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/cart/_status/1.status.js
--rwxr-xr-x   0        0        0     1560 2024-03-07 00:24:06.949064 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/cart/_status/2.status.js
--rwxr-xr-x   0        0        0     1571 2024-03-07 00:24:07.045063 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/cart/_status/3.status.js
--rwxr-xr-x   0        0        0     1227 2024-03-07 00:24:07.125061 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/cart/_status/4_remove.status.js
--rwxr-xr-x   0        0        0       54 2024-01-20 22:13:05.511855 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/cart/cart.s.HTML
--rwxr-xr-x   0        0        0     2040 2024-03-21 18:09:41.617982 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/cart/index.js
--rwxr-xr-x   0        0        0     1607 2024-03-07 00:24:07.245059 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/cart/moves/change_quantity.js
--rwxr-xr-x   0        0        0      716 2024-03-07 00:24:07.353058 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/cart/moves/find_DSLD_ID.js
--rwxr-xr-x   0        0        0      713 2024-03-07 00:24:07.473056 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/cart/moves/find_FDC_ID.js
--rwxr-xr-x   0        0        0     1396 2024-03-07 00:24:07.629053 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/cart/moves/remove.js
--rwxr-xr-x   0        0        0      982 2023-12-09 03:11:02.006950 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/cart/utilities/retrieve_treasures.js
--rwxr-xr-x   0        0        0      913 2024-05-12 21:37:29.717752 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/connections/index.js
--rwxr-xr-x   0        0        0     3017 2024-05-13 02:33:46.495932 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/goals/index.js
--rwxr-xr-x   0        0        0     2205 2024-05-13 17:33:51.484372 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/homestead/index.js
--rwxr-xr-x   0        0        0        2 2023-10-29 23:43:15.460481 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/language/index.js
--rwxr-xr-x   0        0        0      926 2024-03-21 19:28:28.280880 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/layout/index.js
--rwxr-xr-x   0        0        0     2565 2024-03-21 18:22:13.668837 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/storage/index.js
--rwxr-xr-x   0        0        0     1071 2024-02-18 23:59:57.568976 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/terrain--/index.js
--rwxr-xr-x   0        0        0      589 2024-01-16 02:44:42.852499 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/terrain--/index.s.HTML
--rwxr-xr-x   0        0        0      659 2024-03-07 00:24:08.293043 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/theme/_status/1.status.js
--rwxr-xr-x   0        0        0     2707 2024-05-10 20:05:23.682936 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/theme/index.js
--rwxr-xr-x   0        0        0     4811 2024-05-13 22:55:49.447352 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/theme/rooms/palettes.js
--rwxr-xr-x   0        0        0      376 2024-03-15 05:44:08.142235 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/theme/theme.s.HTML
--rwxr-xr-x   0        0        0       79 2024-05-13 21:13:58.600905 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/warehouses.S.HTML
--rwxr-xr-x   0        0        0       75 2024-05-08 19:30:19.000000 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/tsconfig.json--
--rwxr-xr-x   0        0        0      363 2024-05-11 00:11:34.953558 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/vite.config.js
--rwxr-xr-x   0        0        0      556 2024-05-08 21:11:26.687514 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/vitest.config.js
--rwxr-xr-x   0        0        0   358624 2024-05-13 01:01:34.311552 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/bun.lockb
--rwxr-xr-x   0        0        0      521 2024-05-13 00:59:57.104565 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/find_symlinks.py
--rwxr-xr-x   0        0        0      420 2024-05-10 02:12:07.564248 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/package.json
--rwxr-xr-x   0        0        0     2729 2024-05-11 00:13:19.112372 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/shares/glamour/background_effects/particles/money.js
--rwxr-xr-x   0        0        0      327 2024-04-01 01:01:35.808375 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/shares/glamour/background_effects/particles/money.vue
--rwxr-xr-x   0        0        0      268 2024-04-01 00:27:00.389669 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/shares/glamour/background_effects/particles/worker.js
--rwxr-xr-x   0        0        0     2298 2024-03-18 23:20:10.765821 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/shares/glamour/button/glamour.js
--rwxr-xr-x   0        0        0     1534 2024-05-13 21:21:06.312775 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/shares/glamour/button/glamour.vue
--rwxr-xr-x   0        0        0       86 2024-03-16 01:19:46.112564 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/shares/glamour/glamour.S.HTML
--rwxr-xr-x   0        0        0      234 2024-03-29 19:54:30.932386 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/shares/glamour/table/_status/components/name.vue
--rwxr-xr-x   0        0        0     3028 2024-05-11 00:13:19.144372 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/shares/glamour/table/_status/status.js
--rwxr-xr-x   0        0        0      229 2024-03-29 19:39:01.732623 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/shares/glamour/table/_status/status.vue
--rwxr-xr-x   0        0        0      128 2024-03-25 21:46:30.379196 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/shares/glamour/table/components/string_data.vue
--rwxr-xr-x   0        0        0     3064 2024-05-11 00:14:20.847673 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/shares/glamour/table/decor.js
--rwxr-xr-x   0        0        0     3236 2024-03-31 04:06:25.301446 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/shares/glamour/table/decor.vue
--rwxr-xr-x   0        0        0      937 2024-05-11 00:13:19.156372 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/shares/glamour/table/sorting/as_float.js
--rwxr-xr-x   0        0        0      962 2024-03-25 21:01:57.256918 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/shares/glamour/table/table.S.HTML
--rwxr-xr-x   0        0        0      375 2024-05-08 19:30:19.000000 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/sharess/config-eslint/index.js
--rwxr-xr-x   0        0        0      306 2024-05-08 20:00:54.297170 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/sharess/config-eslint/package.json--
--rwxr-xr-x   0        0        0      548 2024-05-08 19:30:19.000000 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/sharess/config-typescript/base.json
--rwxr-xr-x   0        0        0      150 2024-05-08 20:00:54.297170 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/sharess/config-typescript/package.json--
--rwxr-xr-x   0        0        0      369 2024-05-08 19:30:19.000000 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/sharess/config-typescript/vite.json
--rwxr-xr-x   0        0        0      246 2024-05-08 19:30:19.000000 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/sharess/ui/.eslintrc.cjs
--rwxr-xr-x   0        0        0       87 2024-05-08 19:30:19.000000 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/sharess/ui/components/counter.ts
--rwxr-xr-x   0        0        0      138 2024-05-08 19:30:19.000000 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/sharess/ui/components/header.ts
--rwxr-xr-x   0        0        0      166 2024-05-08 19:30:19.000000 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/sharess/ui/index.ts
--rwxr-xr-x   0        0        0      418 2024-05-08 20:00:54.297170 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/sharess/ui/package.json--
--rwxr-xr-x   0        0        0      104 2024-05-08 19:30:19.000000 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/sharess/ui/tsconfig.json
--rwxr-xr-x   0        0        0      278 2024-05-08 19:30:19.000000 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/sharess/ui/utils/counter.ts
--rwxr-xr-x   0        0        0      236 2024-05-08 19:30:19.000000 goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/turbo.json
--rwxr-xr-x   0        0        0      151 2024-04-17 03:33:22.097283 goodest-1.2.1/venues/stages/goodest/besties/affiliates_Amazon/affiliates.s.HTML
--rwxr-xr-x   0        0        0      176 2024-04-27 17:39:04.201558 goodest-1.2.1/venues/stages/goodest/besties/besties.S.HTML
--rwxr-xr-x   0        0        0      596 2024-04-17 03:36:49.119045 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/deliveries/__pycache__/source.cpython-310.pyc
--rwxr-xr-x   0        0        0      738 2024-04-17 03:33:22.097283 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/deliveries/__pycache__/source.cpython-311.pyc
--rwxr-xr-x   0        0        0     1326 2024-05-13 00:59:57.252563 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/deliveries/one/__init__.py
--rwxr-xr-x   0        0        0     1606 2024-05-13 01:08:31.359266 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/deliveries/one/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2127 2024-04-17 03:33:22.097283 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/deliveries/one/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      776 2024-04-17 03:33:22.097283 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/deliveries/one/assertions/__pycache__/BRANDED.cpython-311.pyc
--rwxr-xr-x   0        0        0      450 2024-04-17 03:33:22.097283 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/deliveries/one/assertions/__pycache__/FOUNDATIONAL.cpython-311.pyc
--rwxr-xr-x   0        0        0      652 2024-05-13 01:08:31.359266 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/deliveries/one/assertions/__pycache__/branded.cpython-310.pyc
--rwxr-xr-x   0        0        0      778 2024-04-17 03:33:22.097283 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/deliveries/one/assertions/__pycache__/branded.cpython-311.pyc
--rwxr-xr-x   0        0        0      502 2024-05-13 01:08:31.359266 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/deliveries/one/assertions/__pycache__/foundational.cpython-310.pyc
--rwxr-xr-x   0        0        0      677 2024-04-17 03:33:22.097283 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/deliveries/one/assertions/__pycache__/foundational.cpython-311.pyc
--rwxr-xr-x   0        0        0      510 2024-05-13 00:59:57.252563 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/deliveries/one/assertions/branded.py
--rwxr-xr-x   0        0        0      264 2024-05-13 00:59:57.252563 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/deliveries/one/assertions/foundational.py
--rwxr-xr-x   0        0        0      470 2024-05-13 00:59:57.252563 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/deliveries/one/status/API_status_branded_1.py
--rwxr-xr-x   0        0        0      537 2024-05-13 00:59:57.252563 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/deliveries/one/status/API_status_foundational_1.py
--rwxr-xr-x   0        0        0      747 2024-05-13 01:14:34.865033 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/deliveries/one/status/__pycache__/API_status_branded_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      742 2024-05-13 01:14:34.877033 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/deliveries/one/status/__pycache__/API_status_foundational_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      370 2024-04-17 03:33:22.097283 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/deliveries/source.py
--rwxr-xr-x   0        0        0      945 2024-05-13 00:59:57.244563 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/examples/__init__.py
--rwxr-xr-x   0        0        0     1131 2024-05-13 01:11:04.434433 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/examples/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2082 2024-04-17 03:33:22.097283 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/examples/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      748 2024-05-13 01:11:04.278434 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/examples/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0    37079 2024-04-17 03:33:22.097283 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/examples/branded/Gardein_f'sh_2663758.JSON
--rwxr-xr-x   0        0        0    37079 2024-04-17 03:33:22.097283 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/examples/branded/Gardein_f'sh_2664238.JSON
--rwxr-xr-x   0        0        0     7242 2024-04-17 03:33:22.097283 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/examples/branded/beet_juice_2412474.JSON
--rwxr-xr-x   0        0        0     8522 2024-04-17 03:33:22.097283 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/examples/branded/beet_juice_2642759.JSON
--rwxr-xr-x   0        0        0    10678 2024-04-17 03:33:22.097283 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/examples/branded/goodest_pizza_2672996.JSON
--rwxr-xr-x   0        0        0    33964 2024-04-17 03:33:22.097283 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/examples/branded/impossible_beef_2664238.JSON
--rwxr-xr-x   0        0        0    17926 2024-04-17 03:33:22.097283 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/examples/branded/problems/impossible_2468423.JSON
--rwxr-xr-x   0        0        0      104 2024-04-17 03:33:22.097283 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/examples/branded/problems/problems.r.HTML
--rwxr-xr-x   0        0        0    10670 2024-04-17 03:33:22.097283 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/examples/branded/walnuts_1882785.JSON
--rwxr-xr-x   0        0        0   189146 2024-04-17 03:33:22.097283 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/examples/foundational/2346404_sweet_potatoes.JSON
--rwxr-xr-x   0        0        0      255 2024-04-17 03:33:22.097283 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/examples/mergers.r.HTML
--rwxr-xr-x   0        0        0       88 2024-04-17 03:33:22.097283 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/examples/priorities.r.HTML
--rwxr-xr-x   0        0        0      458 2024-05-13 00:59:57.244563 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/examples/status_1.py
--rwxr-xr-x   0        0        0     1220 2024-05-13 00:59:57.244563 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/food.s.HTML
--rwxr-xr-x   0        0        0     4590 2024-05-13 00:59:57.248563 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/__init__.py
--rwxr-xr-x   0        0        0     2463 2024-05-13 01:08:31.343266 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1752 2024-05-13 00:59:57.252563 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/__init__.py
--rwxr-xr-x   0        0        0     1202 2024-05-13 01:08:31.343266 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2050 2024-04-17 03:33:22.101283 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      571 2024-04-17 03:33:22.101283 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/__pycache__/assertions.cpython-310.pyc
--rwxr-xr-x   0        0        0     1065 2024-04-17 03:33:22.101283 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/__pycache__/assertions.cpython-311.pyc
--rwxr-xr-x   0        0        0     1417 2024-05-13 01:11:05.538426 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      599 2024-04-17 03:33:22.101283 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/assertions/__init__.py
--rwxr-xr-x   0        0        0      596 2024-04-17 03:36:50.207023 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/assertions/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     4182 2024-05-13 00:59:57.252563 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/__init__.py
--rwxr-xr-x   0        0        0     2990 2024-05-13 01:08:31.347266 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     5397 2024-04-17 03:33:22.101283 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1260 2024-05-13 01:11:04.626432 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/__pycache__/status_mass_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1066 2024-05-13 01:11:04.938430 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/__pycache__/status_volume_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      421 2024-04-17 03:33:22.101283 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/label_splitter/__init__.py
--rwxr-xr-x   0        0        0      563 2024-04-17 03:36:50.203023 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/label_splitter/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      946 2024-04-17 03:33:22.101283 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/label_splitter/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1344 2024-05-13 00:59:57.252563 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/status_mass_1.py
--rwxr-xr-x   0        0        0      978 2024-05-13 00:59:57.252563 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/status_volume_1.py
--rwxr-xr-x   0        0        0     1502 2024-05-13 00:59:57.252563 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/status_1.py
--rwxr-xr-x   0        0        0      581 2024-05-13 00:59:57.248563 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_ops/retrieve/API_status_found_1.py
--rwxr-xr-x   0        0        0      591 2024-05-13 00:59:57.248563 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_ops/retrieve/API_status_not_found_1.py
--rwxr-xr-x   0        0        0     2301 2024-05-13 00:59:57.248563 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_ops/retrieve/__init__.py
--rwxr-xr-x   0        0        0      745 2024-04-27 17:18:55.070676 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_ops/retrieve/__pycache__/API_status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      846 2024-05-13 01:14:34.865033 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_ops/retrieve/__pycache__/API_status_found_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      765 2024-05-13 01:14:34.881033 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_ops/retrieve/__pycache__/API_status_not_found_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     2141 2024-05-13 01:08:31.359266 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_ops/retrieve/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1426 2024-05-13 01:11:04.942430 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_status/__pycache__/status_1_description.cpython-310.pyc
--rwxr-xr-x   0        0        0     1835 2024-05-13 01:11:04.722431 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_status/__pycache__/status_2_measures.cpython-310.pyc
--rwxr-xr-x   0        0        0     1550 2024-05-13 01:11:04.942430 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_status/__pycache__/status_3_measured_ingredients.cpython-310.pyc
--rwxr-xr-x   0        0        0     1594 2024-04-25 01:35:26.781309 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_status/__pycache__/status_4_land_essentials.cpython-310.pyc
--rwxr-xr-x   0        0        0     1703 2024-05-13 01:11:05.806424 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_status/__pycache__/status_4_lands.cpython-310.pyc
--rwxr-xr-x   0        0        0     1166 2024-05-13 00:59:57.252563 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_status/status_1_description.py
--rwxr-xr-x   0        0        0     1874 2024-05-13 00:59:57.252563 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_status/status_2_measures.py
--rwxr-xr-x   0        0        0     2081 2024-05-13 00:59:57.252563 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_status/status_3_measured_ingredients.py
--rwxr-xr-x   0        0        0     1503 2024-05-13 00:59:57.252563 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_status/status_4_lands.py
--rwxr-xr-x   0        0        0     2087 2024-05-13 01:11:03.694437 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_status_v1/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1598 2024-05-13 01:11:04.946430 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_status_v1/__pycache__/status_2.cpython-310.pyc
--rwxr-xr-x   0        0        0     1112 2024-05-13 01:11:03.654437 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_status_v1/__pycache__/status_2412474.cpython-310.pyc
--rwxr-xr-x   0        0        0     1453 2024-05-13 01:11:05.070429 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_status_v1/__pycache__/status_3.cpython-310.pyc
--rwxr-xr-x   0        0        0     1215 2024-05-13 01:11:03.610437 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_status_v1/__pycache__/status_loop_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     2777 2024-05-13 00:59:57.244563 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_status_v1/status_1.py
--rwxr-xr-x   0        0        0     1625 2024-05-13 00:59:57.244563 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_status_v1/status_2.py
--rwxr-xr-x   0        0        0      718 2024-05-13 00:59:57.244563 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_status_v1/status_2412474.py
--rwxr-xr-x   0        0        0     1092 2024-05-13 00:59:57.244563 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_status_v1/status_3.py
--rwxr-xr-x   0        0        0      854 2024-05-13 00:59:57.244563 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_status_v1/status_loop_1.py
--rwxr-xr-x   0        0        0     2306 2024-05-13 00:59:57.248563 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/land/__init__.py
--rwxr-xr-x   0        0        0     2113 2024-05-13 01:08:31.355266 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/land/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      466 2024-04-17 03:33:22.101283 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/__init__.py
--rwxr-xr-x   0        0        0      568 2024-04-17 03:36:50.287021 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      957 2024-04-17 03:33:22.101283 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1172 2024-05-13 00:59:57.244563 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/_ops/for_each/__init__.py
--rwxr-xr-x   0        0        0      839 2024-05-13 01:08:31.351266 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/_ops/for_each/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1012 2024-04-17 03:33:22.105283 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/_ops/for_each/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      707 2024-05-13 00:59:57.244563 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/_ops/seek/__init__.py
--rwxr-xr-x   0        0        0      833 2024-05-13 01:08:31.351266 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/_ops/seek/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1272 2024-04-17 03:33:22.105283 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/_ops/seek/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1374 2024-05-13 01:11:04.294433 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/_ops/seek/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1072 2024-05-13 00:59:57.244563 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/_ops/seek/status_1.py
--rwxr-xr-x   0        0        0     1993 2024-05-13 01:11:04.946430 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/_status/__pycache__/status_mass_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1011 2024-05-13 01:11:05.630425 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/_status/__pycache__/status_volume_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     2089 2024-05-13 00:59:57.248563 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/_status/status_mass_1.py
--rwxr-xr-x   0        0        0      724 2024-05-13 00:59:57.248563 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/_status/status_volume_1.py
--rwxr-xr-x   0        0        0     1143 2024-04-17 03:33:22.105283 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured ingredients.S.HTML
--rwxr-xr-x   0        0        0     1427 2024-05-13 00:59:57.244563 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/__init__.py
--rwxr-xr-x   0        0        0     1121 2024-05-13 01:08:31.351266 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1591 2024-04-17 03:33:22.105283 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1675 2024-05-13 01:11:04.774431 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/_status/__pycache__/status_IU_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1517 2024-05-13 01:11:06.258422 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/_status/__pycache__/status_energy_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1615 2024-05-13 01:11:04.510432 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/_status/__pycache__/status_mass_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1776 2024-05-13 00:59:57.248563 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/_status/status_IU_1.py
--rwxr-xr-x   0        0        0     1912 2024-05-13 00:59:57.248563 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/_status/status_energy_1.py
--rwxr-xr-x   0        0        0     1616 2024-05-13 00:59:57.248563 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/_status/status_mass_1.py
--rwxr-xr-x   0        0        0     1726 2024-05-13 00:59:57.244563 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/__init__.py
--rwxr-xr-x   0        0        0     1442 2024-05-13 01:08:31.351266 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     3142 2024-04-17 03:33:22.105283 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1240 2024-05-13 00:59:57.244563 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/biological_activity/__init__.py
--rwxr-xr-x   0        0        0     1259 2024-05-13 01:08:31.351266 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/biological_activity/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1831 2024-04-17 03:33:22.105283 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/biological_activity/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1572 2024-05-13 00:59:57.248563 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/energy/__init__.py
--rwxr-xr-x   0        0        0     1281 2024-05-13 01:08:31.351266 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/energy/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1791 2024-04-17 03:33:22.105283 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/energy/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1497 2024-05-13 00:59:57.248563 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/mass/__init__.py
--rwxr-xr-x   0        0        0     1458 2024-05-13 01:08:31.351266 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/mass/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1842 2024-04-17 03:33:22.105283 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/mass/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      706 2024-04-17 03:36:50.291021 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/__pycache__/food_nutrient.cpython-310.pyc
--rwxr-xr-x   0        0        0     1040 2024-04-17 03:33:22.105283 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/__pycache__/food_nutrient.cpython-311.pyc
--rwxr-xr-x   0        0        0     1899 2024-04-17 03:33:22.105283 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/__pycache__/food_nutrient_calculator.cpython-311.pyc
--rwxr-xr-x   0        0        0      651 2024-04-17 03:33:22.105283 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/__pycache__/label_nutrient.cpython-310.pyc
--rwxr-xr-x   0        0        0      845 2024-04-17 03:33:22.105283 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/__pycache__/label_nutrient.cpython-311.pyc
--rwxr-xr-x   0        0        0      849 2024-04-17 03:33:22.105283 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/__pycache__/label_nutrient_calculator.cpython-311.pyc
--rwxr-xr-x   0        0        0      636 2024-04-17 03:33:22.105283 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/food_nutrient.py
--rwxr-xr-x   0        0        0      483 2024-04-17 03:33:22.105283 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/label_nutrient.py
--rwxr-xr-x   0        0        0      503 2024-04-17 03:33:22.105283 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/ingredient.r.HTML
--rwxr-xr-x   0        0        0      706 2024-04-17 03:33:22.105283 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/ingredient_prototype_1.r.HTML
--rwxr-xr-x   0        0        0     3867 2024-05-13 00:59:57.248563 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measures/form/__init__.py
--rwxr-xr-x   0        0        0     2398 2024-05-13 01:08:31.347266 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measures/form/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     4016 2024-04-17 03:33:22.105283 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measures/form/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1370 2024-05-13 01:11:06.290421 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measures/form/__pycache__/status_mass_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1401 2024-05-13 01:11:04.946430 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measures/form/__pycache__/status_volume_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      110 2024-04-17 03:33:22.105283 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measures/form/form.S.HTML
--rwxr-xr-x   0        0        0     1238 2024-05-13 00:59:57.248563 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measures/form/status_mass_1.py
--rwxr-xr-x   0        0        0     1181 2024-05-13 00:59:57.248563 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measures/form/status_volume_1.py
--rwxr-xr-x   0        0        0      394 2024-05-13 00:59:57.252563 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/nature_v2.S.HTML
--rwxr-xr-x   0        0        0      102 2024-04-17 03:33:22.105283 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/unmeasured_ingredients/__init__.py
--rwxr-xr-x   0        0        0      338 2024-04-17 03:36:50.291021 goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/unmeasured_ingredients/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1046 2024-05-13 00:59:57.256563 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/NIH.s.HTML
--rwxr-xr-x   0        0        0      536 2024-04-27 16:55:09.193236 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/deliveries/__pycache__/source.cpython-310.pyc
--rwxr-xr-x   0        0        0      670 2024-04-17 03:33:22.105283 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/deliveries/__pycache__/source.cpython-311.pyc
--rwxr-xr-x   0        0        0     1090 2024-05-13 00:59:57.292563 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/deliveries/one/__init__.py
--rwxr-xr-x   0        0        0     1201 2024-05-13 01:08:31.367266 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/deliveries/one/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1889 2024-04-17 03:33:22.105283 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/deliveries/one/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      815 2024-04-27 16:55:09.193236 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/deliveries/one/__pycache__/assertions.cpython-310.pyc
--rwxr-xr-x   0        0        0     1399 2024-04-17 03:33:22.105283 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/deliveries/one/__pycache__/assertions.cpython-311.pyc
--rwxr-xr-x   0        0        0     1087 2024-04-17 03:33:22.105283 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/deliveries/one/assertions.py
--rwxr-xr-x   0        0        0      438 2024-05-13 00:59:57.292563 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/deliveries/one/status/API_status_1.py
--rwxr-xr-x   0        0        0      706 2024-05-13 01:14:34.849033 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/deliveries/one/status/__pycache__/API_status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      316 2024-04-17 03:33:22.105283 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/deliveries/source.py
--rwxr-xr-x   0        0        0      848 2024-05-13 00:59:57.252563 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/examples/__init__.py
--rwxr-xr-x   0        0        0     1044 2024-05-13 01:11:09.506402 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/examples/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1918 2024-04-17 03:33:22.105283 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/examples/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0    44599 2024-05-13 00:59:57.256563 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/examples/coated tablets/multivitamin_276336.JSON
--rwxr-xr-x   0        0        0     7111 2024-05-13 00:59:57.256563 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/examples/goodest_capsules/probiotics_248267.JSON
--rwxr-xr-x   0        0        0    22180 2024-04-17 03:33:22.105283 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/examples/other/chia_seeds_214893.JSON
--rwxr-xr-x   0        0        0     6430 2024-04-17 03:33:22.105283 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/examples/powder/mane_270619.JSON
--rwxr-xr-x   0        0        0    72604 2024-05-13 00:59:57.252563 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/examples/powder/nutritional_shake_220884.JSON
--rwxr-xr-x   0        0        0    57378 2024-04-17 03:33:22.105283 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/examples/powder packets/multivitamin_246811.JSON
--rwxr-xr-x   0        0        0    22710 2024-04-17 03:33:22.105283 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/examples/tablets/calcium_261967.JSON
--rwxr-xr-x   0        0        0    43729 2024-05-13 00:59:57.252563 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/examples/tablets/multivitamin_249664.JSON
--rwxr-xr-x   0        0        0     4057 2024-05-13 00:59:57.264563 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/__init__.py
--rwxr-xr-x   0        0        0     2766 2024-05-13 01:08:31.359266 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      271 2024-04-17 03:36:50.963008 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_interpret/ingredientRows/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      383 2024-04-17 03:33:22.105283 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_interpret/ingredientRows/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1151 2024-05-13 00:59:57.284563 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_interpret/ingredientRows/for_each/__init__.py
--rwxr-xr-x   0        0        0      912 2024-05-13 01:08:31.363266 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_interpret/ingredientRows/for_each/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1201 2024-04-17 03:33:22.105283 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_interpret/ingredientRows/for_each/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1237 2024-05-13 01:11:05.510426 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_interpret/ingredientRows/for_each/__pycache__/status_powder_packets_246811.cpython-310.pyc
--rwxr-xr-x   0        0        0      935 2024-05-13 00:59:57.284563 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_interpret/ingredientRows/for_each/status_powder_packets_246811.py
--rwxr-xr-x   0        0        0       56 2024-04-17 03:33:22.109283 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_interpret/servingSizeUnit/__init__.py
--rwxr-xr-x   0        0        0     2278 2024-05-13 00:59:57.264563 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_ops/retrieve/__init__.py
--rwxr-xr-x   0        0        0     2047 2024-05-13 01:08:31.367266 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_ops/retrieve/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1418 2024-05-13 01:11:05.662425 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/__pycache__/status_1_info.cpython-310.pyc
--rwxr-xr-x   0        0        0     1426 2024-05-13 01:11:05.070429 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/__pycache__/status_2_form.cpython-310.pyc
--rwxr-xr-x   0        0        0     1837 2024-05-13 01:11:05.794424 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/__pycache__/status_3_measured_ingredients.cpython-310.pyc
--rwxr-xr-x   0        0        0     1236 2024-04-25 18:59:21.733410 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/__pycache__/status_4_essential_nutrients.cpython-310.pyc
--rwxr-xr-x   0        0        0     1484 2024-05-13 01:11:06.638419 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/__pycache__/status_4_unmeasured_ingredients.cpython-310.pyc
--rwxr-xr-x   0        0        0     1673 2024-05-13 01:11:05.710425 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/__pycache__/status_5_essential_nutrients.cpython-310.pyc
--rwxr-xr-x   0        0        0     1601 2024-05-13 01:11:06.410421 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/__pycache__/status_6_cautionary_ingredients.cpython-310.pyc
--rwxr-xr-x   0        0        0    28721 2024-05-14 01:27:56.970346 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/mane_270619_nature.JSON
--rwxr-xr-x   0        0        0   124537 2024-05-14 01:27:57.074345 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/multivitamin_249664.JSON
--rwxr-xr-x   0        0        0     1040 2024-05-13 00:59:57.288563 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/status_1_info.py
--rwxr-xr-x   0        0        0     1050 2024-05-13 00:59:57.288563 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/status_2_form.py
--rwxr-xr-x   0        0        0     1620 2024-05-13 00:59:57.288563 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/status_3_measured_ingredients.py
--rwxr-xr-x   0        0        0     1071 2024-05-13 00:59:57.288563 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/status_4_unmeasured_ingredients.py
--rwxr-xr-x   0        0        0     1279 2024-05-13 00:59:57.288563 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/status_5_essential_nutrients.py
--rwxr-xr-x   0        0        0     1172 2024-05-13 00:59:57.288563 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/status_6_cautionary_ingredients.py
--rwxr-xr-x   0        0        0      836 2024-05-13 01:11:05.882424 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_status_v1/_loop/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      742 2024-05-13 00:59:57.260563 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_status_v1/_loop/status_1.py
--rwxr-xr-x   0        0        0     1751 2024-05-13 01:11:05.318427 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_status_v1/coated_tablets/__pycache__/status_multivitamin_276336.cpython-310.pyc
--rwxr-xr-x   0        0        0     1563 2024-05-13 00:59:57.260563 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_status_v1/coated_tablets/status_multivitamin_276336.py
--rwxr-xr-x   0        0        0   136807 2024-05-14 01:27:56.506351 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_status_v1/coated_tablets/status_multivitamin_276336_nature.JSON
--rwxr-xr-x   0        0        0     1217 2024-05-13 01:11:05.138428 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_status_v1/other/__pycache__/status_chia_seeds_214893.cpython-310.pyc
--rwxr-xr-x   0        0        0    82230 2024-05-14 01:27:56.994346 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_status_v1/other/chia_seeds_214893_nature.JSON
--rwxr-xr-x   0        0        0      767 2024-05-13 00:59:57.260563 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_status_v1/other/status_chia_seeds_214893.py
--rwxr-xr-x   0        0        0     1180 2024-05-13 01:11:05.570426 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_status_v1/powder/__pycache__/status_mane_270619.cpython-310.pyc
--rwxr-xr-x   0        0        0    28721 2024-05-14 01:27:56.530351 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_status_v1/powder/mane_270619_nature.JSON
--rwxr-xr-x   0        0        0      740 2024-05-13 00:59:57.256563 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_status_v1/powder/status_mane_270619.py
--rwxr-xr-x   0        0        0      568 2024-04-25 04:11:27.433921 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      672 2024-04-17 03:33:22.109283 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      667 2024-05-13 00:59:57.284563 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/amount/__init__.py
--rwxr-xr-x   0        0        0      866 2024-05-13 01:08:31.363266 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/amount/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1333 2024-04-17 03:33:22.109283 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/amount/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      773 2024-05-13 01:11:05.642425 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/amount/__pycache__/status_other_214893.cpython-310.pyc
--rwxr-xr-x   0        0        0      514 2024-05-13 00:59:57.284563 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/amount/status_other_214893.py
--rwxr-xr-x   0        0        0      512 2024-04-17 03:33:22.109283 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/form.S.HTML
--rwxr-xr-x   0        0        0     3998 2024-05-13 00:59:57.284563 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/serving_size/amount/__init__.py
--rwxr-xr-x   0        0        0     2359 2024-05-13 01:08:31.363266 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/serving_size/amount/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-04-17 03:33:22.109283 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/serving_size/amount/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      179 2024-04-17 03:36:51.818991 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/serving_size/amount/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1579 2024-05-13 01:11:06.066423 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/serving_size/amount/__pycache__/status_246811.cpython-310.pyc
--rwxr-xr-x   0        0        0     1556 2024-05-13 01:11:05.866424 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/serving_size/amount/__pycache__/status_276336.cpython-310.pyc
--rwxr-xr-x   0        0        0     1785 2024-05-13 00:59:57.284563 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/serving_size/amount/status_246811.py
--rwxr-xr-x   0        0        0     1672 2024-05-13 00:59:57.284563 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/serving_size/amount/status_276336.py
--rwxr-xr-x   0        0        0     3227 2024-05-13 00:59:57.284563 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/__init__.py
--rwxr-xr-x   0        0        0     2679 2024-05-13 01:08:31.359266 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-04-17 03:33:22.109283 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1203 2024-05-13 01:11:06.354421 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/__pycache__/status_coated_tablet_276336.cpython-310.pyc
--rwxr-xr-x   0        0        0      991 2024-05-13 01:11:06.470420 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/__pycache__/status_goodest_capsule_248267.cpython-310.pyc
--rwxr-xr-x   0        0        0     1004 2024-05-13 01:11:06.042423 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/__pycache__/status_gram_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1010 2024-05-13 01:11:05.230428 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/__pycache__/status_powder_220884.cpython-310.pyc
--rwxr-xr-x   0        0        0     1043 2024-05-13 01:11:06.042423 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/__pycache__/status_powder_270619.cpython-310.pyc
--rwxr-xr-x   0        0        0     1426 2024-05-13 01:11:05.450426 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/__pycache__/status_powder_packets_246811.cpython-310.pyc
--rwxr-xr-x   0        0        0      953 2024-05-13 01:11:04.994429 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/__pycache__/status_tablet_261967.cpython-310.pyc
--rwxr-xr-x   0        0        0      933 2024-05-13 00:59:57.284563 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/status_coated_tablet_276336.py
--rwxr-xr-x   0        0        0      731 2024-05-13 00:59:57.284563 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/status_goodest_capsule_248267.py
--rwxr-xr-x   0        0        0      818 2024-05-13 00:59:57.264563 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/status_gram_1.py
--rwxr-xr-x   0        0        0      822 2024-05-13 00:59:57.284563 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/status_powder_220884.py
--rwxr-xr-x   0        0        0      895 2024-05-13 00:59:57.284563 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/status_powder_270619.py
--rwxr-xr-x   0        0        0     1337 2024-05-13 00:59:57.284563 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/status_powder_packets_246811.py
--rwxr-xr-x   0        0        0      705 2024-05-13 00:59:57.284563 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/status_tablet_261967.py
--rwxr-xr-x   0        0        0     1971 2024-05-13 00:59:57.264563 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/land/__init__.py
--rwxr-xr-x   0        0        0     2058 2024-05-13 01:08:31.367266 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/land/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1703 2024-05-13 00:59:57.260563 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/__init__.py
--rwxr-xr-x   0        0        0     1944 2024-05-13 01:08:31.363266 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2911 2024-04-17 03:33:22.109283 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1121 2024-05-13 00:59:57.260563 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek/__init__.py
--rwxr-xr-x   0        0        0     1085 2024-05-13 01:08:31.363266 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1442 2024-04-17 03:33:22.109283 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      967 2024-05-13 01:11:06.018423 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      666 2024-05-13 00:59:57.260563 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek/status_1.py
--rwxr-xr-x   0        0        0      591 2024-05-13 00:59:57.260563 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek_name/__init__.py
--rwxr-xr-x   0        0        0      998 2024-05-13 01:11:09.506402 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek_name/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1171 2024-04-17 03:33:22.113283 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek_name/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1084 2024-05-13 01:11:05.850424 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/_status/__pycache__/status_chia_seeds_214893.cpython-310.pyc
--rwxr-xr-x   0        0        0      807 2024-05-13 00:59:57.264563 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/_status/status_chia_seeds_214893.py
--rwxr-xr-x   0        0        0     4671 2024-05-13 00:59:57.264563 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/measured_ingredient/__init__.py
--rwxr-xr-x   0        0        0     2809 2024-05-13 01:08:31.363266 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/measured_ingredient/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     4500 2024-04-17 03:33:22.109283 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/measured_ingredient/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1636 2024-05-13 01:11:06.542420 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/measured_ingredient/_status/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1731 2024-05-13 00:59:57.264563 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/measured_ingredient/_status/status_1.py
--rwxr-xr-x   0        0        0     1514 2024-04-17 03:33:22.109283 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/measured_ingredient/measured_ingredient.S.HTML
--rwxr-xr-x   0        0        0      561 2024-04-17 03:33:22.109283 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/measured_ingredients.S.HTML
--rwxr-xr-x   0        0        0        3 2024-04-25 01:50:49.197454 goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/natures_v2.S.HTML
--rwxr-xr-x   0        0        0       87 2024-04-27 20:03:02.828977 goodest-1.2.1/venues/stages/goodest/goals/goals.S.HTML
--rwxr-xr-x   0        0        0     8906 2024-05-13 00:59:57.244563 goodest-1.2.1/venues/stages/goodest/goals/umuntu/FDA.py
--rwxr-xr-x   0        0        0     9794 2024-03-09 19:44:16.627477 goodest-1.2.1/venues/stages/goodest/goals/umuntu/FDA_v1.py
--rwxr-xr-x   0        0        0     4193 2024-03-10 18:32:48.701726 goodest-1.2.1/venues/stages/goodest/goals/umuntu/FDA_v2.py
--rwxr-xr-x   0        0        0     7523 2024-03-12 19:40:02.502146 goodest-1.2.1/venues/stages/goodest/goals/umuntu/FDA_v3.py
--rwxr-xr-x   0        0        0     4343 2024-05-13 02:40:08.095827 goodest-1.2.1/venues/stages/goodest/goals/umuntu/__pycache__/FDA.cpython-310.pyc
--rwxr-xr-x   0        0        0     3847 2024-03-14 19:34:32.350499 goodest-1.2.1/venues/stages/goodest/goals/umuntu/__pycache__/FDA_v3.cpython-310.pyc
--rwxr-xr-x   0        0        0       71 2024-04-27 16:41:36.022921 goodest-1.2.1/venues/stages/goodest/goals/umuntu/_journal/Carbohydrates.s.HTML
--rwxr-xr-x   0        0        0       61 2024-04-27 16:41:31.750949 goodest-1.2.1/venues/stages/goodest/goals/umuntu/_journal/Fat.s.HTML
--rwxr-xr-x   0        0        0       64 2024-04-27 16:41:27.998973 goodest-1.2.1/venues/stages/goodest/goals/umuntu/_journal/Lipids.s.HTML
--rwxr-xr-x   0        0        0      145 2024-04-27 16:41:20.183024 goodest-1.2.1/venues/stages/goodest/goals/umuntu/_journal/Protein.s.HTML
--rwxr-xr-x   0        0        0       16 2024-01-31 21:52:02.234756 goodest-1.2.1/venues/stages/goodest/goals/umuntu/_journal/Vitamin A.s.HTML
--rwxr-xr-x   0        0        0        0 2024-01-31 21:52:25.962491 goodest-1.2.1/venues/stages/goodest/goals/umuntu/_journal/Vitamin B.s.HTML
--rwxr-xr-x   0        0        0       68 2024-04-27 16:40:48.275230 goodest-1.2.1/venues/stages/goodest/goals/umuntu/_journal/Vitamin C.s.HTML
--rwxr-xr-x   0        0        0       65 2024-04-27 16:40:44.111256 goodest-1.2.1/venues/stages/goodest/goals/umuntu/_journal/Vitamin D.s.HTML
--rwxr-xr-x   0        0        0      423 2024-04-27 16:42:29.518570 goodest-1.2.1/venues/stages/goodest/goals/umuntu/_journal/Vitamin E.s.HTML
--rwxr-xr-x   0        0        0      553 2024-04-28 02:16:08.201921 goodest-1.2.1/venues/stages/goodest/goals/umuntu/_ops/__pycache__/retrieve.cpython-310.pyc
--rwxr-xr-x   0        0        0      358 2024-05-13 00:59:57.244563 goodest-1.2.1/venues/stages/goodest/goals/umuntu/_ops/retrieve.py
--rwxr-xr-x   0        0        0        3 2024-03-10 18:23:03.506534 goodest-1.2.1/venues/stages/goodest/goals/umuntu/parse_FDA.proc.py
--rwxr-xr-x   0        0        0      488 2024-04-28 00:30:07.297621 goodest-1.2.1/venues/stages/goodest/goals/umuntu/umuntu.S.HTML
--rwxr-xr-x   0        0        0       14 2024-04-17 03:33:22.129283 goodest-1.2.1/venues/stages/goodest/goodest -- emojis.S.HTML
--rwxr-xr-x   0        0        0     4710 2024-05-13 00:59:01.377145 goodest-1.2.1/venues/stages/goodest/goodest.S.HTML
--rwxr-xr-x   0        0        0      632 2024-04-17 03:33:22.129283 goodest-1.2.1/venues/stages/goodest/goodest.css
--rwxr-xr-x   0        0        0      805 2024-05-13 01:11:03.378439 goodest-1.2.1/venues/stages/goodest/measures/_interpret/__pycache__/status_unit_kind.cpython-310.pyc
--rwxr-xr-x   0        0        0     1473 2024-05-13 01:08:31.347266 goodest-1.2.1/venues/stages/goodest/measures/_interpret/__pycache__/unit_kind.cpython-310.pyc
--rwxr-xr-x   0        0        0     2547 2024-04-17 03:33:22.113283 goodest-1.2.1/venues/stages/goodest/measures/_interpret/__pycache__/unit_kind.cpython-311.pyc
--rwxr-xr-x   0        0        0       61 2024-04-17 03:33:22.113283 goodest-1.2.1/venues/stages/goodest/measures/_interpret/interpret.S.HTML
--rwxr-xr-x   0        0        0      669 2024-05-13 00:59:01.385145 goodest-1.2.1/venues/stages/goodest/measures/_interpret/status_unit_kind.py
--rwxr-xr-x   0        0        0     1677 2024-05-13 00:59:01.385145 goodest-1.2.1/venues/stages/goodest/measures/_interpret/unit_kind.py
--rwxr-xr-x   0        0        0        0 2024-04-17 03:33:22.113283 goodest-1.2.1/venues/stages/goodest/measures/biological_activity/__init__.py
--rwxr-xr-x   0        0        0       59 2024-04-17 03:33:22.113283 goodest-1.2.1/venues/stages/goodest/measures/electric_current/electric_current.S.HTML
--rwxr-xr-x   0        0        0     1355 2024-05-04 16:59:01.497380 goodest-1.2.1/venues/stages/goodest/measures/energy/energy.r.HTML
--rwxr-xr-x   0        0        0     1173 2024-05-13 00:59:01.385145 goodest-1.2.1/venues/stages/goodest/measures/energy/swap/__init__.py
--rwxr-xr-x   0        0        0     1020 2024-05-13 01:08:31.351266 goodest-1.2.1/venues/stages/goodest/measures/energy/swap/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1761 2024-04-17 03:33:22.113283 goodest-1.2.1/venues/stages/goodest/measures/energy/swap/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      624 2024-05-13 01:11:03.798436 goodest-1.2.1/venues/stages/goodest/measures/energy/swap/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      385 2024-05-13 00:59:01.385145 goodest-1.2.1/venues/stages/goodest/measures/energy/swap/status_1.py
--rwxr-xr-x   0        0        0       71 2024-04-17 03:33:22.113283 goodest-1.2.1/venues/stages/goodest/measures/length/length.r.HTML
--rwxr-xr-x   0        0        0       95 2024-04-17 03:33:22.113283 goodest-1.2.1/venues/stages/goodest/measures/mass/e_note.py
--rwxr-xr-x   0        0        0       12 2024-04-17 03:33:22.113283 goodest-1.2.1/venues/stages/goodest/measures/mass/mass.r.html
--rwxr-xr-x   0        0        0     2328 2024-05-13 00:59:01.385145 goodest-1.2.1/venues/stages/goodest/measures/mass/swap/__init__.py
--rwxr-xr-x   0        0        0     1728 2024-05-13 01:08:31.347266 goodest-1.2.1/venues/stages/goodest/measures/mass/swap/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     3229 2024-04-17 03:33:22.113283 goodest-1.2.1/venues/stages/goodest/measures/mass/swap/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1147 2024-05-13 01:11:04.230434 goodest-1.2.1/venues/stages/goodest/measures/mass/swap/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1152 2024-05-13 00:59:01.385145 goodest-1.2.1/venues/stages/goodest/measures/mass/swap/status_1.py
--rwxr-xr-x   0        0        0     2419 2024-04-17 03:33:22.113283 goodest-1.2.1/venues/stages/goodest/measures/mass/system international.r.html
--rwxr-xr-x   0        0        0      768 2024-04-17 03:33:22.113283 goodest-1.2.1/venues/stages/goodest/measures/mass/us customary.r.html
--rwxr-xr-x   0        0        0      522 2024-05-13 00:59:01.385145 goodest-1.2.1/venues/stages/goodest/measures/mass_equivalents/is_an_equivalent/__init__.py
--rwxr-xr-x   0        0        0      636 2024-05-13 01:11:08.834406 goodest-1.2.1/venues/stages/goodest/measures/mass_equivalents/is_an_equivalent/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      945 2024-04-17 03:33:22.113283 goodest-1.2.1/venues/stages/goodest/measures/mass_equivalents/is_an_equivalent/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      611 2024-05-13 01:11:04.754431 goodest-1.2.1/venues/stages/goodest/measures/mass_equivalents/is_an_equivalent/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      341 2024-05-13 00:59:01.385145 goodest-1.2.1/venues/stages/goodest/measures/mass_equivalents/is_an_equivalent/status_1.py
--rwxr-xr-x   0        0        0      861 2024-04-17 03:33:22.113283 goodest-1.2.1/venues/stages/goodest/measures/mass_equivalents/jargon.r.HTML
--rwxr-xr-x   0        0        0     2242 2024-04-17 03:33:22.113283 goodest-1.2.1/venues/stages/goodest/measures/mass_equivalents/mass equivalents.r.HTML
--rwxr-xr-x   0        0        0     2430 2024-05-13 00:59:01.381145 goodest-1.2.1/venues/stages/goodest/measures/number/decimal/reduce/__init__.py
--rwxr-xr-x   0        0        0     1580 2024-05-13 01:08:31.347266 goodest-1.2.1/venues/stages/goodest/measures/number/decimal/reduce/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     3068 2024-04-17 03:33:22.113283 goodest-1.2.1/venues/stages/goodest/measures/number/decimal/reduce/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1144 2024-05-13 01:11:04.222434 goodest-1.2.1/venues/stages/goodest/measures/number/decimal/reduce/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      851 2024-05-13 01:11:03.354439 goodest-1.2.1/venues/stages/goodest/measures/number/decimal/reduce/__pycache__/status_2.cpython-310.pyc
--rwxr-xr-x   0        0        0      919 2024-05-13 01:11:03.250440 goodest-1.2.1/venues/stages/goodest/measures/number/decimal/reduce/__pycache__/status_3.cpython-310.pyc
--rwxr-xr-x   0        0        0      651 2024-05-13 01:11:04.102435 goodest-1.2.1/venues/stages/goodest/measures/number/decimal/reduce/__pycache__/status_sci_note_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1427 2024-05-13 00:59:01.381145 goodest-1.2.1/venues/stages/goodest/measures/number/decimal/reduce/status_1.py
--rwxr-xr-x   0        0        0      900 2024-05-13 00:59:01.381145 goodest-1.2.1/venues/stages/goodest/measures/number/decimal/reduce/status_2.py
--rwxr-xr-x   0        0        0     1114 2024-05-13 00:59:01.381145 goodest-1.2.1/venues/stages/goodest/measures/number/decimal/reduce/status_3.py
--rwxr-xr-x   0        0        0      469 2024-05-13 00:59:01.381145 goodest-1.2.1/venues/stages/goodest/measures/number/decimal/reduce/status_sci_note_1.py
--rwxr-xr-x   0        0        0      168 2024-04-17 03:33:22.113283 goodest-1.2.1/venues/stages/goodest/measures/number/fraction_point/fraction_point.s.HTML
--rwxr-xr-x   0        0        0      713 2024-05-13 01:11:03.514438 goodest-1.2.1/venues/stages/goodest/measures/number/integer/__pycache__/status_string_is_integer.cpython-310.pyc
--rwxr-xr-x   0        0        0      531 2024-05-13 01:08:31.363266 goodest-1.2.1/venues/stages/goodest/measures/number/integer/__pycache__/string_is_integer.cpython-310.pyc
--rwxr-xr-x   0        0        0      749 2024-04-17 03:33:22.113283 goodest-1.2.1/venues/stages/goodest/measures/number/integer/__pycache__/string_is_integer.cpython-311.pyc
--rwxr-xr-x   0        0        0      559 2024-05-13 00:59:01.381145 goodest-1.2.1/venues/stages/goodest/measures/number/integer/status_string_is_integer.py
--rwxr-xr-x   0        0        0      367 2024-05-13 00:59:01.381145 goodest-1.2.1/venues/stages/goodest/measures/number/integer/string_is_integer.py
--rwxr-xr-x   0        0        0      891 2024-05-13 01:11:08.342409 goodest-1.2.1/venues/stages/goodest/measures/number/percentage/__pycache__/from_fraction.cpython-310.pyc
--rwxr-xr-x   0        0        0     1702 2024-04-17 03:33:22.113283 goodest-1.2.1/venues/stages/goodest/measures/number/percentage/__pycache__/from_fraction.cpython-311.pyc
--rwxr-xr-x   0        0        0      744 2024-05-13 01:11:03.342439 goodest-1.2.1/venues/stages/goodest/measures/number/percentage/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      950 2024-05-13 00:59:01.381145 goodest-1.2.1/venues/stages/goodest/measures/number/percentage/from_fraction.py
--rwxr-xr-x   0        0        0      552 2024-05-13 00:59:01.385145 goodest-1.2.1/venues/stages/goodest/measures/number/percentage/status_1.py
--rwxr-xr-x   0        0        0     2209 2024-05-13 00:59:01.381145 goodest-1.2.1/venues/stages/goodest/measures/number/sci_note/__init__.py
--rwxr-xr-x   0        0        0     1362 2024-05-13 01:11:04.386433 goodest-1.2.1/venues/stages/goodest/measures/number/sci_note/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2246 2024-05-13 01:11:03.294439 goodest-1.2.1/venues/stages/goodest/measures/number/sci_note/_status/__pycache__/status_multiples_of_3_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     3223 2024-05-13 00:59:01.381145 goodest-1.2.1/venues/stages/goodest/measures/number/sci_note/_status/status_multiples_of_3_1.py
--rwxr-xr-x   0        0        0      612 2024-04-17 03:33:22.113283 goodest-1.2.1/venues/stages/goodest/measures/number/sci_note/sci_note.S.HTML
--rwxr-xr-x   0        0        0      644 2024-04-17 03:33:22.113283 goodest-1.2.1/venues/stages/goodest/measures/number/sci_note/sci_note_possibilities.S.HTML
--rwxr-xr-x   0        0        0     1341 2024-05-13 00:59:01.381145 goodest-1.2.1/venues/stages/goodest/measures/number/sci_note/sci_note_thoughts.S.HTML
--rwxr-xr-x   0        0        0      362 2024-05-13 00:59:01.381145 goodest-1.2.1/venues/stages/goodest/measures/number/sci_note_2/__init__.py
--rwxr-xr-x   0        0        0      601 2024-05-13 01:08:31.267266 goodest-1.2.1/venues/stages/goodest/measures/number/sci_note_2/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1219 2024-05-13 01:11:04.566432 goodest-1.2.1/venues/stages/goodest/measures/number/sci_note_2/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      935 2024-05-13 00:59:01.381145 goodest-1.2.1/venues/stages/goodest/measures/number/sci_note_2/status_1.py
--rwxr-xr-x   0        0        0       58 2024-04-17 03:33:22.113283 goodest-1.2.1/venues/stages/goodest/measures/temperature/temperature.r.html
--rwxr-xr-x   0        0        0     2204 2024-05-13 00:59:01.385145 goodest-1.2.1/venues/stages/goodest/measures/volume/swap/__init__.py
--rwxr-xr-x   0        0        0     1476 2024-05-13 01:08:31.347266 goodest-1.2.1/venues/stages/goodest/measures/volume/swap/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2595 2024-04-17 03:33:22.113283 goodest-1.2.1/venues/stages/goodest/measures/volume/swap/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1689 2024-05-13 01:11:04.302433 goodest-1.2.1/venues/stages/goodest/measures/volume/swap/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1665 2024-05-13 00:59:01.385145 goodest-1.2.1/venues/stages/goodest/measures/volume/swap/status_1.py
--rwxr-xr-x   0        0        0      510 2024-04-17 03:33:22.113283 goodest-1.2.1/venues/stages/goodest/measures/volume/volume.html
--rwxr-xr-x   0        0        0      911 2024-04-17 03:33:22.113283 goodest-1.2.1/venues/stages/goodest/measures/weight/weight.r.html
--rwxr-xr-x   0        0        0      440 2024-05-13 01:04:39.757620 goodest-1.2.1/venues/stages/goodest/mixes/docks/__pycache__/address.cpython-310.pyc
--rwxr-xr-x   0        0        0      217 2024-05-13 00:59:01.381145 goodest-1.2.1/venues/stages/goodest/mixes/docks/address.py
--rwxr-xr-x   0        0        0      762 2024-05-13 21:38:47.355615 goodest-1.2.1/venues/stages/goodest/mixes/drives/etch/__pycache__/bracket.cpython-310.pyc
--rwxr-xr-x   0        0        0      462 2024-05-13 21:38:40.119718 goodest-1.2.1/venues/stages/goodest/mixes/drives/etch/bracket.py
--rwxr-xr-x   0        0        0     1034 2024-05-13 01:08:31.363266 goodest-1.2.1/venues/stages/goodest/mixes/insure/__pycache__/equalities.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-04-17 03:33:22.113283 goodest-1.2.1/venues/stages/goodest/mixes/insure/__pycache__/equalities.cpython-311.pyc
--rwxr-xr-x   0        0        0      466 2024-05-13 01:11:05.386427 goodest-1.2.1/venues/stages/goodest/mixes/insure/__pycache__/equality.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-04-17 03:33:22.113283 goodest-1.2.1/venues/stages/goodest/mixes/insure/__pycache__/equality.cpython-311.pyc
--rwxr-xr-x   0        0        0      988 2024-05-13 01:11:06.986417 goodest-1.2.1/venues/stages/goodest/mixes/insure/__pycache__/override_print.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-04-17 03:33:22.113283 goodest-1.2.1/venues/stages/goodest/mixes/insure/__pycache__/override_print.cpython-311.pyc
--rwxr-xr-x   0        0        0      585 2024-05-13 01:11:04.214434 goodest-1.2.1/venues/stages/goodest/mixes/insure/__pycache__/status_equalitites_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1090 2024-05-13 00:59:01.381145 goodest-1.2.1/venues/stages/goodest/mixes/insure/equalities.py
--rwxr-xr-x   0        0        0      239 2024-05-13 00:59:01.381145 goodest-1.2.1/venues/stages/goodest/mixes/insure/equality.py
--rwxr-xr-x   0        0        0      783 2024-05-13 00:59:01.381145 goodest-1.2.1/venues/stages/goodest/mixes/insure/override_print.py
--rwxr-xr-x   0        0        0      379 2024-05-13 00:59:01.381145 goodest-1.2.1/venues/stages/goodest/mixes/insure/status_equalitites_1.py
--rwxr-xr-x   0        0        0      579 2024-05-13 00:59:01.381145 goodest-1.2.1/venues/stages/goodest/mixes/procedure/__init__.py
--rwxr-xr-x   0        0        0     1007 2024-05-13 01:04:39.753620 goodest-1.2.1/venues/stages/goodest/mixes/procedure/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1631 2024-05-14 01:15:58.290298 goodest-1.2.1/venues/stages/goodest/readme.md
--rwxr-xr-x   0        0        0     1900 2024-05-13 00:59:01.397145 goodest-1.2.1/venues/stages/goodest/shows_v2/goodness_certifications/certifications.py
--rwxr-xr-x   0        0        0      674 2024-05-13 00:59:01.397145 goodest-1.2.1/venues/stages/goodest/shows_v2/goodness_certifications/goodest.S.HTML
--rwxr-xr-x   0        0        0     1608 2024-05-13 01:11:05.390427 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/_ops/assertions/__pycache__/ingredient.cpython-310.pyc
--rwxr-xr-x   0        0        0     2799 2024-05-13 00:59:01.397145 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/_ops/assertions/ingredient.py
--rwxr-xr-x   0        0        0     1257 2024-05-13 00:59:01.397145 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/_ops/formulate/__init__.py
--rwxr-xr-x   0        0        0      686 2024-05-13 01:08:31.259266 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/_ops/formulate/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1520 2024-05-13 01:11:05.346427 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_empty/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1272 2024-05-13 00:59:01.397145 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_empty/status_1.py
--rwxr-xr-x   0        0        0     1812 2024-05-13 01:11:03.906436 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_food/__pycache__/status_0.cpython-310.pyc
--rwxr-xr-x   0        0        0     3682 2024-05-13 01:11:04.934430 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_food/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     2792 2024-05-13 01:11:03.534438 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_food/__pycache__/status_2.cpython-310.pyc
--rwxr-xr-x   0        0        0     2012 2024-05-13 01:11:05.934424 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_food/__pycache__/status_3.cpython-310.pyc
--rwxr-xr-x   0        0        0     2381 2024-05-13 00:59:01.397145 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_food/status_0.py
--rwxr-xr-x   0        0        0     6527 2024-05-13 00:59:01.397145 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_food/status_1.py
--rwxr-xr-x   0        0        0     3894 2024-05-13 00:59:01.397145 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_food/status_2.py
--rwxr-xr-x   0        0        0     2382 2024-05-13 00:59:01.397145 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_food/status_3.py
--rwxr-xr-x   0        0        0     2782 2024-05-13 01:11:04.162434 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_foods_and_supps/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0   200787 2024-05-14 01:27:54.730371 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_foods_and_supps/status_1.JSON
--rwxr-xr-x   0        0        0     2107 2024-05-13 00:59:01.397145 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_foods_and_supps/status_1.py
--rwxr-xr-x   0        0        0     2676 2024-05-13 01:11:04.262434 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_rational_amounts/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0   112672 2024-05-14 01:27:57.302343 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_rational_amounts/status_1.JSON
--rwxr-xr-x   0        0        0     1931 2024-05-13 00:59:01.397145 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_rational_amounts/status_1.py
--rwxr-xr-x   0        0        0     2351 2024-05-13 01:11:04.270434 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_supp/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1924 2024-05-13 01:11:04.226434 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_supp/__pycache__/status_1_supp_1.cpython-310.pyc
--rwxr-xr-x   0        0        0   109562 2024-05-14 01:27:56.258354 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_supp/status_1.JSON
--rwxr-xr-x   0        0        0     1825 2024-05-13 00:59:01.397145 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_supp/status_1.py
--rwxr-xr-x   0        0        0     1426 2024-05-13 00:59:01.397145 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_supp/status_1_supp_1.py
--rwxr-xr-x   0        0        0     2560 2024-05-13 04:13:39.302285 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/_ops/retrieve/__init__.py
--rwxr-xr-x   0        0        0     1708 2024-05-13 04:13:42.582244 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/_ops/retrieve/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      671 2024-05-13 04:01:03.341098 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/_ops/retrieve/_status/API_status_1.py
--rwxr-xr-x   0        0        0      825 2024-05-13 23:01:43.300966 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/_ops/retrieve/_status/__pycache__/API_status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     2885 2024-05-13 04:15:32.480875 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/land/_ops/formulate/__init__.py
--rwxr-xr-x   0        0        0     2315 2024-05-13 04:16:40.936035 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/land/_ops/formulate/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      235 2024-05-13 00:59:01.397145 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/recipe.S.HTML
--rwxr-xr-x   0        0        0     2532 2024-04-28 00:40:14.210697 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/__pycache__/formulate.cpython-310.pyc
--rwxr-xr-x   0        0        0     1425 2024-05-13 22:03:44.585463 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/for_1_food/__init__.py
--rwxr-xr-x   0        0        0     1056 2024-05-13 22:06:23.071845 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/for_1_food/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1321 2024-05-13 21:52:11.753431 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/for_1_food/_status/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1391 2024-05-13 21:51:59.965570 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/for_1_food/_status/status_1.py
--rwxr-xr-x   0        0        0    92943 2024-05-14 01:27:57.358342 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/for_1_food/_status/status_1_food.JSON
--rwxr-xr-x   0        0        0     1098 2024-05-13 22:15:08.035569 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/for_1_supp/__init__.py
--rwxr-xr-x   0        0        0     1190 2024-05-13 22:15:11.771535 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/for_1_supp/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1337 2024-05-13 22:02:42.690165 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/for_1_supp/_status/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1414 2024-05-13 22:02:38.842208 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/for_1_supp/_status/status_1.py
--rwxr-xr-x   0        0        0   236544 2024-05-14 01:27:56.914347 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/for_1_supp/_status/status_1_supp.JSON
--rwxr-xr-x   0        0        0     1948 2024-05-13 21:54:01.336147 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/__init__.py
--rwxr-xr-x   0        0        0     1399 2024-05-13 21:54:06.060092 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2969 2024-05-13 19:19:14.229533 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status/1_2_recipe_preformulated/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0    93876 2024-05-14 01:27:53.830381 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status/1_2_recipe_preformulated/status_1.JSON
--rwxr-xr-x   0        0        0     2690 2024-05-13 19:19:08.473594 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status/1_2_recipe_preformulated/status_1.py
--rwxr-xr-x   0        0        0     2957 2024-05-13 19:23:38.590709 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status/1_3_recipe_prefomulated/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0   214187 2024-05-14 01:27:57.762337 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status/1_3_recipe_prefomulated/status_1.JSON
--rwxr-xr-x   0        0        0     2403 2024-05-13 19:12:01.686200 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status/1_3_recipe_prefomulated/status_1.py
--rwxr-xr-x   0        0        0     2658 2024-05-13 01:11:04.110435 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status/2_food/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0    58054 2024-05-14 01:27:56.918347 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status/2_food/status_1.JSON
--rwxr-xr-x   0        0        0     1949 2024-05-13 00:59:01.401145 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status/2_food/status_1.py
--rwxr-xr-x   0        0        0     1869 2024-05-13 23:09:11.573526 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_1_recipe/API_status_1.py
--rwxr-xr-x   0        0        0     1899 2024-05-13 23:09:18.509470 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_1_recipe/__pycache__/API_status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1880 2024-04-28 17:59:07.380196 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_1_recipe/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0    93917 2024-05-14 00:55:59.862218 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_1_recipe/status_1.JSON
--rwxr-xr-x   0        0        0     1602 2024-05-13 04:01:55.736218 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_2_recipe/API_status_1.py
--rwxr-xr-x   0        0        0     1872 2024-05-13 23:01:43.324966 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_2_recipe/__pycache__/API_status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1853 2024-04-28 17:57:44.252665 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_2_recipe/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0   214139 2024-05-14 00:56:02.334190 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_2_recipe/status_1.JSON
--rwxr-xr-x   0        0        0     1664 2024-04-28 04:43:21.416236 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status_API/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     2367 2024-05-14 00:10:09.982882 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/modules/__pycache__/add_goals.cpython-310.pyc
--rwxr-xr-x   0        0        0      585 2024-05-13 18:58:53.655214 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/modules/__pycache__/find_goal.cpython-310.pyc
--rwxr-xr-x   0        0        0     2905 2024-05-14 00:10:06.494940 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/modules/add_goals.py
--rwxr-xr-x   0        0        0      481 2024-05-13 18:58:48.467276 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/modules/find_goal.py
--rwxr-xr-x   0        0        0     1421 2024-04-28 02:28:19.421723 goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/recipe_with_goals.S.HTML
--rwxr-xr-x   0        0        0      143 2024-04-17 03:33:22.129283 goodest-1.2.1/venues/stages/goodest/shows_v2/shows.S.HTML
--rwxr-xr-x   0        0        0      563 2024-05-13 00:59:01.393145 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/_assertions/__init__.py
--rwxr-xr-x   0        0        0      798 2024-05-13 01:08:31.343266 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/_assertions/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      224 2024-04-17 03:33:22.117283 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/forward_channel/FDA.s.HTML
--rwxr-xr-x   0        0        0      421 2024-04-17 03:33:22.117283 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/forward_channel/_journal/journal.r.HTML
--rwxr-xr-x   0        0        0        0 2024-04-17 03:33:22.117283 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/forward_channel/_journal/structures/calcium.r.HTML
--rwxr-xr-x   0        0        0      216 2024-04-17 03:33:22.117283 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/forward_channel/_journal/structures/lipids/lipids.r.HTML
--rwxr-xr-x   0        0        0       11 2024-04-17 03:33:22.117283 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/forward_channel/_journal/structures/protein/protein.r.HTML
--rwxr-xr-x   0        0        0     1351 2024-04-17 03:33:22.117283 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/forward_channel/_journal/structures/vitamin a.r.HTML
--rwxr-xr-x   0        0        0      807 2024-04-17 03:33:22.117283 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/forward_channel/_journal/structures/vitamin b.r.HTML
--rwxr-xr-x   0        0        0       93 2024-04-17 03:33:22.117283 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/forward_channel/_journal/structures/vitamin c.r.HTML
--rwxr-xr-x   0        0        0     1298 2024-04-17 03:33:22.117283 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/forward_channel/_journal/structures/vitamin d.r.HTML
--rwxr-xr-x   0        0        0      149 2024-04-17 03:33:22.117283 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/forward_channel/_journal/structures/vitamin e.r.HTML
--rwxr-xr-x   0        0        0      219 2024-04-17 03:33:22.117283 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/forward_channel/channel/river.s.HTML
--rwxr-xr-x   0        0        0      543 2024-04-17 03:33:22.117283 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/forward_channel/forward channel.s.HTML
--rwxr-xr-x   0        0        0      935 2024-04-17 03:33:22.117283 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/forward_channel/structures.s.HTML
--rwxr-xr-x   0        0        0      471 2024-04-17 03:36:50.295021 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      716 2024-05-13 01:08:31.263266 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/__pycache__/develop.cpython-310.pyc
--rwxr-xr-x   0        0        0     4922 2024-05-13 00:59:01.389145 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/__init__.py
--rwxr-xr-x   0        0        0     2290 2024-05-13 01:08:31.355266 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1205 2024-05-13 01:11:03.358439 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_empty_grove/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1038 2024-05-13 00:59:01.389145 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_empty_grove/status_1.py
--rwxr-xr-x   0        0        0     1748 2024-05-13 01:11:04.786430 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_m_and_meq/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1756 2024-05-13 01:11:03.970435 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_m_and_meq/__pycache__/status_2.cpython-310.pyc
--rwxr-xr-x   0        0        0     2143 2024-05-13 00:59:01.389145 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_m_and_meq/status_1.py
--rwxr-xr-x   0        0        0     2120 2024-05-13 00:59:01.389145 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_m_and_meq/status_2.py
--rwxr-xr-x   0        0        0     2138 2024-05-13 01:11:03.794437 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_m_eq_and_ba/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     3700 2024-05-13 00:59:01.389145 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_m_eq_and_ba/status_1.py
--rwxr-xr-x   0        0        0      445 2024-05-13 00:59:01.389145 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/assertions_one/__init__.py
--rwxr-xr-x   0        0        0      568 2024-05-13 01:08:31.355266 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/assertions_one/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     3108 2024-05-13 00:59:01.389145 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/calculate_portions/__init__.py
--rwxr-xr-x   0        0        0     1537 2024-05-13 01:08:31.267266 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/calculate_portions/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1368 2024-05-13 00:59:01.389145 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/cultivate/__init__.py
--rwxr-xr-x   0        0        0     1071 2024-05-13 01:08:31.355266 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/cultivate/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      802 2024-05-13 00:59:01.385145 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/develop.py
--rwxr-xr-x   0        0        0     2566 2024-05-13 00:59:01.385145 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/measures_sums/__init__.py
--rwxr-xr-x   0        0        0     1727 2024-05-13 01:08:31.355266 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/measures_sums/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      705 2024-05-13 01:11:03.510438 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/measures_sums/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      451 2024-05-13 00:59:01.385145 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/measures_sums/status_1.py
--rwxr-xr-x   0        0        0     1781 2024-05-13 00:59:01.385145 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/multiply_amount/__init__.py
--rwxr-xr-x   0        0        0     1414 2024-05-13 01:08:31.263266 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/multiply_amount/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2945 2024-04-17 03:33:22.125283 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/multiply_amount/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     2108 2024-05-13 01:11:04.262434 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/multiply_amount/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     2243 2024-05-13 01:11:04.110435 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/multiply_amount/__pycache__/status_2.cpython-310.pyc
--rwxr-xr-x   0        0        0     1327 2024-05-13 01:11:04.962429 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/multiply_amount/__pycache__/status_loop_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      950 2024-04-17 03:33:22.125283 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/multiply_amount/multiply_measures.s.HTML
--rwxr-xr-x   0        0        0     2561 2024-05-13 00:59:01.385145 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/multiply_amount/status_1.py
--rwxr-xr-x   0        0        0     2945 2024-05-13 00:59:01.389145 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/multiply_amount/status_2.py
--rwxr-xr-x   0        0        0     1088 2024-05-13 00:59:01.385145 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/multiply_amount/status_loop_1.py
--rwxr-xr-x   0        0        0      279 2024-04-24 21:20:53.222120 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      633 2024-05-13 00:59:01.393145 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/assertions/__init__.py
--rwxr-xr-x   0        0        0      794 2024-05-13 01:08:31.355266 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/assertions/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     5622 2024-05-13 00:59:01.393145 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/has_uniters/__init__.py
--rwxr-xr-x   0        0        0     1776 2024-05-13 01:08:31.355266 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/has_uniters/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1248 2024-05-13 01:11:04.930430 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/has_uniters/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1115 2024-05-13 00:59:01.393145 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/has_uniters/status_1.py
--rwxr-xr-x   0        0        0      545 2024-05-13 00:59:01.393145 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/is_story_1/__init__.py
--rwxr-xr-x   0        0        0      785 2024-05-13 01:08:31.355266 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/is_story_1/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      961 2024-05-13 01:11:04.778431 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/is_story_1/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      756 2024-05-13 00:59:01.393145 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/is_story_1/status_1.py
--rwxr-xr-x   0        0        0     2539 2024-05-13 00:59:01.393145 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/nurture/__init__.py
--rwxr-xr-x   0        0        0     2241 2024-05-13 01:08:31.263266 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/nurture/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1094 2024-05-13 01:11:04.262434 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/nurture/__pycache__/status_cautionary.cpython-310.pyc
--rwxr-xr-x   0        0        0     1012 2024-05-13 01:11:05.058429 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/nurture/__pycache__/status_essentials.cpython-310.pyc
--rwxr-xr-x   0        0        0      794 2024-05-13 00:59:01.393145 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/nurture/status_cautionary.py
--rwxr-xr-x   0        0        0      704 2024-05-13 00:59:01.393145 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/nurture/status_essentials.py
--rwxr-xr-x   0        0        0     1299 2024-05-13 00:59:01.393145 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/seek/__init__.py
--rwxr-xr-x   0        0        0     1055 2024-05-13 01:08:31.267266 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/seek/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1096 2024-05-13 01:11:05.430427 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/seek/__pycache__/status_essentials.cpython-310.pyc
--rwxr-xr-x   0        0        0      689 2024-05-13 00:59:01.393145 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/seek/status_essentials.py
--rwxr-xr-x   0        0        0     1361 2024-05-13 00:59:01.393145 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/seek_name_or_accepts/__init__.py
--rwxr-xr-x   0        0        0     1222 2024-05-13 01:08:31.343266 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/seek_name_or_accepts/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      930 2024-05-13 01:11:03.662437 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/seek_name_or_accepts/__pycache__/status_essentials_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      914 2024-05-13 01:11:04.926430 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/seek_name_or_accepts/__pycache__/status_essentials_2.cpython-310.pyc
--rwxr-xr-x   0        0        0      696 2024-05-13 00:59:01.393145 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/seek_name_or_accepts/status_essentials_1.py
--rwxr-xr-x   0        0        0      685 2024-05-13 00:59:01.393145 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/seek_name_or_accepts/status_essentials_2.py
--rwxr-xr-x   0        0        0     1025 2024-05-13 00:59:01.393145 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/seek_uniter/__init__.py
--rwxr-xr-x   0        0        0     1071 2024-05-13 01:08:31.355266 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/seek_uniter/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1026 2024-05-13 01:11:03.814436 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/seek_uniter/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      847 2024-05-13 00:59:01.393145 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/seek_uniter/status_1.py
--rwxr-xr-x   0        0        0     1523 2024-04-17 03:33:22.129283 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/grove.S.HTML
--rwxr-xr-x   0        0        0       58 2024-04-17 03:33:22.129283 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/info/info.S.HTML
--rwxr-xr-x   0        0        0       73 2024-04-17 03:33:22.129283 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/measures/measures.S.HTML
--rwxr-xr-x   0        0        0       59 2024-04-17 03:33:22.129283 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/natures/natures.S.HTML
--rwxr-xr-x   0        0        0     1508 2024-04-17 03:33:22.129283 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/unites/unites.S.HTML
--rwxr-xr-x   0        0        0     2330 2024-04-23 19:28:57.911458 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/land.S.HTML
--rwxr-xr-x   0        0        0      397 2024-05-13 00:59:01.389145 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/measures/__init__.py
--rwxr-xr-x   0        0        0      581 2024-05-13 01:08:31.263266 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/measures/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      459 2024-04-17 03:33:22.129283 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/measures/measures.S.HTML
--rwxr-xr-x   0        0        0     1359 2024-05-13 00:59:01.389145 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/measures/merge/__init__.py
--rwxr-xr-x   0        0        0     1126 2024-05-13 01:08:31.343266 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/measures/merge/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1601 2024-04-17 03:33:22.125283 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/measures/merge/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      943 2024-05-13 01:11:04.174434 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/measures/merge/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      941 2024-05-13 01:11:06.182422 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/measures/merge/__pycache__/status_2.cpython-310.pyc
--rwxr-xr-x   0        0        0      874 2024-05-13 01:11:04.170434 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/measures/merge/__pycache__/status_3.cpython-310.pyc
--rwxr-xr-x   0        0        0     1179 2024-05-13 00:59:01.389145 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/measures/merge/status_1.py
--rwxr-xr-x   0        0        0     1177 2024-05-13 00:59:01.389145 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/measures/merge/status_2.py
--rwxr-xr-x   0        0        0     1019 2024-05-13 00:59:01.389145 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/measures/merge/status_3.py
--rwxr-xr-x   0        0        0      767 2024-05-13 00:59:01.389145 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/measures/multiply/__init__.py
--rwxr-xr-x   0        0        0      869 2024-05-13 01:08:31.267266 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/measures/multiply/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1336 2024-04-17 03:33:22.125283 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/measures/multiply/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1644 2024-05-13 01:11:04.570432 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/measures/multiply/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1693 2024-05-13 00:59:01.389145 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/measures/multiply/status_1.py
--rwxr-xr-x   0        0        0      412 2024-04-17 03:33:22.129283 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/natures/natures.S.HTML
--rwxr-xr-x   0        0        0      405 2024-04-17 03:33:22.129283 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/measured_ingredients/measured_ingredients.S.HTML
--rwxr-xr-x   0        0        0     1066 2024-04-17 03:33:22.129283 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/measures/measures.S.HTML
--rwxr-xr-x   0        0        0      611 2024-04-25 19:49:42.003893 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/nature.S.HTML
--rwxr-xr-x   0        0        0      310 2024-04-25 20:29:19.933549 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/unmeasured_ingredients/UI.S.HTML
--rwxr-xr-x   0        0        0      428 2024-05-13 00:59:01.385145 goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/treasure.S.HTML
--rw-r--r--   0        0        0     2940 1970-01-01 00:00:00.000000 goodest-1.2.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1671 2024-05-14 02:22:22.908866 goodest-1.2.2/pyproject.toml
+-rwxr-xr-x   0        0        0     3153 2024-05-14 02:18:40.626631 goodest-1.2.2/venue.S.HTML
+-rwxr-xr-x   0        0        0      105 2024-04-27 16:44:17.965844 goodest-1.2.2/venue_journal.S.HTML
+-rwxr-xr-x   0        0        0      397 2024-05-13 23:21:53.823261 goodest-1.2.2/venue_monetary.S.HTML
+-rwxr-xr-x   0        0        0      405 2024-04-17 03:33:22.073284 goodest-1.2.2/venues/stages/goodest/[__objectives]/book/Vitamin B.S.HTML
+-rwxr-xr-x   0        0        0       63 2024-04-17 03:33:22.073284 goodest-1.2.2/venues/stages/goodest/[__objectives]/book/Vitamin K.S.HTML
+-rwxr-xr-x   0        0        0      201 2024-04-28 20:53:16.850555 goodest-1.2.2/venues/stages/goodest/[__objectives]/objectives - elliptic.S.HTML
+-rwxr-xr-x   0        0        0     1729 2024-05-13 00:59:01.377145 goodest-1.2.2/venues/stages/goodest/[__objectives]/objectives.S.HTML
+-rwxr-xr-x   0        0        0      533 2024-05-13 00:59:01.385145 goodest-1.2.2/venues/stages/goodest/[_license]/license.s.HTML
+-rwxr-xr-x   0        0        0      116 2024-05-13 00:59:01.385145 goodest-1.2.2/venues/stages/goodest/[_license]/list/goodest.s.HTML
+-rwxr-xr-x   0        0        0    37279 2024-04-17 03:33:22.077284 goodest-1.2.2/venues/stages/goodest/[_license]/list/gpl-3.0-standalone.html
+-rwxr-xr-x   0        0        0      131 2024-04-28 20:54:59.933399 goodest-1.2.2/venues/stages/goodest/[_license]/list/non-commercial.S.HTML
+-rwxr-xr-x   0        0        0     1776 2024-05-13 01:42:44.905899 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves/exports/goodest_inventory/certifications/goodest_inventory.certifications.1.JSON
+-rwxr-xr-x   0        0        0   985917 2024-05-13 01:42:46.309870 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves/exports/goodest_inventory/food/goodest_inventory.food.1.JSON
+-rwxr-xr-x   0        0        0   985917 2024-05-13 23:22:03.551180 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves/exports/goodest_inventory/food/goodest_inventory.food.2.JSON
+-rwxr-xr-x   0        0        0   726299 2024-05-13 01:42:46.301870 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves/exports/goodest_inventory/supp/goodest_inventory.supp.1.JSON
+-rwxr-xr-x   0        0        0   726299 2024-05-13 23:22:03.771178 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves/exports/goodest_inventory/supp/goodest_inventory.supp.2.JSON
+-rwxr-xr-x   0        0        0      118 2024-05-09 02:02:40.749714 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves/exports/goodest_tract/cautionary_ingredients/goodest_tract.cautionary_ingredients.1.JSON
+-rwxr-xr-x   0        0        0      118 2024-05-13 23:22:03.975176 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves/exports/goodest_tract/cautionary_ingredients/goodest_tract.cautionary_ingredients.2.JSON
+-rwxr-xr-x   0        0        0        0 2024-05-09 02:02:41.749703 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves/exports/goodest_tract/certifications/goodest_tract.certifications.1.JSON
+-rwxr-xr-x   0        0        0        0 2024-05-13 23:22:04.959168 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves/exports/goodest_tract/certifications/goodest_tract.certifications.2.JSON
+-rwxr-xr-x   0        0        0     5140 2024-05-09 02:02:40.997712 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves/exports/goodest_tract/essential_nutrients/goodest_tract.essential_nutrients.1.JSON
+-rwxr-xr-x   0        0        0     5140 2024-05-13 23:22:04.239174 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves/exports/goodest_tract/essential_nutrients/goodest_tract.essential_nutrients.2.JSON
+-rwxr-xr-x   0        0        0        0 2024-05-09 02:02:41.245709 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves/exports/goodest_tract/glossary/goodest_tract.glossary.1.JSON
+-rwxr-xr-x   0        0        0        0 2024-05-13 23:22:04.451172 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves/exports/goodest_tract/glossary/goodest_tract.glossary.2.JSON
+-rwxr-xr-x   0        0        0     5771 2024-05-09 02:02:41.509706 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves/exports/goodest_tract/goals/goodest_tract.goals.1.JSON
+-rwxr-xr-x   0        0        0     5782 2024-05-13 23:22:04.739170 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves/exports/goodest_tract/goals/goodest_tract.goals.2.JSON
+-rwxr-xr-x   0        0        0      118 2024-04-17 03:33:22.117283 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v1/exports/goodest_tract/cautionary_ingredients/1.JSON
+-rwxr-xr-x   0        0        0      118 2024-04-23 22:05:34.538523 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v1/exports/goodest_tract/cautionary_ingredients/2.JSON
+-rwxr-xr-x   0        0        0      118 2024-04-23 22:07:10.673303 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v1/exports/goodest_tract/cautionary_ingredients/3.JSON
+-rwxr-xr-x   0        0        0      118 2024-04-27 17:35:00.336394 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v1/exports/goodest_tract/cautionary_ingredients/4.JSON
+-rwxr-xr-x   0        0        0      118 2024-04-28 19:02:50.497975 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v1/exports/goodest_tract/cautionary_ingredients/5.JSON
+-rwxr-xr-x   0        0        0      118 2024-04-28 19:04:10.818025 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v1/exports/goodest_tract/cautionary_ingredients/6.JSON
+-rwxr-xr-x   0        0        0     5140 2024-04-17 03:33:22.117283 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v1/exports/goodest_tract/essential_nutrients/1.JSON
+-rwxr-xr-x   0        0        0     5140 2024-04-23 22:05:35.566512 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v1/exports/goodest_tract/essential_nutrients/2.JSON
+-rwxr-xr-x   0        0        0     5140 2024-04-23 22:07:11.713281 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v1/exports/goodest_tract/essential_nutrients/3.JSON
+-rwxr-xr-x   0        0        0     5140 2024-04-27 17:35:01.316362 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v1/exports/goodest_tract/essential_nutrients/4.JSON
+-rwxr-xr-x   0        0        0     5140 2024-04-28 19:02:51.533976 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v1/exports/goodest_tract/essential_nutrients/5.JSON
+-rwxr-xr-x   0        0        0     5140 2024-04-28 19:04:11.850026 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v1/exports/goodest_tract/essential_nutrients/6.JSON
+-rwxr-xr-x   0        0        0        0 2024-04-23 22:05:36.562502 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v1/exports/goodest_tract/glossary/2.JSON
+-rwxr-xr-x   0        0        0        0 2024-04-23 22:07:12.697261 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v1/exports/goodest_tract/glossary/3.JSON
+-rwxr-xr-x   0        0        0        0 2024-04-27 17:35:02.312330 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v1/exports/goodest_tract/glossary/4.JSON
+-rwxr-xr-x   0        0        0        0 2024-04-28 19:02:52.497976 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v1/exports/goodest_tract/glossary/5.JSON
+-rwxr-xr-x   0        0        0        0 2024-04-28 19:04:12.822027 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v1/exports/goodest_tract/glossary/6.JSON
+-rwxr-xr-x   0        0        0     5771 2024-04-28 19:04:04.554021 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v1/exports/goodest_tract/goals/5.JSON
+-rwxr-xr-x   0        0        0     5771 2024-04-28 19:04:13.826027 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v1/exports/goodest_tract/goals/6.JSON
+-rwxr-xr-x   0        0        0      667 2024-05-02 03:16:33.983190 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v1/saves.S.HTML
+-rwxr-xr-x   0        0        0      416 2024-05-09 02:31:06.501585 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v2/dumps/goodest_tract/cautionary_ingredients/goodest_tract.cautionary_ingredients.1.dump.gzip
+-rwxr-xr-x   0        0        0     1708 2024-05-09 02:31:06.761583 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v2/dumps/goodest_tract/essential_nutrients/goodest_tract.essential_nutrients.1.dump.gzip
+-rwxr-xr-x   0        0        0     1799 2024-05-09 02:31:07.257579 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v2/dumps/goodest_tract/goals/goodest_tract.goals.1.dump.gzip
+-rwxr-xr-x   0        0        0        0 2024-05-09 01:42:50.087325 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v2/exports/goodest_inventory/food/goodest_inventory.foods.1.JSON
+-rwxr-xr-x   0        0        0        0 2024-05-09 02:02:14.490013 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v2/exports/goodest_inventory/food/goodest_inventory.foods.2.JSON
+-rwxr-xr-x   0        0        0        0 2024-05-09 02:02:40.217721 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v2/exports/goodest_inventory/food/goodest_inventory.foods.3.JSON
+-rwxr-xr-x   0        0        0        0 2024-05-09 01:42:51.099313 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v2/exports/goodest_inventory/supp/goodest_inventory.supps.1.JSON
+-rwxr-xr-x   0        0        0        0 2024-05-09 02:02:15.518002 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v2/exports/goodest_inventory/supp/goodest_inventory.supps.2.JSON
+-rwxr-xr-x   0        0        0        0 2024-05-09 02:02:40.489717 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v2/exports/goodest_inventory/supp/goodest_inventory.supps.3.JSON
+-rwxr-xr-x   0        0        0      118 2024-05-09 01:42:52.135301 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v2/exports/goodest_tract/cautionary_ingredients/goodest_tract.cautionary_ingredients.1.JSON
+-rwxr-xr-x   0        0        0      118 2024-05-09 02:02:16.521990 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v2/exports/goodest_tract/cautionary_ingredients/goodest_tract.cautionary_ingredients.2.JSON
+-rwxr-xr-x   0        0        0      118 2024-05-09 02:02:40.749714 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v2/exports/goodest_tract/cautionary_ingredients/goodest_tract.cautionary_ingredients.3.JSON
+-rwxr-xr-x   0        0        0        0 2024-05-09 01:42:56.123255 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v2/exports/goodest_tract/certifications/goodest_tract.certifications.1.JSON
+-rwxr-xr-x   0        0        0        0 2024-05-09 02:02:20.505945 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v2/exports/goodest_tract/certifications/goodest_tract.certifications.2.JSON
+-rwxr-xr-x   0        0        0        0 2024-05-09 02:02:41.749703 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v2/exports/goodest_tract/certifications/goodest_tract.certifications.3.JSON
+-rwxr-xr-x   0        0        0     5140 2024-05-09 01:42:53.139290 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v2/exports/goodest_tract/essential_nutrients/goodest_tract.essential_nutrients.1.JSON
+-rwxr-xr-x   0        0        0     5140 2024-05-09 02:02:17.505979 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v2/exports/goodest_tract/essential_nutrients/goodest_tract.essential_nutrients.2.JSON
+-rwxr-xr-x   0        0        0     5140 2024-05-09 02:02:40.997712 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v2/exports/goodest_tract/essential_nutrients/goodest_tract.essential_nutrients.3.JSON
+-rwxr-xr-x   0        0        0        0 2024-05-09 01:42:54.127278 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v2/exports/goodest_tract/glossary/goodest_tract.glossary.1.JSON
+-rwxr-xr-x   0        0        0        0 2024-05-09 02:02:18.517968 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v2/exports/goodest_tract/glossary/goodest_tract.glossary.2.JSON
+-rwxr-xr-x   0        0        0        0 2024-05-09 02:02:41.245709 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v2/exports/goodest_tract/glossary/goodest_tract.glossary.3.JSON
+-rwxr-xr-x   0        0        0     5771 2024-05-09 01:42:55.151266 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v2/exports/goodest_tract/goals/goodest_tract.goals.1.JSON
+-rwxr-xr-x   0        0        0     5771 2024-05-09 02:02:19.509956 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v2/exports/goodest_tract/goals/goodest_tract.goals.2.JSON
+-rwxr-xr-x   0        0        0     5771 2024-05-09 02:02:41.509706 goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v2/exports/goodest_tract/goals/goodest_tract.goals.3.JSON
+-rwxr-xr-x   0        0        0      378 2024-05-13 00:59:57.244563 goodest-1.2.2/venues/stages/goodest/__dictionary/goodest_1
+-rwxr-xr-x   0        0        0      429 2024-05-13 00:59:01.377145 goodest-1.2.2/venues/stages/goodest/__init__.py
+-rwxr-xr-x   0        0        0   128501 2024-05-14 00:56:03.406178 goodest-1.2.2/venues/stages/goodest/__status/API/DB/records.json
+-rwxr-xr-x   0        0        0     2100 2024-05-13 00:59:57.292563 goodest-1.2.2/venues/stages/goodest/__status/API/status.proc.py
+-rwxr-xr-x   0        0        0     1172 2024-04-17 03:33:22.077284 goodest-1.2.2/venues/stages/goodest/__status/__pycache__/status_API.proc.cpython-310.pyc
+-rwxr-xr-x   0        0        0       11 2024-04-23 21:56:29.284154 goodest-1.2.2/venues/stages/goodest/__status/main/.gitignore
+-rwxr-xr-x   0        0        0    41183 2024-04-25 01:22:42.760494 goodest-1.2.2/venues/stages/goodest/__status/main/output.json
+-rwxr-xr-x   0        0        0     2121 2024-05-13 00:59:58.016555 goodest-1.2.2/venues/stages/goodest/__status/main/status.proc.py
+-rwxr-xr-x   0        0        0     1561 2024-05-13 01:04:39.489623 goodest-1.2.2/venues/stages/goodest/_controls/__pycache__/_clique.cpython-310.pyc
+-rwxr-xr-x   0        0        0      738 2024-04-23 19:31:08.382022 goodest-1.2.2/venues/stages/goodest/_controls/__pycache__/off.cpython-310.pyc
+-rwxr-xr-x   0        0        0      756 2024-04-23 19:30:52.306199 goodest-1.2.2/venues/stages/goodest/_controls/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      544 2024-04-23 19:31:08.382022 goodest-1.2.2/venues/stages/goodest/_controls/__pycache__/refresh.cpython-310.pyc
+-rwxr-xr-x   0        0        0      781 2024-04-23 19:31:08.382022 goodest-1.2.2/venues/stages/goodest/_controls/__pycache__/status.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1643 2024-05-13 00:59:57.240563 goodest-1.2.2/venues/stages/goodest/_controls/_clique.py
+-rwxr-xr-x   0        0        0     1145 2024-05-13 00:59:57.240563 goodest-1.2.2/venues/stages/goodest/_essence/__init__.py
+-rwxr-xr-x   0        0        0      986 2024-05-13 01:04:39.493623 goodest-1.2.2/venues/stages/goodest/_essence/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2438 2024-05-13 00:59:57.240563 goodest-1.2.2/venues/stages/goodest/_essence/activate_alert--/__init__.py
+-rwxr-xr-x   0        0        0     1802 2024-05-02 23:21:54.655013 goodest-1.2.2/venues/stages/goodest/_essence/activate_alert--/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      790 2024-05-02 23:21:54.655013 goodest-1.2.2/venues/stages/goodest/_essence/activate_alert--/__pycache__/parse_exception.cpython-310.pyc
+-rwxr-xr-x   0        0        0      505 2024-05-13 00:59:57.240563 goodest-1.2.2/venues/stages/goodest/_essence/activate_alert--/parse_exception.py
+-rwxr-xr-x   0        0        0      202 2024-04-27 16:49:31.955662 goodest-1.2.2/venues/stages/goodest/_essence/essence.S.HTML
+-rwxr-xr-x   0        0        0     3327 2024-05-14 01:52:37.098267 goodest-1.2.2/venues/stages/goodest/_essence/merge/__init__.py
+-rwxr-xr-x   0        0        0     1991 2024-05-14 01:57:00.168563 goodest-1.2.2/venues/stages/goodest/_essence/merge/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      719 2024-05-02 02:39:12.702510 goodest-1.2.2/venues/stages/goodest/_essence/scan/__init__.py
+-rwxr-xr-x   0        0        0      842 2024-05-02 22:19:11.125002 goodest-1.2.2/venues/stages/goodest/_essence/scan/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      754 2024-05-02 22:19:56.188529 goodest-1.2.2/venues/stages/goodest/_essence/seek/__init__.py
+-rwxr-xr-x   0        0        0      770 2024-05-02 22:20:00.192486 goodest-1.2.2/venues/stages/goodest/_essence/seek/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      735 2024-05-10 19:20:27.044506 goodest-1.2.2/venues/stages/goodest/adventures/DNS/counsellor.S.HTML
+-rwxr-xr-x   0        0        0      590 2024-05-13 00:59:57.240563 goodest-1.2.2/venues/stages/goodest/adventures/HTTPS_Certs/HTTPS_Certs.S.HTML
+-rwxr-xr-x   0        0        0     1538 2024-05-13 01:04:39.489623 goodest-1.2.2/venues/stages/goodest/adventures/_ops/__pycache__/_clique.cpython-310.pyc
+-rwxr-xr-x   0        0        0      882 2024-05-13 01:04:39.757620 goodest-1.2.2/venues/stages/goodest/adventures/_ops/__pycache__/off.cpython-310.pyc
+-rwxr-xr-x   0        0        0      912 2024-05-13 01:04:39.489623 goodest-1.2.2/venues/stages/goodest/adventures/_ops/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      583 2024-05-13 01:04:39.757620 goodest-1.2.2/venues/stages/goodest/adventures/_ops/__pycache__/refresh.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1111 2024-05-13 01:04:39.757620 goodest-1.2.2/venues/stages/goodest/adventures/_ops/__pycache__/status.cpython-310.pyc
+-rwxr-xr-x   0        0        0      861 2024-05-13 00:59:57.232563 goodest-1.2.2/venues/stages/goodest/adventures/_ops/_clique.py
+-rwxr-xr-x   0        0        0      794 2024-04-23 19:52:04.387492 goodest-1.2.2/venues/stages/goodest/adventures/_ops/monitor.py
+-rwxr-xr-x   0        0        0      763 2024-05-13 00:59:57.232563 goodest-1.2.2/venues/stages/goodest/adventures/_ops/off.py
+-rwxr-xr-x   0        0        0      804 2024-05-13 00:59:57.232563 goodest-1.2.2/venues/stages/goodest/adventures/_ops/on.py
+-rwxr-xr-x   0        0        0      434 2024-05-13 00:59:57.232563 goodest-1.2.2/venues/stages/goodest/adventures/_ops/refresh.py
+-rwxr-xr-x   0        0        0     1028 2024-05-13 00:59:57.232563 goodest-1.2.2/venues/stages/goodest/adventures/_ops/status.py
+-rwxr-xr-x   0        0        0      780 2024-05-10 19:21:14.303955 goodest-1.2.2/venues/stages/goodest/adventures/adventures.S.HTML
+-rwxr-xr-x   0        0        0     2491 2024-05-13 18:53:48.503003 goodest-1.2.2/venues/stages/goodest/adventures/alerting/__init__.py
+-rwxr-xr-x   0        0        0     1851 2024-05-13 18:54:07.598756 goodest-1.2.2/venues/stages/goodest/adventures/alerting/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      788 2024-05-13 01:04:39.753620 goodest-1.2.2/venues/stages/goodest/adventures/alerting/__pycache__/parse_exception.cpython-310.pyc
+-rwxr-xr-x   0        0        0      505 2024-05-13 00:59:57.232563 goodest-1.2.2/venues/stages/goodest/adventures/alerting/parse_exception.py
+-rwxr-xr-x   0        0        0      794 2024-05-13 00:59:57.240563 goodest-1.2.2/venues/stages/goodest/adventures/cloud_flares/cloud_flares.S.HTML
+-rwxr-xr-x   0        0        0      160 2024-05-09 04:34:51.673638 goodest-1.2.2/venues/stages/goodest/adventures/customs/__init__.py
+-rwxr-xr-x   0        0        0      630 2024-05-09 04:34:54.301616 goodest-1.2.2/venues/stages/goodest/adventures/customs/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      926 2024-04-17 03:33:22.113283 goodest-1.2.2/venues/stages/goodest/adventures/customs/__pycache__/clique.cpython-310.pyc
+-rwxr-xr-x   0        0        0      245 2024-04-17 03:33:22.113283 goodest-1.2.2/venues/stages/goodest/adventures/customs/__pycache__/off.cpython-310.pyc
+-rwxr-xr-x   0        0        0      345 2024-04-17 03:33:22.113283 goodest-1.2.2/venues/stages/goodest/adventures/customs/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      251 2024-04-17 03:33:22.113283 goodest-1.2.2/venues/stages/goodest/adventures/customs/__pycache__/status.cpython-310.pyc
+-rwxr-xr-x   0        0        0      948 2024-05-13 01:04:39.761620 goodest-1.2.2/venues/stages/goodest/adventures/customs/_ops/__pycache__/_clique.cpython-310.pyc
+-rwxr-xr-x   0        0        0      579 2024-05-13 00:59:57.240563 goodest-1.2.2/venues/stages/goodest/adventures/customs/_ops/_clique.py
+-rwxr-xr-x   0        0        0        2 2024-05-09 04:35:38.109250 goodest-1.2.2/venues/stages/goodest/adventures/customs/_ops/off.py
+-rwxr-xr-x   0        0        0      662 2024-05-09 04:39:09.399469 goodest-1.2.2/venues/stages/goodest/adventures/customs/_ops/on.py
+-rwxr-xr-x   0        0        0        2 2024-04-27 23:15:34.237762 goodest-1.2.2/venues/stages/goodest/adventures/customs/_ops/status.py
+-rwxr-xr-x   0        0        0      285 2024-05-09 04:40:07.774973 goodest-1.2.2/venues/stages/goodest/adventures/customs/configs_school/embargo.NFT
+-rwxr-xr-x   0        0        0      145 2024-04-27 23:16:20.801181 goodest-1.2.2/venues/stages/goodest/adventures/customs/customs.S.HTML
+-rwxr-xr-x   0        0        0     1327 2024-01-25 05:00:54.191593 goodest-1.2.2/venues/stages/goodest/adventures/demux_hap/HA.s.HTML
+-rwxr-xr-x   0        0        0      238 2023-12-02 04:53:31.462384 goodest-1.2.2/venues/stages/goodest/adventures/demux_hap/SSL/SSL.r.HTML
+-rwxr-xr-x   0        0        0      985 2023-12-14 02:01:36.217926 goodest-1.2.2/venues/stages/goodest/adventures/demux_hap/SSL/__init__.py
+-rwxr-xr-x   0        0        0     1086 2024-05-10 01:30:13.387176 goodest-1.2.2/venues/stages/goodest/adventures/demux_hap/SSL/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1872 2023-12-14 02:01:38.764897 goodest-1.2.2/venues/stages/goodest/adventures/demux_hap/SSL/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1757 2023-12-01 23:15:16.435121 goodest-1.2.2/venues/stages/goodest/adventures/demux_hap/SSL/certificate.pem
+-rwxr-xr-x   0        0        0     3272 2023-12-01 23:15:16.430121 goodest-1.2.2/venues/stages/goodest/adventures/demux_hap/SSL/certificate.pem.key
+-rwxr-xr-x   0        0        0      346 2023-12-01 18:00:33.471576 goodest-1.2.2/venues/stages/goodest/adventures/demux_hap/__init__.py
+-rwxr-xr-x   0        0        0      576 2024-05-10 01:29:49.491477 goodest-1.2.2/venues/stages/goodest/adventures/demux_hap/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      737 2024-05-12 19:04:34.064153 goodest-1.2.2/venues/stages/goodest/adventures/demux_hap/_controls/__pycache__/_clique.cpython-310.pyc
+-rwxr-xr-x   0        0        0      617 2024-05-13 01:04:39.761620 goodest-1.2.2/venues/stages/goodest/adventures/demux_hap/_controls/__pycache__/build.cpython-310.pyc
+-rwxr-xr-x   0        0        0      328 2024-05-10 01:44:25.794256 goodest-1.2.2/venues/stages/goodest/adventures/demux_hap/_controls/__pycache__/off.cpython-310.pyc
+-rwxr-xr-x   0        0        0      924 2024-05-13 01:04:39.757620 goodest-1.2.2/venues/stages/goodest/adventures/demux_hap/_controls/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      345 2024-05-12 16:13:33.336331 goodest-1.2.2/venues/stages/goodest/adventures/demux_hap/_controls/_clique.py
+-rwxr-xr-x   0        0        0      312 2024-05-13 00:59:57.232563 goodest-1.2.2/venues/stages/goodest/adventures/demux_hap/_controls/build.py
+-rwxr-xr-x   0        0        0       77 2024-05-10 01:44:23.514282 goodest-1.2.2/venues/stages/goodest/adventures/demux_hap/_controls/off.py
+-rwxr-xr-x   0        0        0      901 2024-05-13 00:59:57.232563 goodest-1.2.2/venues/stages/goodest/adventures/demux_hap/_controls/on.py
+-rwxr-xr-x   0        0        0     1295 2023-12-02 01:06:44.630336 goodest-1.2.2/venues/stages/goodest/adventures/demux_hap/configs/HTTPS_to_HTTP/1.py
+-rwxr-xr-x   0        0        0      567 2023-12-04 23:16:04.198925 goodest-1.2.2/venues/stages/goodest/adventures/demux_hap/configs/HTTPS_to_HTTP/HTTPS_to_HTTP.s.HTML
+-rwxr-xr-x   0        0        0     1892 2024-05-13 00:59:57.232563 goodest-1.2.2/venues/stages/goodest/adventures/demux_hap/configs/HTTPS_to_HTTP/__init__.py
+-rwxr-xr-x   0        0        0     1921 2024-05-13 01:04:39.757620 goodest-1.2.2/venues/stages/goodest/adventures/demux_hap/configs/HTTPS_to_HTTP/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2832 2023-12-14 04:27:42.320026 goodest-1.2.2/venues/stages/goodest/adventures/demux_hap/configs/HTTPS_to_HTTP/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1296 2023-12-01 22:31:43.018311 goodest-1.2.2/venues/stages/goodest/adventures/demux_hap/configs/HTTP_balancer/__init__.py
+-rwxr-xr-x   0        0        0     1774 2023-12-01 22:50:16.802479 goodest-1.2.2/venues/stages/goodest/adventures/demux_hap/configs/HTTP_balancer/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      277 2023-12-01 21:44:47.102165 goodest-1.2.2/venues/stages/goodest/adventures/demux_hap/configs/HTTP_balancer/examples/example_1.cfg
+-rwxr-xr-x   0        0        0     1652 2023-12-01 18:07:24.317812 goodest-1.2.2/venues/stages/goodest/adventures/demux_hap/configs/__pycache__/HTTP_balancer.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3286 2023-12-01 18:05:41.851249 goodest-1.2.2/venues/stages/goodest/adventures/demux_hap/configs/examples/haproxy.cfg
+-rwxr-xr-x   0        0        0     2457 2023-12-01 21:46:11.432916 goodest-1.2.2/venues/stages/goodest/adventures/demux_hap/configs/examples/haproxy_2.cfg
+-rwxr-xr-x   0        0        0     2191 2024-01-25 05:03:52.719628 goodest-1.2.2/venues/stages/goodest/adventures/demux_hap/configs/external_reverse/__init__.py
+-rwxr-xr-x   0        0        0      217 2024-05-10 00:51:31.625387 goodest-1.2.2/venues/stages/goodest/adventures/demux_hap/demux.S.HTML
+-rwxr-xr-x   0        0        0      229 2023-12-02 01:03:02.539647 goodest-1.2.2/venues/stages/goodest/adventures/demux_hap/journalctl/journalctl.r.HTML
+-rwxr-xr-x   0        0        0      227 2023-12-02 01:02:28.789164 goodest-1.2.2/venues/stages/goodest/adventures/demux_hap/systemctl/systemctl.S.HTML
+-rwxr-xr-x   0        0        0       14 2024-04-24 01:06:32.184393 goodest-1.2.2/venues/stages/goodest/adventures/monetary/.gitignore
+-rwxr-xr-x   0        0        0      856 2024-05-13 01:04:39.753620 goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_inventory/__pycache__/connect.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1266 2024-05-13 01:04:39.753620 goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_inventory/_treasures/_indexes/__pycache__/drop_and_create.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1034 2024-05-13 00:59:57.240563 goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_inventory/_treasures/_indexes/drop_and_create.py
+-rwxr-xr-x   0        0        0      905 2024-05-13 00:59:57.240563 goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_inventory/connect.py
+-rwxr-xr-x   0        0        0     1041 2024-05-10 02:47:15.578725 goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_inventory/foods/_indexes/__pycache__/drop_and_create.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1370 2024-05-13 01:08:31.375266 goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_inventory/foods/document/__pycache__/find.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2028 2024-05-13 04:19:23.390074 goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_inventory/foods/document/__pycache__/insert.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1210 2024-05-13 00:59:57.236563 goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_inventory/foods/document/find.py
+-rwxr-xr-x   0        0        0     2182 2024-05-13 04:18:05.491009 goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_inventory/foods/document/insert.py
+-rwxr-xr-x   0        0        0      132 2024-05-13 00:59:57.240563 goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_inventory/goodest_inventory.S.HTML
+-rwxr-xr-x   0        0        0     1327 2024-05-13 01:08:31.375266 goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_inventory/supps/document/__pycache__/find.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1981 2024-05-12 23:53:44.710441 goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_inventory/supps/document/__pycache__/insert.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1156 2024-05-13 00:59:57.236563 goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_inventory/supps/document/find.py
+-rwxr-xr-x   0        0        0     2108 2024-05-13 04:18:36.698634 goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_inventory/supps/document/insert.py
+-rwxr-xr-x   0        0        0       17 2024-04-17 03:33:22.117283 goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_tract/.gitignore
+-rwxr-xr-x   0        0        0      454 2024-04-17 03:33:22.117283 goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_tract/__itinerary/itinerary.S.HTML
+-rwxr-xr-x   0        0        0     1820 2024-04-17 03:33:22.117283 goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_tract/__pycache__/clique.cpython-310.pyc
+-rwxr-xr-x   0        0        0      832 2024-05-13 01:08:31.263266 goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_tract/__pycache__/connect.cpython-310.pyc
+-rwxr-xr-x   0        0        0      799 2024-05-13 01:08:31.359266 goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_tract/_land/__pycache__/find_name.cpython-310.pyc
+-rwxr-xr-x   0        0        0        4 2024-04-28 00:13:51.336698 goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_tract/_land/__pycache__/insert_document.cpython-310.pyc
+-rwxr-xr-x   0        0        0      811 2024-05-13 01:08:31.263266 goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_tract/_land/__pycache__/retrieve_every.cpython-310.pyc
+-rwxr-xr-x   0        0        0      196 2024-04-24 22:53:29.564774 goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_tract/_land/_land.S.HTML
+-rwxr-xr-x   0        0        0      712 2024-05-13 00:59:57.236563 goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_tract/_land/find_name.py
+-rwxr-xr-x   0        0        0      934 2024-05-13 00:59:57.236563 goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_tract/_land/insert_document.py
+-rwxr-xr-x   0        0        0      613 2024-05-13 00:59:57.236563 goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_tract/_land/retrieve_every.py
+-rwxr-xr-x   0        0        0      170 2024-04-17 03:33:22.117283 goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_tract/cautionary_ingredients/cautionary_ingredients.S.HTML
+-rwxr-xr-x   0        0        0     1172 2024-05-13 00:59:57.236563 goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_tract/connect.py
+-rwxr-xr-x   0        0        0      721 2024-04-24 23:09:34.366674 goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_tract/essential_nutrients/essential_nutrients.S.HTML
+-rwxr-xr-x   0        0        0      401 2024-04-24 23:06:14.224847 goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_tract/glossary/glossary.S.HTML
+-rwxr-xr-x   0        0        0     1824 2024-05-14 00:11:11.229872 goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_tract/goals/__pycache__/find_ingredient.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1257 2024-05-13 02:41:11.683142 goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_tract/goals/__pycache__/insert.cpython-310.pyc
+-rwxr-xr-x   0        0        0      732 2024-05-13 02:42:37.938213 goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_tract/goals/__pycache__/retrieve.cpython-310.pyc
+-rwxr-xr-x   0        0        0      725 2024-05-13 21:38:26.763908 goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_tract/goals/__pycache__/retrieve_one.cpython-310.pyc
+-rwxr-xr-x   0        0        0      860 2024-04-28 02:43:34.943005 goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_tract/goals/_indexes/__pycache__/create.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1071 2024-05-02 22:26:24.276333 goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_tract/goals/_indexes/__pycache__/drop_and_create.cpython-310.pyc
+-rwxr-xr-x   0        0        0      840 2024-05-13 00:59:57.236563 goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_tract/goals/_indexes/drop_and_create.py
+-rwxr-xr-x   0        0        0     1843 2024-05-14 00:11:06.453950 goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_tract/goals/find_ingredient.py
+-rwxr-xr-x   0        0        0      117 2024-04-28 02:07:02.567921 goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_tract/goals/goals.S.HTML
+-rwxr-xr-x   0        0        0     1376 2024-05-13 02:41:09.559165 goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_tract/goals/insert.py
+-rwxr-xr-x   0        0        0      653 2024-05-13 02:42:27.038331 goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_tract/goals/retrieve.py
+-rwxr-xr-x   0        0        0      622 2024-05-13 19:28:44.851419 goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_tract/goals/retrieve_one.py
+-rwxr-xr-x   0        0        0     1489 2024-05-13 00:59:57.236563 goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_tract/ingredients.S.HTML
+-rwxr-xr-x   0        0        0        0 2024-04-17 03:33:22.113283 goodest-1.2.2/venues/stages/goodest/adventures/monetary/__init__.py
+-rwxr-xr-x   0        0        0      150 2024-04-17 03:36:48.047066 goodest-1.2.2/venues/stages/goodest/adventures/monetary/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1687 2024-04-17 03:33:22.113283 goodest-1.2.2/venues/stages/goodest/adventures/monetary/__pycache__/clique.cpython-310.pyc
+-rwxr-xr-x   0        0        0      680 2024-04-17 03:33:22.113283 goodest-1.2.2/venues/stages/goodest/adventures/monetary/__pycache__/connect.cpython-310.pyc
+-rwxr-xr-x   0        0        0      857 2024-04-17 03:33:22.113283 goodest-1.2.2/venues/stages/goodest/adventures/monetary/__pycache__/off.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1904 2024-04-17 03:33:22.113283 goodest-1.2.2/venues/stages/goodest/adventures/monetary/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1610 2024-04-23 19:31:08.342022 goodest-1.2.2/venues/stages/goodest/adventures/monetary/__pycache__/status.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1451 2024-05-13 01:04:39.757620 goodest-1.2.2/venues/stages/goodest/adventures/monetary/_ops/__pycache__/_clique.cpython-310.pyc
+-rwxr-xr-x   0        0        0      879 2024-05-13 01:04:39.757620 goodest-1.2.2/venues/stages/goodest/adventures/monetary/_ops/__pycache__/off.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2209 2024-05-13 01:04:39.713620 goodest-1.2.2/venues/stages/goodest/adventures/monetary/_ops/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1659 2024-05-13 01:04:39.713620 goodest-1.2.2/venues/stages/goodest/adventures/monetary/_ops/__pycache__/status.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1087 2024-05-13 00:59:57.232563 goodest-1.2.2/venues/stages/goodest/adventures/monetary/_ops/_clique.py
+-rwxr-xr-x   0        0        0      875 2024-05-13 00:59:57.232563 goodest-1.2.2/venues/stages/goodest/adventures/monetary/_ops/off.py
+-rwxr-xr-x   0        0        0     2712 2024-05-13 00:59:57.232563 goodest-1.2.2/venues/stages/goodest/adventures/monetary/_ops/on.py
+-rwxr-xr-x   0        0        0     1913 2024-05-13 01:04:39.761620 goodest-1.2.2/venues/stages/goodest/adventures/monetary/_ops/saves/__pycache__/_clique.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2152 2024-04-17 03:33:22.117283 goodest-1.2.2/venues/stages/goodest/adventures/monetary/_ops/saves/__pycache__/clique.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1651 2024-05-13 00:59:57.232563 goodest-1.2.2/venues/stages/goodest/adventures/monetary/_ops/saves/_clique.py
+-rwxr-xr-x   0        0        0     1442 2024-05-13 01:04:39.761620 goodest-1.2.2/venues/stages/goodest/adventures/monetary/_ops/saves/dumps/__pycache__/dump.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1428 2024-05-13 01:04:39.761620 goodest-1.2.2/venues/stages/goodest/adventures/monetary/_ops/saves/dumps/__pycache__/restore.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1580 2024-05-13 00:59:57.232563 goodest-1.2.2/venues/stages/goodest/adventures/monetary/_ops/saves/dumps/dump.py
+-rwxr-xr-x   0        0        0     1508 2024-05-13 00:59:57.232563 goodest-1.2.2/venues/stages/goodest/adventures/monetary/_ops/saves/dumps/restore.py
+-rwxr-xr-x   0        0        0     1407 2024-05-13 01:04:39.761620 goodest-1.2.2/venues/stages/goodest/adventures/monetary/_ops/saves/exports/__pycache__/monetary_export.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1398 2024-05-13 01:04:39.761620 goodest-1.2.2/venues/stages/goodest/adventures/monetary/_ops/saves/exports/__pycache__/monetary_import.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1463 2024-05-13 00:59:57.232563 goodest-1.2.2/venues/stages/goodest/adventures/monetary/_ops/saves/exports/monetary_export.py
+-rwxr-xr-x   0        0        0     1420 2024-05-13 00:59:57.232563 goodest-1.2.2/venues/stages/goodest/adventures/monetary/_ops/saves/exports/monetary_import.py
+-rwxr-xr-x   0        0        0      390 2024-04-23 20:10:51.728325 goodest-1.2.2/venues/stages/goodest/adventures/monetary/_ops/saves/memories.S.HTML
+-rwxr-xr-x   0        0        0     1797 2024-05-13 00:59:57.232563 goodest-1.2.2/venues/stages/goodest/adventures/monetary/_ops/status.py
+-rwxr-xr-x   0        0        0      459 2024-05-13 00:59:57.240563 goodest-1.2.2/venues/stages/goodest/adventures/monetary/monetary.S.HTML
+-rwxr-xr-x   0        0        0      631 2024-05-13 01:04:39.713620 goodest-1.2.2/venues/stages/goodest/adventures/monetary/moves/URL/__pycache__/retrieve.cpython-310.pyc
+-rwxr-xr-x   0        0        0      482 2024-05-13 00:59:57.232563 goodest-1.2.2/venues/stages/goodest/adventures/monetary/moves/URL/retrieve.py
+-rwxr-xr-x   0        0        0     1014 2024-05-13 00:59:57.236563 goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/__init__.py
+-rwxr-xr-x   0        0        0     1108 2024-05-13 01:08:31.375266 goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2093 2024-01-20 22:08:03.263097 goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1416 2024-01-18 21:56:05.761257 goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/scan_3.s.HTML
+-rwxr-xr-x   0        0        0      764 2024-05-13 00:41:57.767791 goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/__pycache__/limits.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1242 2024-01-17 21:00:52.050922 goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/__pycache__/limits.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3355 2024-01-18 01:45:49.087517 goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/__pycache__/stats.cpython-311.pyc
+-rwxr-xr-x   0        0        0      578 2024-05-13 00:17:13.283304 goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/limits.py
+-rwxr-xr-x   0        0        0     5944 2024-05-13 02:50:49.488923 goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/__init__.py
+-rwxr-xr-x   0        0        0     4822 2024-05-13 02:50:52.584894 goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     7791 2024-01-20 22:06:11.831292 goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      560 2024-02-05 15:21:50.027143 goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/affirm/__pycache__/direction.cpython-310.pyc
+-rwxr-xr-x   0        0        0      770 2024-01-19 00:57:06.516080 goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/affirm/__pycache__/direction.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1079 2024-01-19 21:24:23.060989 goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/affirm/__pycache__/filters.cpython-311.pyc
+-rwxr-xr-x   0        0        0      386 2024-01-19 00:13:41.687885 goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/affirm/direction.py
+-rwxr-xr-x   0        0        0      693 2024-02-05 15:21:50.035142 goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/__pycache__/before_and_after.cpython-310.pyc
+-rwxr-xr-x   0        0        0      842 2024-01-19 00:57:36.578735 goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/__pycache__/before_and_after.cpython-311.pyc
+-rwxr-xr-x   0        0        0      470 2024-02-05 15:21:50.031142 goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/__pycache__/check_fields.cpython-310.pyc
+-rwxr-xr-x   0        0        0      540 2024-01-19 00:57:36.577735 goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/__pycache__/check_fields.cpython-311.pyc
+-rwxr-xr-x   0        0        0      461 2024-02-05 15:21:50.031142 goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/__pycache__/lower_case_name.cpython-310.pyc
+-rwxr-xr-x   0        0        0      511 2024-01-19 00:57:36.578735 goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/__pycache__/lower_case_name.cpython-311.pyc
+-rwxr-xr-x   0        0        0      509 2024-02-05 15:21:50.031142 goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/__pycache__/sort_name_emblem.cpython-310.pyc
+-rwxr-xr-x   0        0        0      587 2024-01-19 00:57:36.578735 goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/__pycache__/sort_name_emblem.cpython-311.pyc
+-rwxr-xr-x   0        0        0      671 2024-02-05 15:21:50.031142 goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/__pycache__/unionize.cpython-310.pyc
+-rwxr-xr-x   0        0        0      847 2024-01-19 00:57:06.516080 goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/__pycache__/unionize.cpython-311.pyc
+-rwxr-xr-x   0        0        0      848 2024-01-19 00:29:46.750852 goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/before_and_after.py
+-rwxr-xr-x   0        0        0      170 2024-01-18 22:27:33.009237 goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/check_fields.py
+-rwxr-xr-x   0        0        0      514 2024-02-05 15:21:50.035142 goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/filters/__pycache__/limit.cpython-310.pyc
+-rwxr-xr-x   0        0        0      564 2024-01-19 01:20:04.182165 goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/filters/__pycache__/limit.cpython-311.pyc
+-rwxr-xr-x   0        0        0      524 2024-02-05 15:21:50.035142 goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/filters/__pycache__/scan_string.cpython-310.pyc
+-rwxr-xr-x   0        0        0      683 2024-01-19 00:57:36.578735 goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/filters/__pycache__/scan_string.cpython-311.pyc
+-rwxr-xr-x   0        0        0      683 2024-02-05 15:21:50.035142 goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/filters/__pycache__/vector_name.cpython-310.pyc
+-rwxr-xr-x   0        0        0      795 2024-01-19 00:57:36.579735 goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/filters/__pycache__/vector_name.cpython-311.pyc
+-rwxr-xr-x   0        0        0      939 2024-02-05 15:21:50.035142 goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/filters/__pycache__/vector_name_and_emblem.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1143 2024-01-19 21:47:13.310446 goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/filters/__pycache__/vector_name_and_emblem.cpython-311.pyc
+-rwxr-xr-x   0        0        0      618 2024-01-19 00:53:26.187609 goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/filters/filters.s.HTML
+-rwxr-xr-x   0        0        0      290 2024-01-19 01:19:36.215470 goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/filters/limit.py
+-rwxr-xr-x   0        0        0      238 2024-01-18 22:32:50.168704 goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/filters/scan_string.py
+-rwxr-xr-x   0        0        0     1208 2024-01-19 00:52:38.678154 goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/filters/vector_name.py
+-rwxr-xr-x   0        0        0     1977 2024-01-19 21:47:09.259509 goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/filters/vector_name_and_emblem.py
+-rwxr-xr-x   0        0        0      617 2024-02-15 00:15:32.679560 goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/formats/__pycache__/format_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      658 2024-01-20 22:07:26.051496 goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/formats/__pycache__/format_1.cpython-311.pyc
+-rwxr-xr-x   0        0        0      290 2024-02-15 00:15:31.703573 goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/formats/format_1.py
+-rwxr-xr-x   0        0        0      121 2024-01-18 22:29:05.056212 goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/lower_case_name.py
+-rwxr-xr-x   0        0        0      379 2024-01-19 00:29:48.264835 goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/sort_name_emblem.py
+-rwxr-xr-x   0        0        0      591 2024-01-19 00:29:46.767852 goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/unionize.py
+-rwxr-xr-x   0        0        0      665 2024-02-05 15:21:50.027143 goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/spruce/__pycache__/filters.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1169 2024-01-19 21:33:44.004002 goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/spruce/__pycache__/filters.cpython-311.pyc
+-rwxr-xr-x   0        0        0      528 2024-01-19 21:33:42.836021 goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/spruce/filters.py
+-rwxr-xr-x   0        0        0     1304 2024-05-13 00:45:24.741643 goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/stats/__init__.py
+-rwxr-xr-x   0        0        0      972 2024-05-13 00:45:27.617613 goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/stats/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1100 2024-01-19 19:16:29.681719 goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/stats/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3148 2024-01-19 00:55:25.534239 goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/stats/__pycache__/union.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3461 2024-05-13 00:59:57.236563 goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/stats/union.py
+-rwxr-xr-x   0        0        0     1343 2024-04-23 22:34:43.485503 goodest-1.2.2/venues/stages/goodest/adventures/redis_mix/_ops/__pycache__/off.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1759 2024-04-23 22:34:42.625513 goodest-1.2.2/venues/stages/goodest/adventures/redis_mix/_ops/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1288 2024-04-23 22:34:43.489503 goodest-1.2.2/venues/stages/goodest/adventures/redis_mix/_ops/__pycache__/refresh.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1311 2024-04-23 22:34:42.629513 goodest-1.2.2/venues/stages/goodest/adventures/redis_mix/_ops/__pycache__/status.cpython-310.pyc
+-rwxr-xr-x   0        0        0      802 2024-05-13 00:59:57.240563 goodest-1.2.2/venues/stages/goodest/adventures/redis_mix/_ops/_clique.py
+-rwxr-xr-x   0        0        0      332 2024-05-13 00:59:57.240563 goodest-1.2.2/venues/stages/goodest/adventures/redis_mix/_ops/off.py
+-rwxr-xr-x   0        0        0      329 2024-05-13 00:59:57.240563 goodest-1.2.2/venues/stages/goodest/adventures/redis_mix/_ops/on.py
+-rwxr-xr-x   0        0        0      334 2024-05-13 00:59:57.240563 goodest-1.2.2/venues/stages/goodest/adventures/redis_mix/_ops/refresh.py
+-rwxr-xr-x   0        0        0      343 2024-05-13 00:59:57.240563 goodest-1.2.2/venues/stages/goodest/adventures/redis_mix/_ops/status.py
+-rwxr-xr-x   0        0        0      130 2024-04-24 18:57:58.564669 goodest-1.2.2/venues/stages/goodest/adventures/redis_mix/redis_mix.S.HTML
+-rwxr-xr-x   0        0        0      730 2024-05-12 20:01:09.578795 goodest-1.2.2/venues/stages/goodest/adventures/sanique/[objectives]/objectives.S.HTML
+-rwxr-xr-x   0        0        0      188 2024-04-17 03:33:22.117283 goodest-1.2.2/venues/stages/goodest/adventures/sanique/__init__.py
+-rwxr-xr-x   0        0        0      598 2024-04-17 17:46:30.800270 goodest-1.2.2/venues/stages/goodest/adventures/sanique/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1415 2024-05-13 01:04:39.757620 goodest-1.2.2/venues/stages/goodest/adventures/sanique/_ops/__pycache__/off.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1920 2024-05-13 01:04:39.489623 goodest-1.2.2/venues/stages/goodest/adventures/sanique/_ops/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1362 2024-05-13 01:04:39.757620 goodest-1.2.2/venues/stages/goodest/adventures/sanique/_ops/__pycache__/refresh.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1330 2024-05-13 17:13:10.736946 goodest-1.2.2/venues/stages/goodest/adventures/sanique/_ops/__pycache__/status.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1467 2024-05-13 00:59:01.401145 goodest-1.2.2/venues/stages/goodest/adventures/sanique/_ops/off.py
+-rwxr-xr-x   0        0        0     1990 2024-05-13 00:59:01.401145 goodest-1.2.2/venues/stages/goodest/adventures/sanique/_ops/on.py
+-rwxr-xr-x   0        0        0     1235 2024-05-13 00:59:01.401145 goodest-1.2.2/venues/stages/goodest/adventures/sanique/_ops/refresh.py
+-rwxr-xr-x   0        0        0     1303 2024-05-13 17:13:01.173055 goodest-1.2.2/venues/stages/goodest/adventures/sanique/_ops/status.py
+-rwxr-xr-x   0        0        0     1064 2024-05-13 00:59:01.405145 goodest-1.2.2/venues/stages/goodest/adventures/sanique/_status/API_status_besties__food_USDA__nature_v2__FDC_ID_1.py
+-rwxr-xr-x   0        0        0     1199 2024-05-13 01:14:34.821033 goodest-1.2.2/venues/stages/goodest/adventures/sanique/_status/__pycache__/API_status_besties__food_USDA__nature_v2__FDC_ID_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      791 2024-05-13 00:59:01.401145 goodest-1.2.2/venues/stages/goodest/adventures/sanique/clique.py
+-rwxr-xr-x   0        0        0     4380 2024-05-13 23:54:27.255294 goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/__init__.py
+-rwxr-xr-x   0        0        0     3170 2024-05-13 23:54:41.334864 goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3636 2024-05-13 23:56:30.107741 goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/addresses/guest/__init__.py
+-rwxr-xr-x   0        0        0     3506 2024-05-13 23:56:33.579646 goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/addresses/guest/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2960 2024-05-14 01:57:22.804407 goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/addresses/guest/vue/__init__.py
+-rwxr-xr-x   0        0        0     2365 2024-05-14 01:57:30.320356 goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/addresses/guest/vue/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3335 2024-01-21 04:18:08.256227 goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/addresses/guest/vue/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      561 2024-05-08 21:23:06.200098 goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/addresses/guest/vue/caching.S.HTML
+-rwxr-xr-x   0        0        0     1658 2024-05-13 01:10:51.450510 goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/addresses/guest_bits/__init__.py
+-rwxr-xr-x   0        0        0     1187 2024-05-13 01:11:00.310457 goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/addresses/guest_bits/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      168 2024-05-12 20:24:56.030964 goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/addresses/guest_bits/bits.S.HTML
+-rwxr-xr-x   0        0        0     3242 2024-05-13 02:52:14.056108 goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/addresses/guest_goodest_inventory/foods/__init__.py
+-rwxr-xr-x   0        0        0     2485 2024-05-13 02:52:19.484055 goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/addresses/guest_goodest_inventory/foods/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      696 2024-05-13 00:59:01.405145 goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/addresses/guest_goodest_inventory/recipes/__init__.py
+-rwxr-xr-x   0        0        0      907 2024-05-13 01:11:00.310457 goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/addresses/guest_goodest_inventory/recipes/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      687 2024-05-13 00:59:01.405145 goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/addresses/guest_goodest_inventory/supps/__init__.py
+-rwxr-xr-x   0        0        0      892 2024-05-13 01:11:00.310457 goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/addresses/guest_goodest_inventory/supps/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3101 2024-05-13 23:36:01.872117 goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/addresses/staff/__init__.py
+-rwxr-xr-x   0        0        0     2834 2024-05-13 23:47:08.646472 goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/addresses/staff/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1608 2024-05-13 22:57:24.026758 goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/addresses/staff/__pycache__/besties__food_USDA__nature_v2__FDC_ID.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1573 2024-05-13 22:57:24.026758 goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/addresses/staff/__pycache__/besties__supp_NIH__nature_v2__DSLD_ID.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1722 2024-05-13 22:56:54.814945 goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/addresses/staff/besties__food_USDA__nature_v2__FDC_ID.py
+-rwxr-xr-x   0        0        0     1480 2024-05-13 22:56:59.294916 goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/addresses/staff/besties__supp_NIH__nature_v2__DSLD_ID.py
+-rwxr-xr-x   0        0        0      283 2024-05-08 23:22:18.957260 goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/addresses/staff/protected.S.HTML
+-rwxr-xr-x   0        0        0     1734 2024-05-14 00:13:46.691384 goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/addresses/staff_goodest_inventory/foods/__init__.py
+-rwxr-xr-x   0        0        0     2011 2024-05-14 00:16:09.005179 goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/addresses/staff_goodest_inventory/foods/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      837 2024-05-13 23:36:20.623959 goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/addresses/staff_goodest_inventory/recipes/__init__.py
+-rwxr-xr-x   0        0        0     1107 2024-05-13 23:47:08.746471 goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/addresses/staff_goodest_inventory/recipes/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1416 2024-05-14 00:14:11.990987 goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/addresses/staff_goodest_inventory/supps/__init__.py
+-rwxr-xr-x   0        0        0     1590 2024-05-14 00:16:09.009179 goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/addresses/staff_goodest_inventory/supps/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      425 2024-05-13 00:59:01.401145 goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/sockets_guest/__init__.py
+-rwxr-xr-x   0        0        0      726 2024-05-13 01:08:31.003267 goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/sockets_guest/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1008 2024-05-12 22:50:40.664451 goodest-1.2.2/venues/stages/goodest/adventures/sanique/quests_guests/__pycache__/find_food.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1374 2024-05-13 22:06:23.071845 goodest-1.2.2/venues/stages/goodest/adventures/sanique/quests_guests/__pycache__/retrieve_food.cpython-310.pyc
+-rwxr-xr-x   0        0        0      625 2024-05-13 02:35:09.679038 goodest-1.2.2/venues/stages/goodest/adventures/sanique/quests_guests/__pycache__/retrieve_goals.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1191 2024-05-13 03:57:04.720471 goodest-1.2.2/venues/stages/goodest/adventures/sanique/quests_guests/__pycache__/retrieve_recipe.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1167 2024-05-13 22:16:56.062569 goodest-1.2.2/venues/stages/goodest/adventures/sanique/quests_guests/__pycache__/retrieve_supp.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1908 2024-05-13 02:00:30.545915 goodest-1.2.2/venues/stages/goodest/adventures/sanique/quests_guests/__pycache__/search_goods.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1922 2024-05-13 22:06:05.327965 goodest-1.2.2/venues/stages/goodest/adventures/sanique/quests_guests/retrieve_food.py
+-rwxr-xr-x   0        0        0      373 2024-05-13 02:29:10.122901 goodest-1.2.2/venues/stages/goodest/adventures/sanique/quests_guests/retrieve_goal.py
+-rwxr-xr-x   0        0        0      405 2024-05-13 02:35:06.463072 goodest-1.2.2/venues/stages/goodest/adventures/sanique/quests_guests/retrieve_goals.py
+-rwxr-xr-x   0        0        0     1103 2024-05-13 03:57:01.616503 goodest-1.2.2/venues/stages/goodest/adventures/sanique/quests_guests/retrieve_recipe.py
+-rwxr-xr-x   0        0        0     1500 2024-05-13 22:16:53.362595 goodest-1.2.2/venues/stages/goodest/adventures/sanique/quests_guests/retrieve_supp.py
+-rwxr-xr-x   0        0        0     2488 2024-05-13 02:00:26.473964 goodest-1.2.2/venues/stages/goodest/adventures/sanique/quests_guests/search_goods.py
+-rwxr-xr-x   0        0        0      530 2024-05-13 00:59:01.405145 goodest-1.2.2/venues/stages/goodest/adventures/sanique/sanique.S.HTML
+-rwxr-xr-x   0        0        0     1200 2024-05-09 23:05:53.524539 goodest-1.2.2/venues/stages/goodest/adventures/sanique/utilities/__pycache__/generate_inventory_paths.cpython-310.pyc
+-rwxr-xr-x   0        0        0      388 2024-04-17 03:36:47.855070 goodest-1.2.2/venues/stages/goodest/adventures/sanique/utilities/__pycache__/has_sanic_check.cpython-310.pyc
+-rwxr-xr-x   0        0        0      533 2024-05-13 01:14:35.297030 goodest-1.2.2/venues/stages/goodest/adventures/sanique/utilities/__pycache__/retrieve_sanique_URL.cpython-310.pyc
+-rwxr-xr-x   0        0        0      539 2024-05-13 00:59:01.401145 goodest-1.2.2/venues/stages/goodest/adventures/sanique/utilities/check_key/__init__.py
+-rwxr-xr-x   0        0        0      786 2024-05-13 01:08:31.259266 goodest-1.2.2/venues/stages/goodest/adventures/sanique/utilities/check_key/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1538 2024-05-09 23:04:59.513271 goodest-1.2.2/venues/stages/goodest/adventures/sanique/utilities/generate_inventory_paths.py
+-rwxr-xr-x   0        0        0      167 2024-04-17 03:33:22.117283 goodest-1.2.2/venues/stages/goodest/adventures/sanique/utilities/has_sanic_check.py
+-rwxr-xr-x   0        0        0      296 2024-05-13 00:59:01.401145 goodest-1.2.2/venues/stages/goodest/adventures/sanique/utilities/retrieve_sanique_URL.py
+-rwxr-xr-x   0        0        0      127 2024-05-08 19:30:19.000000 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/.eslintrc.js--
+-rwxr-xr-x   0        0        0       94 2024-05-08 19:30:19.000000 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/.gitignore
+-rwxr-xr-x   0        0        0       26 2024-05-08 19:30:19.000000 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/.npmrc
+-rwxr-xr-x   0        0        0      939 2024-05-08 19:30:19.000000 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/README.md
+-rwxr-xr-x   0        0        0     1285 2024-05-08 20:46:06.699827 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/__objectives/objectives -- possibilities.S.HTML
+-rwxr-xr-x   0        0        0       27 2024-05-08 20:45:59.995896 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/__objectives/objectives.S.HTML
+-rwxr-xr-x   0        0        0        2 2024-05-08 21:03:01.449010 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/_controls/off.py
+-rwxr-xr-x   0        0        0        0 2024-05-08 21:06:04.803018 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/_controls/on.py
+-rwxr-xr-x   0        0        0      127 2024-05-08 19:30:19.000000 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/school/.eslintrc.cjs
+-rwxr-xr-x   0        0        0      731 2024-05-14 01:18:18.804759 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/school/dist/assets/index-DQHR7vKm.js
+-rwxr-xr-x   0        0        0      378 2024-05-14 01:18:18.804759 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/school/dist/index.html
+-rwxr-xr-x   0        0        0     1435 2024-05-14 01:18:18.704761 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/school/dist/typescript.svg
+-rwxr-xr-x   0        0        0     1497 2024-05-14 01:18:18.704761 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/school/dist/vite.svg
+-rwxr-xr-x   0        0        0      353 2024-05-09 21:32:18.768121 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/school/index.html
+-rwxr-xr-x   0        0        0      370 2024-05-10 02:14:54.482607 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/school/package.json
+-rwxr-xr-x   0        0        0     1435 2024-05-08 19:30:19.000000 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/school/public/typescript.svg
+-rwxr-xr-x   0        0        0     1497 2024-05-08 19:30:19.000000 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/school/public/vite.svg
+-rwxr-xr-x   0        0        0       23 2024-05-09 21:32:59.207717 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/school/src/main.js
+-rwxr-xr-x   0        0        0       75 2024-05-08 19:30:19.000000 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/school/tsconfig.json--
+-rwxr-xr-x   0        0        0      365 2024-05-10 02:14:10.075052 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/school/vite.config.js
+-rwxr-xr-x   0        0        0      127 2024-05-08 19:30:19.000000 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/staff/.eslintrc.cjs
+-rwxr-xr-x   0        0        0      711 2024-05-14 01:18:18.752760 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/staff/dist/assets/index-B5Qt9EMX.js
+-rwxr-xr-x   0        0        0      388 2024-05-14 01:18:18.752760 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/staff/dist/index.html
+-rwxr-xr-x   0        0        0     1435 2024-05-14 01:18:18.644761 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/staff/dist/typescript.svg
+-rwxr-xr-x   0        0        0     1497 2024-05-14 01:18:18.644761 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/staff/dist/vite.svg
+-rwxr-xr-x   0        0        0      363 2024-05-09 21:34:48.778605 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/staff/index.html
+-rwxr-xr-x   0        0        0      397 2024-05-10 02:10:36.785101 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/staff/package.json
+-rwxr-xr-x   0        0        0     1435 2024-05-08 19:30:19.000000 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/staff/public/typescript.svg
+-rwxr-xr-x   0        0        0     1497 2024-05-08 19:30:19.000000 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/staff/public/vite.svg
+-rwxr-xr-x   0        0        0        1 2024-05-09 21:33:50.275202 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/staff/src/main.js
+-rwxr-xr-x   0        0        0      367 2024-05-10 02:08:38.618156 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/staff/vite.config.js
+-rwxr-xr-x   0        0        0      127 2024-05-08 19:30:19.000000 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/.eslintrc.cjs--
+-rwxr-xr-x   0        0        0      556 2024-05-08 22:05:09.904886 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/.eslintrc.json
+-rwxr-xr-x   0        0        0     1156 2024-05-14 00:06:31.058668 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/index.html
+-rwxr-xr-x   0        0        0     2220 2024-05-14 01:53:23.421983 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/package.json
+-rwxr-xr-x   0        0        0     2369 2024-05-12 21:40:53.463627 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/Earth/app.js
+-rwxr-xr-x   0        0        0     1704 2024-05-14 00:16:03.101269 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/Earth/logistics/guests/index.js
+-rwxr-xr-x   0        0        0      800 2024-05-11 00:47:10.035262 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/Earth/logistics/index.js
+-rwxr-xr-x   0        0        0       27 2023-12-08 17:29:39.919713 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/Earth/logistics/logistics.s.HTML
+-rwxr-xr-x   0        0        0      205 2024-05-11 00:47:10.019262 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/Earth/logistics/staff/index.js
+-rwxr-xr-x   0        0        0      893 2024-05-11 00:12:34.448880 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/Earth/logistics/status/index.js
+-rwxr-xr-x   0        0        0      229 2024-02-02 20:25:55.023588 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/Earth/logistics/workshop/index.js
+-rwxr-xr-x   0        0        0      286 2024-03-06 23:00:24.198272 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/Earth/scenery/planet/components/local_storage_flip/decor.js
+-rwxr-xr-x   0        0        0      335 2024-03-06 23:20:10.831615 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/Earth/scenery/planet/components/local_storage_flip/decor.vue
+-rwxr-xr-x   0        0        0     2544 2024-05-09 19:36:44.871475 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/Earth/scenery/planet/field.js
+-rwxr-xr-x   0        0        0     2442 2024-03-25 23:22:40.575764 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/Earth/scenery/planet/field.vue
+-rwxr-xr-x   0        0        0     1202 2024-03-21 19:29:12.760368 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/Earth/warehouses/layout/index.js
+-rwxr-xr-x   0        0        0       26 2024-02-18 21:37:35.527677 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/apps.S.HTML
+-rwxr-xr-x   0        0        0     1455 2024-03-31 04:39:51.030367 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/fields/app/index.js
+-rwxr-xr-x   0        0        0     1590 2024-03-31 04:39:16.990772 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/fields/append.js
+-rwxr-xr-x   0        0        0      811 2024-02-19 01:14:44.725717 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/fields/boundary/embellishments.js
+-rwxr-xr-x   0        0        0     3144 2024-02-19 03:39:47.599945 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/fields/boundary/embellishments.vue
+-rwxr-xr-x   0        0        0      716 2024-05-09 19:36:44.871475 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/fields/fields.S.HTML
+-rwxr-xr-x   0        0        0     2024 2024-02-20 02:24:26.825728 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/fields/hacienda/eco.js
+-rwxr-xr-x   0        0        0      762 2024-03-30 03:27:25.126133 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/fields/hacienda/eco.vue
+-rwxr-xr-x   0        0        0     1215 2024-02-19 03:34:56.055049 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/fields/hacienda/methods/fn/keypress.js
+-rwxr-xr-x   0        0        0     1950 2024-02-19 03:11:56.242621 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/fields/hacienda/methods/index.js
+-rwxr-xr-x   0        0        0      330 2023-12-13 05:57:32.245095 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/fields/moves/build_field_element.js
+-rwxr-xr-x   0        0        0      208 2023-12-13 05:58:02.416723 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/fields/moves/get_next_coordinate.js
+-rwxr-xr-x   0        0        0      153 2023-12-13 05:44:37.428631 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/fields/moves/variables.js
+-rwxr-xr-x   0        0        0      739 2024-03-30 19:18:20.469563 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/fields/remove.js
+-rwxr-xr-x   0        0        0     2015 2023-08-08 03:01:34.460945 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/assets/base--.css
+-rwxr-xr-x   0        0        0      276 2023-08-08 02:05:29.442900 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/assets/logo.svg
+-rwxr-xr-x   0        0        0      373 2023-11-14 00:07:17.821680 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/assets/main.css
+-rwxr-xr-x   0        0        0      107 2024-05-10 22:52:00.937025 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/constants/index.js
+-rwxr-xr-x   0        0        0     1248 2024-05-13 00:59:57.080565 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/fleet/ask/get.js
+-rwxr-xr-x   0        0        0      218 2024-05-12 22:34:30.027372 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/fleet/fleet.s.HTML
+-rwxr-xr-x   0        0        0      744 2024-05-13 03:57:29.508215 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/fleet/goodest_DB/essential_nutrients/recipe/index.js
+-rwxr-xr-x   0        0        0      628 2024-05-13 17:41:19.302286 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/fleet/goodest_DB/food/retrieve/index.js
+-rwxr-xr-x   0        0        0      602 2024-05-13 17:41:43.085996 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/fleet/goodest_DB/supp/retrieve/index.js
+-rwxr-xr-x   0        0        0      596 2024-05-13 00:59:57.080565 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/fleet/goodest_DB/treasures/search/index.js
+-rwxr-xr-x   0        0        0      389 2024-05-13 02:27:50.727752 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/fleet/nutrition_meadow/goals/scan.js
+-rwxr-xr-x   0        0        0      397 2024-05-13 02:27:55.755698 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/fleet/nutrition_meadow/goals/scan_emblem.js
+-rwxr-xr-x   0        0        0     1115 2024-05-13 00:49:31.551077 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/fleet/syllabus/lap/index.js
+-rwxr-xr-x   0        0        0      131 2024-02-13 05:37:01.717416 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/fleet/syllabus/lap/index.s.HTML
+-rwxr-xr-x   0        0        0      881 2023-12-08 23:49:09.502834 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/Fraction/to_float.ST.js
+-rwxr-xr-x   0        0        0      702 2023-12-12 01:06:28.803271 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/Fraction/to_float.js
+-rwxr-xr-x   0        0        0      204 2023-09-13 18:17:19.482855 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/PERCENTIZE/FRACTION.ST.js
+-rwxr-xr-x   0        0        0      159 2023-11-07 02:46:35.479079 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/PERCENTIZE/FRACTION.js
+-rwxr-xr-x   0        0        0      497 2024-02-13 05:22:20.703032 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/PERSIST/index.js
+-rwxr-xr-x   0        0        0      212 2023-12-08 02:24:16.484912 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/assert/equal.js
+-rwxr-xr-x   0        0        0      348 2023-11-02 01:04:18.515660 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/circuit/index.js
+-rwxr-xr-x   0        0        0      373 2024-02-05 20:27:55.449652 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/document_title/document_title.s.HTML
+-rwxr-xr-x   0        0        0      273 2024-02-12 00:35:32.740011 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/element-tree/element-tree.s.HTML
+-rwxr-xr-x   0        0        0     1090 2024-02-02 19:24:05.871600 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/food/FIND_ENERGY_PER_GRAM.js
+-rwxr-xr-x   0        0        0      227 2024-02-02 19:24:05.914600 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/food/FIND_TEAM.js
+-rwxr-xr-x   0        0        0      208 2023-11-02 01:35:32.692959 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/food/find_name.js
+-rwxr-xr-x   0        0        0      198 2024-02-02 19:24:05.892600 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/food/find_stats_link.js
+-rwxr-xr-x   0        0        0      174 2023-11-02 01:36:19.736289 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/food/food.r.html
+-rwxr-xr-x   0        0        0      841 2024-02-12 01:38:07.918853 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/furnish/array.js
+-rwxr-xr-x   0        0        0      676 2024-02-12 01:38:26.850644 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/furnish/array.status.js
+-rwxr-xr-x   0        0        0      994 2024-02-12 01:39:02.930246 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/furnish/index.js
+-rwxr-xr-x   0        0        0      407 2023-11-07 01:16:23.318853 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/furnish/index.status.js
+-rwxr-xr-x   0        0        0      828 2024-02-12 01:39:31.409932 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/furnish/string.js
+-rwxr-xr-x   0        0        0      753 2023-11-02 01:53:09.683957 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/furnish/string.status.js
+-rwxr-xr-x   0        0        0     1443 2023-11-01 23:25:43.495916 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/monitors/focus.js
+-rwxr-xr-x   0        0        0      307 2023-12-16 01:10:42.413067 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/brand/name.js
+-rwxr-xr-x   0        0        0    19575 2023-12-08 22:35:11.870201 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/essential_nutrients/grove/calc_linear_grove/grove-1.js
+-rwxr-xr-x   0        0        0      986 2023-12-08 22:47:39.547348 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/essential_nutrients/grove/calc_linear_grove/index.ST.js
+-rwxr-xr-x   0        0        0     1098 2024-03-29 22:13:21.370645 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/essential_nutrients/grove/calc_linear_grove/index.js
+-rwxr-xr-x   0        0        0      534 2023-12-17 02:09:13.722149 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/essential_nutrients/grove/ingredient/biological_activity.js
+-rwxr-xr-x   0        0        0      451 2023-12-09 01:07:30.680541 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/essential_nutrients/grove/ingredient/mass_plus_mass_eq.js
+-rwxr-xr-x   0        0        0      307 2023-12-16 01:00:27.201226 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/essential_nutrients/grove/ingredient/name_0.js
+-rwxr-xr-x   0        0        0    19583 2023-12-09 00:19:43.841136 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/essential_nutrients/grove/sort/cryo/grove-1.js
+-rwxr-xr-x   0        0        0     1033 2023-12-09 00:47:16.810756 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/essential_nutrients/grove/sort/index.2.ST.js
+-rwxr-xr-x   0        0        0      762 2024-03-29 21:09:30.234921 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/essential_nutrients/grove/sort/index.ST.js
+-rwxr-xr-x   0        0        0     2893 2024-03-29 21:07:07.864628 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/essential_nutrients/grove/sort/index.js
+-rwxr-xr-x   0        0        0      318 2023-12-16 01:07:05.372883 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/identity/name.js
+-rwxr-xr-x   0        0        0      321 2023-12-08 17:26:20.969221 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/product/find_brand_name.js
+-rwxr-xr-x   0        0        0      370 2023-11-02 03:41:07.550130 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/product/find_name.js
+-rwxr-xr-x   0        0        0      333 2023-12-08 17:22:41.038887 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/product/find_product_name.js
+-rwxr-xr-x   0        0        0      367 2023-11-02 03:39:40.191371 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/product/find_stats_link.js
+-rwxr-xr-x   0        0        0      522 2023-11-02 02:34:36.978741 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/product/is.js
+-rwxr-xr-x   0        0        0      281 2023-11-15 03:58:43.852449 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/product/kind.ST.js
+-rwxr-xr-x   0        0        0      291 2023-11-15 03:59:01.299303 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/product/kind.js
+-rwxr-xr-x   0        0        0        0 2023-11-13 20:01:59.479392 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/product/mass/index.js
+-rwxr-xr-x   0        0        0      375 2023-11-13 21:26:12.604024 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/product/quantified_grove/sort.ST.js
+-rwxr-xr-x   0        0        0     1921 2023-12-08 04:04:27.829816 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/product/quantified_grove/sort.js
+-rwxr-xr-x   0        0        0     3116 2024-02-02 20:18:47.275475 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nutrients--/sort/index.ST.js
+-rwxr-xr-x   0        0        0     1456 2023-09-13 19:07:48.507970 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nutrients--/sort/index.js
+-rwxr-xr-x   0        0        0      196 2023-11-07 01:47:24.334036 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/object/has_field.js
+-rwxr-xr-x   0        0        0        9 2023-09-22 19:27:47.727905 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/processor/index.js
+-rwxr-xr-x   0        0        0        8 2023-09-22 19:27:42.190982 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/queue/index.js
+-rwxr-xr-x   0        0        0      882 2023-12-08 23:08:26.437630 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/round_quantity/index.ST.js
+-rwxr-xr-x   0        0        0      645 2023-12-09 04:44:44.573476 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/round_quantity/index.js
+-rwxr-xr-x   0        0        0     2106 2023-11-13 20:35:06.226320 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/struct_2/ingredient/mass.ST.js
+-rwxr-xr-x   0        0        0     1463 2023-11-13 20:35:15.278220 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/struct_2/ingredient/mass.js
+-rwxr-xr-x   0        0        0      349 2023-11-02 03:40:22.158775 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/struct_2/product/find_brand_name.js
+-rwxr-xr-x   0        0        0      370 2023-11-02 03:41:07.550130 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/struct_2/product/find_name.js
+-rwxr-xr-x   0        0        0      363 2023-11-02 03:49:19.294141 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/struct_2/product/find_product_name.js
+-rwxr-xr-x   0        0        0      367 2023-11-02 03:39:40.191371 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/struct_2/product/find_stats_link.js
+-rwxr-xr-x   0        0        0      522 2023-11-02 02:34:36.978741 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/struct_2/product/is.js
+-rwxr-xr-x   0        0        0      281 2023-11-15 03:58:43.852449 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/struct_2/product/kind.ST.js
+-rwxr-xr-x   0        0        0      291 2023-11-15 03:59:01.299303 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/struct_2/product/kind.js
+-rwxr-xr-x   0        0        0        0 2023-11-13 20:01:59.479392 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/struct_2/product/mass/index.js
+-rwxr-xr-x   0        0        0      375 2023-11-13 21:26:12.604024 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/struct_2/product/quantified_grove/sort.ST.js
+-rwxr-xr-x   0        0        0     1920 2023-12-08 23:49:54.502496 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/struct_2/product/quantified_grove/sort.js
+-rwxr-xr-x   0        0        0      205 2024-02-02 20:05:48.697210 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/wait_for.js
+-rwxr-xr-x   0        0        0       59 2024-02-11 19:01:30.792959 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/main.js
+-rwxr-xr-x   0        0        0      282 2024-02-02 20:07:26.009544 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/_template/field.js
+-rwxr-xr-x   0        0        0      165 2023-12-13 00:55:20.087280 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/_template/field.vue
+-rwxr-xr-x   0        0        0       85 2024-03-21 19:09:31.608077 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/about/about.S.HTML
+-rwxr-xr-x   0        0        0      564 2024-01-19 23:32:34.020141 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/about/decor.js
+-rwxr-xr-x   0        0        0     2922 2024-05-13 00:59:57.100565 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/about/decor.vue
+-rwxr-xr-x   0        0        0      253 2024-03-30 19:18:20.557562 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/about/open.js
+-rwxr-xr-x   0        0        0      897 2024-05-11 00:16:05.358492 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/controls/decor/custom/decor.vue
+-rwxr-xr-x   0        0        0     2338 2024-05-11 00:16:31.550197 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/controls/decor/generic/decor.vue
+-rwxr-xr-x   0        0        0      676 2023-11-10 00:33:31.498239 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/controls/decor/references/decor.vue
+-rwxr-xr-x   0        0        0      915 2024-05-10 22:56:04.106070 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/controls/decor.js
+-rwxr-xr-x   0        0        0      474 2024-05-11 00:40:59.670388 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/controls/decor.s.HTML
+-rwxr-xr-x   0        0        0     1043 2024-05-10 21:22:09.919119 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/controls/decor.vue
+-rwxr-xr-x   0        0        0     1119 2023-09-21 01:20:42.255138 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/controls/notes/ARIA/roles.r.html
+-rwxr-xr-x   0        0        0      303 2023-11-26 17:48:20.650243 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/controls/notes/Windows/notes.r.html
+-rwxr-xr-x   0        0        0       82 2023-09-27 22:36:56.542685 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/controls/notes/linux/NOTES.HTML
+-rwxr-xr-x   0        0        0     1050 2023-11-26 17:48:20.630243 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/controls/notes/notes.r.html
+-rwxr-xr-x   0        0        0     1148 2024-03-30 03:28:33.537352 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/controls/priorities/possibilities.s.HTML
+-rwxr-xr-x   0        0        0      620 2024-03-30 19:18:20.553562 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/empty_cart/field.js
+-rwxr-xr-x   0        0        0      650 2023-12-13 06:11:58.148410 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/empty_cart/field.vue
+-rwxr-xr-x   0        0        0      501 2024-03-15 03:09:43.926060 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/goal/features.js
+-rwxr-xr-x   0        0        0      300 2024-03-15 00:08:58.070241 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/goal/features.vue
+-rwxr-xr-x   0        0        0      249 2024-03-30 19:18:20.553562 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/goal/open.js
+-rwxr-xr-x   0        0        0       55 2024-03-31 04:40:52.717638 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/ingredient/feature.js
+-rwxr-xr-x   0        0        0      569 2024-03-31 04:42:03.016814 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/ingredient/feature.vue
+-rwxr-xr-x   0        0        0      380 2024-03-31 04:39:06.150901 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/ingredient/open.js
+-rwxr-xr-x   0        0        0     2738 2024-02-12 01:43:57.151144 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/navigation-lab/field.js
+-rwxr-xr-x   0        0        0     2257 2024-02-11 23:57:55.473669 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/navigation-lab/field.vue
+-rwxr-xr-x   0        0        0      179 2024-05-10 22:53:28.043951 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/parcels.s.HTML
+-rwxr-xr-x   0        0        0     1852 2024-05-09 19:36:44.919475 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/physics/field.js
+-rwxr-xr-x   0        0        0     1259 2024-03-21 17:53:56.773315 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/physics/field.vue
+-rwxr-xr-x   0        0        0      261 2024-05-09 19:36:44.919475 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/physics/open.js
+-rwxr-xr-x   0        0        0      864 2024-05-14 00:40:55.296193 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/scan_filter_by/field.js
+-rwxr-xr-x   0        0        0      866 2024-05-14 00:41:11.672024 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/scan_filter_by/field.vue
+-rwxr-xr-x   0        0        0      321 2024-03-30 19:18:20.549562 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/scan_filter_by/open.js
+-rwxr-xr-x   0        0        0      286 2024-02-18 23:10:18.011339 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/scan_sort_by/field.js
+-rwxr-xr-x   0        0        0      350 2024-02-11 23:57:55.657667 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/scan_sort_by/field.vue
+-rwxr-xr-x   0        0        0      309 2024-03-30 19:18:20.549562 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/scan_sort_by/open.js
+-rwxr-xr-x   0        0        0       29 2024-02-05 20:30:45.897227 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/search filter/field.js
+-rwxr-xr-x   0        0        0      352 2024-02-11 23:57:55.825665 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/search filter/field.vue
+-rwxr-xr-x   0        0        0     1475 2024-05-09 01:16:32.527415 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/sink-filter/field.js
+-rwxr-xr-x   0        0        0     6354 2024-05-09 01:02:12.873953 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/sink-filter/field.vue
+-rwxr-xr-x   0        0        0      302 2024-03-30 19:18:20.553562 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/sink-filter/open.js
+-rwxr-xr-x   0        0        0       44 2024-02-19 04:49:00.682527 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/sink-filter/slides/slide-1/scenery.vue
+-rwxr-xr-x   0        0        0     1042 2024-05-13 00:59:57.100565 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/sink-filter/steps.S.HTML
+-rwxr-xr-x   0        0        0     1112 2024-02-16 03:50:07.925341 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/sink-filter/steps_v1.S.HTML
+-rwxr-xr-x   0        0        0     1072 2024-05-13 00:59:57.100565 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/sink-filter/steps_v2.S.HTML
+-rwxr-xr-x   0        0        0      240 2024-03-30 19:18:20.541562 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/unit_systems/decor/system_international_with_food_calories_and_IU/field.js
+-rwxr-xr-x   0        0        0     2352 2024-02-05 20:31:31.369067 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/unit_systems/decor/system_international_with_food_calories_and_IU/field.vue
+-rwxr-xr-x   0        0        0      418 2024-03-30 19:18:20.541562 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/unit_systems/field.js
+-rwxr-xr-x   0        0        0      384 2024-03-30 19:18:20.537562 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/unit_systems/field.vue
+-rwxr-xr-x   0        0        0       25 2024-02-05 20:32:55.188729 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/unreported/field.js
+-rwxr-xr-x   0        0        0      725 2024-02-11 23:57:55.953664 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/unreported/field.vue
+-rwxr-xr-x   0        0        0     1392 2024-03-30 19:18:20.497563 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/__shows_d3/decor.vue
+-rwxr-xr-x   0        0        0      159 2023-11-07 02:31:40.330665 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/__shows_d3/theatrics/ERROR.vue
+-rwxr-xr-x   0        0        0     1165 2024-03-30 19:18:20.493563 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/__shows_d3/theatrics/NETWORK_2/field.js
+-rwxr-xr-x   0        0        0      135 2024-03-30 19:18:20.489563 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/__shows_d3/theatrics/NETWORK_2/field.vue
+-rwxr-xr-x   0        0        0     5571 2023-10-16 00:06:58.093758 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/__shows_d3/theatrics/NETWORK_D3_2/PHYSICAL/index.js
+-rwxr-xr-x   0        0        0     1923 2024-03-30 19:18:20.493563 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/__shows_d3/theatrics/NETWORK_D3_2/field.js
+-rwxr-xr-x   0        0        0      251 2024-03-30 19:18:20.493563 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/__shows_d3/theatrics/NETWORK_D3_2/field.vue
+-rwxr-xr-x   0        0        0     2649 2024-03-30 19:18:20.497563 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/__shows_d3/theatrics/NETWORK_D3_3/field.js
+-rwxr-xr-x   0        0        0      341 2024-03-30 19:18:20.497563 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/__shows_d3/theatrics/NETWORK_D3_3/field.vue
+-rwxr-xr-x   0        0        0      262 2023-10-16 00:43:32.202900 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/__shows_d3/theatrics/NETWORK_D3_3/methods/FIND_STRUCTURE.js
+-rwxr-xr-x   0        0        0     6029 2023-11-09 01:36:29.097181 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/__shows_d3/theatrics/NETWORK_D3_3/methods/PHYSICAL/index.js
+-rwxr-xr-x   0        0        0     1802 2023-11-09 01:35:18.334938 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/__shows_d3/theatrics/NETWORK_D3_3/methods/reinvigorate.js
+-rwxr-xr-x   0        0        0        2 2023-11-09 02:22:38.537393 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/__shows_d3/theatrics/intro/show.js
+-rwxr-xr-x   0        0        0      792 2023-11-09 02:23:32.503812 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/__shows_d3/theatrics/intro/show.vue
+-rwxr-xr-x   0        0        0     4310 2023-11-09 01:27:57.103654 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/__shows_d3/theatrics/net/field.js
+-rwxr-xr-x   0        0        0      135 2023-11-09 01:26:19.886675 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/__shows_d3/theatrics/net/field.vue
+-rwxr-xr-x   0        0        0      172 2024-05-13 00:59:57.092565 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/bests/decor.vue
+-rwxr-xr-x   0        0        0     2053 2024-05-13 04:20:41.973139 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/cart/decor.js
+-rwxr-xr-x   0        0        0     2540 2024-03-22 00:08:58.862157 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/cart/decor.vue
+-rwxr-xr-x   0        0        0        0 2023-09-01 01:58:11.319246 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/comparisons/region.js
+-rwxr-xr-x   0        0        0       38 2023-09-01 02:02:20.555211 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/comparisons/region.vue
+-rwxr-xr-x   0        0        0       14 2024-03-07 01:00:36.002731 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/customer.s.HTML
+-rwxr-xr-x   0        0        0      105 2023-11-16 17:27:03.728124 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/emblem/decor.js
+-rwxr-xr-x   0        0        0       99 2023-11-16 17:27:21.384926 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/emblem/decor.vue
+-rwxr-xr-x   0        0        0      395 2023-12-08 17:28:03.400445 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor/brands/decor.js
+-rwxr-xr-x   0        0        0      318 2024-02-12 02:52:00.985418 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor/brands/decor.vue
+-rwxr-xr-x   0        0        0      342 2024-02-02 19:55:15.353779 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor/comments.vue
+-rwxr-xr-x   0        0        0      888 2024-03-11 02:46:39.110041 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor/composition/decor.js
+-rwxr-xr-x   0        0        0     1039 2024-03-11 02:46:15.522334 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor/composition/decor.vue
+-rwxr-xr-x   0        0        0      294 2023-11-02 04:14:07.392983 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor/composition--/composition.r.html
+-rwxr-xr-x   0        0        0      935 2023-11-12 23:41:04.957885 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor/composition--/field.js
+-rwxr-xr-x   0        0        0      887 2024-02-02 19:55:38.510667 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor/composition--/field.vue
+-rwxr-xr-x   0        0        0      396 2023-12-17 02:24:04.194955 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor/ingredients_unmeasured/decor.vue
+-rwxr-xr-x   0        0        0      135 2024-02-12 02:50:10.018607 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor/kind.vue
+-rwxr-xr-x   0        0        0      995 2024-03-31 22:51:44.207173 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor/product/decor.js
+-rwxr-xr-x   0        0        0     1148 2024-03-31 22:53:25.562095 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor/product/decor.vue
+-rwxr-xr-x   0        0        0      211 2023-11-14 00:45:18.997484 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor/quantity/decor.vue
+-rwxr-xr-x   0        0        0        0 2023-11-02 04:09:32.993886 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor/recommendations/decor.js
+-rwxr-xr-x   0        0        0     1226 2024-02-02 19:55:57.099620 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor/recommendations/decor.vue
+-rwxr-xr-x   0        0        0     1055 2023-12-17 02:27:33.154567 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor/references/decor.vue
+-rwxr-xr-x   0        0        0      371 2024-02-12 02:50:42.554259 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor/warnings.vue
+-rwxr-xr-x   0        0        0      106 2024-02-02 19:28:46.031884 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor/zone.vue
+-rwxr-xr-x   0        0        0     1727 2024-03-31 22:35:01.749748 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor.js
+-rwxr-xr-x   0        0        0     4080 2024-05-13 04:23:09.363403 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor.vue
+-rwxr-xr-x   0        0        0      921 2024-05-13 00:59:57.092565 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/methods/index.js
+-rwxr-xr-x   0        0        0     1375 2024-03-12 20:01:19.748652 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/goal/room.js
+-rwxr-xr-x   0        0        0     1810 2024-03-22 01:23:27.394386 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/goal/room.vue
+-rwxr-xr-x   0        0        0     2762 2024-03-09 19:36:31.563195 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/goal/room_v1.vue
+-rwxr-xr-x   0        0        0     3219 2024-05-13 00:59:57.096565 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/goods/cycles/methods.js
+-rwxr-xr-x   0        0        0      805 2024-05-09 19:36:44.887475 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/goods/decor/food--/decor.js
+-rwxr-xr-x   0        0        0     1241 2024-03-06 23:29:46.725085 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/goods/decor/food--/decor.vue
+-rwxr-xr-x   0        0        0     2074 2024-03-21 23:11:47.526494 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/goods/decor/search_controls/decor.vue
+-rwxr-xr-x   0        0        0      702 2024-05-09 19:36:44.887475 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/goods/decor/supplement/decor.js
+-rwxr-xr-x   0        0        0     1110 2024-02-05 20:44:18.272696 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/goods/decor/supplement/decor.vue
+-rwxr-xr-x   0        0        0     1193 2024-05-10 22:58:59.788002 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/goods/decor.js
+-rwxr-xr-x   0        0        0       84 2024-05-10 22:57:41.412919 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/goods/decor.s.HTML
+-rwxr-xr-x   0        0        0     4097 2024-05-10 23:00:15.635121 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/goods/decor.vue
+-rwxr-xr-x   0        0        0       52 2024-05-09 19:36:44.887475 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/goods/physics/index.js
+-rwxr-xr-x   0        0        0     2110 2024-05-13 00:59:57.096565 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/habitat/decor.js
+-rwxr-xr-x   0        0        0      307 2024-05-13 19:42:04.890785 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/habitat/decor.vue
+-rwxr-xr-x   0        0        0      273 2024-02-03 01:10:33.156562 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/habitat/panels/image_styles.js
+-rwxr-xr-x   0        0        0     2750 2024-05-13 17:24:05.206246 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/habitat/panels/panel_1.vue
+-rwxr-xr-x   0        0        0     3186 2024-05-13 00:59:57.096565 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/habitat/panels/panel_goodness.vue
+-rwxr-xr-x   0        0        0     3610 2024-05-13 19:56:47.025810 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/habitat/panels/panel_health.vue
+-rwxr-xr-x   0        0        0     4052 2024-05-13 19:45:58.980254 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/habitat/panels/panel_moon.vue
+-rwxr-xr-x   0        0        0     3129 2024-05-13 19:14:53.224302 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/habitat/panels/panel_organic_crop_farming.vue
+-rwxr-xr-x   0        0        0     3763 2024-05-13 20:39:28.652548 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/habitat/panels/panel_physics.vue
+-rwxr-xr-x   0        0        0     3245 2024-05-13 02:14:33.692290 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/habitat/panels/panel_sink.vue
+-rwxr-xr-x   0        0        0     2478 2024-05-13 00:59:57.096565 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/habitat/panels/panel_sink_caution.vue
+-rwxr-xr-x   0        0        0     2317 2024-05-09 01:10:44.396492 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/habitat/panels/panel_sloop.vue
+-rwxr-xr-x   0        0        0     3309 2024-05-13 19:47:52.367028 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/habitat/panels/panel_tech.vue
+-rwxr-xr-x   0        0        0     1242 2024-02-12 02:21:47.246129 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/map/decor.js
+-rwxr-xr-x   0        0        0      869 2024-02-12 02:21:30.222335 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/map/decor.vue
+-rwxr-xr-x   0        0        0       64 2024-03-21 19:37:18.810900 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/recipes/decor.vue
+-rwxr-xr-x   0        0        0      493 2024-03-07 01:00:36.426725 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor/brands/decor.js
+-rwxr-xr-x   0        0        0      316 2023-12-16 01:11:08.924844 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor/brands/decor.vue
+-rwxr-xr-x   0        0        0      344 2024-02-02 19:55:46.154059 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor/comments.vue
+-rwxr-xr-x   0        0        0      938 2023-11-12 17:32:45.874714 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor/composition--/field.js
+-rwxr-xr-x   0        0        0      916 2023-11-12 17:31:30.962525 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor/composition--/field.vue
+-rwxr-xr-x   0        0        0       79 2023-09-20 21:35:51.996726 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor/films/field.vue
+-rwxr-xr-x   0        0        0      148 2023-11-09 21:59:10.425347 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor/kind.vue
+-rwxr-xr-x   0        0        0     2408 2024-03-11 02:24:13.877519 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor/measured_ingredients/fountains.js
+-rwxr-xr-x   0        0        0     3341 2024-03-11 02:27:03.199709 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor/measured_ingredients/fountains.vue
+-rwxr-xr-x   0        0        0     1095 2024-03-31 23:39:17.593025 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor/product/decor.js
+-rwxr-xr-x   0        0        0     1575 2024-04-01 02:00:57.182789 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor/product/decor.vue
+-rwxr-xr-x   0        0        0     1096 2023-12-20 19:19:58.798510 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor/references/decor.vue
+-rwxr-xr-x   0        0        0       68 2023-09-18 16:29:02.330860 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor/stat.vue
+-rwxr-xr-x   0        0        0      304 2023-12-16 03:54:22.787318 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor/statements/decor.js
+-rwxr-xr-x   0        0        0      807 2023-12-16 03:54:15.119382 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor/statements/decor.vue
+-rwxr-xr-x   0        0        0       77 2023-12-16 04:08:24.127308 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor/unmeasured_ingredients/fountain.js
+-rwxr-xr-x   0        0        0      393 2023-12-16 04:10:08.207440 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor/unmeasured_ingredients/fountain.vue
+-rwxr-xr-x   0        0        0     1663 2023-11-13 18:59:31.232825 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor/warnings.vue
+-rwxr-xr-x   0        0        0       58 2023-11-09 22:29:37.646696 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor/zone.vue
+-rwxr-xr-x   0        0        0     1663 2024-03-31 22:55:12.260954 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor.js
+-rwxr-xr-x   0        0        0     4316 2024-05-13 04:23:06.535436 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor.vue
+-rwxr-xr-x   0        0        0      934 2024-05-13 00:59:57.096565 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/methods/index.js
+-rwxr-xr-x   0        0        0       69 2023-11-10 19:36:19.034821 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/variables/index.js
+-rwxr-xr-x   0        0        0      188 2023-12-17 02:39:17.775516 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/not_found.vue
+-rwxr-xr-x   0        0        0      146 2024-04-01 00:02:44.025380 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/regions.s.HTML
+-rwxr-xr-x   0        0        0       62 2023-11-15 01:52:25.248899 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/staff/food/decor.vue
+-rwxr-xr-x   0        0        0       40 2024-05-11 00:47:10.035262 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/staff/habitat/decor.vue
+-rwxr-xr-x   0        0        0       69 2024-03-07 02:39:01.545825 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/staff/supplement/decor.vue
+-rwxr-xr-x   0        0        0      137 2024-02-02 20:39:47.327551 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/status/DAC/region.js
+-rwxr-xr-x   0        0        0      123 2024-02-02 20:40:09.375901 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/status/DAC/region.vue
+-rwxr-xr-x   0        0        0      420 2023-12-16 01:38:10.714287 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/status/index/scenery.vue
+-rwxr-xr-x   0        0        0      138 2024-02-02 20:36:54.688872 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/status/waterfall/region.js
+-rwxr-xr-x   0        0        0      284 2024-02-02 20:24:03.258300 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/status/waterfall/region.vue
+-rwxr-xr-x   0        0        0      401 2024-03-10 04:32:12.206055 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/workshop/scenery/region.js
+-rwxr-xr-x   0        0        0      455 2024-03-10 04:32:42.525826 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/workshop/scenery/region.vue
+-rwxr-xr-x   0        0        0      374 2023-12-16 01:26:20.040221 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/_example/_status/_example.status.js
+-rwxr-xr-x   0        0        0       44 2024-02-02 20:31:12.955078 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/_example/_status/region.vue
+-rwxr-xr-x   0        0        0       38 2023-12-16 01:24:25.483179 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/_example/example.vue
+-rwxr-xr-x   0        0        0      402 2024-02-12 00:41:59.519874 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/_status_Se/region.vue
+-rwxr-xr-x   0        0        0       52 2024-01-20 23:13:27.680787 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/alerts/decor.js
+-rwxr-xr-x   0        0        0      300 2024-01-20 23:16:22.966890 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/alerts/decor.vue
+-rwxr-xr-x   0        0        0     2109 2024-05-09 19:36:44.767476 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/browser_storage/component.vue
+-rwxr-xr-x   0        0        0      365 2024-02-12 01:41:42.400514 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/button/_status/button.status.js
+-rwxr-xr-x   0        0        0      772 2024-05-13 17:30:41.938573 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/button/decor.js
+-rwxr-xr-x   0        0        0     1027 2024-05-13 21:20:48.464951 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/button/decor.vue
+-rwxr-xr-x   0        0        0      365 2024-02-12 01:41:42.400514 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/button_3D/_status/button.status.js
+-rwxr-xr-x   0        0        0     3177 2024-03-16 01:40:22.479063 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/button_3D/decor--.js
+-rwxr-xr-x   0        0        0     1640 2024-05-12 21:48:37.116802 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/button_3D/decor--.vue
+-rwxr-xr-x   0        0        0      716 2024-05-11 00:12:32.840898 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/button_3D/decor.js
+-rwxr-xr-x   0        0        0      982 2024-05-12 21:48:30.780836 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/button_3D/decor.vue
+-rwxr-xr-x   0        0        0      478 2024-05-10 22:58:52.960081 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/canvases/canvases.S.HTML
+-rwxr-xr-x   0        0        0    89476 2024-05-13 00:59:57.064565 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/caution-sign/goodestSink-export.svg
+-rwxr-xr-x   0        0        0    88829 2024-05-13 00:59:57.064565 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/caution-sign/scenery.vue
+-rwxr-xr-x   0        0        0      654 2024-02-02 15:30:27.876924 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/change_indicator/indicators/spinner/indicator.js
+-rwxr-xr-x   0        0        0     1421 2023-12-12 22:09:16.041899 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/change_indicator/indicators/spinner/indicator.vue
+-rwxr-xr-x   0        0        0      341 2024-01-12 03:15:22.087200 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/change_indicator/scenery.js
+-rwxr-xr-x   0        0        0     1775 2024-01-12 03:42:31.305006 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/change_indicator/scenery.vue
+-rwxr-xr-x   0        0        0     2650 2024-02-02 20:38:35.056936 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/charts/composition_DAC/chart.js
+-rwxr-xr-x   0        0        0      437 2024-02-02 20:38:42.538683 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/charts/composition_DAC/chart.vue
+-rwxr-xr-x   0        0        0      262 2023-10-16 00:43:32.202900 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/charts/composition_DAC/methods/FIND_STRUCTURE.js
+-rwxr-xr-x   0        0        0     6029 2023-11-09 01:36:29.097181 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/charts/composition_DAC/methods/PHYSICAL/index.js
+-rwxr-xr-x   0        0        0     1802 2023-11-09 01:35:18.334938 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/charts/composition_DAC/methods/reinvigorate.js
+-rwxr-xr-x   0        0        0     3390 2024-02-11 21:15:24.477394 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/charts/composition_waterfall/chart.js
+-rwxr-xr-x   0        0        0      332 2024-05-09 19:36:44.855476 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/charts/composition_waterfall/chart.vue
+-rwxr-xr-x   0        0        0      484 2023-08-25 23:43:27.103848 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/charts/composition_waterfall/data.js
+-rwxr-xr-x   0        0        0      195 2023-12-11 23:36:26.510190 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/charts/pie/_status/pie.status.js
+-rwxr-xr-x   0        0        0     1182 2024-02-11 19:38:54.408096 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/charts/pie/make/build/data.js
+-rwxr-xr-x   0        0        0     1208 2024-02-11 19:41:21.790449 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/charts/pie/make/build/options.js
+-rwxr-xr-x   0        0        0     1131 2023-12-12 04:00:52.936450 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/charts/pie/make/build/plugins.js
+-rwxr-xr-x   0        0        0      660 2024-02-12 00:52:23.817062 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/charts/pie/make/index.js
+-rwxr-xr-x   0        0        0      945 2024-02-11 23:52:07.861502 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/charts/pie/make/utilities/--find_value.js
+-rwxr-xr-x   0        0        0      570 2024-02-11 19:34:33.475199 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/charts/pie/make/utilities/find_name.js
+-rwxr-xr-x   0        0        0       55 2024-02-11 19:37:20.529181 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/charts/pie/model.Se.vue
+-rwxr-xr-x   0        0        0     2827 2024-02-12 01:03:07.501975 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/charts/pie/veranda.js
+-rwxr-xr-x   0        0        0      298 2023-12-12 01:13:33.273737 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/charts/pie/veranda.vue
+-rwxr-xr-x   0        0        0     1180 2024-05-13 22:39:05.317211 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/checkbox/decor.js
+-rwxr-xr-x   0        0        0     1372 2024-05-13 22:38:54.385324 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/checkbox/decor.vue
+-rwxr-xr-x   0        0        0     1100 2024-02-12 01:03:31.757707 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/curtain/decor.js
+-rwxr-xr-x   0        0        0     1095 2024-05-12 19:46:18.226920 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/curtain/decor.vue
+-rwxr-xr-x   0        0        0      988 2024-02-11 19:09:26.348094 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/example/_status/decor.ST.js
+-rwxr-xr-x   0        0        0      267 2023-10-29 02:14:14.575679 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/example/_status/palette.js
+-rwxr-xr-x   0        0        0      383 2024-02-12 01:43:33.199389 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/example/decor.js
+-rwxr-xr-x   0        0        0      235 2023-10-29 02:35:27.283997 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/example/decor.vue
+-rwxr-xr-x   0        0        0      335 2024-02-12 00:39:43.917336 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/example_two/decor.vue
+-rwxr-xr-x   0        0        0      711 2024-02-02 19:24:25.841602 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/exception/field.vue
+-rwxr-xr-x   0        0        0     1135 2024-03-06 22:37:09.225730 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/flip/decor--.js
+-rwxr-xr-x   0        0        0      329 2024-03-06 23:06:49.208941 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/flip/decor.js
+-rwxr-xr-x   0        0        0     1270 2024-05-09 19:36:44.771476 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/flip/decor.vue
+-rwxr-xr-x   0        0        0      213 2023-11-02 00:22:56.985169 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/focusable/decor.vue
+-rwxr-xr-x   0        0        0      921 2024-03-06 23:58:15.605648 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/food_or_supp_summary/decor.js
+-rwxr-xr-x   0        0        0     2064 2024-03-09 19:22:16.538125 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/food_or_supp_summary/decor.vue
+-rwxr-xr-x   0        0        0        2 2024-02-18 23:29:05.402268 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/foundations/eagle/scene.js
+-rwxr-xr-x   0        0        0     1473 2024-05-09 01:10:44.432492 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/foundations/eagle/scene.vue
+-rwxr-xr-x   0        0        0      112 2024-02-12 00:38:00.794440 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/gesture/gesture.s.HTML
+-rwxr-xr-x   0        0        0      791 2024-03-21 18:05:53.908624 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/goal/components/goal_amount.vue
+-rwxr-xr-x   0        0        0       84 2024-03-12 19:53:20.149662 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/goal/components/include.vue
+-rwxr-xr-x   0        0        0     1713 2024-03-14 23:56:32.550876 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/goal/decor.js
+-rwxr-xr-x   0        0        0     3387 2024-03-15 00:06:57.047615 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/goal/decor.vue
+-rwxr-xr-x   0        0        0     1799 2024-03-09 21:58:48.378771 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/goal/decor_1.vue
+-rwxr-xr-x   0        0        0        0 2023-10-29 19:45:47.360285 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/hw_button/decor.js
+-rwxr-xr-x   0        0        0      767 2024-05-10 23:57:45.139416 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/hw_button/decor.vue
+-rwxr-xr-x   0        0        0      771 2024-05-10 23:53:11.467027 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/hw_button/decor_v1.vue
+-rwxr-xr-x   0        0        0     1121 2024-05-13 22:25:07.653778 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/icons/book/field.vue
+-rwxr-xr-x   0        0        0       67 2024-03-30 03:59:23.274857 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/icons/icons.S.HTML
+-rwxr-xr-x   0        0        0        0 2023-11-01 23:46:29.107176 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/input/_status/decor.status.js
+-rwxr-xr-x   0        0        0     1331 2024-01-15 22:18:55.662581 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/input/decor.js
+-rwxr-xr-x   0        0        0     2461 2024-05-13 22:31:58.481608 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/input/decor.vue
+-rwxr-xr-x   0        0        0      451 2024-02-11 23:57:56.457658 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/line/decor.vue
+-rwxr-xr-x   0        0        0     1064 2024-05-14 00:04:16.069185 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/link/outer/decor.vue
+-rwxr-xr-x   0        0        0     1596 2024-05-12 21:50:04.432303 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/lounge/decor.js
+-rwxr-xr-x   0        0        0      693 2024-02-13 06:25:25.937282 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/lounge/decor.s.HTML
+-rwxr-xr-x   0        0        0      291 2024-05-09 19:36:44.771476 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/lounge/decor.vue
+-rwxr-xr-x   0        0        0    22053 2024-01-21 01:14:15.300256 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/mascot/craft.vue
+-rwxr-xr-x   0        0        0    11002 2024-01-17 17:58:07.993655 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/mascot/craft_v1.vue
+-rwxr-xr-x   0        0        0    11973 2024-01-17 17:46:49.047355 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/mascot/mascot-1.svg
+-rwxr-xr-x   0        0        0   199059 2024-01-21 00:48:09.525250 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/mascot/mascot.svg
+-rwxr-xr-x   0        0        0     3653 2023-12-20 18:33:55.488744 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/name/_assets/Rugged Vegan.svg
+-rwxr-xr-x   0        0        0   523296 2024-05-13 00:59:57.032565 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/name/_assets/Vegan Lantern - Export.svg
+-rwxr-xr-x   0        0        0   724519 2024-05-13 00:59:57.004566 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/name/_assets/goodest sloop - mural - v1.svg
+-rwxr-xr-x   0        0        0   724643 2024-05-13 00:59:57.028566 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/name/_assets/goodest sloop - mural - v2.svg
+-rwxr-xr-x   0        0        0   724823 2024-05-13 00:59:57.060565 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/name/_assets/goodest sloop - mural - v3.svg
+-rwxr-xr-x   0        0        0   724891 2024-05-13 00:59:57.004566 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/name/mural.vue
+-rwxr-xr-x   0        0        0    61548 2023-12-13 03:15:36.204804 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/name/mural_v1.vue
+-rwxr-xr-x   0        0        0     3557 2024-01-15 21:06:50.292544 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/name/mural_v2.vue
+-rwxr-xr-x   0        0        0     4104 2024-01-16 02:07:39.029898 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/name/mural_v3.vue
+-rwxr-xr-x   0        0        0     3987 2024-02-02 05:33:49.728771 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/name/mural_v4.vue
+-rwxr-xr-x   0        0        0   523241 2024-05-13 00:59:57.000566 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/name/mural_v5.vue
+-rwxr-xr-x   0        0        0     2761 2023-12-16 18:51:32.031662 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nature_cautionary_ingredients/shack.js
+-rwxr-xr-x   0        0        0     2233 2024-03-30 02:18:06.952972 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nature_cautionary_ingredients/shack.vue
+-rwxr-xr-x   0        0        0       30 2024-02-11 19:32:07.085089 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nature_essentials_nutrients/model.vue
+-rwxr-xr-x   0        0        0     2980 2024-03-30 02:07:54.200279 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nature_essentials_nutrients/shack.js
+-rwxr-xr-x   0        0        0     3919 2024-03-30 02:18:12.832902 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nature_essentials_nutrients/shack.vue
+-rwxr-xr-x   0        0        0       51 2023-12-16 01:51:11.241801 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nature_ingredients_table/_status/region.vue
+-rwxr-xr-x   0        0        0      367 2024-03-30 00:57:37.706848 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nature_ingredients_table/components/mass.vue
+-rwxr-xr-x   0        0        0      873 2024-03-30 03:42:25.810936 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nature_ingredients_table/components/name.vue
+-rwxr-xr-x   0        0        0      360 2024-03-30 03:33:49.781346 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nature_ingredients_table/components/the_percent.vue
+-rwxr-xr-x   0        0        0     2805 2024-05-13 22:08:50.078779 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nature_ingredients_table/fields/methods.js
+-rwxr-xr-x   0        0        0     5724 2024-05-11 00:12:32.852898 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nature_ingredients_table/fields/methods_/prepare_columns.js
+-rwxr-xr-x   0        0        0     1793 2024-03-30 03:23:07.753064 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nature_ingredients_table/fields/methods_/prepare_rows.js
+-rwxr-xr-x   0        0        0     2131 2024-05-11 00:12:32.864898 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nature_ingredients_table/fountains.js
+-rwxr-xr-x   0        0        0      346 2024-03-31 04:02:30.811735 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nature_ingredients_table/fountains.vue
+-rwxr-xr-x   0        0        0       51 2023-12-16 01:51:11.241801 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nature_ingredients_table_v1/_status/region.vue
+-rwxr-xr-x   0        0        0     3842 2024-05-11 00:12:32.868898 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nature_ingredients_table_v1/fountains.js
+-rwxr-xr-x   0        0        0     3125 2024-03-26 02:31:39.534326 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nature_ingredients_table_v1/fountains.vue
+-rwxr-xr-x   0        0        0      495 2024-05-09 19:36:44.863475 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nav_1/decor.js
+-rwxr-xr-x   0        0        0     1550 2024-05-13 17:23:17.158703 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nav_1/decor.vue
+-rwxr-xr-x   0        0        0      654 2024-02-12 01:42:45.279877 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nav_1/navs/mobile_top/field.js
+-rwxr-xr-x   0        0        0      631 2024-01-21 03:51:57.002319 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nav_1/navs/mobile_top/field.vue
+-rwxr-xr-x   0        0        0     1705 2024-05-10 22:52:19.472795 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nav_1/navs/top/field.js
+-rwxr-xr-x   0        0        0     2402 2024-05-14 00:15:30.677767 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nav_1/navs/top/field.vue
+-rwxr-xr-x   0        0        0      595 2024-05-09 19:36:44.767476 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nav_2/decor.js
+-rwxr-xr-x   0        0        0     1175 2024-05-14 00:15:45.821534 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nav_2/decor.vue
+-rwxr-xr-x   0        0        0     1009 2024-02-12 01:27:50.397664 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/navigation infrastructure/methods/awareness/keydown.js
+-rwxr-xr-x   0        0        0      278 2024-02-12 01:25:04.639492 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/navigation infrastructure/methods/awareness/keys.s.HTML
+-rwxr-xr-x   0        0        0      237 2024-02-12 01:28:10.421443 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/navigation infrastructure/methods/find_element_index.js
+-rwxr-xr-x   0        0        0     1493 2024-02-12 01:28:47.309037 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/navigation infrastructure/methods/focus_land_mark.js
+-rwxr-xr-x   0        0        0      237 2024-02-12 01:28:20.997327 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/navigation infrastructure/methods/index.js
+-rwxr-xr-x   0        0        0       29 2023-11-26 17:48:20.457245 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/navigation infrastructure/notes/notes.html
+-rwxr-xr-x   0        0        0      362 2023-11-10 01:55:44.853516 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/navigation infrastructure/priorities.s.HTML
+-rwxr-xr-x   0        0        0      914 2024-03-18 23:29:59.338994 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/navigation infrastructure/structure.js
+-rwxr-xr-x   0        0        0     1774 2024-03-18 23:32:06.137547 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/navigation infrastructure/structure.vue
+-rwxr-xr-x   0        0        0        0 2023-10-29 19:36:27.733924 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/panel/decor.js
+-rwxr-xr-x   0        0        0     1537 2024-05-11 00:10:56.545996 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/panel/decor.vue
+-rwxr-xr-x   0        0        0       19 2024-02-02 19:21:05.508081 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/paragraph/scenery.js
+-rwxr-xr-x   0        0        0      245 2024-02-02 19:22:31.236941 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/paragraph/scenery.vue
+-rwxr-xr-x   0        0        0     2516 2024-03-07 00:24:06.697068 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/quantity_chooser/decor.js
+-rwxr-xr-x   0        0        0      993 2024-03-21 23:12:03.846331 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/quantity_chooser/decor.vue
+-rwxr-xr-x   0        0        0      197 2023-12-09 04:41:31.507002 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/router_link/_status/1.status.js
+-rwxr-xr-x   0        0        0      934 2024-01-15 21:55:41.717670 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/router_link/decor.js
+-rwxr-xr-x   0        0        0     1632 2024-05-13 21:30:16.487247 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/router_link/decor.vue
+-rwxr-xr-x   0        0        0      223 2024-03-16 01:03:10.281823 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/scenery.s.HTML
+-rwxr-xr-x   0        0        0     1010 2024-03-06 21:32:00.501591 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/select/decor.js
+-rwxr-xr-x   0        0        0      590 2024-02-05 21:07:41.006147 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/select/decor.status.js
+-rwxr-xr-x   0        0        0     1476 2024-05-13 22:19:54.176871 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/select/decor.vue
+-rwxr-xr-x   0        0        0      331 2023-11-09 01:39:06.154492 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/select/show.vue
+-rwxr-xr-x   0        0        0       76 2023-11-29 19:31:03.919410 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/service/error/scenery.vue
+-rwxr-xr-x   0        0        0       57 2023-11-29 19:30:41.590672 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/service/not_found/scenery.vue
+-rwxr-xr-x   0        0        0       78 2024-02-19 04:56:48.625281 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/slides/scenery.js
+-rwxr-xr-x   0        0        0      288 2024-02-19 04:47:31.307536 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/slides/scenery.vue
+-rwxr-xr-x   0        0        0     1281 2023-12-08 04:01:35.070938 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/struct_2/composition/decor.js
+-rwxr-xr-x   0        0        0     1023 2023-11-18 05:08:17.333020 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/struct_2/composition/decor.vue
+-rwxr-xr-x   0        0        0      823 2023-12-08 21:43:22.157591 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/struct_2/composition/furniture/mass_of_quantified_ingredients.vue
+-rwxr-xr-x   0        0        0      404 2023-11-07 02:46:35.565079 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/struct_2/quantified_grove/decor/mass.vue
+-rwxr-xr-x   0        0        0     2254 2024-03-30 19:18:20.305565 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/struct_2/quantified_grove/fields/methods.js
+-rwxr-xr-x   0        0        0      609 2024-03-30 19:18:20.305565 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/struct_2/quantified_grove/table.js
+-rwxr-xr-x   0        0        0     2953 2024-02-11 23:57:56.641656 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/struct_2/quantified_grove/table.vue
+-rwxr-xr-x   0        0        0       72 2023-11-07 00:13:33.997933 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/table/decor.js
+-rwxr-xr-x   0        0        0     2260 2024-03-14 22:09:35.613243 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/table/decor.vue
+-rwxr-xr-x   0        0        0       96 2023-11-07 00:14:30.745330 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/table/status/check_1.se.js
+-rwxr-xr-x   0        0        0        2 2024-03-14 21:55:36.298300 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/table/table.S.HTML
+-rwxr-xr-x   0        0        0     1048 2024-05-14 00:05:03.588280 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/treasure/affiliates/decor.vue
+-rwxr-xr-x   0        0        0     1512 2024-03-31 22:53:45.469882 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/treasure/goodness_certifications/money.vue
+-rwxr-xr-x   0        0        0       15 2019-02-15 21:43:43.000000 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/.gitignore
+-rwxr-xr-x   0        0        0     1078 2019-02-15 21:43:43.000000 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/LICENSE.md
+-rwxr-xr-x   0        0        0     1097 2019-02-15 21:43:43.000000 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/README.md
+-rwxr-xr-x   0        0        0      463 2019-02-15 21:43:43.000000 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/bower.json
+-rwxr-xr-x   0        0        0     5389 2019-02-15 21:43:43.000000 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/index.html
+-rwxr-xr-x   0        0        0     4712 2019-02-15 21:43:43.000000 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/site-assets/images/download-btn.png
+-rwxr-xr-x   0        0        0     3733 2019-02-15 21:43:43.000000 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/site-assets/images/tweet-btn.png
+-rwxr-xr-x   0        0        0     1347 2019-02-15 21:43:43.000000 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/svg-loaders/audio.svg
+-rwxr-xr-x   0        0        0     1926 2019-02-15 21:43:43.000000 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/svg-loaders/ball-triangle.svg
+-rwxr-xr-x   0        0        0     2319 2019-02-15 21:43:43.000000 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/svg-loaders/bars.svg
+-rwxr-xr-x   0        0        0     1923 2019-02-15 21:43:43.000000 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/svg-loaders/circles.svg
+-rwxr-xr-x   0        0        0     2048 2019-02-15 21:43:43.000000 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/svg-loaders/grid.svg
+-rwxr-xr-x   0        0        0     1357 2019-02-15 21:43:43.000000 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/svg-loaders/hearts.svg
+-rwxr-xr-x   0        0        0      694 2019-02-15 21:43:43.000000 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/svg-loaders/oval.svg
+-rwxr-xr-x   0        0        0     1460 2019-02-15 21:43:43.000000 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/svg-loaders/puff.svg
+-rwxr-xr-x   0        0        0     1784 2019-02-15 21:43:43.000000 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/svg-loaders/rings.svg
+-rwxr-xr-x   0        0        0     2782 2019-02-15 21:43:43.000000 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/svg-loaders/spinning-circles.svg
+-rwxr-xr-x   0        0        0     1309 2019-02-15 21:43:43.000000 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/svg-loaders/tail-spin.svg
+-rwxr-xr-x   0        0        0     1510 2019-02-15 21:43:43.000000 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/svg-loaders/three-dots.svg
+-rwxr-xr-x   0        0        0        1 2024-01-12 03:13:03.137742 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/scenery/action/drawing.svg
+-rwxr-xr-x   0        0        0      655 2024-01-12 03:23:52.078508 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/scenery/action/scenery.js
+-rwxr-xr-x   0        0        0    12705 2024-02-02 15:29:43.493436 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/scenery/action/scenery.vue
+-rwxr-xr-x   0        0        0    12243 2024-01-12 03:25:38.748314 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/scenery/action/scenery_v1.vue
+-rwxr-xr-x   0        0        0     1371 2024-02-11 23:56:32.126588 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/_research/observables.js
+-rwxr-xr-x   0        0        0     1701 2024-03-07 00:24:06.801066 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/cart/_status/1.status.js
+-rwxr-xr-x   0        0        0     1560 2024-03-07 00:24:06.949064 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/cart/_status/2.status.js
+-rwxr-xr-x   0        0        0     1571 2024-03-07 00:24:07.045063 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/cart/_status/3.status.js
+-rwxr-xr-x   0        0        0     1227 2024-03-07 00:24:07.125061 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/cart/_status/4_remove.status.js
+-rwxr-xr-x   0        0        0       54 2024-01-20 22:13:05.511855 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/cart/cart.s.HTML
+-rwxr-xr-x   0        0        0     2040 2024-03-21 18:09:41.617982 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/cart/index.js
+-rwxr-xr-x   0        0        0     1607 2024-03-07 00:24:07.245059 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/cart/moves/change_quantity.js
+-rwxr-xr-x   0        0        0      716 2024-03-07 00:24:07.353058 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/cart/moves/find_DSLD_ID.js
+-rwxr-xr-x   0        0        0      713 2024-03-07 00:24:07.473056 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/cart/moves/find_FDC_ID.js
+-rwxr-xr-x   0        0        0     1396 2024-03-07 00:24:07.629053 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/cart/moves/remove.js
+-rwxr-xr-x   0        0        0      982 2023-12-09 03:11:02.006950 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/cart/utilities/retrieve_treasures.js
+-rwxr-xr-x   0        0        0      913 2024-05-12 21:37:29.717752 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/connections/index.js
+-rwxr-xr-x   0        0        0     3017 2024-05-13 02:33:46.495932 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/goals/index.js
+-rwxr-xr-x   0        0        0     2205 2024-05-13 17:33:51.484372 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/homestead/index.js
+-rwxr-xr-x   0        0        0        2 2023-10-29 23:43:15.460481 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/language/index.js
+-rwxr-xr-x   0        0        0      926 2024-03-21 19:28:28.280880 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/layout/index.js
+-rwxr-xr-x   0        0        0     2565 2024-03-21 18:22:13.668837 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/storage/index.js
+-rwxr-xr-x   0        0        0     1071 2024-02-18 23:59:57.568976 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/terrain--/index.js
+-rwxr-xr-x   0        0        0      589 2024-01-16 02:44:42.852499 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/terrain--/index.s.HTML
+-rwxr-xr-x   0        0        0      659 2024-03-07 00:24:08.293043 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/theme/_status/1.status.js
+-rwxr-xr-x   0        0        0     2707 2024-05-10 20:05:23.682936 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/theme/index.js
+-rwxr-xr-x   0        0        0     4811 2024-05-13 22:55:49.447352 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/theme/rooms/palettes.js
+-rwxr-xr-x   0        0        0      376 2024-03-15 05:44:08.142235 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/theme/theme.s.HTML
+-rwxr-xr-x   0        0        0       79 2024-05-13 21:13:58.600905 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/warehouses.S.HTML
+-rwxr-xr-x   0        0        0    17897 2024-05-14 02:01:34.030618 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/the_build/assets/decor-015b0f33.js
+-rwxr-xr-x   0        0        0      177 2024-05-14 02:01:34.030618 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/the_build/assets/decor-25a431cc.css
+-rwxr-xr-x   0        0        0      856 2024-05-14 02:01:34.030618 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/the_build/assets/decor-2ed9a230.js
+-rwxr-xr-x   0        0        0      671 2024-05-14 02:01:34.030618 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/the_build/assets/decor-5193c01d.js
+-rwxr-xr-x   0        0        0  1648886 2024-05-14 02:01:34.050618 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/the_build/assets/decor-5eab20fb.js
+-rwxr-xr-x   0        0        0     5299 2024-05-14 02:01:34.030618 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/the_build/assets/decor-5fd94eca.css
+-rwxr-xr-x   0        0        0      559 2024-05-14 02:01:34.030618 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/the_build/assets/decor-6cea4756.js
+-rwxr-xr-x   0        0        0    53006 2024-05-14 02:01:34.030618 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/the_build/assets/decor-6e28e7ef.js
+-rwxr-xr-x   0        0        0      226 2024-05-14 02:01:34.030618 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/the_build/assets/decor-841ca039.css
+-rwxr-xr-x   0        0        0    12069 2024-05-14 02:01:34.030618 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/the_build/assets/decor-8e219cfa.js
+-rwxr-xr-x   0        0        0    28337 2024-05-14 02:01:34.030618 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/the_build/assets/decor-96894bcb.js
+-rwxr-xr-x   0        0        0   119829 2024-05-14 02:01:34.030618 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/the_build/assets/decor-a754c497.js
+-rwxr-xr-x   0        0        0      177 2024-05-14 02:01:34.030618 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/the_build/assets/decor-a9590bef.css
+-rwxr-xr-x   0        0        0     9474 2024-05-14 02:01:34.030618 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/the_build/assets/decor-afa10235.js
+-rwxr-xr-x   0        0        0    35348 2024-05-14 02:01:34.030618 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/the_build/assets/decor-c53f6aed.js
+-rwxr-xr-x   0        0        0       49 2024-05-14 02:01:34.030618 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/the_build/assets/decor-d42139e0.css
+-rwxr-xr-x   0        0        0    64245 2024-05-14 02:01:34.030618 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/the_build/assets/decor-de2803b9.js
+-rwxr-xr-x   0        0        0    14399 2024-05-14 02:01:34.030618 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/the_build/assets/decor-ebc19d4a.js
+-rwxr-xr-x   0        0        0    23674 2024-05-14 02:01:34.030618 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/the_build/assets/decor-fdb1c7b9.js
+-rwxr-xr-x   0        0        0     2670 2024-05-14 02:01:34.030618 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/the_build/assets/feature-c1fba25d.js
+-rwxr-xr-x   0        0        0     3224 2024-05-14 02:01:34.030618 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/the_build/assets/features-716bf8fe.js
+-rwxr-xr-x   0        0        0     4407 2024-05-14 02:01:34.030618 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/the_build/assets/field-2fd232c7.js
+-rwxr-xr-x   0        0        0     2560 2024-05-14 02:01:34.030618 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/the_build/assets/field-5f91724e.js
+-rwxr-xr-x   0        0        0   471908 2024-05-14 02:01:34.046618 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/the_build/assets/field-8561b8fb.js
+-rwxr-xr-x   0        0        0     9898 2024-05-14 02:01:34.030618 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/the_build/assets/field-a31efeca.js
+-rwxr-xr-x   0        0        0    20889 2024-05-14 02:01:34.030618 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/the_build/assets/field-a77631ec.css
+-rwxr-xr-x   0        0        0    16919 2024-05-14 02:01:34.030618 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/the_build/assets/field-c89c2300.js
+-rwxr-xr-x   0        0        0     5411 2024-05-14 02:01:34.030618 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/the_build/assets/field-e2ebd0ad.js
+-rwxr-xr-x   0        0        0      906 2024-05-14 02:01:34.030618 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/the_build/assets/index-0adfbe82.css
+-rwxr-xr-x   0        0        0  4284023 2024-05-14 02:01:34.050618 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/the_build/assets/index-a0b775e5.js
+-rwxr-xr-x   0        0        0    11553 2024-05-14 02:01:34.030618 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/the_build/assets/money-e4108053.js
+-rwxr-xr-x   0        0        0      940 2024-05-14 02:01:34.030618 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/the_build/assets/not_found-e5379e86.js
+-rwxr-xr-x   0        0        0   143198 2024-05-14 02:01:34.030618 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/the_build/assets/region-1928b31b.js
+-rwxr-xr-x   0        0        0      570 2024-05-14 02:01:34.030618 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/the_build/assets/region-5fabcc50.js
+-rwxr-xr-x   0        0        0      500 2024-05-14 02:01:34.030618 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/the_build/assets/region-cf456570.js
+-rwxr-xr-x   0        0        0    66762 2024-05-14 02:01:34.030618 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/the_build/assets/region-e63ac034.js
+-rwxr-xr-x   0        0        0     3358 2024-05-14 02:01:34.030618 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/the_build/assets/region-efd06052.js
+-rwxr-xr-x   0        0        0    31743 2024-05-14 02:01:34.030618 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/the_build/assets/room-1b1799cf.js
+-rwxr-xr-x   0        0        0      674 2024-05-14 02:01:34.030618 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/the_build/assets/scenery-b3179ad4.css
+-rwxr-xr-x   0        0        0     2188 2024-05-14 02:01:34.030618 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/the_build/assets/scenery-b6263767.js
+-rwxr-xr-x   0        0        0    47367 2024-05-14 02:01:34.030618 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/the_build/assets/scenery-f58f903f.js
+-rwxr-xr-x   0        0        0  1625254 2024-05-14 02:01:34.050618 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/the_build/assets/shack-0e3927fb.js
+-rwxr-xr-x   0        0        0    11377 2024-05-14 02:01:34.030618 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/the_build/assets/status-306755ec.js
+-rwxr-xr-x   0        0        0     5077 2024-05-14 02:01:34.030618 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/the_build/assets/string-ba766c78.js
+-rwxr-xr-x   0        0        0   240659 2024-05-14 02:01:34.046618 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/the_build/assets/transform-21ef9c51.js
+-rwxr-xr-x   0        0        0     1141 2024-05-14 02:01:34.046618 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/the_build/assets/worker-abbf90d8.js
+-rwxr-xr-x   0        0        0     1244 2024-05-14 02:01:34.046618 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/the_build/index.html
+-rwxr-xr-x   0        0        0       75 2024-05-08 19:30:19.000000 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/tsconfig.json--
+-rwxr-xr-x   0        0        0      363 2024-05-11 00:11:34.953558 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/vite.config.js
+-rwxr-xr-x   0        0        0      556 2024-05-08 21:11:26.687514 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/vitest.config.js
+-rwxr-xr-x   0        0        0   358624 2024-05-13 01:01:34.311552 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/bun.lockb
+-rwxr-xr-x   0        0        0      521 2024-05-13 00:59:57.104565 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/find_symlinks.py
+-rwxr-xr-x   0        0        0      420 2024-05-10 02:12:07.564248 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/package.json
+-rwxr-xr-x   0        0        0     2729 2024-05-11 00:13:19.112372 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/shares/glamour/background_effects/particles/money.js
+-rwxr-xr-x   0        0        0      327 2024-04-01 01:01:35.808375 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/shares/glamour/background_effects/particles/money.vue
+-rwxr-xr-x   0        0        0      268 2024-04-01 00:27:00.389669 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/shares/glamour/background_effects/particles/worker.js
+-rwxr-xr-x   0        0        0     2298 2024-03-18 23:20:10.765821 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/shares/glamour/button/glamour.js
+-rwxr-xr-x   0        0        0     1534 2024-05-13 21:21:06.312775 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/shares/glamour/button/glamour.vue
+-rwxr-xr-x   0        0        0       86 2024-03-16 01:19:46.112564 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/shares/glamour/glamour.S.HTML
+-rwxr-xr-x   0        0        0      234 2024-03-29 19:54:30.932386 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/shares/glamour/table/_status/components/name.vue
+-rwxr-xr-x   0        0        0     3028 2024-05-11 00:13:19.144372 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/shares/glamour/table/_status/status.js
+-rwxr-xr-x   0        0        0      229 2024-03-29 19:39:01.732623 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/shares/glamour/table/_status/status.vue
+-rwxr-xr-x   0        0        0      128 2024-03-25 21:46:30.379196 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/shares/glamour/table/components/string_data.vue
+-rwxr-xr-x   0        0        0     3064 2024-05-11 00:14:20.847673 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/shares/glamour/table/decor.js
+-rwxr-xr-x   0        0        0     3236 2024-03-31 04:06:25.301446 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/shares/glamour/table/decor.vue
+-rwxr-xr-x   0        0        0      937 2024-05-11 00:13:19.156372 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/shares/glamour/table/sorting/as_float.js
+-rwxr-xr-x   0        0        0      962 2024-03-25 21:01:57.256918 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/shares/glamour/table/table.S.HTML
+-rwxr-xr-x   0        0        0      375 2024-05-08 19:30:19.000000 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/sharess/config-eslint/index.js
+-rwxr-xr-x   0        0        0      306 2024-05-08 20:00:54.297170 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/sharess/config-eslint/package.json--
+-rwxr-xr-x   0        0        0      548 2024-05-08 19:30:19.000000 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/sharess/config-typescript/base.json
+-rwxr-xr-x   0        0        0      150 2024-05-08 20:00:54.297170 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/sharess/config-typescript/package.json--
+-rwxr-xr-x   0        0        0      369 2024-05-08 19:30:19.000000 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/sharess/config-typescript/vite.json
+-rwxr-xr-x   0        0        0      246 2024-05-08 19:30:19.000000 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/sharess/ui/.eslintrc.cjs
+-rwxr-xr-x   0        0        0       49 2024-05-08 22:05:26.488661 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/sharess/ui/.turbo/turbo-lint.log
+-rwxr-xr-x   0        0        0       87 2024-05-08 19:30:19.000000 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/sharess/ui/components/counter.ts
+-rwxr-xr-x   0        0        0      138 2024-05-08 19:30:19.000000 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/sharess/ui/components/header.ts
+-rwxr-xr-x   0        0        0      166 2024-05-08 19:30:19.000000 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/sharess/ui/index.ts
+-rwxr-xr-x   0        0        0      418 2024-05-08 20:00:54.297170 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/sharess/ui/package.json--
+-rwxr-xr-x   0        0        0      104 2024-05-08 19:30:19.000000 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/sharess/ui/tsconfig.json
+-rwxr-xr-x   0        0        0      278 2024-05-08 19:30:19.000000 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/sharess/ui/utils/counter.ts
+-rwxr-xr-x   0        0        0      236 2024-05-08 19:30:19.000000 goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/turbo.json
+-rwxr-xr-x   0        0        0      151 2024-04-17 03:33:22.097283 goodest-1.2.2/venues/stages/goodest/besties/affiliates_Amazon/affiliates.s.HTML
+-rwxr-xr-x   0        0        0      176 2024-04-27 17:39:04.201558 goodest-1.2.2/venues/stages/goodest/besties/besties.S.HTML
+-rwxr-xr-x   0        0        0      596 2024-04-17 03:36:49.119045 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/deliveries/__pycache__/source.cpython-310.pyc
+-rwxr-xr-x   0        0        0      738 2024-04-17 03:33:22.097283 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/deliveries/__pycache__/source.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1326 2024-05-13 00:59:57.252563 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/deliveries/one/__init__.py
+-rwxr-xr-x   0        0        0     1606 2024-05-13 01:08:31.359266 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/deliveries/one/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2127 2024-04-17 03:33:22.097283 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/deliveries/one/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      776 2024-04-17 03:33:22.097283 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/deliveries/one/assertions/__pycache__/BRANDED.cpython-311.pyc
+-rwxr-xr-x   0        0        0      450 2024-04-17 03:33:22.097283 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/deliveries/one/assertions/__pycache__/FOUNDATIONAL.cpython-311.pyc
+-rwxr-xr-x   0        0        0      652 2024-05-13 01:08:31.359266 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/deliveries/one/assertions/__pycache__/branded.cpython-310.pyc
+-rwxr-xr-x   0        0        0      778 2024-04-17 03:33:22.097283 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/deliveries/one/assertions/__pycache__/branded.cpython-311.pyc
+-rwxr-xr-x   0        0        0      502 2024-05-13 01:08:31.359266 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/deliveries/one/assertions/__pycache__/foundational.cpython-310.pyc
+-rwxr-xr-x   0        0        0      677 2024-04-17 03:33:22.097283 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/deliveries/one/assertions/__pycache__/foundational.cpython-311.pyc
+-rwxr-xr-x   0        0        0      510 2024-05-13 00:59:57.252563 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/deliveries/one/assertions/branded.py
+-rwxr-xr-x   0        0        0      264 2024-05-13 00:59:57.252563 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/deliveries/one/assertions/foundational.py
+-rwxr-xr-x   0        0        0      470 2024-05-13 00:59:57.252563 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/deliveries/one/status/API_status_branded_1.py
+-rwxr-xr-x   0        0        0      537 2024-05-13 00:59:57.252563 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/deliveries/one/status/API_status_foundational_1.py
+-rwxr-xr-x   0        0        0      747 2024-05-13 01:14:34.865033 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/deliveries/one/status/__pycache__/API_status_branded_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      742 2024-05-13 01:14:34.877033 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/deliveries/one/status/__pycache__/API_status_foundational_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      370 2024-04-17 03:33:22.097283 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/deliveries/source.py
+-rwxr-xr-x   0        0        0      945 2024-05-13 00:59:57.244563 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/examples/__init__.py
+-rwxr-xr-x   0        0        0     1131 2024-05-13 01:11:04.434433 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/examples/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2082 2024-04-17 03:33:22.097283 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/examples/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      748 2024-05-13 01:11:04.278434 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/examples/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0    37079 2024-04-17 03:33:22.097283 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/examples/branded/Gardein_f'sh_2663758.JSON
+-rwxr-xr-x   0        0        0    37079 2024-04-17 03:33:22.097283 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/examples/branded/Gardein_f'sh_2664238.JSON
+-rwxr-xr-x   0        0        0     7242 2024-04-17 03:33:22.097283 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/examples/branded/beet_juice_2412474.JSON
+-rwxr-xr-x   0        0        0     8522 2024-04-17 03:33:22.097283 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/examples/branded/beet_juice_2642759.JSON
+-rwxr-xr-x   0        0        0    10678 2024-04-17 03:33:22.097283 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/examples/branded/goodest_pizza_2672996.JSON
+-rwxr-xr-x   0        0        0    33964 2024-04-17 03:33:22.097283 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/examples/branded/impossible_beef_2664238.JSON
+-rwxr-xr-x   0        0        0    17926 2024-04-17 03:33:22.097283 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/examples/branded/problems/impossible_2468423.JSON
+-rwxr-xr-x   0        0        0      104 2024-04-17 03:33:22.097283 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/examples/branded/problems/problems.r.HTML
+-rwxr-xr-x   0        0        0    10670 2024-04-17 03:33:22.097283 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/examples/branded/walnuts_1882785.JSON
+-rwxr-xr-x   0        0        0   189146 2024-04-17 03:33:22.097283 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/examples/foundational/2346404_sweet_potatoes.JSON
+-rwxr-xr-x   0        0        0      255 2024-04-17 03:33:22.097283 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/examples/mergers.r.HTML
+-rwxr-xr-x   0        0        0       88 2024-04-17 03:33:22.097283 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/examples/priorities.r.HTML
+-rwxr-xr-x   0        0        0      458 2024-05-13 00:59:57.244563 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/examples/status_1.py
+-rwxr-xr-x   0        0        0     1220 2024-05-13 00:59:57.244563 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/food.s.HTML
+-rwxr-xr-x   0        0        0     4590 2024-05-13 00:59:57.248563 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/__init__.py
+-rwxr-xr-x   0        0        0     2463 2024-05-13 01:08:31.343266 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1752 2024-05-13 00:59:57.252563 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/__init__.py
+-rwxr-xr-x   0        0        0     1202 2024-05-13 01:08:31.343266 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2050 2024-04-17 03:33:22.101283 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      571 2024-04-17 03:33:22.101283 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/__pycache__/assertions.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1065 2024-04-17 03:33:22.101283 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/__pycache__/assertions.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1417 2024-05-13 01:11:05.538426 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      599 2024-04-17 03:33:22.101283 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/assertions/__init__.py
+-rwxr-xr-x   0        0        0      596 2024-04-17 03:36:50.207023 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/assertions/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4182 2024-05-13 00:59:57.252563 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/__init__.py
+-rwxr-xr-x   0        0        0     2990 2024-05-13 01:08:31.347266 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     5397 2024-04-17 03:33:22.101283 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1260 2024-05-13 01:11:04.626432 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/__pycache__/status_mass_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1066 2024-05-13 01:11:04.938430 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/__pycache__/status_volume_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      421 2024-04-17 03:33:22.101283 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/label_splitter/__init__.py
+-rwxr-xr-x   0        0        0      563 2024-04-17 03:36:50.203023 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/label_splitter/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      946 2024-04-17 03:33:22.101283 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/label_splitter/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1344 2024-05-13 00:59:57.252563 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/status_mass_1.py
+-rwxr-xr-x   0        0        0      978 2024-05-13 00:59:57.252563 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/status_volume_1.py
+-rwxr-xr-x   0        0        0     1502 2024-05-13 00:59:57.252563 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/status_1.py
+-rwxr-xr-x   0        0        0      581 2024-05-13 00:59:57.248563 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_ops/retrieve/API_status_found_1.py
+-rwxr-xr-x   0        0        0      591 2024-05-13 00:59:57.248563 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_ops/retrieve/API_status_not_found_1.py
+-rwxr-xr-x   0        0        0     2301 2024-05-13 00:59:57.248563 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_ops/retrieve/__init__.py
+-rwxr-xr-x   0        0        0      745 2024-04-27 17:18:55.070676 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_ops/retrieve/__pycache__/API_status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      846 2024-05-13 01:14:34.865033 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_ops/retrieve/__pycache__/API_status_found_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      765 2024-05-13 01:14:34.881033 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_ops/retrieve/__pycache__/API_status_not_found_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2141 2024-05-13 01:08:31.359266 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_ops/retrieve/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1426 2024-05-13 01:11:04.942430 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_status/__pycache__/status_1_description.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1835 2024-05-13 01:11:04.722431 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_status/__pycache__/status_2_measures.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1550 2024-05-13 01:11:04.942430 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_status/__pycache__/status_3_measured_ingredients.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1594 2024-04-25 01:35:26.781309 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_status/__pycache__/status_4_land_essentials.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1703 2024-05-13 01:11:05.806424 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_status/__pycache__/status_4_lands.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1166 2024-05-13 00:59:57.252563 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_status/status_1_description.py
+-rwxr-xr-x   0        0        0     1874 2024-05-13 00:59:57.252563 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_status/status_2_measures.py
+-rwxr-xr-x   0        0        0     2081 2024-05-13 00:59:57.252563 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_status/status_3_measured_ingredients.py
+-rwxr-xr-x   0        0        0     1503 2024-05-13 00:59:57.252563 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_status/status_4_lands.py
+-rwxr-xr-x   0        0        0     2087 2024-05-13 01:11:03.694437 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_status_v1/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1598 2024-05-13 01:11:04.946430 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_status_v1/__pycache__/status_2.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1112 2024-05-13 01:11:03.654437 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_status_v1/__pycache__/status_2412474.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1453 2024-05-13 01:11:05.070429 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_status_v1/__pycache__/status_3.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1215 2024-05-13 01:11:03.610437 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_status_v1/__pycache__/status_loop_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2777 2024-05-13 00:59:57.244563 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_status_v1/status_1.py
+-rwxr-xr-x   0        0        0     1625 2024-05-13 00:59:57.244563 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_status_v1/status_2.py
+-rwxr-xr-x   0        0        0      718 2024-05-13 00:59:57.244563 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_status_v1/status_2412474.py
+-rwxr-xr-x   0        0        0     1092 2024-05-13 00:59:57.244563 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_status_v1/status_3.py
+-rwxr-xr-x   0        0        0      854 2024-05-13 00:59:57.244563 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_status_v1/status_loop_1.py
+-rwxr-xr-x   0        0        0     2306 2024-05-13 00:59:57.248563 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/land/__init__.py
+-rwxr-xr-x   0        0        0     2113 2024-05-13 01:08:31.355266 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/land/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      466 2024-04-17 03:33:22.101283 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/__init__.py
+-rwxr-xr-x   0        0        0      568 2024-04-17 03:36:50.287021 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      957 2024-04-17 03:33:22.101283 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1172 2024-05-13 00:59:57.244563 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/_ops/for_each/__init__.py
+-rwxr-xr-x   0        0        0      839 2024-05-13 01:08:31.351266 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/_ops/for_each/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1012 2024-04-17 03:33:22.105283 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/_ops/for_each/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      707 2024-05-13 00:59:57.244563 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/_ops/seek/__init__.py
+-rwxr-xr-x   0        0        0      833 2024-05-13 01:08:31.351266 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/_ops/seek/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1272 2024-04-17 03:33:22.105283 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/_ops/seek/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1374 2024-05-13 01:11:04.294433 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/_ops/seek/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1072 2024-05-13 00:59:57.244563 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/_ops/seek/status_1.py
+-rwxr-xr-x   0        0        0     1993 2024-05-13 01:11:04.946430 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/_status/__pycache__/status_mass_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1011 2024-05-13 01:11:05.630425 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/_status/__pycache__/status_volume_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2089 2024-05-13 00:59:57.248563 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/_status/status_mass_1.py
+-rwxr-xr-x   0        0        0      724 2024-05-13 00:59:57.248563 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/_status/status_volume_1.py
+-rwxr-xr-x   0        0        0     1143 2024-04-17 03:33:22.105283 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured ingredients.S.HTML
+-rwxr-xr-x   0        0        0     1427 2024-05-13 00:59:57.244563 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/__init__.py
+-rwxr-xr-x   0        0        0     1121 2024-05-13 01:08:31.351266 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1591 2024-04-17 03:33:22.105283 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1675 2024-05-13 01:11:04.774431 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/_status/__pycache__/status_IU_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1517 2024-05-13 01:11:06.258422 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/_status/__pycache__/status_energy_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1615 2024-05-13 01:11:04.510432 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/_status/__pycache__/status_mass_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1776 2024-05-13 00:59:57.248563 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/_status/status_IU_1.py
+-rwxr-xr-x   0        0        0     1912 2024-05-13 00:59:57.248563 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/_status/status_energy_1.py
+-rwxr-xr-x   0        0        0     1616 2024-05-13 00:59:57.248563 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/_status/status_mass_1.py
+-rwxr-xr-x   0        0        0     1726 2024-05-13 00:59:57.244563 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/__init__.py
+-rwxr-xr-x   0        0        0     1442 2024-05-13 01:08:31.351266 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3142 2024-04-17 03:33:22.105283 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1240 2024-05-13 00:59:57.244563 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/biological_activity/__init__.py
+-rwxr-xr-x   0        0        0     1259 2024-05-13 01:08:31.351266 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/biological_activity/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1831 2024-04-17 03:33:22.105283 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/biological_activity/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1572 2024-05-13 00:59:57.248563 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/energy/__init__.py
+-rwxr-xr-x   0        0        0     1281 2024-05-13 01:08:31.351266 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/energy/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1791 2024-04-17 03:33:22.105283 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/energy/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1497 2024-05-13 00:59:57.248563 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/mass/__init__.py
+-rwxr-xr-x   0        0        0     1458 2024-05-13 01:08:31.351266 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/mass/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1842 2024-04-17 03:33:22.105283 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/mass/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      706 2024-04-17 03:36:50.291021 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/__pycache__/food_nutrient.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1040 2024-04-17 03:33:22.105283 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/__pycache__/food_nutrient.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1899 2024-04-17 03:33:22.105283 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/__pycache__/food_nutrient_calculator.cpython-311.pyc
+-rwxr-xr-x   0        0        0      651 2024-04-17 03:33:22.105283 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/__pycache__/label_nutrient.cpython-310.pyc
+-rwxr-xr-x   0        0        0      845 2024-04-17 03:33:22.105283 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/__pycache__/label_nutrient.cpython-311.pyc
+-rwxr-xr-x   0        0        0      849 2024-04-17 03:33:22.105283 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/__pycache__/label_nutrient_calculator.cpython-311.pyc
+-rwxr-xr-x   0        0        0      636 2024-04-17 03:33:22.105283 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/food_nutrient.py
+-rwxr-xr-x   0        0        0      483 2024-04-17 03:33:22.105283 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/label_nutrient.py
+-rwxr-xr-x   0        0        0      503 2024-04-17 03:33:22.105283 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/ingredient.r.HTML
+-rwxr-xr-x   0        0        0      706 2024-04-17 03:33:22.105283 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/ingredient_prototype_1.r.HTML
+-rwxr-xr-x   0        0        0     3867 2024-05-13 00:59:57.248563 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measures/form/__init__.py
+-rwxr-xr-x   0        0        0     2398 2024-05-13 01:08:31.347266 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measures/form/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4016 2024-04-17 03:33:22.105283 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measures/form/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1370 2024-05-13 01:11:06.290421 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measures/form/__pycache__/status_mass_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1401 2024-05-13 01:11:04.946430 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measures/form/__pycache__/status_volume_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      110 2024-04-17 03:33:22.105283 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measures/form/form.S.HTML
+-rwxr-xr-x   0        0        0     1238 2024-05-13 00:59:57.248563 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measures/form/status_mass_1.py
+-rwxr-xr-x   0        0        0     1181 2024-05-13 00:59:57.248563 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measures/form/status_volume_1.py
+-rwxr-xr-x   0        0        0      394 2024-05-13 00:59:57.252563 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/nature_v2.S.HTML
+-rwxr-xr-x   0        0        0      102 2024-04-17 03:33:22.105283 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/unmeasured_ingredients/__init__.py
+-rwxr-xr-x   0        0        0      338 2024-04-17 03:36:50.291021 goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/unmeasured_ingredients/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1046 2024-05-13 00:59:57.256563 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/NIH.s.HTML
+-rwxr-xr-x   0        0        0      536 2024-04-27 16:55:09.193236 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/deliveries/__pycache__/source.cpython-310.pyc
+-rwxr-xr-x   0        0        0      670 2024-04-17 03:33:22.105283 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/deliveries/__pycache__/source.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1090 2024-05-13 00:59:57.292563 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/deliveries/one/__init__.py
+-rwxr-xr-x   0        0        0     1201 2024-05-13 01:08:31.367266 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/deliveries/one/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1889 2024-04-17 03:33:22.105283 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/deliveries/one/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      815 2024-04-27 16:55:09.193236 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/deliveries/one/__pycache__/assertions.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1399 2024-04-17 03:33:22.105283 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/deliveries/one/__pycache__/assertions.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1087 2024-04-17 03:33:22.105283 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/deliveries/one/assertions.py
+-rwxr-xr-x   0        0        0      438 2024-05-13 00:59:57.292563 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/deliveries/one/status/API_status_1.py
+-rwxr-xr-x   0        0        0      706 2024-05-13 01:14:34.849033 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/deliveries/one/status/__pycache__/API_status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      316 2024-04-17 03:33:22.105283 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/deliveries/source.py
+-rwxr-xr-x   0        0        0      848 2024-05-13 00:59:57.252563 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/examples/__init__.py
+-rwxr-xr-x   0        0        0     1044 2024-05-13 01:11:09.506402 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/examples/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1918 2024-04-17 03:33:22.105283 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/examples/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0    44599 2024-05-13 00:59:57.256563 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/examples/coated tablets/multivitamin_276336.JSON
+-rwxr-xr-x   0        0        0     7111 2024-05-13 00:59:57.256563 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/examples/goodest_capsules/probiotics_248267.JSON
+-rwxr-xr-x   0        0        0    22180 2024-04-17 03:33:22.105283 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/examples/other/chia_seeds_214893.JSON
+-rwxr-xr-x   0        0        0     6430 2024-04-17 03:33:22.105283 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/examples/powder/mane_270619.JSON
+-rwxr-xr-x   0        0        0    72604 2024-05-13 00:59:57.252563 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/examples/powder/nutritional_shake_220884.JSON
+-rwxr-xr-x   0        0        0    57378 2024-04-17 03:33:22.105283 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/examples/powder packets/multivitamin_246811.JSON
+-rwxr-xr-x   0        0        0    22710 2024-04-17 03:33:22.105283 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/examples/tablets/calcium_261967.JSON
+-rwxr-xr-x   0        0        0    43729 2024-05-13 00:59:57.252563 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/examples/tablets/multivitamin_249664.JSON
+-rwxr-xr-x   0        0        0     4057 2024-05-13 00:59:57.264563 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/__init__.py
+-rwxr-xr-x   0        0        0     2766 2024-05-13 01:08:31.359266 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      271 2024-04-17 03:36:50.963008 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_interpret/ingredientRows/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      383 2024-04-17 03:33:22.105283 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_interpret/ingredientRows/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1151 2024-05-13 00:59:57.284563 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_interpret/ingredientRows/for_each/__init__.py
+-rwxr-xr-x   0        0        0      912 2024-05-13 01:08:31.363266 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_interpret/ingredientRows/for_each/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1201 2024-04-17 03:33:22.105283 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_interpret/ingredientRows/for_each/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1237 2024-05-13 01:11:05.510426 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_interpret/ingredientRows/for_each/__pycache__/status_powder_packets_246811.cpython-310.pyc
+-rwxr-xr-x   0        0        0      935 2024-05-13 00:59:57.284563 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_interpret/ingredientRows/for_each/status_powder_packets_246811.py
+-rwxr-xr-x   0        0        0       56 2024-04-17 03:33:22.109283 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_interpret/servingSizeUnit/__init__.py
+-rwxr-xr-x   0        0        0     2278 2024-05-13 00:59:57.264563 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_ops/retrieve/__init__.py
+-rwxr-xr-x   0        0        0     2047 2024-05-13 01:08:31.367266 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_ops/retrieve/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1418 2024-05-13 01:11:05.662425 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/__pycache__/status_1_info.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1426 2024-05-13 01:11:05.070429 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/__pycache__/status_2_form.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1837 2024-05-13 01:11:05.794424 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/__pycache__/status_3_measured_ingredients.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1236 2024-04-25 18:59:21.733410 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/__pycache__/status_4_essential_nutrients.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1484 2024-05-13 01:11:06.638419 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/__pycache__/status_4_unmeasured_ingredients.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1673 2024-05-13 01:11:05.710425 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/__pycache__/status_5_essential_nutrients.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1601 2024-05-13 01:11:06.410421 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/__pycache__/status_6_cautionary_ingredients.cpython-310.pyc
+-rwxr-xr-x   0        0        0    28721 2024-05-14 01:27:56.970346 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/mane_270619_nature.JSON
+-rwxr-xr-x   0        0        0   124537 2024-05-14 01:27:57.074345 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/multivitamin_249664.JSON
+-rwxr-xr-x   0        0        0     1040 2024-05-13 00:59:57.288563 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/status_1_info.py
+-rwxr-xr-x   0        0        0     1050 2024-05-13 00:59:57.288563 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/status_2_form.py
+-rwxr-xr-x   0        0        0     1620 2024-05-13 00:59:57.288563 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/status_3_measured_ingredients.py
+-rwxr-xr-x   0        0        0     1071 2024-05-13 00:59:57.288563 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/status_4_unmeasured_ingredients.py
+-rwxr-xr-x   0        0        0     1279 2024-05-13 00:59:57.288563 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/status_5_essential_nutrients.py
+-rwxr-xr-x   0        0        0     1172 2024-05-13 00:59:57.288563 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/status_6_cautionary_ingredients.py
+-rwxr-xr-x   0        0        0      836 2024-05-13 01:11:05.882424 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_status_v1/_loop/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      742 2024-05-13 00:59:57.260563 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_status_v1/_loop/status_1.py
+-rwxr-xr-x   0        0        0     1751 2024-05-13 01:11:05.318427 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_status_v1/coated_tablets/__pycache__/status_multivitamin_276336.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1563 2024-05-13 00:59:57.260563 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_status_v1/coated_tablets/status_multivitamin_276336.py
+-rwxr-xr-x   0        0        0   136807 2024-05-14 01:27:56.506351 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_status_v1/coated_tablets/status_multivitamin_276336_nature.JSON
+-rwxr-xr-x   0        0        0     1217 2024-05-13 01:11:05.138428 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_status_v1/other/__pycache__/status_chia_seeds_214893.cpython-310.pyc
+-rwxr-xr-x   0        0        0    82230 2024-05-14 01:27:56.994346 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_status_v1/other/chia_seeds_214893_nature.JSON
+-rwxr-xr-x   0        0        0      767 2024-05-13 00:59:57.260563 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_status_v1/other/status_chia_seeds_214893.py
+-rwxr-xr-x   0        0        0     1180 2024-05-13 01:11:05.570426 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_status_v1/powder/__pycache__/status_mane_270619.cpython-310.pyc
+-rwxr-xr-x   0        0        0    28721 2024-05-14 01:27:56.530351 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_status_v1/powder/mane_270619_nature.JSON
+-rwxr-xr-x   0        0        0      740 2024-05-13 00:59:57.256563 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_status_v1/powder/status_mane_270619.py
+-rwxr-xr-x   0        0        0      568 2024-04-25 04:11:27.433921 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      672 2024-04-17 03:33:22.109283 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      667 2024-05-13 00:59:57.284563 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/amount/__init__.py
+-rwxr-xr-x   0        0        0      866 2024-05-13 01:08:31.363266 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/amount/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1333 2024-04-17 03:33:22.109283 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/amount/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      773 2024-05-13 01:11:05.642425 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/amount/__pycache__/status_other_214893.cpython-310.pyc
+-rwxr-xr-x   0        0        0      514 2024-05-13 00:59:57.284563 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/amount/status_other_214893.py
+-rwxr-xr-x   0        0        0      512 2024-04-17 03:33:22.109283 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/form.S.HTML
+-rwxr-xr-x   0        0        0     3998 2024-05-13 00:59:57.284563 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/serving_size/amount/__init__.py
+-rwxr-xr-x   0        0        0     2359 2024-05-13 01:08:31.363266 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/serving_size/amount/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0        5 2024-04-17 03:33:22.109283 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/serving_size/amount/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      179 2024-04-17 03:36:51.818991 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/serving_size/amount/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1579 2024-05-13 01:11:06.066423 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/serving_size/amount/__pycache__/status_246811.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1556 2024-05-13 01:11:05.866424 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/serving_size/amount/__pycache__/status_276336.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1785 2024-05-13 00:59:57.284563 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/serving_size/amount/status_246811.py
+-rwxr-xr-x   0        0        0     1672 2024-05-13 00:59:57.284563 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/serving_size/amount/status_276336.py
+-rwxr-xr-x   0        0        0     3227 2024-05-13 00:59:57.284563 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/__init__.py
+-rwxr-xr-x   0        0        0     2679 2024-05-13 01:08:31.359266 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0        5 2024-04-17 03:33:22.109283 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1203 2024-05-13 01:11:06.354421 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/__pycache__/status_coated_tablet_276336.cpython-310.pyc
+-rwxr-xr-x   0        0        0      991 2024-05-13 01:11:06.470420 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/__pycache__/status_goodest_capsule_248267.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1004 2024-05-13 01:11:06.042423 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/__pycache__/status_gram_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1010 2024-05-13 01:11:05.230428 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/__pycache__/status_powder_220884.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1043 2024-05-13 01:11:06.042423 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/__pycache__/status_powder_270619.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1426 2024-05-13 01:11:05.450426 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/__pycache__/status_powder_packets_246811.cpython-310.pyc
+-rwxr-xr-x   0        0        0      953 2024-05-13 01:11:04.994429 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/__pycache__/status_tablet_261967.cpython-310.pyc
+-rwxr-xr-x   0        0        0      933 2024-05-13 00:59:57.284563 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/status_coated_tablet_276336.py
+-rwxr-xr-x   0        0        0      731 2024-05-13 00:59:57.284563 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/status_goodest_capsule_248267.py
+-rwxr-xr-x   0        0        0      818 2024-05-13 00:59:57.264563 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/status_gram_1.py
+-rwxr-xr-x   0        0        0      822 2024-05-13 00:59:57.284563 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/status_powder_220884.py
+-rwxr-xr-x   0        0        0      895 2024-05-13 00:59:57.284563 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/status_powder_270619.py
+-rwxr-xr-x   0        0        0     1337 2024-05-13 00:59:57.284563 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/status_powder_packets_246811.py
+-rwxr-xr-x   0        0        0      705 2024-05-13 00:59:57.284563 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/status_tablet_261967.py
+-rwxr-xr-x   0        0        0     1971 2024-05-13 00:59:57.264563 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/land/__init__.py
+-rwxr-xr-x   0        0        0     2058 2024-05-13 01:08:31.367266 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/land/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1703 2024-05-13 00:59:57.260563 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/__init__.py
+-rwxr-xr-x   0        0        0     1944 2024-05-13 01:08:31.363266 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2911 2024-04-17 03:33:22.109283 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1121 2024-05-13 00:59:57.260563 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek/__init__.py
+-rwxr-xr-x   0        0        0     1085 2024-05-13 01:08:31.363266 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1442 2024-04-17 03:33:22.109283 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      967 2024-05-13 01:11:06.018423 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      666 2024-05-13 00:59:57.260563 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek/status_1.py
+-rwxr-xr-x   0        0        0      591 2024-05-13 00:59:57.260563 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek_name/__init__.py
+-rwxr-xr-x   0        0        0      998 2024-05-13 01:11:09.506402 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek_name/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1171 2024-04-17 03:33:22.113283 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek_name/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1084 2024-05-13 01:11:05.850424 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/_status/__pycache__/status_chia_seeds_214893.cpython-310.pyc
+-rwxr-xr-x   0        0        0      807 2024-05-13 00:59:57.264563 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/_status/status_chia_seeds_214893.py
+-rwxr-xr-x   0        0        0     4671 2024-05-13 00:59:57.264563 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/measured_ingredient/__init__.py
+-rwxr-xr-x   0        0        0     2809 2024-05-13 01:08:31.363266 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/measured_ingredient/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4500 2024-04-17 03:33:22.109283 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/measured_ingredient/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1636 2024-05-13 01:11:06.542420 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/measured_ingredient/_status/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1731 2024-05-13 00:59:57.264563 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/measured_ingredient/_status/status_1.py
+-rwxr-xr-x   0        0        0     1514 2024-04-17 03:33:22.109283 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/measured_ingredient/measured_ingredient.S.HTML
+-rwxr-xr-x   0        0        0      561 2024-04-17 03:33:22.109283 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/measured_ingredients.S.HTML
+-rwxr-xr-x   0        0        0        3 2024-04-25 01:50:49.197454 goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/natures_v2.S.HTML
+-rwxr-xr-x   0        0        0       87 2024-04-27 20:03:02.828977 goodest-1.2.2/venues/stages/goodest/goals/goals.S.HTML
+-rwxr-xr-x   0        0        0     8906 2024-05-13 00:59:57.244563 goodest-1.2.2/venues/stages/goodest/goals/umuntu/FDA.py
+-rwxr-xr-x   0        0        0     9794 2024-03-09 19:44:16.627477 goodest-1.2.2/venues/stages/goodest/goals/umuntu/FDA_v1.py
+-rwxr-xr-x   0        0        0     4193 2024-03-10 18:32:48.701726 goodest-1.2.2/venues/stages/goodest/goals/umuntu/FDA_v2.py
+-rwxr-xr-x   0        0        0     7523 2024-03-12 19:40:02.502146 goodest-1.2.2/venues/stages/goodest/goals/umuntu/FDA_v3.py
+-rwxr-xr-x   0        0        0     4343 2024-05-13 02:40:08.095827 goodest-1.2.2/venues/stages/goodest/goals/umuntu/__pycache__/FDA.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3847 2024-03-14 19:34:32.350499 goodest-1.2.2/venues/stages/goodest/goals/umuntu/__pycache__/FDA_v3.cpython-310.pyc
+-rwxr-xr-x   0        0        0       71 2024-04-27 16:41:36.022921 goodest-1.2.2/venues/stages/goodest/goals/umuntu/_journal/Carbohydrates.s.HTML
+-rwxr-xr-x   0        0        0       61 2024-04-27 16:41:31.750949 goodest-1.2.2/venues/stages/goodest/goals/umuntu/_journal/Fat.s.HTML
+-rwxr-xr-x   0        0        0       64 2024-04-27 16:41:27.998973 goodest-1.2.2/venues/stages/goodest/goals/umuntu/_journal/Lipids.s.HTML
+-rwxr-xr-x   0        0        0      145 2024-04-27 16:41:20.183024 goodest-1.2.2/venues/stages/goodest/goals/umuntu/_journal/Protein.s.HTML
+-rwxr-xr-x   0        0        0       16 2024-01-31 21:52:02.234756 goodest-1.2.2/venues/stages/goodest/goals/umuntu/_journal/Vitamin A.s.HTML
+-rwxr-xr-x   0        0        0        0 2024-01-31 21:52:25.962491 goodest-1.2.2/venues/stages/goodest/goals/umuntu/_journal/Vitamin B.s.HTML
+-rwxr-xr-x   0        0        0       68 2024-04-27 16:40:48.275230 goodest-1.2.2/venues/stages/goodest/goals/umuntu/_journal/Vitamin C.s.HTML
+-rwxr-xr-x   0        0        0       65 2024-04-27 16:40:44.111256 goodest-1.2.2/venues/stages/goodest/goals/umuntu/_journal/Vitamin D.s.HTML
+-rwxr-xr-x   0        0        0      423 2024-04-27 16:42:29.518570 goodest-1.2.2/venues/stages/goodest/goals/umuntu/_journal/Vitamin E.s.HTML
+-rwxr-xr-x   0        0        0      553 2024-04-28 02:16:08.201921 goodest-1.2.2/venues/stages/goodest/goals/umuntu/_ops/__pycache__/retrieve.cpython-310.pyc
+-rwxr-xr-x   0        0        0      358 2024-05-13 00:59:57.244563 goodest-1.2.2/venues/stages/goodest/goals/umuntu/_ops/retrieve.py
+-rwxr-xr-x   0        0        0        3 2024-03-10 18:23:03.506534 goodest-1.2.2/venues/stages/goodest/goals/umuntu/parse_FDA.proc.py
+-rwxr-xr-x   0        0        0      488 2024-04-28 00:30:07.297621 goodest-1.2.2/venues/stages/goodest/goals/umuntu/umuntu.S.HTML
+-rwxr-xr-x   0        0        0       14 2024-04-17 03:33:22.129283 goodest-1.2.2/venues/stages/goodest/goodest -- emojis.S.HTML
+-rwxr-xr-x   0        0        0     4710 2024-05-13 00:59:01.377145 goodest-1.2.2/venues/stages/goodest/goodest.S.HTML
+-rwxr-xr-x   0        0        0      632 2024-04-17 03:33:22.129283 goodest-1.2.2/venues/stages/goodest/goodest.css
+-rwxr-xr-x   0        0        0      805 2024-05-13 01:11:03.378439 goodest-1.2.2/venues/stages/goodest/measures/_interpret/__pycache__/status_unit_kind.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1473 2024-05-13 01:08:31.347266 goodest-1.2.2/venues/stages/goodest/measures/_interpret/__pycache__/unit_kind.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2547 2024-04-17 03:33:22.113283 goodest-1.2.2/venues/stages/goodest/measures/_interpret/__pycache__/unit_kind.cpython-311.pyc
+-rwxr-xr-x   0        0        0       61 2024-04-17 03:33:22.113283 goodest-1.2.2/venues/stages/goodest/measures/_interpret/interpret.S.HTML
+-rwxr-xr-x   0        0        0      669 2024-05-13 00:59:01.385145 goodest-1.2.2/venues/stages/goodest/measures/_interpret/status_unit_kind.py
+-rwxr-xr-x   0        0        0     1677 2024-05-13 00:59:01.385145 goodest-1.2.2/venues/stages/goodest/measures/_interpret/unit_kind.py
+-rwxr-xr-x   0        0        0        0 2024-04-17 03:33:22.113283 goodest-1.2.2/venues/stages/goodest/measures/biological_activity/__init__.py
+-rwxr-xr-x   0        0        0       59 2024-04-17 03:33:22.113283 goodest-1.2.2/venues/stages/goodest/measures/electric_current/electric_current.S.HTML
+-rwxr-xr-x   0        0        0     1355 2024-05-04 16:59:01.497380 goodest-1.2.2/venues/stages/goodest/measures/energy/energy.r.HTML
+-rwxr-xr-x   0        0        0     1173 2024-05-13 00:59:01.385145 goodest-1.2.2/venues/stages/goodest/measures/energy/swap/__init__.py
+-rwxr-xr-x   0        0        0     1020 2024-05-13 01:08:31.351266 goodest-1.2.2/venues/stages/goodest/measures/energy/swap/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1761 2024-04-17 03:33:22.113283 goodest-1.2.2/venues/stages/goodest/measures/energy/swap/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      624 2024-05-13 01:11:03.798436 goodest-1.2.2/venues/stages/goodest/measures/energy/swap/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      385 2024-05-13 00:59:01.385145 goodest-1.2.2/venues/stages/goodest/measures/energy/swap/status_1.py
+-rwxr-xr-x   0        0        0       71 2024-04-17 03:33:22.113283 goodest-1.2.2/venues/stages/goodest/measures/length/length.r.HTML
+-rwxr-xr-x   0        0        0       95 2024-04-17 03:33:22.113283 goodest-1.2.2/venues/stages/goodest/measures/mass/e_note.py
+-rwxr-xr-x   0        0        0       12 2024-04-17 03:33:22.113283 goodest-1.2.2/venues/stages/goodest/measures/mass/mass.r.html
+-rwxr-xr-x   0        0        0     2328 2024-05-13 00:59:01.385145 goodest-1.2.2/venues/stages/goodest/measures/mass/swap/__init__.py
+-rwxr-xr-x   0        0        0     1728 2024-05-13 01:08:31.347266 goodest-1.2.2/venues/stages/goodest/measures/mass/swap/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3229 2024-04-17 03:33:22.113283 goodest-1.2.2/venues/stages/goodest/measures/mass/swap/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1147 2024-05-13 01:11:04.230434 goodest-1.2.2/venues/stages/goodest/measures/mass/swap/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1152 2024-05-13 00:59:01.385145 goodest-1.2.2/venues/stages/goodest/measures/mass/swap/status_1.py
+-rwxr-xr-x   0        0        0     2419 2024-04-17 03:33:22.113283 goodest-1.2.2/venues/stages/goodest/measures/mass/system international.r.html
+-rwxr-xr-x   0        0        0      768 2024-04-17 03:33:22.113283 goodest-1.2.2/venues/stages/goodest/measures/mass/us customary.r.html
+-rwxr-xr-x   0        0        0      522 2024-05-13 00:59:01.385145 goodest-1.2.2/venues/stages/goodest/measures/mass_equivalents/is_an_equivalent/__init__.py
+-rwxr-xr-x   0        0        0      636 2024-05-13 01:11:08.834406 goodest-1.2.2/venues/stages/goodest/measures/mass_equivalents/is_an_equivalent/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      945 2024-04-17 03:33:22.113283 goodest-1.2.2/venues/stages/goodest/measures/mass_equivalents/is_an_equivalent/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      611 2024-05-13 01:11:04.754431 goodest-1.2.2/venues/stages/goodest/measures/mass_equivalents/is_an_equivalent/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      341 2024-05-13 00:59:01.385145 goodest-1.2.2/venues/stages/goodest/measures/mass_equivalents/is_an_equivalent/status_1.py
+-rwxr-xr-x   0        0        0      861 2024-04-17 03:33:22.113283 goodest-1.2.2/venues/stages/goodest/measures/mass_equivalents/jargon.r.HTML
+-rwxr-xr-x   0        0        0     2242 2024-04-17 03:33:22.113283 goodest-1.2.2/venues/stages/goodest/measures/mass_equivalents/mass equivalents.r.HTML
+-rwxr-xr-x   0        0        0     2430 2024-05-13 00:59:01.381145 goodest-1.2.2/venues/stages/goodest/measures/number/decimal/reduce/__init__.py
+-rwxr-xr-x   0        0        0     1580 2024-05-13 01:08:31.347266 goodest-1.2.2/venues/stages/goodest/measures/number/decimal/reduce/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3068 2024-04-17 03:33:22.113283 goodest-1.2.2/venues/stages/goodest/measures/number/decimal/reduce/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1144 2024-05-13 01:11:04.222434 goodest-1.2.2/venues/stages/goodest/measures/number/decimal/reduce/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      851 2024-05-13 01:11:03.354439 goodest-1.2.2/venues/stages/goodest/measures/number/decimal/reduce/__pycache__/status_2.cpython-310.pyc
+-rwxr-xr-x   0        0        0      919 2024-05-13 01:11:03.250440 goodest-1.2.2/venues/stages/goodest/measures/number/decimal/reduce/__pycache__/status_3.cpython-310.pyc
+-rwxr-xr-x   0        0        0      651 2024-05-13 01:11:04.102435 goodest-1.2.2/venues/stages/goodest/measures/number/decimal/reduce/__pycache__/status_sci_note_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1427 2024-05-13 00:59:01.381145 goodest-1.2.2/venues/stages/goodest/measures/number/decimal/reduce/status_1.py
+-rwxr-xr-x   0        0        0      900 2024-05-13 00:59:01.381145 goodest-1.2.2/venues/stages/goodest/measures/number/decimal/reduce/status_2.py
+-rwxr-xr-x   0        0        0     1114 2024-05-13 00:59:01.381145 goodest-1.2.2/venues/stages/goodest/measures/number/decimal/reduce/status_3.py
+-rwxr-xr-x   0        0        0      469 2024-05-13 00:59:01.381145 goodest-1.2.2/venues/stages/goodest/measures/number/decimal/reduce/status_sci_note_1.py
+-rwxr-xr-x   0        0        0      168 2024-04-17 03:33:22.113283 goodest-1.2.2/venues/stages/goodest/measures/number/fraction_point/fraction_point.s.HTML
+-rwxr-xr-x   0        0        0      713 2024-05-13 01:11:03.514438 goodest-1.2.2/venues/stages/goodest/measures/number/integer/__pycache__/status_string_is_integer.cpython-310.pyc
+-rwxr-xr-x   0        0        0      531 2024-05-13 01:08:31.363266 goodest-1.2.2/venues/stages/goodest/measures/number/integer/__pycache__/string_is_integer.cpython-310.pyc
+-rwxr-xr-x   0        0        0      749 2024-04-17 03:33:22.113283 goodest-1.2.2/venues/stages/goodest/measures/number/integer/__pycache__/string_is_integer.cpython-311.pyc
+-rwxr-xr-x   0        0        0      559 2024-05-13 00:59:01.381145 goodest-1.2.2/venues/stages/goodest/measures/number/integer/status_string_is_integer.py
+-rwxr-xr-x   0        0        0      367 2024-05-13 00:59:01.381145 goodest-1.2.2/venues/stages/goodest/measures/number/integer/string_is_integer.py
+-rwxr-xr-x   0        0        0      891 2024-05-13 01:11:08.342409 goodest-1.2.2/venues/stages/goodest/measures/number/percentage/__pycache__/from_fraction.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1702 2024-04-17 03:33:22.113283 goodest-1.2.2/venues/stages/goodest/measures/number/percentage/__pycache__/from_fraction.cpython-311.pyc
+-rwxr-xr-x   0        0        0      744 2024-05-13 01:11:03.342439 goodest-1.2.2/venues/stages/goodest/measures/number/percentage/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      950 2024-05-13 00:59:01.381145 goodest-1.2.2/venues/stages/goodest/measures/number/percentage/from_fraction.py
+-rwxr-xr-x   0        0        0      552 2024-05-13 00:59:01.385145 goodest-1.2.2/venues/stages/goodest/measures/number/percentage/status_1.py
+-rwxr-xr-x   0        0        0     2209 2024-05-13 00:59:01.381145 goodest-1.2.2/venues/stages/goodest/measures/number/sci_note/__init__.py
+-rwxr-xr-x   0        0        0     1362 2024-05-13 01:11:04.386433 goodest-1.2.2/venues/stages/goodest/measures/number/sci_note/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2246 2024-05-13 01:11:03.294439 goodest-1.2.2/venues/stages/goodest/measures/number/sci_note/_status/__pycache__/status_multiples_of_3_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3223 2024-05-13 00:59:01.381145 goodest-1.2.2/venues/stages/goodest/measures/number/sci_note/_status/status_multiples_of_3_1.py
+-rwxr-xr-x   0        0        0      612 2024-04-17 03:33:22.113283 goodest-1.2.2/venues/stages/goodest/measures/number/sci_note/sci_note.S.HTML
+-rwxr-xr-x   0        0        0      644 2024-04-17 03:33:22.113283 goodest-1.2.2/venues/stages/goodest/measures/number/sci_note/sci_note_possibilities.S.HTML
+-rwxr-xr-x   0        0        0     1341 2024-05-13 00:59:01.381145 goodest-1.2.2/venues/stages/goodest/measures/number/sci_note/sci_note_thoughts.S.HTML
+-rwxr-xr-x   0        0        0      362 2024-05-13 00:59:01.381145 goodest-1.2.2/venues/stages/goodest/measures/number/sci_note_2/__init__.py
+-rwxr-xr-x   0        0        0      601 2024-05-13 01:08:31.267266 goodest-1.2.2/venues/stages/goodest/measures/number/sci_note_2/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1219 2024-05-13 01:11:04.566432 goodest-1.2.2/venues/stages/goodest/measures/number/sci_note_2/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      935 2024-05-13 00:59:01.381145 goodest-1.2.2/venues/stages/goodest/measures/number/sci_note_2/status_1.py
+-rwxr-xr-x   0        0        0       58 2024-04-17 03:33:22.113283 goodest-1.2.2/venues/stages/goodest/measures/temperature/temperature.r.html
+-rwxr-xr-x   0        0        0     2204 2024-05-13 00:59:01.385145 goodest-1.2.2/venues/stages/goodest/measures/volume/swap/__init__.py
+-rwxr-xr-x   0        0        0     1476 2024-05-13 01:08:31.347266 goodest-1.2.2/venues/stages/goodest/measures/volume/swap/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2595 2024-04-17 03:33:22.113283 goodest-1.2.2/venues/stages/goodest/measures/volume/swap/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1689 2024-05-13 01:11:04.302433 goodest-1.2.2/venues/stages/goodest/measures/volume/swap/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1665 2024-05-13 00:59:01.385145 goodest-1.2.2/venues/stages/goodest/measures/volume/swap/status_1.py
+-rwxr-xr-x   0        0        0      510 2024-04-17 03:33:22.113283 goodest-1.2.2/venues/stages/goodest/measures/volume/volume.html
+-rwxr-xr-x   0        0        0      911 2024-04-17 03:33:22.113283 goodest-1.2.2/venues/stages/goodest/measures/weight/weight.r.html
+-rwxr-xr-x   0        0        0      440 2024-05-13 01:04:39.757620 goodest-1.2.2/venues/stages/goodest/mixes/docks/__pycache__/address.cpython-310.pyc
+-rwxr-xr-x   0        0        0      217 2024-05-13 00:59:01.381145 goodest-1.2.2/venues/stages/goodest/mixes/docks/address.py
+-rwxr-xr-x   0        0        0      762 2024-05-13 21:38:47.355615 goodest-1.2.2/venues/stages/goodest/mixes/drives/etch/__pycache__/bracket.cpython-310.pyc
+-rwxr-xr-x   0        0        0      462 2024-05-13 21:38:40.119718 goodest-1.2.2/venues/stages/goodest/mixes/drives/etch/bracket.py
+-rwxr-xr-x   0        0        0     1034 2024-05-13 01:08:31.363266 goodest-1.2.2/venues/stages/goodest/mixes/insure/__pycache__/equalities.cpython-310.pyc
+-rwxr-xr-x   0        0        0        5 2024-04-17 03:33:22.113283 goodest-1.2.2/venues/stages/goodest/mixes/insure/__pycache__/equalities.cpython-311.pyc
+-rwxr-xr-x   0        0        0      466 2024-05-13 01:11:05.386427 goodest-1.2.2/venues/stages/goodest/mixes/insure/__pycache__/equality.cpython-310.pyc
+-rwxr-xr-x   0        0        0        5 2024-04-17 03:33:22.113283 goodest-1.2.2/venues/stages/goodest/mixes/insure/__pycache__/equality.cpython-311.pyc
+-rwxr-xr-x   0        0        0      988 2024-05-13 01:11:06.986417 goodest-1.2.2/venues/stages/goodest/mixes/insure/__pycache__/override_print.cpython-310.pyc
+-rwxr-xr-x   0        0        0        5 2024-04-17 03:33:22.113283 goodest-1.2.2/venues/stages/goodest/mixes/insure/__pycache__/override_print.cpython-311.pyc
+-rwxr-xr-x   0        0        0      585 2024-05-13 01:11:04.214434 goodest-1.2.2/venues/stages/goodest/mixes/insure/__pycache__/status_equalitites_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1090 2024-05-13 00:59:01.381145 goodest-1.2.2/venues/stages/goodest/mixes/insure/equalities.py
+-rwxr-xr-x   0        0        0      239 2024-05-13 00:59:01.381145 goodest-1.2.2/venues/stages/goodest/mixes/insure/equality.py
+-rwxr-xr-x   0        0        0      783 2024-05-13 00:59:01.381145 goodest-1.2.2/venues/stages/goodest/mixes/insure/override_print.py
+-rwxr-xr-x   0        0        0      379 2024-05-13 00:59:01.381145 goodest-1.2.2/venues/stages/goodest/mixes/insure/status_equalitites_1.py
+-rwxr-xr-x   0        0        0      579 2024-05-13 00:59:01.381145 goodest-1.2.2/venues/stages/goodest/mixes/procedure/__init__.py
+-rwxr-xr-x   0        0        0     1007 2024-05-13 01:04:39.753620 goodest-1.2.2/venues/stages/goodest/mixes/procedure/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1631 2024-05-14 01:15:58.290298 goodest-1.2.2/venues/stages/goodest/readme.md
+-rwxr-xr-x   0        0        0     1900 2024-05-13 00:59:01.397145 goodest-1.2.2/venues/stages/goodest/shows_v2/goodness_certifications/certifications.py
+-rwxr-xr-x   0        0        0      674 2024-05-13 00:59:01.397145 goodest-1.2.2/venues/stages/goodest/shows_v2/goodness_certifications/goodest.S.HTML
+-rwxr-xr-x   0        0        0     1608 2024-05-13 01:11:05.390427 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/_ops/assertions/__pycache__/ingredient.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2799 2024-05-13 00:59:01.397145 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/_ops/assertions/ingredient.py
+-rwxr-xr-x   0        0        0     1257 2024-05-13 00:59:01.397145 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/_ops/formulate/__init__.py
+-rwxr-xr-x   0        0        0      686 2024-05-13 01:08:31.259266 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/_ops/formulate/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1520 2024-05-13 01:11:05.346427 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_empty/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1272 2024-05-13 00:59:01.397145 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_empty/status_1.py
+-rwxr-xr-x   0        0        0     1812 2024-05-13 01:11:03.906436 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_food/__pycache__/status_0.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3682 2024-05-13 01:11:04.934430 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_food/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2792 2024-05-13 01:11:03.534438 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_food/__pycache__/status_2.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2012 2024-05-13 01:11:05.934424 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_food/__pycache__/status_3.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2381 2024-05-13 00:59:01.397145 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_food/status_0.py
+-rwxr-xr-x   0        0        0     6527 2024-05-13 00:59:01.397145 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_food/status_1.py
+-rwxr-xr-x   0        0        0     3894 2024-05-13 00:59:01.397145 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_food/status_2.py
+-rwxr-xr-x   0        0        0     2382 2024-05-13 00:59:01.397145 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_food/status_3.py
+-rwxr-xr-x   0        0        0     2782 2024-05-13 01:11:04.162434 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_foods_and_supps/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0   200787 2024-05-14 01:27:54.730371 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_foods_and_supps/status_1.JSON
+-rwxr-xr-x   0        0        0     2107 2024-05-13 00:59:01.397145 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_foods_and_supps/status_1.py
+-rwxr-xr-x   0        0        0     2676 2024-05-13 01:11:04.262434 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_rational_amounts/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0   112672 2024-05-14 01:27:57.302343 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_rational_amounts/status_1.JSON
+-rwxr-xr-x   0        0        0     1931 2024-05-13 00:59:01.397145 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_rational_amounts/status_1.py
+-rwxr-xr-x   0        0        0     2351 2024-05-13 01:11:04.270434 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_supp/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1924 2024-05-13 01:11:04.226434 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_supp/__pycache__/status_1_supp_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0   109562 2024-05-14 01:27:56.258354 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_supp/status_1.JSON
+-rwxr-xr-x   0        0        0     1825 2024-05-13 00:59:01.397145 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_supp/status_1.py
+-rwxr-xr-x   0        0        0     1426 2024-05-13 00:59:01.397145 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_supp/status_1_supp_1.py
+-rwxr-xr-x   0        0        0     2560 2024-05-13 04:13:39.302285 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/_ops/retrieve/__init__.py
+-rwxr-xr-x   0        0        0     1708 2024-05-13 04:13:42.582244 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/_ops/retrieve/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      671 2024-05-13 04:01:03.341098 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/_ops/retrieve/_status/API_status_1.py
+-rwxr-xr-x   0        0        0      825 2024-05-13 23:01:43.300966 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/_ops/retrieve/_status/__pycache__/API_status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2885 2024-05-13 04:15:32.480875 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/land/_ops/formulate/__init__.py
+-rwxr-xr-x   0        0        0     2315 2024-05-13 04:16:40.936035 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/land/_ops/formulate/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      235 2024-05-13 00:59:01.397145 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/recipe.S.HTML
+-rwxr-xr-x   0        0        0     2532 2024-04-28 00:40:14.210697 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/__pycache__/formulate.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1425 2024-05-13 22:03:44.585463 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/for_1_food/__init__.py
+-rwxr-xr-x   0        0        0     1056 2024-05-13 22:06:23.071845 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/for_1_food/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1321 2024-05-13 21:52:11.753431 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/for_1_food/_status/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1391 2024-05-13 21:51:59.965570 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/for_1_food/_status/status_1.py
+-rwxr-xr-x   0        0        0    92943 2024-05-14 01:27:57.358342 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/for_1_food/_status/status_1_food.JSON
+-rwxr-xr-x   0        0        0     1098 2024-05-13 22:15:08.035569 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/for_1_supp/__init__.py
+-rwxr-xr-x   0        0        0     1190 2024-05-13 22:15:11.771535 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/for_1_supp/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1337 2024-05-13 22:02:42.690165 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/for_1_supp/_status/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1414 2024-05-13 22:02:38.842208 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/for_1_supp/_status/status_1.py
+-rwxr-xr-x   0        0        0   236544 2024-05-14 01:27:56.914347 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/for_1_supp/_status/status_1_supp.JSON
+-rwxr-xr-x   0        0        0     1948 2024-05-13 21:54:01.336147 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/__init__.py
+-rwxr-xr-x   0        0        0     1399 2024-05-13 21:54:06.060092 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2969 2024-05-13 19:19:14.229533 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status/1_2_recipe_preformulated/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0    93876 2024-05-14 01:27:53.830381 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status/1_2_recipe_preformulated/status_1.JSON
+-rwxr-xr-x   0        0        0     2690 2024-05-13 19:19:08.473594 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status/1_2_recipe_preformulated/status_1.py
+-rwxr-xr-x   0        0        0     2957 2024-05-13 19:23:38.590709 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status/1_3_recipe_prefomulated/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0   214187 2024-05-14 01:27:57.762337 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status/1_3_recipe_prefomulated/status_1.JSON
+-rwxr-xr-x   0        0        0     2403 2024-05-13 19:12:01.686200 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status/1_3_recipe_prefomulated/status_1.py
+-rwxr-xr-x   0        0        0     2658 2024-05-13 01:11:04.110435 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status/2_food/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0    58054 2024-05-14 01:27:56.918347 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status/2_food/status_1.JSON
+-rwxr-xr-x   0        0        0     1949 2024-05-13 00:59:01.401145 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status/2_food/status_1.py
+-rwxr-xr-x   0        0        0     1869 2024-05-13 23:09:11.573526 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_1_recipe/API_status_1.py
+-rwxr-xr-x   0        0        0     1899 2024-05-13 23:09:18.509470 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_1_recipe/__pycache__/API_status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1880 2024-04-28 17:59:07.380196 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_1_recipe/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0    93917 2024-05-14 00:55:59.862218 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_1_recipe/status_1.JSON
+-rwxr-xr-x   0        0        0     1602 2024-05-13 04:01:55.736218 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_2_recipe/API_status_1.py
+-rwxr-xr-x   0        0        0     1872 2024-05-13 23:01:43.324966 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_2_recipe/__pycache__/API_status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1853 2024-04-28 17:57:44.252665 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_2_recipe/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0   214139 2024-05-14 00:56:02.334190 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_2_recipe/status_1.JSON
+-rwxr-xr-x   0        0        0     1664 2024-04-28 04:43:21.416236 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status_API/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2367 2024-05-14 00:10:09.982882 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/modules/__pycache__/add_goals.cpython-310.pyc
+-rwxr-xr-x   0        0        0      585 2024-05-13 18:58:53.655214 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/modules/__pycache__/find_goal.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2905 2024-05-14 00:10:06.494940 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/modules/add_goals.py
+-rwxr-xr-x   0        0        0      481 2024-05-13 18:58:48.467276 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/modules/find_goal.py
+-rwxr-xr-x   0        0        0     1421 2024-04-28 02:28:19.421723 goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/recipe_with_goals.S.HTML
+-rwxr-xr-x   0        0        0      143 2024-04-17 03:33:22.129283 goodest-1.2.2/venues/stages/goodest/shows_v2/shows.S.HTML
+-rwxr-xr-x   0        0        0      563 2024-05-13 00:59:01.393145 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/_assertions/__init__.py
+-rwxr-xr-x   0        0        0      798 2024-05-13 01:08:31.343266 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/_assertions/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      224 2024-04-17 03:33:22.117283 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/forward_channel/FDA.s.HTML
+-rwxr-xr-x   0        0        0      421 2024-04-17 03:33:22.117283 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/forward_channel/_journal/journal.r.HTML
+-rwxr-xr-x   0        0        0        0 2024-04-17 03:33:22.117283 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/forward_channel/_journal/structures/calcium.r.HTML
+-rwxr-xr-x   0        0        0      216 2024-04-17 03:33:22.117283 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/forward_channel/_journal/structures/lipids/lipids.r.HTML
+-rwxr-xr-x   0        0        0       11 2024-04-17 03:33:22.117283 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/forward_channel/_journal/structures/protein/protein.r.HTML
+-rwxr-xr-x   0        0        0     1351 2024-04-17 03:33:22.117283 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/forward_channel/_journal/structures/vitamin a.r.HTML
+-rwxr-xr-x   0        0        0      807 2024-04-17 03:33:22.117283 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/forward_channel/_journal/structures/vitamin b.r.HTML
+-rwxr-xr-x   0        0        0       93 2024-04-17 03:33:22.117283 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/forward_channel/_journal/structures/vitamin c.r.HTML
+-rwxr-xr-x   0        0        0     1298 2024-04-17 03:33:22.117283 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/forward_channel/_journal/structures/vitamin d.r.HTML
+-rwxr-xr-x   0        0        0      149 2024-04-17 03:33:22.117283 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/forward_channel/_journal/structures/vitamin e.r.HTML
+-rwxr-xr-x   0        0        0      219 2024-04-17 03:33:22.117283 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/forward_channel/channel/river.s.HTML
+-rwxr-xr-x   0        0        0      543 2024-04-17 03:33:22.117283 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/forward_channel/forward channel.s.HTML
+-rwxr-xr-x   0        0        0      935 2024-04-17 03:33:22.117283 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/forward_channel/structures.s.HTML
+-rwxr-xr-x   0        0        0      471 2024-04-17 03:36:50.295021 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      716 2024-05-13 01:08:31.263266 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/__pycache__/develop.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4922 2024-05-13 00:59:01.389145 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/__init__.py
+-rwxr-xr-x   0        0        0     2290 2024-05-13 01:08:31.355266 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1205 2024-05-13 01:11:03.358439 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_empty_grove/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1038 2024-05-13 00:59:01.389145 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_empty_grove/status_1.py
+-rwxr-xr-x   0        0        0     1748 2024-05-13 01:11:04.786430 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_m_and_meq/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1756 2024-05-13 01:11:03.970435 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_m_and_meq/__pycache__/status_2.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2143 2024-05-13 00:59:01.389145 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_m_and_meq/status_1.py
+-rwxr-xr-x   0        0        0     2120 2024-05-13 00:59:01.389145 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_m_and_meq/status_2.py
+-rwxr-xr-x   0        0        0     2138 2024-05-13 01:11:03.794437 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_m_eq_and_ba/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3700 2024-05-13 00:59:01.389145 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_m_eq_and_ba/status_1.py
+-rwxr-xr-x   0        0        0      445 2024-05-13 00:59:01.389145 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/assertions_one/__init__.py
+-rwxr-xr-x   0        0        0      568 2024-05-13 01:08:31.355266 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/assertions_one/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3108 2024-05-13 00:59:01.389145 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/calculate_portions/__init__.py
+-rwxr-xr-x   0        0        0     1537 2024-05-13 01:08:31.267266 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/calculate_portions/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1368 2024-05-13 00:59:01.389145 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/cultivate/__init__.py
+-rwxr-xr-x   0        0        0     1071 2024-05-13 01:08:31.355266 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/cultivate/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      802 2024-05-13 00:59:01.385145 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/develop.py
+-rwxr-xr-x   0        0        0     2566 2024-05-13 00:59:01.385145 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/measures_sums/__init__.py
+-rwxr-xr-x   0        0        0     1727 2024-05-13 01:08:31.355266 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/measures_sums/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      705 2024-05-13 01:11:03.510438 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/measures_sums/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      451 2024-05-13 00:59:01.385145 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/measures_sums/status_1.py
+-rwxr-xr-x   0        0        0     1781 2024-05-13 00:59:01.385145 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/multiply_amount/__init__.py
+-rwxr-xr-x   0        0        0     1414 2024-05-13 01:08:31.263266 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/multiply_amount/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2945 2024-04-17 03:33:22.125283 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/multiply_amount/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2108 2024-05-13 01:11:04.262434 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/multiply_amount/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2243 2024-05-13 01:11:04.110435 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/multiply_amount/__pycache__/status_2.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1327 2024-05-13 01:11:04.962429 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/multiply_amount/__pycache__/status_loop_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      950 2024-04-17 03:33:22.125283 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/multiply_amount/multiply_measures.s.HTML
+-rwxr-xr-x   0        0        0     2561 2024-05-13 00:59:01.385145 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/multiply_amount/status_1.py
+-rwxr-xr-x   0        0        0     2945 2024-05-13 00:59:01.389145 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/multiply_amount/status_2.py
+-rwxr-xr-x   0        0        0     1088 2024-05-13 00:59:01.385145 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/multiply_amount/status_loop_1.py
+-rwxr-xr-x   0        0        0      279 2024-04-24 21:20:53.222120 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      633 2024-05-13 00:59:01.393145 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/assertions/__init__.py
+-rwxr-xr-x   0        0        0      794 2024-05-13 01:08:31.355266 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/assertions/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     5622 2024-05-13 00:59:01.393145 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/has_uniters/__init__.py
+-rwxr-xr-x   0        0        0     1776 2024-05-13 01:08:31.355266 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/has_uniters/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1248 2024-05-13 01:11:04.930430 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/has_uniters/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1115 2024-05-13 00:59:01.393145 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/has_uniters/status_1.py
+-rwxr-xr-x   0        0        0      545 2024-05-13 00:59:01.393145 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/is_story_1/__init__.py
+-rwxr-xr-x   0        0        0      785 2024-05-13 01:08:31.355266 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/is_story_1/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      961 2024-05-13 01:11:04.778431 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/is_story_1/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      756 2024-05-13 00:59:01.393145 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/is_story_1/status_1.py
+-rwxr-xr-x   0        0        0     2539 2024-05-13 00:59:01.393145 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/nurture/__init__.py
+-rwxr-xr-x   0        0        0     2241 2024-05-13 01:08:31.263266 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/nurture/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1094 2024-05-13 01:11:04.262434 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/nurture/__pycache__/status_cautionary.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1012 2024-05-13 01:11:05.058429 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/nurture/__pycache__/status_essentials.cpython-310.pyc
+-rwxr-xr-x   0        0        0      794 2024-05-13 00:59:01.393145 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/nurture/status_cautionary.py
+-rwxr-xr-x   0        0        0      704 2024-05-13 00:59:01.393145 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/nurture/status_essentials.py
+-rwxr-xr-x   0        0        0     1299 2024-05-13 00:59:01.393145 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/seek/__init__.py
+-rwxr-xr-x   0        0        0     1055 2024-05-13 01:08:31.267266 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/seek/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1096 2024-05-13 01:11:05.430427 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/seek/__pycache__/status_essentials.cpython-310.pyc
+-rwxr-xr-x   0        0        0      689 2024-05-13 00:59:01.393145 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/seek/status_essentials.py
+-rwxr-xr-x   0        0        0     1361 2024-05-13 00:59:01.393145 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/seek_name_or_accepts/__init__.py
+-rwxr-xr-x   0        0        0     1222 2024-05-13 01:08:31.343266 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/seek_name_or_accepts/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      930 2024-05-13 01:11:03.662437 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/seek_name_or_accepts/__pycache__/status_essentials_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      914 2024-05-13 01:11:04.926430 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/seek_name_or_accepts/__pycache__/status_essentials_2.cpython-310.pyc
+-rwxr-xr-x   0        0        0      696 2024-05-13 00:59:01.393145 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/seek_name_or_accepts/status_essentials_1.py
+-rwxr-xr-x   0        0        0      685 2024-05-13 00:59:01.393145 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/seek_name_or_accepts/status_essentials_2.py
+-rwxr-xr-x   0        0        0     1025 2024-05-13 00:59:01.393145 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/seek_uniter/__init__.py
+-rwxr-xr-x   0        0        0     1071 2024-05-13 01:08:31.355266 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/seek_uniter/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1026 2024-05-13 01:11:03.814436 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/seek_uniter/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      847 2024-05-13 00:59:01.393145 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/seek_uniter/status_1.py
+-rwxr-xr-x   0        0        0     1523 2024-04-17 03:33:22.129283 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/grove.S.HTML
+-rwxr-xr-x   0        0        0       58 2024-04-17 03:33:22.129283 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/info/info.S.HTML
+-rwxr-xr-x   0        0        0       73 2024-04-17 03:33:22.129283 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/measures/measures.S.HTML
+-rwxr-xr-x   0        0        0       59 2024-04-17 03:33:22.129283 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/natures/natures.S.HTML
+-rwxr-xr-x   0        0        0     1508 2024-04-17 03:33:22.129283 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/unites/unites.S.HTML
+-rwxr-xr-x   0        0        0     2330 2024-04-23 19:28:57.911458 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/land.S.HTML
+-rwxr-xr-x   0        0        0      397 2024-05-13 00:59:01.389145 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/measures/__init__.py
+-rwxr-xr-x   0        0        0      581 2024-05-13 01:08:31.263266 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/measures/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      459 2024-04-17 03:33:22.129283 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/measures/measures.S.HTML
+-rwxr-xr-x   0        0        0     1359 2024-05-13 00:59:01.389145 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/measures/merge/__init__.py
+-rwxr-xr-x   0        0        0     1126 2024-05-13 01:08:31.343266 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/measures/merge/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1601 2024-04-17 03:33:22.125283 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/measures/merge/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      943 2024-05-13 01:11:04.174434 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/measures/merge/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      941 2024-05-13 01:11:06.182422 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/measures/merge/__pycache__/status_2.cpython-310.pyc
+-rwxr-xr-x   0        0        0      874 2024-05-13 01:11:04.170434 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/measures/merge/__pycache__/status_3.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1179 2024-05-13 00:59:01.389145 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/measures/merge/status_1.py
+-rwxr-xr-x   0        0        0     1177 2024-05-13 00:59:01.389145 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/measures/merge/status_2.py
+-rwxr-xr-x   0        0        0     1019 2024-05-13 00:59:01.389145 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/measures/merge/status_3.py
+-rwxr-xr-x   0        0        0      767 2024-05-13 00:59:01.389145 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/measures/multiply/__init__.py
+-rwxr-xr-x   0        0        0      869 2024-05-13 01:08:31.267266 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/measures/multiply/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1336 2024-04-17 03:33:22.125283 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/measures/multiply/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1644 2024-05-13 01:11:04.570432 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/measures/multiply/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1693 2024-05-13 00:59:01.389145 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/measures/multiply/status_1.py
+-rwxr-xr-x   0        0        0      412 2024-04-17 03:33:22.129283 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/natures/natures.S.HTML
+-rwxr-xr-x   0        0        0      405 2024-04-17 03:33:22.129283 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/measured_ingredients/measured_ingredients.S.HTML
+-rwxr-xr-x   0        0        0     1066 2024-04-17 03:33:22.129283 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/measures/measures.S.HTML
+-rwxr-xr-x   0        0        0      611 2024-04-25 19:49:42.003893 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/nature.S.HTML
+-rwxr-xr-x   0        0        0      310 2024-04-25 20:29:19.933549 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/unmeasured_ingredients/UI.S.HTML
+-rwxr-xr-x   0        0        0      428 2024-05-13 00:59:01.385145 goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/treasure.S.HTML
+-rw-r--r--   0        0        0     2940 1970-01-01 00:00:00.000000 goodest-1.2.2/PKG-INFO
```

### Comparing `goodest-1.2.1/pyproject.toml` & `goodest-1.2.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -3,38 +3,54 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "goodest"
-version = "1.2.1"
+version = "1.2.2"
 description = "goodest vegan health"
 authors = []
 readme = "venues/stages/goodest/readme.md"
+keywords = [
+	"goodest"
+]
+license = ">1 [Vegan + GPL 3.0 + Non-Commercial]"
+
 
 packages = [
     { include = "goodest", from = "venues/stages" }
 ]
 exclude = [
+	"venues/stages/goodest/__status/main/DB/**",
+
 	"venues/stages/goodest/adventures/vv_turbo/node_modules",
+	"venues/stages/goodest/adventures/vv_turbo/.turbo",
+
 	"venues/stages/goodest/adventures/vv_turbo/apps/web/node_modules",
+	"venues/stages/goodest/adventures/vv_turbo/apps/web/.turbo",
+	
 	"venues/stages/goodest/adventures/vv_turbo/apps/staff/node_modules",
+	"venues/stages/goodest/adventures/vv_turbo/apps/staff/.turbo",
+
 	"venues/stages/goodest/adventures/vv_turbo/apps/school/node_modules",
+	"venues/stages/goodest/adventures/vv_turbo/apps/school/.turbo",
 	
 	"node_modules/**"
 ]
+include = [ 
+	"venues/stages/goodest/adventures/vv_turbo/apps/web/the_build/*",
+	"*.HTML",
+	"*.html", 
+	"*.JSON", 
+	"*.json" 
+]
 
-include = [ "*.HTML", "*.html", "*.JSON", "*.json" ]
 
-license = ">1 [Vegan + GPL 3.0 + Non-Commercial]"
 
-keywords = [
-	"goodest"
-]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 biotech = "^1.1.10"
 click = "^8.1.7"
 docker = "^7.0.0"
 law_dictionary = "^1.0.12"
@@ -51,14 +67,15 @@
 setuptools = "^69.5.1"
 ships = "^1.2.6"
 somatic = "^3.0.1"
 tinydb = "^4.8.0"
 vegan_bits_1 = "1.0.0"
 
 
+
 [tool.poetry.scripts]
 goodest = 'goodest:clique'
 
 [tool.poetry.urls]
 GitLab = "https://gitlab.com/reptilian_climates/modules_series_4/goodest"
```

### Comparing `goodest-1.2.1/venue.S.HTML` & `goodest-1.2.2/venue.S.HTML`

 * *Files 4% similar despite different names*

```diff
@@ -107,19 +107,41 @@
 		<h3>publish</h3>
 			#
 			#	[ ] poetry auth
 			#
 			#
 			pip install poetry && cd /habitat && rm -rf dist && poetry build --verbose && poetry publish --verbose;
 			(pip install poetry && cd /habitat && rm -rf dist && poetry build --format sdist --verbose && chmod -R 777 /habitat && poetry publish --verbose;)
-		
+			
+			
+			#
+			#	statistics
+			#
+			find . -type d -exec du -sh {} \;
+			du -h --max-depth=1 .
+
+	
+		<h3>notes</h3>
+			[tool.poetry.source]
+			include = [
+				"venues/stages/goodest/adventures/vv_turbo/apps/web/the_build/*"
+			]
 
 	<h2>important</h2>
 		poetry show --tree
 
 
 	<h2>docker</h2>
 		docker compose up -d
 		docker exec -it goodest bash
 		docker exec -it goodest bash -c "source /goodest/moves/source_2.sh && bash"
 
+	<h2>hatch</h2>
+		#
+		#	https://github.com/pypa/pipx
+		#
+		#
+		apt install pipx -y
+		pipx ensurepath
+		pipx install hatch
+
 </pre>
```

### Comparing `goodest-1.2.1/venues/stages/goodest/[__objectives]/objectives.S.HTML` & `goodest-1.2.2/venues/stages/goodest/[__objectives]/objectives.S.HTML`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/[_license]/license.s.HTML` & `goodest-1.2.2/venues/stages/goodest/[_license]/license.s.HTML`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/[_license]/list/gpl-3.0-standalone.html` & `goodest-1.2.2/venues/stages/goodest/[_license]/list/gpl-3.0-standalone.html`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves/exports/goodest_inventory/certifications/goodest_inventory.certifications.1.JSON` & `goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves/exports/goodest_inventory/certifications/goodest_inventory.certifications.1.JSON`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves/exports/goodest_inventory/food/goodest_inventory.food.1.JSON` & `goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves/exports/goodest_inventory/food/goodest_inventory.food.1.JSON`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves/exports/goodest_inventory/food/goodest_inventory.food.2.JSON` & `goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves/exports/goodest_inventory/food/goodest_inventory.food.2.JSON`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves/exports/goodest_inventory/supp/goodest_inventory.supp.1.JSON` & `goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves/exports/goodest_inventory/supp/goodest_inventory.supp.1.JSON`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves/exports/goodest_inventory/supp/goodest_inventory.supp.2.JSON` & `goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves/exports/goodest_inventory/supp/goodest_inventory.supp.2.JSON`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves/exports/goodest_tract/essential_nutrients/goodest_tract.essential_nutrients.1.JSON` & `goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves/exports/goodest_tract/essential_nutrients/goodest_tract.essential_nutrients.1.JSON`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves/exports/goodest_tract/essential_nutrients/goodest_tract.essential_nutrients.2.JSON` & `goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves/exports/goodest_tract/essential_nutrients/goodest_tract.essential_nutrients.2.JSON`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves/exports/goodest_tract/goals/goodest_tract.goals.1.JSON` & `goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves/exports/goodest_tract/goals/goodest_tract.goals.1.JSON`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves/exports/goodest_tract/goals/goodest_tract.goals.2.JSON` & `goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves/exports/goodest_tract/goals/goodest_tract.goals.2.JSON`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v1/exports/goodest_tract/essential_nutrients/1.JSON` & `goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v1/exports/goodest_tract/essential_nutrients/1.JSON`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v1/exports/goodest_tract/essential_nutrients/2.JSON` & `goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v1/exports/goodest_tract/essential_nutrients/2.JSON`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v1/exports/goodest_tract/essential_nutrients/3.JSON` & `goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v1/exports/goodest_tract/essential_nutrients/3.JSON`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v1/exports/goodest_tract/essential_nutrients/4.JSON` & `goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v1/exports/goodest_tract/essential_nutrients/4.JSON`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v1/exports/goodest_tract/essential_nutrients/5.JSON` & `goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v1/exports/goodest_tract/essential_nutrients/5.JSON`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v1/exports/goodest_tract/essential_nutrients/6.JSON` & `goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v1/exports/goodest_tract/essential_nutrients/6.JSON`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v1/exports/goodest_tract/goals/5.JSON` & `goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v1/exports/goodest_tract/goals/5.JSON`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v1/exports/goodest_tract/goals/6.JSON` & `goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v1/exports/goodest_tract/goals/6.JSON`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v1/saves.S.HTML` & `goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v1/saves.S.HTML`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v2/dumps/goodest_tract/essential_nutrients/goodest_tract.essential_nutrients.1.dump.gzip` & `goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v2/dumps/goodest_tract/essential_nutrients/goodest_tract.essential_nutrients.1.dump.gzip`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v2/dumps/goodest_tract/goals/goodest_tract.goals.1.dump.gzip` & `goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v2/dumps/goodest_tract/goals/goodest_tract.goals.1.dump.gzip`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v2/exports/goodest_tract/essential_nutrients/goodest_tract.essential_nutrients.1.JSON` & `goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v2/exports/goodest_tract/essential_nutrients/goodest_tract.essential_nutrients.1.JSON`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v2/exports/goodest_tract/essential_nutrients/goodest_tract.essential_nutrients.2.JSON` & `goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v2/exports/goodest_tract/essential_nutrients/goodest_tract.essential_nutrients.2.JSON`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v2/exports/goodest_tract/essential_nutrients/goodest_tract.essential_nutrients.3.JSON` & `goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v2/exports/goodest_tract/essential_nutrients/goodest_tract.essential_nutrients.3.JSON`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v2/exports/goodest_tract/goals/goodest_tract.goals.1.JSON` & `goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v2/exports/goodest_tract/goals/goodest_tract.goals.1.JSON`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v2/exports/goodest_tract/goals/goodest_tract.goals.2.JSON` & `goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v2/exports/goodest_tract/goals/goodest_tract.goals.2.JSON`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/[saves]/monetary_saves_v2/exports/goodest_tract/goals/goodest_tract.goals.3.JSON` & `goodest-1.2.2/venues/stages/goodest/[saves]/monetary_saves_v2/exports/goodest_tract/goals/goodest_tract.goals.3.JSON`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/__status/API/DB/records.json` & `goodest-1.2.2/venues/stages/goodest/__status/API/DB/records.json`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/__status/API/status.proc.py` & `goodest-1.2.2/venues/stages/goodest/__status/API/status.proc.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/__status/__pycache__/status_API.proc.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/__status/__pycache__/status_API.proc.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/__status/main/output.json` & `goodest-1.2.2/venues/stages/goodest/__status/main/output.json`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/__status/main/status.proc.py` & `goodest-1.2.2/venues/stages/goodest/__status/main/status.proc.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/_controls/__pycache__/_clique.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/_controls/__pycache__/_clique.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/_controls/__pycache__/off.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/_controls/__pycache__/off.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/_controls/__pycache__/on.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/_controls/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/_controls/__pycache__/refresh.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/_controls/__pycache__/refresh.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/_controls/__pycache__/status.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/_controls/__pycache__/status.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/_controls/_clique.py` & `goodest-1.2.2/venues/stages/goodest/_controls/_clique.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/_essence/__init__.py` & `goodest-1.2.2/venues/stages/goodest/_essence/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/_essence/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/_essence/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/_essence/activate_alert--/__init__.py` & `goodest-1.2.2/venues/stages/goodest/_essence/activate_alert--/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/_essence/activate_alert--/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/_essence/activate_alert--/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/_essence/activate_alert--/__pycache__/parse_exception.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/_essence/activate_alert--/__pycache__/parse_exception.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/_essence/merge/__init__.py` & `goodest-1.2.2/venues/stages/goodest/_essence/merge/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 			"mode": "business",
 			
 			"CWD": os.getcwd (),
 			
 			"vv_turbo": {
 				"dist_path": str (normpath (join (
 					the_mix_directory, 
-					"adventures/vv_turbo/apps/web/dist"
+					"adventures/vv_turbo/apps/web/the_build"
 				)))
 			},
 			"bits": {
 				"sequences_path": str (normpath (join (
 					the_mix_directory, 
 					"adventures/bits/sequences"
 				)))
```

### Comparing `goodest-1.2.1/venues/stages/goodest/_essence/merge/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/_essence/merge/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon May 13 01:45:50 2024 UTC, .py size: 3322 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ce70 4166 fa0c 0000  o........pAf....
+00000000: 6f0d 0d0a 0000 0000 e5c3 4266 ff0c 0000  o.........Bf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 4800 0000 6400  .....@...sH...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 6d04 5a04 0100 6400 6401 6c05  m.Z.m.Z...d.d.l.
 00000050: 5a05 6400 6401 6c06 5a06 6400 6401 6c07  Z.d.d.l.Z.d.d.l.
 00000060: 5a07 6403 6404 8400 5a08 6405 6406 8400  Z.d.d...Z.d.d...
 00000070: 5a09 6401 5300 2907 e900 0000 004e 2903  Z.d.S.)......N).
@@ -48,78 +48,78 @@
 000002f0: 0574 0674 077c 0264 1c83 0283 0183 0174  .t.t.|.d.......t
 00000300: 0574 0674 077c 0264 1d83 0283 0183 0164  .t.t.|.d.......d
 00000310: 1e9c 0264 1f9c 087c 00a1 027d 0374 0c7c  ...d...|...}.t.|
 00000320: 0364 2019 0083 017c 0364 213c 0074 0d64  .d ....|.d!<.t.d
 00000330: 227c 0364 2119 0083 0201 007c 0353 0029  "|.d!......|.S.)
 00000340: 234e 7a05 2e2e 2f2e 2e72 0700 0000 da08  #Nz.../..r......
 00000350: 6275 7369 6e65 7373 da09 6469 7374 5f70  business..dist_p
-00000360: 6174 687a 2161 6476 656e 7475 7265 732f  athz!adventures/
+00000360: 6174 687a 2661 6476 656e 7475 7265 732f  athz&adventures/
 00000370: 7676 5f74 7572 626f 2f61 7070 732f 7765  vv_turbo/apps/we
-00000380: 622f 6469 7374 da0e 7365 7175 656e 6365  b/dist..sequence
-00000390: 735f 7061 7468 7a19 6164 7665 6e74 7572  s_pathz.adventur
-000003a0: 6573 2f62 6974 732f 7365 7175 656e 6365  es/bits/sequence
-000003b0: 73da 1167 6f6f 6465 7374 5f69 6e76 656e  s..goodest_inven
-000003c0: 746f 7279 da04 666f 6f64 da04 7375 7070  tory..food..supp
-000003d0: 2902 da05 616c 6961 73da 0b63 6f6c 6c65  )...alias..colle
-000003e0: 6374 696f 6e73 da0d 676f 6f64 6573 745f  ctions..goodest_
-000003f0: 7472 6163 7429 05da 1663 6175 7469 6f6e  tract)...caution
-00000400: 6172 795f 696e 6772 6564 6965 6e74 73da  ary_ingredients.
-00000410: 1365 7373 656e 7469 616c 5f6e 7574 7269  .essential_nutri
-00000420: 656e 7473 da08 676c 6f73 7361 7279 da05  ents..glossary..
-00000430: 676f 616c 73da 0e63 6572 7469 6669 6361  goals..certifica
-00000440: 7469 6f6e 7329 0272 1600 0000 721b 0000  tions).r....r...
-00000450: 007a 165b 7361 7665 735d 2f6d 6f6e 6574  .z.[saves]/monet
-00000460: 6172 795f 7361 7665 73da 0470 6174 687a  ary_saves..pathz
-00000470: 1e5b 7361 7665 735d 2f6d 6f6e 6574 6172  .[saves]/monetar
-00000480: 795f 7361 7665 732f 6578 706f 7274 737a  y_saves/exportsz
-00000490: 1c5b 7361 7665 735d 2f6d 6f6e 6574 6172  .[saves]/monetar
-000004a0: 795f 7361 7665 732f 6475 6d70 7329 0372  y_saves/dumps).r
-000004b0: 2100 0000 da07 6578 706f 7274 73da 0564  !.....exports..d
-000004c0: 756d 7073 2902 da09 6461 7461 6261 7365  umps)...database
-000004d0: 73da 0573 6176 6573 7a12 6164 7665 6e74  s..savesz.advent
-000004e0: 7572 6573 2f73 616e 6971 7565 7a24 6164  ures/saniquez$ad
-000004f0: 7665 6e74 7572 6573 2f73 616e 6971 7565  ventures/sanique
-00000500: 2f68 6172 626f 722f 6f6e 2e70 726f 632e  /harbor/on.proc.
-00000510: 7079 da04 3830 3030 7a07 302e 302e 302e  py..8000z.0.0.0.
-00000520: 30da 0437 3435 3729 02da 0470 6f72 74da  0..7457)...port.
-00000530: 0468 6f73 7429 05da 0964 6972 6563 746f  .host)...directo
-00000540: 7279 7221 0000 0072 2800 0000 7229 0000  ryr!...r(...r)..
-00000550: 00da 0969 6e73 7065 6374 6f72 da0c 5f5f  ...inspector..__
-00000560: 6469 6374 696f 6e61 7279 7a14 5f5f 6469  dictionaryz.__di
-00000570: 6374 696f 6e61 7279 2f67 6f6f 6465 7374  ctionary/goodest
-00000580: 2902 7221 0000 00da 0767 6f6f 6465 7374  ).r!.....goodest
-00000590: 2908 720b 0000 00da 046d 6f64 65da 0343  ).r......mode..C
-000005a0: 5744 da08 7676 5f74 7572 626f da04 6269  WD..vv_turbo..bi
-000005b0: 7473 da08 6d6f 6e65 7461 7279 da07 7361  ts..monetary..sa
-000005c0: 6e69 7175 65da 0a64 6963 7469 6f6e 6172  nique..dictionar
-000005d0: 7972 0b00 0000 da0e 616c 6c6f 7765 645f  yr......allowed_
-000005e0: 616c 6572 7473 7a0e 616c 6c6f 7765 6420  alertsz.allowed 
-000005f0: 616c 6572 7473 290e da07 7061 7468 6c69  alerts)...pathli
-00000600: 62da 0450 6174 68da 085f 5f66 696c 655f  b..Path..__file_
-00000610: 5fda 0670 6172 656e 74da 0772 6573 6f6c  _..parent..resol
-00000620: 7665 da03 7374 7272 0400 0000 7203 0000  ve..strr....r...
-00000630: 00da 0670 7964 6173 68da 056d 6572 6765  ...pydash..merge
-00000640: da02 6f73 da06 6765 7463 7764 7212 0000  ..os..getcwdr...
-00000650: 00da 0570 7269 6e74 2904 da10 6578 7465  ...print)...exte
-00000660: 726e 616c 5f65 7373 656e 6365 da0e 7468  rnal_essence..th
-00000670: 6973 5f64 6972 6563 746f 7279 da11 7468  is_directory..th
-00000680: 655f 6d69 785f 6469 7265 6374 6f72 79da  e_mix_directory.
-00000690: 1274 6865 5f6d 6572 6765 645f 6573 7365  .the_merged_esse
-000006a0: 6e63 6572 1000 0000 7210 0000 0072 1100  ncer....r....r..
-000006b0: 0000 da0d 6d65 7267 655f 6573 7365 6e63  ....merge_essenc
-000006c0: 6521 0000 0073 8600 0000 1001 1201 0202  e!...s..........
-000006d0: 040a 0205 0205 0602 0803 0201 0201 06fe  ................
-000006e0: 02ff 0807 0201 0201 06fe 02ff 020a 0202  ................
-000006f0: 0201 02fe 04fe 0208 0601 04fe 04f8 061a  ................
-00000700: 0201 0201 06fe 0805 0201 0201 06fe 02ff  ................
-00000710: 0807 0201 0201 06fe 02ff 04f5 04e6 0631  ...............1
-00000720: 0201 0201 06fe 0605 0201 0201 06fe 0205  ................
-00000730: 0201 020b 0201 04fe 04ea 101c 1001 04fe  ................
-00000740: 049b 026a 0495 0270 0601 08ff 0e04 0403  ...j...p........
-00000750: 7245 0000 0029 0a72 3600 0000 da07 6f73  rE...).r6.....os
-00000760: 2e70 6174 6872 0200 0000 7203 0000 0072  .pathr....r....r
-00000770: 0400 0000 da03 7379 7372 3e00 0000 723c  ......sysr>...r<
-00000780: 0000 0072 1200 0000 7245 0000 0072 1000  ...r....rE...r..
-00000790: 0000 7210 0000 0072 1000 0000 7211 0000  ..r....r....r...
-000007a0: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
-000007b0: 0e00 0000 0804 1401 0801 0801 0803 0804  ................
-000007c0: 0c12                                     ..
+00000380: 622f 7468 655f 6275 696c 64da 0e73 6571  b/the_build..seq
+00000390: 7565 6e63 6573 5f70 6174 687a 1961 6476  uences_pathz.adv
+000003a0: 656e 7475 7265 732f 6269 7473 2f73 6571  entures/bits/seq
+000003b0: 7565 6e63 6573 da11 676f 6f64 6573 745f  uences..goodest_
+000003c0: 696e 7665 6e74 6f72 79da 0466 6f6f 64da  inventory..food.
+000003d0: 0473 7570 7029 02da 0561 6c69 6173 da0b  .supp)...alias..
+000003e0: 636f 6c6c 6563 7469 6f6e 73da 0d67 6f6f  collections..goo
+000003f0: 6465 7374 5f74 7261 6374 2905 da16 6361  dest_tract)...ca
+00000400: 7574 696f 6e61 7279 5f69 6e67 7265 6469  utionary_ingredi
+00000410: 656e 7473 da13 6573 7365 6e74 6961 6c5f  ents..essential_
+00000420: 6e75 7472 6965 6e74 73da 0867 6c6f 7373  nutrients..gloss
+00000430: 6172 79da 0567 6f61 6c73 da0e 6365 7274  ary..goals..cert
+00000440: 6966 6963 6174 696f 6e73 2902 7216 0000  ifications).r...
+00000450: 0072 1b00 0000 7a16 5b73 6176 6573 5d2f  .r....z.[saves]/
+00000460: 6d6f 6e65 7461 7279 5f73 6176 6573 da04  monetary_saves..
+00000470: 7061 7468 7a1e 5b73 6176 6573 5d2f 6d6f  pathz.[saves]/mo
+00000480: 6e65 7461 7279 5f73 6176 6573 2f65 7870  netary_saves/exp
+00000490: 6f72 7473 7a1c 5b73 6176 6573 5d2f 6d6f  ortsz.[saves]/mo
+000004a0: 6e65 7461 7279 5f73 6176 6573 2f64 756d  netary_saves/dum
+000004b0: 7073 2903 7221 0000 00da 0765 7870 6f72  ps).r!.....expor
+000004c0: 7473 da05 6475 6d70 7329 02da 0964 6174  ts..dumps)...dat
+000004d0: 6162 6173 6573 da05 7361 7665 737a 1261  abases..savesz.a
+000004e0: 6476 656e 7475 7265 732f 7361 6e69 7175  dventures/saniqu
+000004f0: 657a 2461 6476 656e 7475 7265 732f 7361  ez$adventures/sa
+00000500: 6e69 7175 652f 6861 7262 6f72 2f6f 6e2e  nique/harbor/on.
+00000510: 7072 6f63 2e70 79da 0438 3030 307a 0730  proc.py..8000z.0
+00000520: 2e30 2e30 2e30 da04 3734 3537 2902 da04  .0.0.0..7457)...
+00000530: 706f 7274 da04 686f 7374 2905 da09 6469  port..host)...di
+00000540: 7265 6374 6f72 7972 2100 0000 7228 0000  rectoryr!...r(..
+00000550: 0072 2900 0000 da09 696e 7370 6563 746f  .r).....inspecto
+00000560: 72da 0c5f 5f64 6963 7469 6f6e 6172 797a  r..__dictionaryz
+00000570: 145f 5f64 6963 7469 6f6e 6172 792f 676f  .__dictionary/go
+00000580: 6f64 6573 7429 0272 2100 0000 da07 676f  odest).r!.....go
+00000590: 6f64 6573 7429 0872 0b00 0000 da04 6d6f  odest).r......mo
+000005a0: 6465 da03 4357 44da 0876 765f 7475 7262  de..CWD..vv_turb
+000005b0: 6fda 0462 6974 73da 086d 6f6e 6574 6172  o..bits..monetar
+000005c0: 79da 0773 616e 6971 7565 da0a 6469 6374  y..sanique..dict
+000005d0: 696f 6e61 7279 720b 0000 00da 0e61 6c6c  ionaryr......all
+000005e0: 6f77 6564 5f61 6c65 7274 737a 0e61 6c6c  owed_alertsz.all
+000005f0: 6f77 6564 2061 6c65 7274 7329 0eda 0770  owed alerts)...p
+00000600: 6174 686c 6962 da04 5061 7468 da08 5f5f  athlib..Path..__
+00000610: 6669 6c65 5f5f da06 7061 7265 6e74 da07  file__..parent..
+00000620: 7265 736f 6c76 65da 0373 7472 7204 0000  resolve..strr...
+00000630: 0072 0300 0000 da06 7079 6461 7368 da05  .r......pydash..
+00000640: 6d65 7267 65da 026f 73da 0667 6574 6377  merge..os..getcw
+00000650: 6472 1200 0000 da05 7072 696e 7429 04da  dr......print)..
+00000660: 1065 7874 6572 6e61 6c5f 6573 7365 6e63  .external_essenc
+00000670: 65da 0e74 6869 735f 6469 7265 6374 6f72  e..this_director
+00000680: 79da 1174 6865 5f6d 6978 5f64 6972 6563  y..the_mix_direc
+00000690: 746f 7279 da12 7468 655f 6d65 7267 6564  tory..the_merged
+000006a0: 5f65 7373 656e 6365 7210 0000 0072 1000  _essencer....r..
+000006b0: 0000 7211 0000 00da 0d6d 6572 6765 5f65  ..r......merge_e
+000006c0: 7373 656e 6365 2100 0000 7386 0000 0010  ssence!...s.....
+000006d0: 0112 0102 0204 0a02 0502 0506 0208 0302  ................
+000006e0: 0102 0106 fe02 ff08 0702 0102 0106 fe02  ................
+000006f0: ff02 0a02 0202 0102 fe04 fe02 0806 0104  ................
+00000700: fe04 f806 1a02 0102 0106 fe08 0502 0102  ................
+00000710: 0106 fe02 ff08 0702 0102 0106 fe02 ff04  ................
+00000720: f504 e606 3102 0102 0106 fe06 0502 0102  ....1...........
+00000730: 0106 fe02 0502 0102 0b02 0104 fe04 ea10  ................
+00000740: 1c10 0104 fe04 9b02 6a04 9502 7006 0108  ........j...p...
+00000750: ff0e 0404 0372 4500 0000 290a 7236 0000  .....rE...).r6..
+00000760: 00da 076f 732e 7061 7468 7202 0000 0072  ...os.pathr....r
+00000770: 0300 0000 7204 0000 00da 0373 7973 723e  ....r......sysr>
+00000780: 0000 0072 3c00 0000 7212 0000 0072 4500  ...r<...r....rE.
+00000790: 0000 7210 0000 0072 1000 0000 7210 0000  ..r....r....r...
+000007a0: 0072 1100 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+000007b0: 0100 0000 730e 0000 0008 0414 0108 0108  ....s...........
+000007c0: 0108 0308 040c 12                        .......
```

### Comparing `goodest-1.2.1/venues/stages/goodest/_essence/scan/__init__.py` & `goodest-1.2.2/venues/stages/goodest/_essence/scan/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/_essence/scan/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/_essence/scan/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/_essence/seek/__init__.py` & `goodest-1.2.2/venues/stages/goodest/_essence/seek/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/_essence/seek/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/_essence/seek/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/DNS/counsellor.S.HTML` & `goodest-1.2.2/venues/stages/goodest/adventures/DNS/counsellor.S.HTML`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/HTTPS_Certs/HTTPS_Certs.S.HTML` & `goodest-1.2.2/venues/stages/goodest/adventures/HTTPS_Certs/HTTPS_Certs.S.HTML`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/_ops/__pycache__/_clique.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/_ops/__pycache__/_clique.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/_ops/__pycache__/off.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/_ops/__pycache__/off.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/_ops/__pycache__/on.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/_ops/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/_ops/__pycache__/refresh.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/_ops/__pycache__/refresh.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/_ops/__pycache__/status.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/_ops/__pycache__/status.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/_ops/_clique.py` & `goodest-1.2.2/venues/stages/goodest/adventures/_ops/_clique.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/_ops/monitor.py` & `goodest-1.2.2/venues/stages/goodest/adventures/_ops/monitor.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/_ops/off.py` & `goodest-1.2.2/venues/stages/goodest/adventures/_ops/off.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/_ops/on.py` & `goodest-1.2.2/venues/stages/goodest/adventures/_ops/on.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/_ops/status.py` & `goodest-1.2.2/venues/stages/goodest/adventures/_ops/status.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/adventures.S.HTML` & `goodest-1.2.2/venues/stages/goodest/adventures/adventures.S.HTML`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/alerting/__init__.py` & `goodest-1.2.2/venues/stages/goodest/adventures/alerting/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/alerting/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/alerting/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/alerting/__pycache__/parse_exception.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/alerting/__pycache__/parse_exception.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/cloud_flares/cloud_flares.S.HTML` & `goodest-1.2.2/venues/stages/goodest/adventures/cloud_flares/cloud_flares.S.HTML`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/customs/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/customs/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/customs/__pycache__/clique.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/customs/__pycache__/clique.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/customs/_ops/__pycache__/_clique.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/customs/_ops/__pycache__/_clique.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/customs/_ops/_clique.py` & `goodest-1.2.2/venues/stages/goodest/adventures/customs/_ops/_clique.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/customs/_ops/on.py` & `goodest-1.2.2/venues/stages/goodest/adventures/customs/_ops/on.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/demux_hap/HA.s.HTML` & `goodest-1.2.2/venues/stages/goodest/adventures/demux_hap/HA.s.HTML`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/demux_hap/SSL/__init__.py` & `goodest-1.2.2/venues/stages/goodest/adventures/demux_hap/SSL/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/demux_hap/SSL/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/demux_hap/SSL/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/demux_hap/SSL/__pycache__/__init__.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/demux_hap/SSL/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/demux_hap/SSL/certificate.pem` & `goodest-1.2.2/venues/stages/goodest/adventures/demux_hap/SSL/certificate.pem`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/demux_hap/SSL/certificate.pem.key` & `goodest-1.2.2/venues/stages/goodest/adventures/demux_hap/SSL/certificate.pem.key`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/demux_hap/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/demux_hap/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/demux_hap/_controls/__pycache__/_clique.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/demux_hap/_controls/__pycache__/_clique.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/demux_hap/_controls/__pycache__/build.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/demux_hap/_controls/__pycache__/build.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/demux_hap/_controls/__pycache__/on.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/demux_hap/_controls/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/demux_hap/_controls/on.py` & `goodest-1.2.2/venues/stages/goodest/adventures/demux_hap/_controls/on.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/demux_hap/configs/HTTPS_to_HTTP/1.py` & `goodest-1.2.2/venues/stages/goodest/adventures/demux_hap/configs/HTTPS_to_HTTP/1.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/demux_hap/configs/HTTPS_to_HTTP/HTTPS_to_HTTP.s.HTML` & `goodest-1.2.2/venues/stages/goodest/adventures/demux_hap/configs/HTTPS_to_HTTP/HTTPS_to_HTTP.s.HTML`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/demux_hap/configs/HTTPS_to_HTTP/__init__.py` & `goodest-1.2.2/venues/stages/goodest/adventures/demux_hap/configs/HTTPS_to_HTTP/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/demux_hap/configs/HTTPS_to_HTTP/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/demux_hap/configs/HTTPS_to_HTTP/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/demux_hap/configs/HTTPS_to_HTTP/__pycache__/__init__.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/demux_hap/configs/HTTPS_to_HTTP/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/demux_hap/configs/HTTP_balancer/__init__.py` & `goodest-1.2.2/venues/stages/goodest/adventures/demux_hap/configs/HTTP_balancer/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/demux_hap/configs/HTTP_balancer/__pycache__/__init__.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/demux_hap/configs/HTTP_balancer/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/demux_hap/configs/__pycache__/HTTP_balancer.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/demux_hap/configs/__pycache__/HTTP_balancer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/demux_hap/configs/examples/haproxy.cfg` & `goodest-1.2.2/venues/stages/goodest/adventures/demux_hap/configs/examples/haproxy.cfg`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/demux_hap/configs/examples/haproxy_2.cfg` & `goodest-1.2.2/venues/stages/goodest/adventures/demux_hap/configs/examples/haproxy_2.cfg`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/demux_hap/configs/external_reverse/__init__.py` & `goodest-1.2.2/venues/stages/goodest/adventures/demux_hap/configs/external_reverse/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_inventory/__pycache__/connect.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_inventory/__pycache__/connect.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_inventory/_treasures/_indexes/__pycache__/drop_and_create.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_inventory/_treasures/_indexes/__pycache__/drop_and_create.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_inventory/_treasures/_indexes/drop_and_create.py` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_inventory/_treasures/_indexes/drop_and_create.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_inventory/connect.py` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_inventory/connect.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_inventory/foods/_indexes/__pycache__/drop_and_create.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_inventory/foods/_indexes/__pycache__/drop_and_create.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_inventory/foods/document/__pycache__/find.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_inventory/foods/document/__pycache__/find.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_inventory/foods/document/__pycache__/insert.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_inventory/foods/document/__pycache__/insert.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_inventory/foods/document/find.py` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_inventory/foods/document/find.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_inventory/foods/document/insert.py` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_inventory/foods/document/insert.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_inventory/supps/document/__pycache__/find.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_inventory/supps/document/__pycache__/find.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_inventory/supps/document/__pycache__/insert.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_inventory/supps/document/__pycache__/insert.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_inventory/supps/document/find.py` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_inventory/supps/document/find.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_inventory/supps/document/insert.py` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_inventory/supps/document/insert.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_tract/__pycache__/clique.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_tract/__pycache__/clique.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_tract/__pycache__/connect.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_tract/__pycache__/connect.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_tract/_land/__pycache__/find_name.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_tract/_land/__pycache__/find_name.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_tract/_land/__pycache__/retrieve_every.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_tract/_land/__pycache__/retrieve_every.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_tract/_land/find_name.py` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_tract/_land/find_name.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_tract/_land/insert_document.py` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_tract/_land/insert_document.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_tract/_land/retrieve_every.py` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_tract/_land/retrieve_every.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_tract/connect.py` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_tract/connect.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_tract/essential_nutrients/essential_nutrients.S.HTML` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_tract/essential_nutrients/essential_nutrients.S.HTML`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_tract/goals/__pycache__/find_ingredient.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_tract/goals/__pycache__/find_ingredient.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_tract/goals/__pycache__/insert.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_tract/goals/__pycache__/insert.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_tract/goals/__pycache__/retrieve.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_tract/goals/__pycache__/retrieve.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_tract/goals/__pycache__/retrieve_one.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_tract/goals/__pycache__/retrieve_one.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_tract/goals/_indexes/__pycache__/create.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_tract/goals/_indexes/__pycache__/create.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_tract/goals/_indexes/__pycache__/drop_and_create.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_tract/goals/_indexes/__pycache__/drop_and_create.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_tract/goals/_indexes/drop_and_create.py` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_tract/goals/_indexes/drop_and_create.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_tract/goals/find_ingredient.py` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_tract/goals/find_ingredient.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_tract/goals/insert.py` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_tract/goals/insert.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_tract/goals/retrieve.py` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_tract/goals/retrieve.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_tract/goals/retrieve_one.py` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_tract/goals/retrieve_one.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/DB/goodest_tract/ingredients.S.HTML` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/DB/goodest_tract/ingredients.S.HTML`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/__pycache__/clique.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/__pycache__/clique.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/__pycache__/connect.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/__pycache__/connect.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/__pycache__/off.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/__pycache__/off.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/__pycache__/on.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/__pycache__/status.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/__pycache__/status.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/_ops/__pycache__/_clique.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/_ops/__pycache__/_clique.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/_ops/__pycache__/off.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/_ops/__pycache__/off.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/_ops/__pycache__/on.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/_ops/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/_ops/__pycache__/status.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/_ops/__pycache__/status.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/_ops/_clique.py` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/_ops/_clique.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/_ops/off.py` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/_ops/off.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/_ops/on.py` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/_ops/on.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/_ops/saves/__pycache__/_clique.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/_ops/saves/__pycache__/_clique.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/_ops/saves/__pycache__/clique.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/_ops/saves/__pycache__/clique.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/_ops/saves/_clique.py` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/_ops/saves/_clique.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/_ops/saves/dumps/__pycache__/dump.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/_ops/saves/dumps/__pycache__/dump.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/_ops/saves/dumps/__pycache__/restore.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/_ops/saves/dumps/__pycache__/restore.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/_ops/saves/dumps/dump.py` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/_ops/saves/dumps/dump.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/_ops/saves/dumps/restore.py` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/_ops/saves/dumps/restore.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/_ops/saves/exports/__pycache__/monetary_export.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/_ops/saves/exports/__pycache__/monetary_export.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/_ops/saves/exports/__pycache__/monetary_import.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/_ops/saves/exports/__pycache__/monetary_import.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/_ops/saves/exports/monetary_export.py` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/_ops/saves/exports/monetary_export.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/_ops/saves/exports/monetary_import.py` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/_ops/saves/exports/monetary_import.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/_ops/status.py` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/_ops/status.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/moves/URL/__pycache__/retrieve.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/moves/URL/__pycache__/retrieve.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/__init__.py` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/__pycache__/__init__.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/scan_3.s.HTML` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/scan_3.s.HTML`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/__pycache__/limits.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/__pycache__/limits.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/__pycache__/limits.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/__pycache__/limits.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/__pycache__/stats.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/__pycache__/stats.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/limits.py` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/limits.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/__init__.py` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/__pycache__/__init__.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/affirm/__pycache__/direction.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/affirm/__pycache__/direction.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/affirm/__pycache__/direction.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/affirm/__pycache__/direction.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/affirm/__pycache__/filters.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/affirm/__pycache__/filters.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/__pycache__/before_and_after.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/__pycache__/before_and_after.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/__pycache__/before_and_after.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/__pycache__/before_and_after.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/__pycache__/check_fields.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/__pycache__/check_fields.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/__pycache__/sort_name_emblem.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/__pycache__/sort_name_emblem.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/__pycache__/unionize.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/__pycache__/unionize.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/__pycache__/unionize.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/__pycache__/unionize.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/before_and_after.py` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/before_and_after.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/filters/__pycache__/limit.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/filters/__pycache__/limit.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/filters/__pycache__/limit.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/filters/__pycache__/limit.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/filters/__pycache__/scan_string.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/filters/__pycache__/scan_string.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/filters/__pycache__/scan_string.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/filters/__pycache__/scan_string.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/filters/__pycache__/vector_name.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/filters/__pycache__/vector_name.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/filters/__pycache__/vector_name.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/filters/__pycache__/vector_name.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/filters/__pycache__/vector_name_and_emblem.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/filters/__pycache__/vector_name_and_emblem.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/filters/__pycache__/vector_name_and_emblem.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/filters/__pycache__/vector_name_and_emblem.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/filters/filters.s.HTML` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/filters/filters.s.HTML`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/filters/vector_name.py` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/filters/vector_name.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/filters/vector_name_and_emblem.py` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/filters/vector_name_and_emblem.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/formats/__pycache__/format_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/formats/__pycache__/format_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/formats/__pycache__/format_1.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/formats/__pycache__/format_1.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/unionize.py` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/aggregation_steps/unionize.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/spruce/__pycache__/filters.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/spruce/__pycache__/filters.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/spruce/__pycache__/filters.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/spruce/__pycache__/filters.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/spruce/filters.py` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/obtain_proceeds/spruce/filters.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/stats/__init__.py` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/stats/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/stats/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/stats/__pycache__/__init__.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/stats/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/stats/__pycache__/union.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/stats/__pycache__/union.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/stats/union.py` & `goodest-1.2.2/venues/stages/goodest/adventures/monetary/quests/search_goods/techniques/stats/union.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/redis_mix/_ops/__pycache__/off.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/redis_mix/_ops/__pycache__/off.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/redis_mix/_ops/__pycache__/on.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/redis_mix/_ops/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/redis_mix/_ops/__pycache__/refresh.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/redis_mix/_ops/__pycache__/refresh.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/redis_mix/_ops/__pycache__/status.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/redis_mix/_ops/__pycache__/status.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/redis_mix/_ops/_clique.py` & `goodest-1.2.2/venues/stages/goodest/adventures/redis_mix/_ops/_clique.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/sanique/[objectives]/objectives.S.HTML` & `goodest-1.2.2/venues/stages/goodest/adventures/sanique/[objectives]/objectives.S.HTML`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/sanique/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/sanique/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/sanique/_ops/__pycache__/off.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/sanique/_ops/__pycache__/off.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/sanique/_ops/__pycache__/on.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/sanique/_ops/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/sanique/_ops/__pycache__/refresh.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/sanique/_ops/__pycache__/refresh.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/sanique/_ops/__pycache__/status.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/sanique/_ops/__pycache__/status.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/sanique/_ops/off.py` & `goodest-1.2.2/venues/stages/goodest/adventures/sanique/_ops/off.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/sanique/_ops/on.py` & `goodest-1.2.2/venues/stages/goodest/adventures/sanique/_ops/on.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/sanique/_ops/refresh.py` & `goodest-1.2.2/venues/stages/goodest/adventures/sanique/_ops/refresh.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/sanique/_ops/status.py` & `goodest-1.2.2/venues/stages/goodest/adventures/sanique/_ops/status.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/sanique/_status/API_status_besties__food_USDA__nature_v2__FDC_ID_1.py` & `goodest-1.2.2/venues/stages/goodest/adventures/sanique/_status/API_status_besties__food_USDA__nature_v2__FDC_ID_1.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/sanique/_status/__pycache__/API_status_besties__food_USDA__nature_v2__FDC_ID_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/sanique/_status/__pycache__/API_status_besties__food_USDA__nature_v2__FDC_ID_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/sanique/clique.py` & `goodest-1.2.2/venues/stages/goodest/adventures/sanique/clique.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/__init__.py` & `goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/addresses/guest/__init__.py` & `goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/addresses/guest/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/addresses/guest/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/addresses/guest/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/addresses/guest/vue/__init__.py` & `goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/addresses/guest/vue/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,12 +109,11 @@
 			return sanic_response.html (front_inventory_paths ["index.html"] ["content"])
 
 
 		
 		@guest_addresses.route ("/front/<encoded_path:path>")
 		async def handle_path (request, encoded_path):
 			path = unquote (encoded_path)
-			return sanic_response.html (the_index)
 			return sanic_response.html (front_inventory_paths ["index.html"] ["content"])
```

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/addresses/guest/vue/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/addresses/guest/vue/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue May 14 01:19:21 2024 UTC, .py size: 3002 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 19bc 4266 ba0b 0000  o.........Bf....
+00000000: 6f0d 0d0a 0000 0000 02c5 4266 900b 0000  o.........Bf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 9c00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 5a04 6400  m.Z...d.d.l.Z.d.
 00000050: 6404 6c04 6d05 5a05 0100 6400 6405 6c06  d.l.m.Z...d.d.l.
 00000060: 6d07 5a07 0100 6400 6403 6c08 6d09 5a0a  m.Z...d.d.l.m.Z.
 00000070: 0100 6400 6406 6c0b 6d0c 5a0c 6d0d 5a0d  ..d.d.l.m.Z.m.Z.
@@ -17,132 +17,132 @@
 00000100: 734e 2901 da05 5361 6e69 6329 01da 076f  sN)...Sanic)...o
 00000110: 7065 6e61 7069 2902 da07 4c69 6d69 7465  penapi)...Limite
 00000120: 72da 1267 6574 5f72 656d 6f74 655f 6164  r..get_remote_ad
 00000130: 6472 6573 7329 04da 0665 7869 7374 73da  dress)...exists.
 00000140: 0764 6972 6e61 6d65 da08 6e6f 726d 7061  .dirname..normpa
 00000150: 7468 da04 6a6f 696e 2901 da07 756e 7175  th..join)...unqu
 00000160: 6f74 6563 0100 0000 0000 0000 0000 0000  otec............
-00000170: 0800 0000 0500 0000 0300 0000 73e8 0000  ............s...
+00000170: 0800 0000 0500 0000 0300 0000 73e6 0000  ............s...
 00000180: 0074 0083 007d 017c 0064 0119 007d 027c  .t...}.|.d...}.|
 00000190: 0064 0219 007d 0374 017c 0164 0319 0064  .d...}.t.|.d...d
 000001a0: 0419 0083 0189 007c 0164 0319 0064 0419  .......|.d...d..
 000001b0: 0064 0517 0089 017c 0164 0319 0064 0419  .d.....|.d...d..
 000001c0: 0064 0617 007d 0409 007c 0164 0719 0064  .d...}...|.d...d
 000001d0: 086b 0272 507c 026a 0264 067c 0164 0319  .k.rP|.j.d.|.d..
 000001e0: 0064 0419 0064 0617 0064 0964 0a8d 0301  .d...d...d.d....
 000001f0: 007c 03a0 0364 0ba1 0187 0166 0164 0c64  .|...d.....f.d.d
 00000200: 0d84 0883 017d 057c 03a0 0364 0ea1 0187  .....}.|...d....
 00000210: 0166 0164 0f64 1084 0883 017d 0664 0053  .f.d.d.....}.d.S
 00000220: 007c 03a0 0364 11a1 0187 0066 0164 1264  .|...d.....f.d.d
 00000230: 1384 0883 017d 077c 03a0 0364 0ba1 0187  .....}.|...d....
 00000240: 0066 0164 1464 0d84 0883 017d 057c 03a0  .f.d.d.....}.|..
-00000250: 0364 0ea1 0187 0087 0166 0264 1564 1084  .d.......f.d.d..
-00000260: 0883 017d 0664 0053 0029 164e da03 6170  ...}.d.S.).N..ap
-00000270: 70da 0f67 7565 7374 5f61 6464 7265 7373  p..guest_address
-00000280: 6573 da08 7676 5f74 7572 626f da09 6469  es..vv_turbo..di
-00000290: 7374 5f70 6174 687a 0b2f 696e 6465 782e  st_pathz./index.
-000002a0: 6874 6d6c 7a07 2f61 7373 6574 73da 046d  htmlz./assets..m
-000002b0: 6f64 65da 076e 7572 7475 7265 da06 6173  ode..nurture..as
-000002c0: 7365 7473 2901 da04 6e61 6d65 fa01 2f63  sets)...name../c
-000002d0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-000002e0: 0300 0000 9300 0000 f312 0000 0081 0174  ...............t
-000002f0: 00a0 0188 00a1 0149 0064 0048 0053 00a9  .......I.d.H.S..
-00000300: 014e a902 da0e 7361 6e69 635f 7265 7370  .N....sanic_resp
-00000310: 6f6e 7365 da04 6669 6c65 2901 da07 7265  onse..file)...re
-00000320: 7175 6573 74a9 01da 0974 6865 5f69 6e64  quest....the_ind
-00000330: 6578 a900 fa58 2f68 6162 6974 6174 2f76  ex...X/habitat/v
-00000340: 656e 7565 732f 7374 6167 6573 2f67 6f6f  enues/stages/goo
-00000350: 6465 7374 2f61 6476 656e 7475 7265 732f  dest/adventures/
-00000360: 7361 6e69 7175 652f 6861 7262 6f72 2f61  sanique/harbor/a
-00000370: 6464 7265 7373 6573 2f67 7565 7374 2f76  ddresses/guest/v
-00000380: 7565 2f5f 5f69 6e69 745f 5f2e 7079 da04  ue/__init__.py..
-00000390: 686f 6d65 4500 0000 7304 0000 0002 8010  homeE...s.......
-000003a0: 027a 1976 7565 5f72 6567 696f 6e73 2e3c  .z.vue_regions.<
-000003b0: 6c6f 6361 6c73 3e2e 686f 6d65 7a1a 2f66  locals>.homez./f
-000003c0: 726f 6e74 2f3c 656e 636f 6465 645f 7061  ront/<encoded_pa
-000003d0: 7468 3a70 6174 683e 6302 0000 0000 0000  th:path>c.......
-000003e0: 0000 0000 0002 0000 0003 0000 0093 0000  ................
-000003f0: 0072 1600 0000 7217 0000 0072 1800 0000  .r....r....r....
-00000400: 2902 721b 0000 00da 0c65 6e63 6f64 6564  ).r......encoded
-00000410: 5f70 6174 6872 1c00 0000 721e 0000 0072  _pathr....r....r
-00000420: 1f00 0000 da0b 6861 6e64 6c65 5f70 6174  ......handle_pat
-00000430: 684a 0000 0073 0400 0000 0280 1003 7a20  hJ...s........z 
-00000440: 7675 655f 7265 6769 6f6e 732e 3c6c 6f63  vue_regions.<loc
-00000450: 616c 733e 2e68 616e 646c 655f 7061 7468  als>.handle_path
-00000460: 7a13 2f61 7373 6574 732f 3c70 6174 683a  z./assets/<path:
-00000470: 7061 7468 3e63 0200 0000 0000 0000 0000  path>c..........
-00000480: 0000 0600 0000 0a00 0000 9300 0000 737e  ..............s~
-00000490: 0000 0081 017a 1f64 017c 019b 009d 027d  .....z.d.|.....}
-000004a0: 027c 0288 0076 0072 1f88 007c 0219 0064  .|...v.r...|...d
-000004b0: 0219 007d 0388 007c 0219 0064 0319 007d  ...}...|...d...}
-000004c0: 0474 006a 017c 047c 0364 048d 0257 0053  .t.j.|.|.d...W.S
-000004d0: 0057 006e 1704 0074 0279 3701 007d 0501  .W.n...t.y7..}..
-000004e0: 007a 0b74 0364 057c 0583 0201 0057 0059  .z.t.d.|.....W.Y
-000004f0: 0064 007d 057e 056e 0564 007d 057e 0577  .d.}.~.n.d.}.~.w
-00000500: 0177 0074 006a 0464 0664 0764 088d 0253  .w.t.j.d.d.d...S
-00000510: 0029 094e 7a07 6173 7365 7473 2fda 046d  .).Nz.assets/..m
-00000520: 696d 65da 0763 6f6e 7465 6e74 2901 da0c  ime..content)...
-00000530: 636f 6e74 656e 745f 7479 7065 7a02 453a  content_typez.E:
-00000540: 7a25 416e 2061 6e6f 6d61 6c79 206f 6363  z%An anomaly occ
-00000550: 7572 7265 6420 7768 696c 6520 7072 6f63  urred while proc
-00000560: 6573 7369 6e67 2e69 5802 0000 2901 da06  essing.iX...)...
-00000570: 7374 6174 7573 2905 7219 0000 00da 0372  status).r......r
-00000580: 6177 da09 4578 6365 7074 696f 6eda 0570  aw..Exception..p
-00000590: 7269 6e74 da04 7465 7874 2906 721b 0000  rint..text).r...
-000005a0: 00da 0470 6174 68da 0966 756c 6c5f 7061  ...path..full_pa
-000005b0: 7468 7225 0000 0072 2400 0000 da01 45a9  thr%...r$.....E.
-000005c0: 01da 1566 726f 6e74 5f69 6e76 656e 746f  ...front_invento
-000005d0: 7279 5f70 6174 6873 721e 0000 0072 1f00  ry_pathsr....r..
-000005e0: 0000 da0c 6173 7365 7473 5f72 6f75 7465  ....assets_route
-000005f0: 5000 0000 731a 0000 0002 8002 030a 0108  P...s...........
-00000600: 010c 010c 0110 0204 fc0e 0516 0108 8002  ................
-00000610: ff0e 037a 2176 7565 5f72 6567 696f 6e73  ...z!vue_regions
-00000620: 2e3c 6c6f 6361 6c73 3e2e 6173 7365 7473  .<locals>.assets
-00000630: 5f72 6f75 7465 6301 0000 0000 0000 0000  _routec.........
-00000640: 0000 0002 0000 0004 0000 0093 0000 0073  ...............s
-00000650: 1a00 0000 8101 7400 8300 7d01 7401 a002  ......t...}.t...
-00000660: 8800 6401 1900 6402 1900 a101 5300 2903  ..d...d.....S.).
-00000670: 4e7a 0a69 6e64 6578 2e68 746d 6c72 2400  Nz.index.htmlr$.
-00000680: 0000 2903 7202 0000 0072 1900 0000 da04  ..).r....r......
-00000690: 6874 6d6c 2902 721b 0000 00da 0765 7373  html).r......ess
-000006a0: 656e 6365 722e 0000 0072 1e00 0000 721f  encer....r....r.
-000006b0: 0000 0072 2000 0000 6300 0000 7306 0000  ...r ...c...s...
-000006c0: 0002 8006 0212 0863 0200 0000 0000 0000  .......c........
-000006d0: 0000 0000 0300 0000 0300 0000 9300 0000  ................
-000006e0: 7314 0000 0081 0174 007c 0183 017d 0274  s......t.|...}.t
-000006f0: 01a0 0288 01a1 0153 0072 1700 0000 2903  .......S.r....).
-00000700: 720c 0000 0072 1900 0000 7231 0000 0029  r....r....r1...)
-00000710: 0372 1b00 0000 7221 0000 0072 2b00 0000  .r....r!...r+...
-00000720: a902 722f 0000 0072 1d00 0000 721e 0000  ..r/...r....r...
-00000730: 0072 1f00 0000 7222 0000 0071 0000 0073  .r....r"...q...s
-00000740: 0600 0000 0280 0802 0a01 2904 7202 0000  ..........).r...
-00000750: 0072 0300 0000 da06 7374 6174 6963 da05  .r......static..
-00000760: 726f 7574 6529 08da 1276 7565 5f72 6567  route)...vue_reg
-00000770: 696f 6e73 5f70 6163 6b65 7472 3200 0000  ions_packetr2...
-00000780: 720d 0000 0072 0e00 0000 da0a 7468 655f  r....r......the_
-00000790: 6173 7365 7473 7220 0000 0072 2200 0000  assetsr ...r"...
-000007a0: 7230 0000 0072 1e00 0000 7233 0000 0072  r0...r....r3...r
-000007b0: 1f00 0000 da0b 7675 655f 7265 6769 6f6e  ......vue_region
-000007c0: 7319 0000 0073 2a00 0000 0601 0802 0801  s....s*.........
-000007d0: 0203 0a01 04ff 1004 1001 0207 0c11 1c01  ................
-000007e0: 0807 0e01 0804 1201 0805 0e01 0812 0e01  ................
-000007f0: 080d 1401 7238 0000 0029 19da 1067 6f6f  ....r8...)...goo
-00000800: 6465 7374 2e5f 6573 7365 6e63 6572 0200  dest._essencer..
-00000810: 0000 da3d 676f 6f64 6573 742e 6164 7665  ...=goodest.adve
-00000820: 6e74 7572 6573 2e73 616e 6971 7565 2e75  ntures.sanique.u
-00000830: 7469 6c69 7469 6573 2e67 656e 6572 6174  tilities.generat
-00000840: 655f 696e 7665 6e74 6f72 795f 7061 7468  e_inventory_path
-00000850: 7372 0300 0000 da05 7361 6e69 6372 0400  sr......sanicr..
-00000860: 0000 da09 7361 6e69 635f 6578 7472 0500  ....sanic_extr..
-00000870: 0000 da0e 7361 6e69 632e 7265 7370 6f6e  ....sanic.respon
-00000880: 7365 da08 7265 7370 6f6e 7365 7219 0000  se..responser...
-00000890: 00da 0d73 616e 6963 5f6c 696d 6974 6572  ...sanic_limiter
-000008a0: 7206 0000 0072 0700 0000 da04 6a73 6f6e  r....r......json
-000008b0: da07 6f73 2e70 6174 6872 0800 0000 7209  ..os.pathr....r.
-000008c0: 0000 0072 0a00 0000 720b 0000 00da 0c75  ...r....r......u
-000008d0: 726c 6c69 622e 7061 7273 6572 0c00 0000  rllib.parser....
-000008e0: da09 7468 7265 6164 696e 67da 0474 696d  ..threading..tim
-000008f0: 6572 3800 0000 721e 0000 0072 1e00 0000  er8...r....r....
-00000900: 721e 0000 0072 1f00 0000 da08 3c6d 6f64  r....r......<mod
-00000910: 756c 653e 0100 0000 731a 0000 000c 040c  ule>....s.......
-00000920: 0108 030c 010c 010c 0110 0108 0418 010c  ................
-00000930: 0108 0108 010c 04                        .......
+00000250: 0364 0ea1 0187 0066 0164 1564 1084 0883  .d.....f.d.d....
+00000260: 017d 0664 0053 0029 164e da03 6170 70da  .}.d.S.).N..app.
+00000270: 0f67 7565 7374 5f61 6464 7265 7373 6573  .guest_addresses
+00000280: da08 7676 5f74 7572 626f da09 6469 7374  ..vv_turbo..dist
+00000290: 5f70 6174 687a 0b2f 696e 6465 782e 6874  _pathz./index.ht
+000002a0: 6d6c 7a07 2f61 7373 6574 73da 046d 6f64  mlz./assets..mod
+000002b0: 65da 076e 7572 7475 7265 da06 6173 7365  e..nurture..asse
+000002c0: 7473 2901 da04 6e61 6d65 fa01 2f63 0100  ts)...name../c..
+000002d0: 0000 0000 0000 0000 0000 0100 0000 0300  ................
+000002e0: 0000 9300 0000 f312 0000 0081 0174 00a0  .............t..
+000002f0: 0188 00a1 0149 0064 0048 0053 00a9 014e  .....I.d.H.S...N
+00000300: a902 da0e 7361 6e69 635f 7265 7370 6f6e  ....sanic_respon
+00000310: 7365 da04 6669 6c65 2901 da07 7265 7175  se..file)...requ
+00000320: 6573 74a9 01da 0974 6865 5f69 6e64 6578  est....the_index
+00000330: a900 fa58 2f68 6162 6974 6174 2f76 656e  ...X/habitat/ven
+00000340: 7565 732f 7374 6167 6573 2f67 6f6f 6465  ues/stages/goode
+00000350: 7374 2f61 6476 656e 7475 7265 732f 7361  st/adventures/sa
+00000360: 6e69 7175 652f 6861 7262 6f72 2f61 6464  nique/harbor/add
+00000370: 7265 7373 6573 2f67 7565 7374 2f76 7565  resses/guest/vue
+00000380: 2f5f 5f69 6e69 745f 5f2e 7079 da04 686f  /__init__.py..ho
+00000390: 6d65 4500 0000 7304 0000 0002 8010 027a  meE...s........z
+000003a0: 1976 7565 5f72 6567 696f 6e73 2e3c 6c6f  .vue_regions.<lo
+000003b0: 6361 6c73 3e2e 686f 6d65 7a1a 2f66 726f  cals>.homez./fro
+000003c0: 6e74 2f3c 656e 636f 6465 645f 7061 7468  nt/<encoded_path
+000003d0: 3a70 6174 683e 6302 0000 0000 0000 0000  :path>c.........
+000003e0: 0000 0002 0000 0003 0000 0093 0000 0072  ...............r
+000003f0: 1600 0000 7217 0000 0072 1800 0000 2902  ....r....r....).
+00000400: 721b 0000 00da 0c65 6e63 6f64 6564 5f70  r......encoded_p
+00000410: 6174 6872 1c00 0000 721e 0000 0072 1f00  athr....r....r..
+00000420: 0000 da0b 6861 6e64 6c65 5f70 6174 684a  ....handle_pathJ
+00000430: 0000 0073 0400 0000 0280 1003 7a20 7675  ...s........z vu
+00000440: 655f 7265 6769 6f6e 732e 3c6c 6f63 616c  e_regions.<local
+00000450: 733e 2e68 616e 646c 655f 7061 7468 7a13  s>.handle_pathz.
+00000460: 2f61 7373 6574 732f 3c70 6174 683a 7061  /assets/<path:pa
+00000470: 7468 3e63 0200 0000 0000 0000 0000 0000  th>c............
+00000480: 0600 0000 0a00 0000 9300 0000 737e 0000  ............s~..
+00000490: 0081 017a 1f64 017c 019b 009d 027d 027c  ...z.d.|.....}.|
+000004a0: 0288 0076 0072 1f88 007c 0219 0064 0219  ...v.r...|...d..
+000004b0: 007d 0388 007c 0219 0064 0319 007d 0474  .}...|...d...}.t
+000004c0: 006a 017c 047c 0364 048d 0257 0053 0057  .j.|.|.d...W.S.W
+000004d0: 006e 1704 0074 0279 3701 007d 0501 007a  .n...t.y7..}...z
+000004e0: 0b74 0364 057c 0583 0201 0057 0059 0064  .t.d.|.....W.Y.d
+000004f0: 007d 057e 056e 0564 007d 057e 0577 0177  .}.~.n.d.}.~.w.w
+00000500: 0074 006a 0464 0664 0764 088d 0253 0029  .t.j.d.d.d...S.)
+00000510: 094e 7a07 6173 7365 7473 2fda 046d 696d  .Nz.assets/..mim
+00000520: 65da 0763 6f6e 7465 6e74 2901 da0c 636f  e..content)...co
+00000530: 6e74 656e 745f 7479 7065 7a02 453a 7a25  ntent_typez.E:z%
+00000540: 416e 2061 6e6f 6d61 6c79 206f 6363 7572  An anomaly occur
+00000550: 7265 6420 7768 696c 6520 7072 6f63 6573  red while proces
+00000560: 7369 6e67 2e69 5802 0000 2901 da06 7374  sing.iX...)...st
+00000570: 6174 7573 2905 7219 0000 00da 0372 6177  atus).r......raw
+00000580: da09 4578 6365 7074 696f 6eda 0570 7269  ..Exception..pri
+00000590: 6e74 da04 7465 7874 2906 721b 0000 00da  nt..text).r.....
+000005a0: 0470 6174 68da 0966 756c 6c5f 7061 7468  .path..full_path
+000005b0: 7225 0000 0072 2400 0000 da01 45a9 01da  r%...r$.....E...
+000005c0: 1566 726f 6e74 5f69 6e76 656e 746f 7279  .front_inventory
+000005d0: 5f70 6174 6873 721e 0000 0072 1f00 0000  _pathsr....r....
+000005e0: da0c 6173 7365 7473 5f72 6f75 7465 5000  ..assets_routeP.
+000005f0: 0000 731a 0000 0002 8002 030a 0108 010c  ..s.............
+00000600: 010c 0110 0204 fc0e 0516 0108 8002 ff0e  ................
+00000610: 037a 2176 7565 5f72 6567 696f 6e73 2e3c  .z!vue_regions.<
+00000620: 6c6f 6361 6c73 3e2e 6173 7365 7473 5f72  locals>.assets_r
+00000630: 6f75 7465 6301 0000 0000 0000 0000 0000  outec...........
+00000640: 0002 0000 0004 0000 0093 0000 0073 1a00  .............s..
+00000650: 0000 8101 7400 8300 7d01 7401 a002 8800  ....t...}.t.....
+00000660: 6401 1900 6402 1900 a101 5300 a903 4e7a  d...d.....S...Nz
+00000670: 0a69 6e64 6578 2e68 746d 6c72 2400 0000  .index.htmlr$...
+00000680: 2903 7202 0000 0072 1900 0000 da04 6874  ).r....r......ht
+00000690: 6d6c 2902 721b 0000 00da 0765 7373 656e  ml).r......essen
+000006a0: 6365 722e 0000 0072 1e00 0000 721f 0000  cer....r....r...
+000006b0: 0072 2000 0000 6300 0000 7306 0000 0002  .r ...c...s.....
+000006c0: 8006 0212 0863 0200 0000 0000 0000 0000  .....c..........
+000006d0: 0000 0300 0000 0400 0000 9300 0000 731c  ..............s.
+000006e0: 0000 0081 0174 007c 0183 017d 0274 01a0  .....t.|...}.t..
+000006f0: 0288 0064 0119 0064 0219 00a1 0153 0072  ...d...d.....S.r
+00000700: 3100 0000 2903 720c 0000 0072 1900 0000  1...).r....r....
+00000710: 7232 0000 0029 0372 1b00 0000 7221 0000  r2...).r....r!..
+00000720: 0072 2b00 0000 722e 0000 0072 1e00 0000  .r+...r....r....
+00000730: 721f 0000 0072 2200 0000 7100 0000 7306  r....r"...q...s.
+00000740: 0000 0002 8008 0212 0129 0472 0200 0000  .........).r....
+00000750: 7203 0000 00da 0673 7461 7469 63da 0572  r......static..r
+00000760: 6f75 7465 2908 da12 7675 655f 7265 6769  oute)...vue_regi
+00000770: 6f6e 735f 7061 636b 6574 7233 0000 0072  ons_packetr3...r
+00000780: 0d00 0000 720e 0000 00da 0a74 6865 5f61  ....r......the_a
+00000790: 7373 6574 7372 2000 0000 7222 0000 0072  ssetsr ...r"...r
+000007a0: 3000 0000 721e 0000 0029 0272 2f00 0000  0...r....).r/...
+000007b0: 721d 0000 0072 1f00 0000 da0b 7675 655f  r....r......vue_
+000007c0: 7265 6769 6f6e 7319 0000 0073 2a00 0000  regions....s*...
+000007d0: 0601 0802 0801 0203 0a01 04ff 1004 1001  ................
+000007e0: 0207 0c11 1c01 0807 0e01 0804 1201 0805  ................
+000007f0: 0e01 0812 0e01 080d 1201 7238 0000 0029  ..........r8...)
+00000800: 19da 1067 6f6f 6465 7374 2e5f 6573 7365  ...goodest._esse
+00000810: 6e63 6572 0200 0000 da3d 676f 6f64 6573  ncer.....=goodes
+00000820: 742e 6164 7665 6e74 7572 6573 2e73 616e  t.adventures.san
+00000830: 6971 7565 2e75 7469 6c69 7469 6573 2e67  ique.utilities.g
+00000840: 656e 6572 6174 655f 696e 7665 6e74 6f72  enerate_inventor
+00000850: 795f 7061 7468 7372 0300 0000 da05 7361  y_pathsr......sa
+00000860: 6e69 6372 0400 0000 da09 7361 6e69 635f  nicr......sanic_
+00000870: 6578 7472 0500 0000 da0e 7361 6e69 632e  extr......sanic.
+00000880: 7265 7370 6f6e 7365 da08 7265 7370 6f6e  response..respon
+00000890: 7365 7219 0000 00da 0d73 616e 6963 5f6c  ser......sanic_l
+000008a0: 696d 6974 6572 7206 0000 0072 0700 0000  imiterr....r....
+000008b0: da04 6a73 6f6e da07 6f73 2e70 6174 6872  ..json..os.pathr
+000008c0: 0800 0000 7209 0000 0072 0a00 0000 720b  ....r....r....r.
+000008d0: 0000 00da 0c75 726c 6c69 622e 7061 7273  .....urllib.pars
+000008e0: 6572 0c00 0000 da09 7468 7265 6164 696e  er......threadin
+000008f0: 67da 0474 696d 6572 3800 0000 721e 0000  g..timer8...r...
+00000900: 0072 1e00 0000 721e 0000 0072 1f00 0000  .r....r....r....
+00000910: da08 3c6d 6f64 756c 653e 0100 0000 731a  ..<module>....s.
+00000920: 0000 000c 040c 0108 030c 010c 010c 0110  ................
+00000930: 0108 0418 010c 0108 0108 010c 04         .............
```

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/addresses/guest/vue/__pycache__/__init__.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/addresses/guest/vue/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/addresses/guest/vue/caching.S.HTML` & `goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/addresses/guest/vue/caching.S.HTML`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/addresses/guest_bits/__init__.py` & `goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/addresses/guest_bits/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/addresses/guest_bits/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/addresses/guest_bits/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/addresses/guest_goodest_inventory/foods/__init__.py` & `goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/addresses/guest_goodest_inventory/foods/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/addresses/guest_goodest_inventory/foods/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/addresses/guest_goodest_inventory/foods/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/addresses/guest_goodest_inventory/recipes/__init__.py` & `goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/addresses/guest_goodest_inventory/recipes/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/addresses/guest_goodest_inventory/recipes/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/addresses/guest_goodest_inventory/recipes/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/addresses/guest_goodest_inventory/supps/__init__.py` & `goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/addresses/guest_goodest_inventory/supps/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/addresses/guest_goodest_inventory/supps/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/addresses/guest_goodest_inventory/supps/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/addresses/staff/__init__.py` & `goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/addresses/staff/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/addresses/staff/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/addresses/staff/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/addresses/staff/__pycache__/besties__food_USDA__nature_v2__FDC_ID.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/addresses/staff/__pycache__/besties__food_USDA__nature_v2__FDC_ID.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/addresses/staff/__pycache__/besties__supp_NIH__nature_v2__DSLD_ID.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/addresses/staff/__pycache__/besties__supp_NIH__nature_v2__DSLD_ID.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/addresses/staff/besties__food_USDA__nature_v2__FDC_ID.py` & `goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/addresses/staff/besties__food_USDA__nature_v2__FDC_ID.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/addresses/staff/besties__supp_NIH__nature_v2__DSLD_ID.py` & `goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/addresses/staff/besties__supp_NIH__nature_v2__DSLD_ID.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/addresses/staff_goodest_inventory/foods/__init__.py` & `goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/addresses/staff_goodest_inventory/foods/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/addresses/staff_goodest_inventory/foods/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/addresses/staff_goodest_inventory/foods/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/addresses/staff_goodest_inventory/recipes/__init__.py` & `goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/addresses/staff_goodest_inventory/recipes/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/addresses/staff_goodest_inventory/recipes/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/addresses/staff_goodest_inventory/recipes/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/addresses/staff_goodest_inventory/supps/__init__.py` & `goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/addresses/staff_goodest_inventory/supps/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/addresses/staff_goodest_inventory/supps/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/addresses/staff_goodest_inventory/supps/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/sanique/harbor/sockets_guest/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/sanique/harbor/sockets_guest/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/sanique/quests_guests/__pycache__/find_food.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/sanique/quests_guests/__pycache__/find_food.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/sanique/quests_guests/__pycache__/retrieve_food.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/sanique/quests_guests/__pycache__/retrieve_food.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/sanique/quests_guests/__pycache__/retrieve_goals.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/sanique/quests_guests/__pycache__/retrieve_goals.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/sanique/quests_guests/__pycache__/retrieve_recipe.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/sanique/quests_guests/__pycache__/retrieve_recipe.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/sanique/quests_guests/__pycache__/retrieve_supp.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/sanique/quests_guests/__pycache__/retrieve_supp.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/sanique/quests_guests/__pycache__/search_goods.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/sanique/quests_guests/__pycache__/search_goods.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/sanique/quests_guests/retrieve_food.py` & `goodest-1.2.2/venues/stages/goodest/adventures/sanique/quests_guests/retrieve_food.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/sanique/quests_guests/retrieve_recipe.py` & `goodest-1.2.2/venues/stages/goodest/adventures/sanique/quests_guests/retrieve_recipe.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/sanique/quests_guests/retrieve_supp.py` & `goodest-1.2.2/venues/stages/goodest/adventures/sanique/quests_guests/retrieve_supp.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/sanique/quests_guests/search_goods.py` & `goodest-1.2.2/venues/stages/goodest/adventures/sanique/quests_guests/search_goods.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/sanique/sanique.S.HTML` & `goodest-1.2.2/venues/stages/goodest/adventures/sanique/sanique.S.HTML`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/sanique/utilities/__pycache__/generate_inventory_paths.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/sanique/utilities/__pycache__/generate_inventory_paths.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/sanique/utilities/__pycache__/retrieve_sanique_URL.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/sanique/utilities/__pycache__/retrieve_sanique_URL.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/sanique/utilities/check_key/__init__.py` & `goodest-1.2.2/venues/stages/goodest/adventures/sanique/utilities/check_key/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/sanique/utilities/check_key/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/adventures/sanique/utilities/check_key/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/sanique/utilities/generate_inventory_paths.py` & `goodest-1.2.2/venues/stages/goodest/adventures/sanique/utilities/generate_inventory_paths.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/README.md` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/README.md`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/__objectives/objectives -- possibilities.S.HTML` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/__objectives/objectives -- possibilities.S.HTML`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/school/public/typescript.svg` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/school/dist/typescript.svg`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/school/public/vite.svg` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/school/dist/vite.svg`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/staff/public/typescript.svg` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/school/public/typescript.svg`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/staff/public/vite.svg` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/school/public/vite.svg`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/.eslintrc.json` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/.eslintrc.json`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/index.html` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/index.html`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/package.json` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/package.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9880952380952381%*

 * *Differences: {"'scripts'": "{'build': 'vite build --watch --outDir the_build', delete: ['build-monitor']}"}*

```diff
@@ -64,16 +64,15 @@
         "vitest": "^0.33.0",
         "wait-on": "^7.0.1"
     },
     "name": "web",
     "private": true,
     "scripts": {
         "----": "----",
-        "build": "vite build --watch",
-        "build-monitor": "vite build --watch",
+        "build": "vite build --watch --outDir the_build",
         "build-tsc": "tsc && vite build",
         "dev": "vite --host 0.0.0.0 --port 9000 --clearScreen false",
         "lint": "eslint -c ./.eslintrc.json src",
         "lint--": "eslint \"src/**/*.ts\"",
         "preview": "vite preview",
         "status": "vitest run"
     },
```

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/Earth/app.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/Earth/app.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/Earth/logistics/guests/index.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/Earth/logistics/guests/index.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/Earth/logistics/index.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/Earth/logistics/index.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/Earth/logistics/status/index.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/Earth/logistics/status/index.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/Earth/scenery/planet/field.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/Earth/scenery/planet/field.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/Earth/scenery/planet/field.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/Earth/scenery/planet/field.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/Earth/warehouses/layout/index.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/Earth/warehouses/layout/index.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/fields/app/index.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/fields/app/index.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/fields/append.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/fields/append.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/fields/boundary/embellishments.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/fields/boundary/embellishments.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/fields/boundary/embellishments.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/fields/boundary/embellishments.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/fields/fields.S.HTML` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/fields/fields.S.HTML`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/fields/hacienda/eco.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/fields/hacienda/eco.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/fields/hacienda/eco.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/fields/hacienda/eco.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/fields/hacienda/methods/fn/keypress.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/fields/hacienda/methods/fn/keypress.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/fields/hacienda/methods/index.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/fields/hacienda/methods/index.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/fields/remove.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/apps/fields/remove.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/assets/base--.css` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/assets/base--.css`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/fleet/ask/get.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/fleet/ask/get.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/fleet/goodest_DB/essential_nutrients/recipe/index.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/fleet/goodest_DB/essential_nutrients/recipe/index.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/fleet/goodest_DB/food/retrieve/index.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/fleet/goodest_DB/food/retrieve/index.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/fleet/goodest_DB/supp/retrieve/index.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/fleet/goodest_DB/supp/retrieve/index.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/fleet/goodest_DB/treasures/search/index.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/fleet/goodest_DB/treasures/search/index.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/fleet/syllabus/lap/index.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/fleet/syllabus/lap/index.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/Fraction/to_float.ST.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/Fraction/to_float.ST.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/Fraction/to_float.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/Fraction/to_float.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/food/FIND_ENERGY_PER_GRAM.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/food/FIND_ENERGY_PER_GRAM.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/furnish/array.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/furnish/array.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/furnish/array.status.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/furnish/array.status.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/furnish/index.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/furnish/index.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/furnish/string.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/furnish/string.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/furnish/string.status.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/furnish/string.status.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/monitors/focus.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/monitors/focus.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/essential_nutrients/grove/calc_linear_grove/grove-1.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/essential_nutrients/grove/calc_linear_grove/grove-1.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/essential_nutrients/grove/calc_linear_grove/index.ST.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/essential_nutrients/grove/calc_linear_grove/index.ST.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/essential_nutrients/grove/calc_linear_grove/index.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/essential_nutrients/grove/calc_linear_grove/index.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/essential_nutrients/grove/ingredient/biological_activity.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/essential_nutrients/grove/ingredient/biological_activity.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/essential_nutrients/grove/sort/cryo/grove-1.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/essential_nutrients/grove/sort/cryo/grove-1.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/essential_nutrients/grove/sort/index.2.ST.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/essential_nutrients/grove/sort/index.2.ST.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/essential_nutrients/grove/sort/index.ST.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/essential_nutrients/grove/sort/index.ST.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/essential_nutrients/grove/sort/index.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/essential_nutrients/grove/sort/index.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/product/is.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/product/is.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/product/quantified_grove/sort.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nature/product/quantified_grove/sort.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nutrients--/sort/index.ST.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nutrients--/sort/index.ST.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nutrients--/sort/index.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/nutrients--/sort/index.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/round_quantity/index.ST.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/round_quantity/index.ST.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/round_quantity/index.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/round_quantity/index.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/struct_2/ingredient/mass.ST.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/struct_2/ingredient/mass.ST.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/struct_2/ingredient/mass.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/struct_2/ingredient/mass.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/struct_2/product/is.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/struct_2/product/is.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/struct_2/product/quantified_grove/sort.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/grid/struct_2/product/quantified_grove/sort.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/about/decor.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/about/decor.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/about/decor.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/about/decor.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/controls/decor/custom/decor.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/controls/decor/custom/decor.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/controls/decor/generic/decor.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/controls/decor/generic/decor.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/controls/decor/references/decor.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/controls/decor/references/decor.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/controls/decor.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/controls/decor.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/controls/decor.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/controls/decor.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/controls/notes/ARIA/roles.r.html` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/controls/notes/ARIA/roles.r.html`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/controls/notes/notes.r.html` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/controls/notes/notes.r.html`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/controls/priorities/possibilities.s.HTML` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/controls/priorities/possibilities.s.HTML`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/empty_cart/field.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/empty_cart/field.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/empty_cart/field.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/empty_cart/field.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/ingredient/feature.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/ingredient/feature.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/navigation-lab/field.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/navigation-lab/field.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/navigation-lab/field.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/navigation-lab/field.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/physics/field.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/physics/field.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/physics/field.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/physics/field.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/scan_filter_by/field.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/scan_filter_by/field.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/scan_filter_by/field.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/scan_filter_by/field.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/sink-filter/field.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/sink-filter/field.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/sink-filter/field.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/sink-filter/field.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/sink-filter/steps.S.HTML` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/sink-filter/steps.S.HTML`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/sink-filter/steps_v1.S.HTML` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/sink-filter/steps_v1.S.HTML`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/sink-filter/steps_v2.S.HTML` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/sink-filter/steps_v2.S.HTML`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/unit_systems/decor/system_international_with_food_calories_and_IU/field.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/unit_systems/decor/system_international_with_food_calories_and_IU/field.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/unreported/field.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/parcels/unreported/field.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/__shows_d3/decor.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/__shows_d3/decor.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/__shows_d3/theatrics/NETWORK_2/field.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/__shows_d3/theatrics/NETWORK_2/field.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/__shows_d3/theatrics/NETWORK_D3_2/PHYSICAL/index.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/__shows_d3/theatrics/NETWORK_D3_2/PHYSICAL/index.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/__shows_d3/theatrics/NETWORK_D3_2/field.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/__shows_d3/theatrics/NETWORK_D3_2/field.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/__shows_d3/theatrics/NETWORK_D3_3/field.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/__shows_d3/theatrics/NETWORK_D3_3/field.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/__shows_d3/theatrics/NETWORK_D3_3/methods/PHYSICAL/index.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/__shows_d3/theatrics/NETWORK_D3_3/methods/PHYSICAL/index.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/__shows_d3/theatrics/NETWORK_D3_3/methods/reinvigorate.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/__shows_d3/theatrics/NETWORK_D3_3/methods/reinvigorate.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/__shows_d3/theatrics/intro/show.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/__shows_d3/theatrics/intro/show.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/__shows_d3/theatrics/net/field.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/__shows_d3/theatrics/net/field.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/cart/decor.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/cart/decor.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/cart/decor.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/cart/decor.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor/composition/decor.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor/composition/decor.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor/composition/decor.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor/composition/decor.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor/composition--/field.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor/composition--/field.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor/composition--/field.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor/composition--/field.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor/product/decor.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor/product/decor.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor/product/decor.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor/product/decor.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor/recommendations/decor.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor/recommendations/decor.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor/references/decor.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor/references/decor.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/decor.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/methods/index.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/food/methods/index.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/goal/room.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/goal/room.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/goal/room.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/goal/room.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/goal/room_v1.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/goal/room_v1.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/goods/cycles/methods.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/goods/cycles/methods.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/goods/decor/food--/decor.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/goods/decor/food--/decor.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/goods/decor/food--/decor.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/goods/decor/food--/decor.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/goods/decor/search_controls/decor.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/goods/decor/search_controls/decor.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/goods/decor/supplement/decor.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/goods/decor/supplement/decor.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/goods/decor/supplement/decor.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/goods/decor/supplement/decor.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/goods/decor.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/goods/decor.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/goods/decor.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/goods/decor.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/habitat/decor.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/habitat/decor.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/habitat/panels/panel_1.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/habitat/panels/panel_1.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/habitat/panels/panel_goodness.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/habitat/panels/panel_goodness.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/habitat/panels/panel_health.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/habitat/panels/panel_health.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/habitat/panels/panel_moon.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/habitat/panels/panel_moon.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/habitat/panels/panel_organic_crop_farming.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/habitat/panels/panel_organic_crop_farming.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/habitat/panels/panel_physics.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/habitat/panels/panel_physics.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/habitat/panels/panel_sink.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/habitat/panels/panel_sink.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/habitat/panels/panel_sink_caution.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/habitat/panels/panel_sink_caution.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/habitat/panels/panel_sloop.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/habitat/panels/panel_sloop.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/habitat/panels/panel_tech.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/habitat/panels/panel_tech.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/map/decor.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/map/decor.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/map/decor.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/map/decor.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor/composition--/field.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor/composition--/field.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor/composition--/field.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor/composition--/field.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor/measured_ingredients/fountains.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor/measured_ingredients/fountains.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor/measured_ingredients/fountains.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor/measured_ingredients/fountains.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor/product/decor.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor/product/decor.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor/product/decor.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor/product/decor.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor/references/decor.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor/references/decor.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor/statements/decor.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor/statements/decor.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor/warnings.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor/warnings.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/decor.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/methods/index.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/regions/guests/supp/methods/index.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/browser_storage/component.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/browser_storage/component.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/button/decor.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/button/decor.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/button/decor.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/button/decor.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/button_3D/decor--.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/button_3D/decor--.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/button_3D/decor--.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/button_3D/decor--.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/button_3D/decor.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/button_3D/decor.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/button_3D/decor.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/button_3D/decor.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/caution-sign/goodestSink-export.svg` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/caution-sign/goodestSink-export.svg`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/caution-sign/scenery.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/caution-sign/scenery.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/change_indicator/indicators/spinner/indicator.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/change_indicator/indicators/spinner/indicator.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/change_indicator/indicators/spinner/indicator.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/change_indicator/indicators/spinner/indicator.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/change_indicator/scenery.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/change_indicator/scenery.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/charts/composition_DAC/chart.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/charts/composition_DAC/chart.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/charts/composition_DAC/methods/PHYSICAL/index.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/charts/composition_DAC/methods/PHYSICAL/index.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/charts/composition_DAC/methods/reinvigorate.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/charts/composition_DAC/methods/reinvigorate.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/charts/composition_waterfall/chart.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/charts/composition_waterfall/chart.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/charts/pie/make/build/data.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/charts/pie/make/build/data.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/charts/pie/make/build/options.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/charts/pie/make/build/options.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/charts/pie/make/build/plugins.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/charts/pie/make/build/plugins.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/charts/pie/make/index.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/charts/pie/make/index.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/charts/pie/make/utilities/--find_value.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/charts/pie/make/utilities/--find_value.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/charts/pie/make/utilities/find_name.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/charts/pie/make/utilities/find_name.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/charts/pie/veranda.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/charts/pie/veranda.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/checkbox/decor.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/checkbox/decor.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/checkbox/decor.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/checkbox/decor.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/curtain/decor.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/curtain/decor.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/curtain/decor.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/curtain/decor.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/example/_status/decor.ST.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/example/_status/decor.ST.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/exception/field.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/exception/field.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/flip/decor--.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/flip/decor--.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/flip/decor.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/flip/decor.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/food_or_supp_summary/decor.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/food_or_supp_summary/decor.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/food_or_supp_summary/decor.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/food_or_supp_summary/decor.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/foundations/eagle/scene.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/foundations/eagle/scene.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/goal/components/goal_amount.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/goal/components/goal_amount.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/goal/decor.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/goal/decor.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/goal/decor.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/goal/decor.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/goal/decor_1.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/goal/decor_1.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/hw_button/decor.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/hw_button/decor.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/hw_button/decor_v1.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/hw_button/decor_v1.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/icons/book/field.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/icons/book/field.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/input/decor.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/input/decor.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/input/decor.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/input/decor.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/link/outer/decor.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/link/outer/decor.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/lounge/decor.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/lounge/decor.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/lounge/decor.s.HTML` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/lounge/decor.s.HTML`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/mascot/craft.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/mascot/craft.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/mascot/craft_v1.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/mascot/craft_v1.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/mascot/mascot-1.svg` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/mascot/mascot-1.svg`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/mascot/mascot.svg` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/mascot/mascot.svg`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/name/_assets/Rugged Vegan.svg` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/name/_assets/Rugged Vegan.svg`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/name/_assets/Vegan Lantern - Export.svg` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/name/_assets/Vegan Lantern - Export.svg`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/name/_assets/goodest sloop - mural - v1.svg` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/name/_assets/goodest sloop - mural - v1.svg`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/name/_assets/goodest sloop - mural - v2.svg` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/name/_assets/goodest sloop - mural - v2.svg`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/name/_assets/goodest sloop - mural - v3.svg` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/name/_assets/goodest sloop - mural - v3.svg`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/name/mural.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/name/mural.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/name/mural_v1.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/name/mural_v1.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/name/mural_v2.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/name/mural_v2.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/name/mural_v3.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/name/mural_v3.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/name/mural_v4.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/name/mural_v4.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/name/mural_v5.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/name/mural_v5.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nature_cautionary_ingredients/shack.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nature_cautionary_ingredients/shack.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nature_cautionary_ingredients/shack.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nature_cautionary_ingredients/shack.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nature_essentials_nutrients/shack.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nature_essentials_nutrients/shack.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nature_essentials_nutrients/shack.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nature_essentials_nutrients/shack.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nature_ingredients_table/components/name.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nature_ingredients_table/components/name.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nature_ingredients_table/fields/methods.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nature_ingredients_table/fields/methods.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nature_ingredients_table/fields/methods_/prepare_columns.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nature_ingredients_table/fields/methods_/prepare_columns.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nature_ingredients_table/fields/methods_/prepare_rows.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nature_ingredients_table/fields/methods_/prepare_rows.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nature_ingredients_table/fountains.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nature_ingredients_table/fountains.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nature_ingredients_table_v1/fountains.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nature_ingredients_table_v1/fountains.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nature_ingredients_table_v1/fountains.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nature_ingredients_table_v1/fountains.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nav_1/decor.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nav_1/decor.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nav_1/navs/mobile_top/field.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nav_1/navs/mobile_top/field.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nav_1/navs/mobile_top/field.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nav_1/navs/mobile_top/field.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nav_1/navs/top/field.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nav_1/navs/top/field.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nav_1/navs/top/field.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nav_1/navs/top/field.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nav_2/decor.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nav_2/decor.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nav_2/decor.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/nav_2/decor.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/navigation infrastructure/methods/awareness/keydown.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/navigation infrastructure/methods/awareness/keydown.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/navigation infrastructure/methods/focus_land_mark.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/navigation infrastructure/methods/focus_land_mark.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/navigation infrastructure/structure.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/navigation infrastructure/structure.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/navigation infrastructure/structure.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/navigation infrastructure/structure.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/panel/decor.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/panel/decor.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/quantity_chooser/decor.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/quantity_chooser/decor.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/quantity_chooser/decor.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/quantity_chooser/decor.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/router_link/decor.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/router_link/decor.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/router_link/decor.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/router_link/decor.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/select/decor.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/select/decor.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/select/decor.status.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/select/decor.status.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/select/decor.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/select/decor.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/struct_2/composition/decor.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/struct_2/composition/decor.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/struct_2/composition/decor.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/struct_2/composition/decor.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/struct_2/composition/furniture/mass_of_quantified_ingredients.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/struct_2/composition/furniture/mass_of_quantified_ingredients.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/struct_2/quantified_grove/fields/methods.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/struct_2/quantified_grove/fields/methods.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/struct_2/quantified_grove/table.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/struct_2/quantified_grove/table.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/struct_2/quantified_grove/table.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/struct_2/quantified_grove/table.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/table/decor.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/table/decor.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/treasure/affiliates/decor.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/treasure/affiliates/decor.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/treasure/goodness_certifications/money.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/scenery/treasure/goodness_certifications/money.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/LICENSE.md` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/LICENSE.md`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/README.md` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/README.md`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/index.html` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/index.html`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/site-assets/images/download-btn.png` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/site-assets/images/download-btn.png`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/site-assets/images/tweet-btn.png` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/site-assets/images/tweet-btn.png`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/svg-loaders/audio.svg` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/svg-loaders/audio.svg`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/svg-loaders/ball-triangle.svg` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/svg-loaders/ball-triangle.svg`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/svg-loaders/bars.svg` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/svg-loaders/bars.svg`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/svg-loaders/circles.svg` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/svg-loaders/circles.svg`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/svg-loaders/grid.svg` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/svg-loaders/grid.svg`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/svg-loaders/hearts.svg` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/svg-loaders/hearts.svg`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/svg-loaders/oval.svg` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/svg-loaders/oval.svg`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/svg-loaders/puff.svg` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/svg-loaders/puff.svg`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/svg-loaders/rings.svg` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/svg-loaders/rings.svg`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/svg-loaders/spinning-circles.svg` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/svg-loaders/spinning-circles.svg`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/svg-loaders/tail-spin.svg` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/svg-loaders/tail-spin.svg`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/svg-loaders/three-dots.svg` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/SVG-Loaders/svg-loaders/three-dots.svg`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/scenery/action/scenery.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/scenery/action/scenery.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/scenery/action/scenery.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/scenery/action/scenery.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/scenery/action/scenery_v1.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/vendor/scenery/action/scenery_v1.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/_research/observables.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/_research/observables.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/cart/_status/1.status.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/cart/_status/1.status.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/cart/_status/2.status.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/cart/_status/2.status.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/cart/_status/3.status.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/cart/_status/3.status.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/cart/_status/4_remove.status.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/cart/_status/4_remove.status.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/cart/index.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/cart/index.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/cart/moves/change_quantity.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/cart/moves/change_quantity.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/cart/moves/find_DSLD_ID.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/cart/moves/find_DSLD_ID.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/cart/moves/find_FDC_ID.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/cart/moves/find_FDC_ID.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/cart/moves/remove.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/cart/moves/remove.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/cart/utilities/retrieve_treasures.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/cart/utilities/retrieve_treasures.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/connections/index.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/connections/index.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/goals/index.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/goals/index.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/homestead/index.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/homestead/index.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/layout/index.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/layout/index.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/storage/index.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/storage/index.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/terrain--/index.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/terrain--/index.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/terrain--/index.s.HTML` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/terrain--/index.s.HTML`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/theme/_status/1.status.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/theme/_status/1.status.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/theme/index.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/theme/index.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/theme/rooms/palettes.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/src/warehouses/theme/rooms/palettes.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/apps/web/vitest.config.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/apps/web/vitest.config.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/bun.lockb` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/bun.lockb`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/find_symlinks.py` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/find_symlinks.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/shares/glamour/background_effects/particles/money.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/shares/glamour/background_effects/particles/money.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/shares/glamour/button/glamour.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/shares/glamour/button/glamour.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/shares/glamour/button/glamour.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/shares/glamour/button/glamour.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/shares/glamour/table/_status/status.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/shares/glamour/table/_status/status.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/shares/glamour/table/decor.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/shares/glamour/table/decor.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/shares/glamour/table/decor.vue` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/shares/glamour/table/decor.vue`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/shares/glamour/table/sorting/as_float.js` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/shares/glamour/table/sorting/as_float.js`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/shares/glamour/table/table.S.HTML` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/shares/glamour/table/table.S.HTML`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/adventures/vv_turbo/sharess/config-typescript/base.json` & `goodest-1.2.2/venues/stages/goodest/adventures/vv_turbo/sharess/config-typescript/base.json`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/deliveries/__pycache__/source.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/deliveries/__pycache__/source.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/deliveries/__pycache__/source.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/deliveries/__pycache__/source.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/deliveries/one/__init__.py` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/deliveries/one/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/deliveries/one/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/deliveries/one/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/deliveries/one/__pycache__/__init__.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/deliveries/one/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/deliveries/one/assertions/__pycache__/BRANDED.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/deliveries/one/assertions/__pycache__/BRANDED.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/deliveries/one/assertions/__pycache__/branded.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/deliveries/one/assertions/__pycache__/branded.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/deliveries/one/assertions/__pycache__/branded.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/deliveries/one/assertions/__pycache__/branded.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/deliveries/one/assertions/__pycache__/foundational.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/deliveries/one/assertions/__pycache__/foundational.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/deliveries/one/status/API_status_foundational_1.py` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/deliveries/one/status/API_status_foundational_1.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/deliveries/one/status/__pycache__/API_status_branded_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/deliveries/one/status/__pycache__/API_status_branded_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/deliveries/one/status/__pycache__/API_status_foundational_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/deliveries/one/status/__pycache__/API_status_foundational_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/examples/__init__.py` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/examples/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/examples/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/examples/__pycache__/__init__.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/examples/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/examples/__pycache__/status_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/examples/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/examples/branded/Gardein_f'sh_2663758.JSON` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/examples/branded/Gardein_f'sh_2663758.JSON`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/examples/branded/Gardein_f'sh_2664238.JSON` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/examples/branded/Gardein_f'sh_2664238.JSON`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/examples/branded/beet_juice_2412474.JSON` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/examples/branded/beet_juice_2412474.JSON`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/examples/branded/beet_juice_2642759.JSON` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/examples/branded/beet_juice_2642759.JSON`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/examples/branded/goodest_pizza_2672996.JSON` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/examples/branded/goodest_pizza_2672996.JSON`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/examples/branded/impossible_beef_2664238.JSON` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/examples/branded/impossible_beef_2664238.JSON`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/examples/branded/problems/impossible_2468423.JSON` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/examples/branded/problems/impossible_2468423.JSON`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/examples/branded/walnuts_1882785.JSON` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/examples/branded/walnuts_1882785.JSON`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/examples/foundational/2346404_sweet_potatoes.JSON` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/examples/foundational/2346404_sweet_potatoes.JSON`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/food.s.HTML` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/food.s.HTML`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/__init__.py` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/__init__.py` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/__pycache__/__init__.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/__pycache__/assertions.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/__pycache__/assertions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/__pycache__/assertions.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/__pycache__/assertions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/__pycache__/status_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/assertions/__init__.py` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/assertions/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/assertions/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/assertions/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/__init__.py` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/__pycache__/__init__.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/__pycache__/status_mass_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/__pycache__/status_mass_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/__pycache__/status_volume_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/__pycache__/status_volume_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/label_splitter/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/label_splitter/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/label_splitter/__pycache__/__init__.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/label_splitter/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/status_mass_1.py` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/status_mass_1.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/status_volume_1.py` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/status_volume_1.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/status_1.py` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_interpret/packageWeight/status_1.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_ops/retrieve/API_status_found_1.py` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_ops/retrieve/API_status_found_1.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_ops/retrieve/API_status_not_found_1.py` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_ops/retrieve/API_status_not_found_1.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_ops/retrieve/__init__.py` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_ops/retrieve/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_ops/retrieve/__pycache__/API_status_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_ops/retrieve/__pycache__/API_status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_ops/retrieve/__pycache__/API_status_found_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_ops/retrieve/__pycache__/API_status_found_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_ops/retrieve/__pycache__/API_status_not_found_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_ops/retrieve/__pycache__/API_status_not_found_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_ops/retrieve/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_ops/retrieve/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_status/__pycache__/status_1_description.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_status/__pycache__/status_1_description.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_status/__pycache__/status_2_measures.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_status/__pycache__/status_2_measures.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_status/__pycache__/status_3_measured_ingredients.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_status/__pycache__/status_3_measured_ingredients.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_status/__pycache__/status_4_land_essentials.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_status/__pycache__/status_4_land_essentials.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_status/__pycache__/status_4_lands.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_status/__pycache__/status_4_lands.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_status/status_1_description.py` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_status/status_1_description.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_status/status_2_measures.py` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_status/status_2_measures.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_status/status_3_measured_ingredients.py` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_status/status_3_measured_ingredients.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_status/status_4_lands.py` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_status/status_4_lands.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_status_v1/__pycache__/status_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_status_v1/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_status_v1/__pycache__/status_2.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_status_v1/__pycache__/status_2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_status_v1/__pycache__/status_2412474.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_status_v1/__pycache__/status_2412474.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_status_v1/__pycache__/status_3.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_status_v1/__pycache__/status_3.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_status_v1/__pycache__/status_loop_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_status_v1/__pycache__/status_loop_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_status_v1/status_1.py` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_status_v1/status_1.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_status_v1/status_2.py` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_status_v1/status_2.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_status_v1/status_2412474.py` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_status_v1/status_2412474.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_status_v1/status_3.py` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_status_v1/status_3.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/_status_v1/status_loop_1.py` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/_status_v1/status_loop_1.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/land/__init__.py` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/land/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/land/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/land/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/__pycache__/__init__.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/_ops/for_each/__init__.py` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/_ops/for_each/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/_ops/for_each/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/_ops/for_each/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/_ops/for_each/__pycache__/__init__.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/_ops/for_each/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/_ops/seek/__init__.py` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/_ops/seek/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/_ops/seek/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/_ops/seek/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/_ops/seek/__pycache__/__init__.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/_ops/seek/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/_ops/seek/__pycache__/status_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/_ops/seek/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/_ops/seek/status_1.py` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/_ops/seek/status_1.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/_status/__pycache__/status_mass_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/_status/__pycache__/status_mass_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/_status/__pycache__/status_volume_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/_status/__pycache__/status_volume_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/_status/status_mass_1.py` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/_status/status_mass_1.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/_status/status_volume_1.py` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/_status/status_volume_1.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured ingredients.S.HTML` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured ingredients.S.HTML`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/__init__.py` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/__pycache__/__init__.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/_status/__pycache__/status_IU_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/_status/__pycache__/status_IU_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/_status/__pycache__/status_energy_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/_status/__pycache__/status_energy_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/_status/__pycache__/status_mass_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/_status/__pycache__/status_mass_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/_status/status_IU_1.py` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/_status/status_IU_1.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/_status/status_energy_1.py` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/_status/status_energy_1.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/_status/status_mass_1.py` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/_status/status_mass_1.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/__init__.py` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/__pycache__/__init__.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/biological_activity/__init__.py` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/biological_activity/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/biological_activity/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/biological_activity/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/biological_activity/__pycache__/__init__.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/biological_activity/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/energy/__init__.py` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/energy/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/energy/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/energy/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/energy/__pycache__/__init__.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/energy/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/mass/__init__.py` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/mass/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/mass/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/mass/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/mass/__pycache__/__init__.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/mass/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/__pycache__/food_nutrient.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/__pycache__/food_nutrient.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/__pycache__/food_nutrient.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/__pycache__/food_nutrient.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/__pycache__/food_nutrient_calculator.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/__pycache__/food_nutrient_calculator.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/__pycache__/label_nutrient.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/__pycache__/label_nutrient.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/__pycache__/label_nutrient.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/__pycache__/label_nutrient.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/__pycache__/label_nutrient_calculator.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/__pycache__/label_nutrient_calculator.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/food_nutrient.py` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/food_nutrient.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/ingredient_prototype_1.r.HTML` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/ingredient_prototype_1.r.HTML`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measures/form/__init__.py` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measures/form/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measures/form/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measures/form/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measures/form/__pycache__/__init__.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measures/form/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measures/form/__pycache__/status_mass_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measures/form/__pycache__/status_mass_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measures/form/__pycache__/status_volume_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measures/form/__pycache__/status_volume_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measures/form/status_mass_1.py` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measures/form/status_mass_1.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/food_USDA/nature_v2/measures/form/status_volume_1.py` & `goodest-1.2.2/venues/stages/goodest/besties/food_USDA/nature_v2/measures/form/status_volume_1.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/NIH.s.HTML` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/NIH.s.HTML`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/deliveries/__pycache__/source.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/deliveries/__pycache__/source.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/deliveries/__pycache__/source.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/deliveries/__pycache__/source.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/deliveries/one/__init__.py` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/deliveries/one/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/deliveries/one/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/deliveries/one/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/deliveries/one/__pycache__/__init__.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/deliveries/one/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/deliveries/one/__pycache__/assertions.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/deliveries/one/__pycache__/assertions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/deliveries/one/__pycache__/assertions.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/deliveries/one/__pycache__/assertions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/deliveries/one/assertions.py` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/deliveries/one/assertions.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/deliveries/one/status/__pycache__/API_status_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/deliveries/one/status/__pycache__/API_status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/examples/__init__.py` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/examples/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/examples/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/examples/__pycache__/__init__.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/examples/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/examples/coated tablets/multivitamin_276336.JSON` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/examples/coated tablets/multivitamin_276336.JSON`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/examples/goodest_capsules/probiotics_248267.JSON` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/examples/goodest_capsules/probiotics_248267.JSON`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/examples/other/chia_seeds_214893.JSON` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/examples/other/chia_seeds_214893.JSON`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/examples/powder/mane_270619.JSON` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/examples/powder/mane_270619.JSON`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/examples/powder/nutritional_shake_220884.JSON` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/examples/powder/nutritional_shake_220884.JSON`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/examples/powder packets/multivitamin_246811.JSON` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/examples/powder packets/multivitamin_246811.JSON`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/examples/tablets/calcium_261967.JSON` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/examples/tablets/calcium_261967.JSON`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/examples/tablets/multivitamin_249664.JSON` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/examples/tablets/multivitamin_249664.JSON`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/__init__.py` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_interpret/ingredientRows/for_each/__init__.py` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_interpret/ingredientRows/for_each/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_interpret/ingredientRows/for_each/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_interpret/ingredientRows/for_each/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_interpret/ingredientRows/for_each/__pycache__/__init__.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_interpret/ingredientRows/for_each/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_interpret/ingredientRows/for_each/__pycache__/status_powder_packets_246811.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_interpret/ingredientRows/for_each/__pycache__/status_powder_packets_246811.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_interpret/ingredientRows/for_each/status_powder_packets_246811.py` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_interpret/ingredientRows/for_each/status_powder_packets_246811.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_ops/retrieve/__init__.py` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_ops/retrieve/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_ops/retrieve/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_ops/retrieve/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/__pycache__/status_1_info.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/__pycache__/status_1_info.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/__pycache__/status_2_form.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/__pycache__/status_2_form.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/__pycache__/status_3_measured_ingredients.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/__pycache__/status_3_measured_ingredients.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/__pycache__/status_4_essential_nutrients.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/__pycache__/status_4_essential_nutrients.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/__pycache__/status_4_unmeasured_ingredients.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/__pycache__/status_4_unmeasured_ingredients.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/__pycache__/status_5_essential_nutrients.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/__pycache__/status_5_essential_nutrients.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/__pycache__/status_6_cautionary_ingredients.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/__pycache__/status_6_cautionary_ingredients.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/mane_270619_nature.JSON` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/mane_270619_nature.JSON`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/multivitamin_249664.JSON` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/multivitamin_249664.JSON`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/status_1_info.py` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/status_1_info.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/status_2_form.py` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/status_2_form.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/status_3_measured_ingredients.py` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/status_3_measured_ingredients.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/status_4_unmeasured_ingredients.py` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/status_4_unmeasured_ingredients.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/status_5_essential_nutrients.py` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/status_5_essential_nutrients.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/status_6_cautionary_ingredients.py` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_status/status_6_cautionary_ingredients.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_status_v1/_loop/__pycache__/status_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_status_v1/_loop/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_status_v1/_loop/status_1.py` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_status_v1/_loop/status_1.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_status_v1/coated_tablets/__pycache__/status_multivitamin_276336.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_status_v1/coated_tablets/__pycache__/status_multivitamin_276336.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_status_v1/coated_tablets/status_multivitamin_276336.py` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_status_v1/coated_tablets/status_multivitamin_276336.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_status_v1/coated_tablets/status_multivitamin_276336_nature.JSON` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_status_v1/coated_tablets/status_multivitamin_276336_nature.JSON`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_status_v1/other/__pycache__/status_chia_seeds_214893.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_status_v1/other/__pycache__/status_chia_seeds_214893.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_status_v1/other/chia_seeds_214893_nature.JSON` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_status_v1/other/chia_seeds_214893_nature.JSON`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_status_v1/other/status_chia_seeds_214893.py` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_status_v1/other/status_chia_seeds_214893.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_status_v1/powder/__pycache__/status_mane_270619.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_status_v1/powder/__pycache__/status_mane_270619.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_status_v1/powder/mane_270619_nature.JSON` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_status_v1/powder/mane_270619_nature.JSON`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/_status_v1/powder/status_mane_270619.py` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/_status_v1/powder/status_mane_270619.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/__pycache__/__init__.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/amount/__init__.py` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/amount/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/amount/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/amount/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/amount/__pycache__/__init__.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/amount/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/amount/__pycache__/status_other_214893.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/amount/__pycache__/status_other_214893.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/amount/status_other_214893.py` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/amount/status_other_214893.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/form.S.HTML` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/form.S.HTML`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/serving_size/amount/__init__.py` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/serving_size/amount/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/serving_size/amount/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/serving_size/amount/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/serving_size/amount/__pycache__/status_246811.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/serving_size/amount/__pycache__/status_246811.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/serving_size/amount/__pycache__/status_276336.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/serving_size/amount/__pycache__/status_276336.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/serving_size/amount/status_246811.py` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/serving_size/amount/status_246811.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/serving_size/amount/status_276336.py` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/serving_size/amount/status_276336.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/__init__.py` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/__pycache__/status_coated_tablet_276336.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/__pycache__/status_coated_tablet_276336.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/__pycache__/status_goodest_capsule_248267.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/__pycache__/status_goodest_capsule_248267.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/__pycache__/status_gram_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/__pycache__/status_gram_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/__pycache__/status_powder_220884.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/__pycache__/status_powder_220884.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/__pycache__/status_powder_270619.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/__pycache__/status_powder_270619.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/__pycache__/status_powder_packets_246811.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/__pycache__/status_powder_packets_246811.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/__pycache__/status_tablet_261967.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/__pycache__/status_tablet_261967.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/status_coated_tablet_276336.py` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/status_coated_tablet_276336.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/status_goodest_capsule_248267.py` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/status_goodest_capsule_248267.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/status_gram_1.py` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/status_gram_1.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/status_powder_220884.py` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/status_powder_220884.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/status_powder_270619.py` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/status_powder_270619.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/status_powder_packets_246811.py` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/status_powder_packets_246811.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/status_tablet_261967.py` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/form/unit/status_tablet_261967.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/land/__init__.py` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/land/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/land/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/land/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/__init__.py` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/__pycache__/__init__.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek/__init__.py` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek/__pycache__/__init__.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek/__pycache__/status_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek/status_1.py` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek/status_1.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek_name/__init__.py` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek_name/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek_name/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek_name/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek_name/__pycache__/__init__.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek_name/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/_status/__pycache__/status_chia_seeds_214893.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/_status/__pycache__/status_chia_seeds_214893.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/_status/status_chia_seeds_214893.py` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/_status/status_chia_seeds_214893.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/measured_ingredient/__init__.py` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/measured_ingredient/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/measured_ingredient/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/measured_ingredient/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/measured_ingredient/__pycache__/__init__.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/measured_ingredient/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/measured_ingredient/_status/__pycache__/status_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/measured_ingredient/_status/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/measured_ingredient/_status/status_1.py` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/measured_ingredient/_status/status_1.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/measured_ingredient/measured_ingredient.S.HTML` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/measured_ingredient/measured_ingredient.S.HTML`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/measured_ingredients.S.HTML` & `goodest-1.2.2/venues/stages/goodest/besties/supp_NIH/nature_v2/measured_ingredients/measured_ingredients.S.HTML`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/goals/umuntu/FDA.py` & `goodest-1.2.2/venues/stages/goodest/goals/umuntu/FDA.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/goals/umuntu/FDA_v1.py` & `goodest-1.2.2/venues/stages/goodest/goals/umuntu/FDA_v1.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/goals/umuntu/FDA_v2.py` & `goodest-1.2.2/venues/stages/goodest/goals/umuntu/FDA_v2.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/goals/umuntu/FDA_v3.py` & `goodest-1.2.2/venues/stages/goodest/goals/umuntu/FDA_v3.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/goals/umuntu/__pycache__/FDA.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/goals/umuntu/__pycache__/FDA.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/goals/umuntu/__pycache__/FDA_v3.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/goals/umuntu/__pycache__/FDA_v3.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/goals/umuntu/_ops/__pycache__/retrieve.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/goals/umuntu/_ops/__pycache__/retrieve.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/goodest.S.HTML` & `goodest-1.2.2/venues/stages/goodest/goodest.S.HTML`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/goodest.css` & `goodest-1.2.2/venues/stages/goodest/goodest.css`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/measures/_interpret/__pycache__/status_unit_kind.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/measures/_interpret/__pycache__/status_unit_kind.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/measures/_interpret/__pycache__/unit_kind.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/measures/_interpret/__pycache__/unit_kind.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/measures/_interpret/__pycache__/unit_kind.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/measures/_interpret/__pycache__/unit_kind.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/measures/_interpret/status_unit_kind.py` & `goodest-1.2.2/venues/stages/goodest/measures/_interpret/status_unit_kind.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/measures/_interpret/unit_kind.py` & `goodest-1.2.2/venues/stages/goodest/measures/_interpret/unit_kind.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/measures/energy/energy.r.HTML` & `goodest-1.2.2/venues/stages/goodest/measures/energy/energy.r.HTML`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/measures/energy/swap/__init__.py` & `goodest-1.2.2/venues/stages/goodest/measures/energy/swap/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/measures/energy/swap/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/measures/energy/swap/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/measures/energy/swap/__pycache__/__init__.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/measures/energy/swap/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/measures/energy/swap/__pycache__/status_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/measures/energy/swap/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/measures/mass/swap/__init__.py` & `goodest-1.2.2/venues/stages/goodest/measures/mass/swap/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/measures/mass/swap/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/measures/mass/swap/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/measures/mass/swap/__pycache__/__init__.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/measures/mass/swap/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/measures/mass/swap/__pycache__/status_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/measures/mass/swap/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/measures/mass/swap/status_1.py` & `goodest-1.2.2/venues/stages/goodest/measures/mass/swap/status_1.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/measures/mass/system international.r.html` & `goodest-1.2.2/venues/stages/goodest/measures/mass/system international.r.html`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/measures/mass/us customary.r.html` & `goodest-1.2.2/venues/stages/goodest/measures/mass/us customary.r.html`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/measures/mass_equivalents/is_an_equivalent/__init__.py` & `goodest-1.2.2/venues/stages/goodest/measures/mass_equivalents/is_an_equivalent/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/measures/mass_equivalents/is_an_equivalent/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/measures/mass_equivalents/is_an_equivalent/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/measures/mass_equivalents/is_an_equivalent/__pycache__/__init__.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/measures/mass_equivalents/is_an_equivalent/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/measures/mass_equivalents/is_an_equivalent/__pycache__/status_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/measures/mass_equivalents/is_an_equivalent/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/measures/mass_equivalents/jargon.r.HTML` & `goodest-1.2.2/venues/stages/goodest/measures/mass_equivalents/jargon.r.HTML`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/measures/mass_equivalents/mass equivalents.r.HTML` & `goodest-1.2.2/venues/stages/goodest/measures/mass_equivalents/mass equivalents.r.HTML`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/measures/number/decimal/reduce/__init__.py` & `goodest-1.2.2/venues/stages/goodest/measures/number/decimal/reduce/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/measures/number/decimal/reduce/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/measures/number/decimal/reduce/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/measures/number/decimal/reduce/__pycache__/__init__.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/measures/number/decimal/reduce/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/measures/number/decimal/reduce/__pycache__/status_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/measures/number/decimal/reduce/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/measures/number/decimal/reduce/__pycache__/status_2.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/measures/number/decimal/reduce/__pycache__/status_2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/measures/number/decimal/reduce/__pycache__/status_3.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/measures/number/decimal/reduce/__pycache__/status_3.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/measures/number/decimal/reduce/__pycache__/status_sci_note_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/measures/number/decimal/reduce/__pycache__/status_sci_note_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/measures/number/decimal/reduce/status_1.py` & `goodest-1.2.2/venues/stages/goodest/measures/number/decimal/reduce/status_1.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/measures/number/decimal/reduce/status_2.py` & `goodest-1.2.2/venues/stages/goodest/measures/number/decimal/reduce/status_2.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/measures/number/decimal/reduce/status_3.py` & `goodest-1.2.2/venues/stages/goodest/measures/number/decimal/reduce/status_3.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/measures/number/integer/__pycache__/status_string_is_integer.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/measures/number/integer/__pycache__/status_string_is_integer.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/measures/number/integer/__pycache__/string_is_integer.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/measures/number/integer/__pycache__/string_is_integer.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/measures/number/integer/__pycache__/string_is_integer.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/measures/number/integer/__pycache__/string_is_integer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/measures/number/integer/status_string_is_integer.py` & `goodest-1.2.2/venues/stages/goodest/measures/number/integer/status_string_is_integer.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/measures/number/percentage/__pycache__/from_fraction.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/measures/number/percentage/__pycache__/from_fraction.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/measures/number/percentage/__pycache__/from_fraction.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/measures/number/percentage/__pycache__/from_fraction.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/measures/number/percentage/__pycache__/status_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/measures/number/percentage/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/measures/number/percentage/from_fraction.py` & `goodest-1.2.2/venues/stages/goodest/measures/number/percentage/from_fraction.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/measures/number/percentage/status_1.py` & `goodest-1.2.2/venues/stages/goodest/measures/number/percentage/status_1.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/measures/number/sci_note/__init__.py` & `goodest-1.2.2/venues/stages/goodest/measures/number/sci_note/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/measures/number/sci_note/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/measures/number/sci_note/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/measures/number/sci_note/_status/__pycache__/status_multiples_of_3_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/measures/number/sci_note/_status/__pycache__/status_multiples_of_3_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/measures/number/sci_note/_status/status_multiples_of_3_1.py` & `goodest-1.2.2/venues/stages/goodest/measures/number/sci_note/_status/status_multiples_of_3_1.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/measures/number/sci_note/sci_note.S.HTML` & `goodest-1.2.2/venues/stages/goodest/measures/number/sci_note/sci_note.S.HTML`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/measures/number/sci_note/sci_note_possibilities.S.HTML` & `goodest-1.2.2/venues/stages/goodest/measures/number/sci_note/sci_note_possibilities.S.HTML`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/measures/number/sci_note/sci_note_thoughts.S.HTML` & `goodest-1.2.2/venues/stages/goodest/measures/number/sci_note/sci_note_thoughts.S.HTML`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/measures/number/sci_note_2/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/measures/number/sci_note_2/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/measures/number/sci_note_2/__pycache__/status_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/measures/number/sci_note_2/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/measures/number/sci_note_2/status_1.py` & `goodest-1.2.2/venues/stages/goodest/measures/number/sci_note_2/status_1.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/measures/volume/swap/__init__.py` & `goodest-1.2.2/venues/stages/goodest/measures/volume/swap/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/measures/volume/swap/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/measures/volume/swap/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/measures/volume/swap/__pycache__/__init__.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/measures/volume/swap/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/measures/volume/swap/__pycache__/status_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/measures/volume/swap/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/measures/volume/swap/status_1.py` & `goodest-1.2.2/venues/stages/goodest/measures/volume/swap/status_1.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/measures/weight/weight.r.html` & `goodest-1.2.2/venues/stages/goodest/measures/weight/weight.r.html`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/mixes/drives/etch/__pycache__/bracket.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/mixes/drives/etch/__pycache__/bracket.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/mixes/insure/__pycache__/equalities.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/mixes/insure/__pycache__/equalities.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/mixes/insure/__pycache__/override_print.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/mixes/insure/__pycache__/override_print.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/mixes/insure/__pycache__/status_equalitites_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/mixes/insure/__pycache__/status_equalitites_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/mixes/insure/equalities.py` & `goodest-1.2.2/venues/stages/goodest/mixes/insure/equalities.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/mixes/insure/override_print.py` & `goodest-1.2.2/venues/stages/goodest/mixes/insure/override_print.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/mixes/procedure/__init__.py` & `goodest-1.2.2/venues/stages/goodest/mixes/procedure/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/mixes/procedure/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/mixes/procedure/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/readme.md` & `goodest-1.2.2/venues/stages/goodest/readme.md`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/goodness_certifications/certifications.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/goodness_certifications/certifications.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/goodness_certifications/goodest.S.HTML` & `goodest-1.2.2/venues/stages/goodest/shows_v2/goodness_certifications/goodest.S.HTML`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/_ops/assertions/__pycache__/ingredient.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/_ops/assertions/__pycache__/ingredient.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/_ops/assertions/ingredient.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/_ops/assertions/ingredient.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/_ops/formulate/__init__.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/_ops/formulate/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/_ops/formulate/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/_ops/formulate/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_empty/__pycache__/status_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_empty/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_empty/status_1.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_empty/status_1.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_food/__pycache__/status_0.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_food/__pycache__/status_0.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_food/__pycache__/status_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_food/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_food/__pycache__/status_2.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_food/__pycache__/status_2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_food/__pycache__/status_3.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_food/__pycache__/status_3.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_food/status_0.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_food/status_0.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_food/status_1.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_food/status_1.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_food/status_2.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_food/status_2.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_food/status_3.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_food/status_3.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_foods_and_supps/__pycache__/status_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_foods_and_supps/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_foods_and_supps/status_1.JSON` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_foods_and_supps/status_1.JSON`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_foods_and_supps/status_1.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_foods_and_supps/status_1.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_rational_amounts/__pycache__/status_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_rational_amounts/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_rational_amounts/status_1.JSON` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_rational_amounts/status_1.JSON`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_rational_amounts/status_1.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_rational_amounts/status_1.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_supp/__pycache__/status_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_supp/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_supp/__pycache__/status_1_supp_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_supp/__pycache__/status_1_supp_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_supp/status_1.JSON` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_supp/status_1.JSON`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_supp/status_1.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_supp/status_1.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_supp/status_1_supp_1.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/_ops/formulate/_status/status_supp/status_1_supp_1.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/_ops/retrieve/__init__.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/_ops/retrieve/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/_ops/retrieve/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/_ops/retrieve/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/_ops/retrieve/_status/API_status_1.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/_ops/retrieve/_status/API_status_1.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/_ops/retrieve/_status/__pycache__/API_status_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/_ops/retrieve/_status/__pycache__/API_status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/land/_ops/formulate/__init__.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/land/_ops/formulate/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe/land/_ops/formulate/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe/land/_ops/formulate/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/__pycache__/formulate.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/__pycache__/formulate.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/for_1_food/__init__.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/for_1_food/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/for_1_food/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/for_1_food/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/for_1_food/_status/__pycache__/status_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/for_1_food/_status/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/for_1_food/_status/status_1.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/for_1_food/_status/status_1.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/for_1_food/_status/status_1_food.JSON` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/for_1_food/_status/status_1_food.JSON`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/for_1_supp/__init__.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/for_1_supp/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/for_1_supp/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/for_1_supp/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/for_1_supp/_status/__pycache__/status_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/for_1_supp/_status/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/for_1_supp/_status/status_1.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/for_1_supp/_status/status_1.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/for_1_supp/_status/status_1_supp.JSON` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/for_1_supp/_status/status_1_supp.JSON`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/__init__.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status/1_2_recipe_preformulated/__pycache__/status_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status/1_2_recipe_preformulated/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status/1_2_recipe_preformulated/status_1.JSON` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status/1_2_recipe_preformulated/status_1.JSON`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status/1_2_recipe_preformulated/status_1.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status/1_2_recipe_preformulated/status_1.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status/1_3_recipe_prefomulated/__pycache__/status_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status/1_3_recipe_prefomulated/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status/1_3_recipe_prefomulated/status_1.JSON` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status/1_3_recipe_prefomulated/status_1.JSON`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status/1_3_recipe_prefomulated/status_1.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status/1_3_recipe_prefomulated/status_1.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status/2_food/__pycache__/status_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status/2_food/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status/2_food/status_1.JSON` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status/2_food/status_1.JSON`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status/2_food/status_1.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status/2_food/status_1.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_1_recipe/API_status_1.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_1_recipe/API_status_1.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_1_recipe/__pycache__/API_status_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_1_recipe/__pycache__/API_status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_1_recipe/__pycache__/status_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_1_recipe/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_1_recipe/status_1.JSON` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_1_recipe/status_1.JSON`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_2_recipe/API_status_1.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_2_recipe/API_status_1.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_2_recipe/__pycache__/API_status_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_2_recipe/__pycache__/API_status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_2_recipe/__pycache__/status_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_2_recipe/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_2_recipe/status_1.JSON` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_2_recipe/status_1.JSON`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status_API/__pycache__/status_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/_status_API/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/modules/__pycache__/add_goals.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/modules/__pycache__/add_goals.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/modules/__pycache__/find_goal.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/modules/__pycache__/find_goal.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/modules/add_goals.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/_ops/formulate/modules/add_goals.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/recipe_with_goals/recipe_with_goals.S.HTML` & `goodest-1.2.2/venues/stages/goodest/shows_v2/recipe_with_goals/recipe_with_goals.S.HTML`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/_assertions/__init__.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/_assertions/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/_assertions/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/_assertions/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/forward_channel/_journal/structures/vitamin a.r.HTML` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/forward_channel/_journal/structures/vitamin a.r.HTML`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/forward_channel/_journal/structures/vitamin b.r.HTML` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/forward_channel/_journal/structures/vitamin b.r.HTML`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/forward_channel/_journal/structures/vitamin d.r.HTML` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/forward_channel/_journal/structures/vitamin d.r.HTML`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/forward_channel/forward channel.s.HTML` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/forward_channel/forward channel.s.HTML`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/forward_channel/structures.s.HTML` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/forward_channel/structures.s.HTML`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/__pycache__/develop.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/__pycache__/develop.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/__init__.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_empty_grove/__pycache__/status_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_empty_grove/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_empty_grove/status_1.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_empty_grove/status_1.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_m_and_meq/__pycache__/status_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_m_and_meq/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_m_and_meq/__pycache__/status_2.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_m_and_meq/__pycache__/status_2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_m_and_meq/status_1.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_m_and_meq/status_1.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_m_and_meq/status_2.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_m_and_meq/status_2.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_m_eq_and_ba/__pycache__/status_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_m_eq_and_ba/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_m_eq_and_ba/status_1.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_m_eq_and_ba/status_1.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/assertions_one/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/assertions_one/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/calculate_portions/__init__.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/calculate_portions/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/calculate_portions/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/calculate_portions/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/cultivate/__init__.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/cultivate/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/cultivate/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/cultivate/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/develop.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/develop.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/measures_sums/__init__.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/measures_sums/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/measures_sums/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/measures_sums/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/measures_sums/__pycache__/status_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/measures_sums/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/multiply_amount/__init__.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/multiply_amount/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/multiply_amount/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/multiply_amount/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/multiply_amount/__pycache__/__init__.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/multiply_amount/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/multiply_amount/__pycache__/status_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/multiply_amount/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/multiply_amount/__pycache__/status_2.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/multiply_amount/__pycache__/status_2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/multiply_amount/__pycache__/status_loop_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/multiply_amount/__pycache__/status_loop_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/multiply_amount/multiply_measures.s.HTML` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/multiply_amount/multiply_measures.s.HTML`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/multiply_amount/status_1.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/multiply_amount/status_1.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/multiply_amount/status_2.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/multiply_amount/status_2.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/multiply_amount/status_loop_1.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/_ops/multiply_amount/status_loop_1.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/assertions/__init__.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/assertions/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/assertions/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/assertions/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/has_uniters/__init__.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/has_uniters/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/has_uniters/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/has_uniters/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/has_uniters/__pycache__/status_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/has_uniters/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/has_uniters/status_1.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/has_uniters/status_1.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/is_story_1/__init__.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/is_story_1/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/is_story_1/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/is_story_1/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/is_story_1/__pycache__/status_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/is_story_1/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/is_story_1/status_1.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/is_story_1/status_1.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/nurture/__init__.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/nurture/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/nurture/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/nurture/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/nurture/__pycache__/status_cautionary.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/nurture/__pycache__/status_cautionary.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/nurture/__pycache__/status_essentials.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/nurture/__pycache__/status_essentials.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/nurture/status_cautionary.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/nurture/status_cautionary.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/nurture/status_essentials.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/nurture/status_essentials.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/seek/__init__.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/seek/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/seek/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/seek/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/seek/__pycache__/status_essentials.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/seek/__pycache__/status_essentials.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/seek/status_essentials.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/seek/status_essentials.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/seek_name_or_accepts/__init__.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/seek_name_or_accepts/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/seek_name_or_accepts/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/seek_name_or_accepts/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/seek_name_or_accepts/__pycache__/status_essentials_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/seek_name_or_accepts/__pycache__/status_essentials_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/seek_name_or_accepts/__pycache__/status_essentials_2.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/seek_name_or_accepts/__pycache__/status_essentials_2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/seek_name_or_accepts/status_essentials_1.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/seek_name_or_accepts/status_essentials_1.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/seek_name_or_accepts/status_essentials_2.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/seek_name_or_accepts/status_essentials_2.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/seek_uniter/__init__.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/seek_uniter/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/seek_uniter/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/seek_uniter/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/seek_uniter/__pycache__/status_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/seek_uniter/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/seek_uniter/status_1.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/_ops/seek_uniter/status_1.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/grove.S.HTML` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/grove.S.HTML`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/grove/unites/unites.S.HTML` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/grove/unites/unites.S.HTML`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/land.S.HTML` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/land.S.HTML`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/measures/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/measures/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/measures/merge/__init__.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/measures/merge/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/measures/merge/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/measures/merge/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/measures/merge/__pycache__/__init__.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/measures/merge/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/measures/merge/__pycache__/status_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/measures/merge/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/measures/merge/__pycache__/status_2.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/measures/merge/__pycache__/status_2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/measures/merge/__pycache__/status_3.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/measures/merge/__pycache__/status_3.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/measures/merge/status_1.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/measures/merge/status_1.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/measures/merge/status_2.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/measures/merge/status_2.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/measures/merge/status_3.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/measures/merge/status_3.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/measures/multiply/__init__.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/measures/multiply/__init__.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/measures/multiply/__pycache__/__init__.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/measures/multiply/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/measures/multiply/__pycache__/__init__.cpython-311.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/measures/multiply/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/measures/multiply/__pycache__/status_1.cpython-310.pyc` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/measures/multiply/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/land/measures/multiply/status_1.py` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/land/measures/multiply/status_1.py`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/measures/measures.S.HTML` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/measures/measures.S.HTML`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/venues/stages/goodest/shows_v2/treasure/nature/nature.S.HTML` & `goodest-1.2.2/venues/stages/goodest/shows_v2/treasure/nature/nature.S.HTML`

 * *Files identical despite different names*

### Comparing `goodest-1.2.1/PKG-INFO` & `goodest-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goodest
-Version: 1.2.1
+Version: 1.2.2
 Summary: goodest vegan health
 License: >1 [Vegan + GPL 3.0 + Non-Commercial]
 Keywords: goodest
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```
