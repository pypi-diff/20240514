# Comparing `tmp/beancount_reds_importers-0.8.0.tar.gz` & `tmp/beancount_reds_importers-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beancount_reds_importers-0.8.0.tar", last modified: Sat Nov 25 07:41:27 2023, max compression
+gzip compressed data, was "beancount_reds_importers-0.9.0.tar", last modified: Tue May 14 08:22:26 2024, max compression
```

## Comparing `beancount_reds_importers-0.8.0.tar` & `beancount_reds_importers-0.9.0.tar`

### file list

```diff
@@ -1,189 +1,217 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 07:41:27.974792 beancount_reds_importers-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)    10816 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/.gitchangelog.rc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 07:41:27.942791 beancount_reds_importers-0.8.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 07:41:27.950791 beancount_reds_importers-0.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/.github/workflows/pythonpackage.yml
--rw-r--r--   0 runner    (1001) docker     (127)      846 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    15107 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       72 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10214 2023-11-25 07:41:27.974792 beancount_reds_importers-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9094 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 07:41:27.950791 beancount_reds_importers-0.8.0/beancount_reds_importers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 07:41:27.954791 beancount_reds_importers-0.8.0/beancount_reds_importers/example/
--rw-r--r--   0 runner    (1001) docker     (127)     2923 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/example/OfxDownload.qfx
--rw-r--r--   0 runner    (1001) docker     (127)       79 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/example/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     1540 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/example/fund_info.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      275 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/example/import.sh
--rw-r--r--   0 runner    (1001) docker     (127)      619 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/example/my-smart.import
--rw-r--r--   0 runner    (1001) docker     (127)      751 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/example/my.beancount
--rw-r--r--   0 runner    (1001) docker     (127)     3503 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/example/my.import
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/example/transactions.qfx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 07:41:27.954791 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 07:41:27.954791 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/ally/
--rw-r--r--   0 runner    (1001) docker     (127)      462 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/ally/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 07:41:27.954791 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/ally/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/ally/tests/ally_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/ally/tests/transactions.qfx
--rw-r--r--   0 runner    (1001) docker     (127)      222 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/ally/tests/transactions.qfx.extract
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/ally/tests/transactions.qfx.file_account
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/ally/tests/transactions.qfx.file_date
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/ally/tests/transactions.qfx.file_name
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 07:41:27.954791 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/amazongc/
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/amazongc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 07:41:27.954791 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/amex/
--rw-r--r--   0 runner    (1001) docker     (127)      468 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/amex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 07:41:27.954791 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/becu/
--rw-r--r--   0 runner    (1001) docker     (127)      476 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/becu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 07:41:27.954791 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/capitalonebank/
--rw-r--r--   0 runner    (1001) docker     (127)      504 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/capitalonebank/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 07:41:27.954791 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/capitalonebank/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/capitalonebank/tests/360Checking.qfx
--rw-r--r--   0 runner    (1001) docker     (127)      437 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/capitalonebank/tests/360Checking.qfx.extract
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/capitalonebank/tests/360Checking.qfx.file_account
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/capitalonebank/tests/360Checking.qfx.file_date
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/capitalonebank/tests/360Checking.qfx.file_name
--rw-r--r--   0 runner    (1001) docker     (127)      419 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/capitalonebank/tests/capitalone_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 07:41:27.954791 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/chase/
--rw-r--r--   0 runner    (1001) docker     (127)      462 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/chase/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 07:41:27.958792 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/citi/
--rw-r--r--   0 runner    (1001) docker     (127)      456 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/citi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 07:41:27.958792 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/discover/
--rw-r--r--   0 runner    (1001) docker     (127)      980 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/discover/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/discover/discover_ofx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 07:41:27.958792 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/etrade/
--rw-r--r--   0 runner    (1001) docker     (127)      555 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/etrade/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 07:41:27.958792 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/etrade/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/etrade/tests/etrade_09092023.QFX
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/etrade/tests/etrade_09092023.QFX.extract
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/etrade/tests/etrade_09092023.QFX.file_account
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/etrade/tests/etrade_09092023.QFX.file_date
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/etrade/tests/etrade_09092023.QFX.file_name
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/etrade/tests/etrade_qfx_brokerage_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 07:41:27.958792 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/fidelity/
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/fidelity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/fidelity/fidelity_cma_csv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 07:41:27.958792 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/fidelity/fidelity_cma_csv_examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2625 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/fidelity/fidelity_cma_csv_examples/History_for_Account_X8YYYYYYY.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)     1016 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/fidelity/fidelity_cma_csv_examples/fidelity-cma-csv.import
--rwxr-xr-x   0 runner    (1001) docker     (127)       71 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/fidelity/fidelity_cma_csv_examples/run_test.bash
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 07:41:27.958792 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/morganstanley/
--rw-r--r--   0 runner    (1001) docker     (127)      467 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/morganstanley/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 07:41:27.958792 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/schwab/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/schwab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/schwab/schwab_csv_balances.py
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/schwab/schwab_csv_brokerage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/schwab/schwab_csv_checking.py
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/schwab/schwab_csv_positions.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/schwab/schwab_ofx_bank_ofx.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/schwab/schwab_ofx_brokerage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 07:41:27.946792 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/schwab/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 07:41:27.962792 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/schwab/tests/schwab_csv_brokerage/
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/schwab/tests/schwab_csv_brokerage/schwab_csv_brokerage_Transactions_123.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/schwab/tests/schwab_csv_brokerage/schwab_csv_brokerage_Transactions_123.csv.extract
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/schwab/tests/schwab_csv_brokerage/schwab_csv_brokerage_Transactions_123.csv.file_account
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/schwab/tests/schwab_csv_brokerage/schwab_csv_brokerage_Transactions_123.csv.file_date
--rw-r--r--   0 runner    (1001) docker     (127)       42 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/schwab/tests/schwab_csv_brokerage/schwab_csv_brokerage_Transactions_123.csv.file_name
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/schwab/tests/schwab_csv_brokerage/schwab_csv_brokerage_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 07:41:27.962792 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/schwab/tests/schwab_csv_checking/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/schwab/tests/schwab_csv_checking/schwab_Checking_Transactions_1234.csv
--rw-r--r--   0 runner    (1001) docker     (127)      362 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/schwab/tests/schwab_csv_checking/schwab_Checking_Transactions_1234.csv.extract
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/schwab/tests/schwab_csv_checking/schwab_Checking_Transactions_1234.csv.file_account
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/schwab/tests/schwab_csv_checking/schwab_Checking_Transactions_1234.csv.file_date
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/schwab/tests/schwab_csv_checking/schwab_Checking_Transactions_1234.csv.file_name
--rw-r--r--   0 runner    (1001) docker     (127)      491 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/schwab/tests/schwab_csv_checking/schwab_csv_checking_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 07:41:27.962792 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/stanchart/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/stanchart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2878 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/stanchart/scbbank.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/stanchart/scbcard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 07:41:27.962792 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/target/
--rw-r--r--   0 runner    (1001) docker     (127)      478 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/target/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 07:41:27.962792 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/tdameritrade/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/tdameritrade/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 07:41:27.962792 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/techcubank/
--rw-r--r--   0 runner    (1001) docker     (127)      494 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/techcubank/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 07:41:27.962792 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/unitedoverseas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/unitedoverseas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 07:41:27.966792 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/unitedoverseas/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    26112 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/unitedoverseas/tests/ACC_TXN_History_1234_clean.xls
--rw-r--r--   0 runner    (1001) docker     (127)      727 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/unitedoverseas/tests/ACC_TXN_History_1234_clean.xls.extract
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/unitedoverseas/tests/ACC_TXN_History_1234_clean.xls.file_account
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/unitedoverseas/tests/ACC_TXN_History_1234_clean.xls.file_date
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/unitedoverseas/tests/ACC_TXN_History_1234_clean.xls.file_name
--rw-r--r--   0 runner    (1001) docker     (127)      464 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/unitedoverseas/tests/uobbank_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/unitedoverseas/uobbank.py
--rw-r--r--   0 runner    (1001) docker     (127)     3246 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/unitedoverseas/uobcard.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/unitedoverseas/uobsrs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 07:41:27.966792 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/vanguard/
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/vanguard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 07:41:27.966792 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/vanguard/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6819 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/vanguard/tests/OfxDownload-401k.qfx
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/vanguard/tests/OfxDownload-401k.qfx.extract
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/vanguard/tests/OfxDownload-401k.qfx.file_account
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/vanguard/tests/OfxDownload-401k.qfx.file_date
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/vanguard/tests/OfxDownload-401k.qfx.file_name
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/vanguard/tests/vanguard_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/vanguard/vanguard_screenscrape.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 07:41:27.966792 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/workday/
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/importers/workday/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 07:41:27.966792 beancount_reds_importers-0.8.0/beancount_reds_importers/libreader/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/libreader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3263 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/libreader/csv_multitable_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    10169 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/libreader/csvreader.py
--rw-r--r--   0 runner    (1001) docker     (127)     7806 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/libreader/ofxreader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/libreader/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 07:41:27.946792 beancount_reds_importers-0.8.0/beancount_reds_importers/libreader/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 07:41:27.946792 beancount_reds_importers-0.8.0/beancount_reds_importers/libreader/tests/balance_assertion_date/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 07:41:27.970792 beancount_reds_importers-0.8.0/beancount_reds_importers/libreader/tests/balance_assertion_date/last_transaction/
--rw-r--r--   0 runner    (1001) docker     (127)      426 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/libreader/tests/balance_assertion_date/last_transaction/last_transaction_date_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/libreader/tests/balance_assertion_date/last_transaction/transactions.qfx
--rw-r--r--   0 runner    (1001) docker     (127)      222 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/libreader/tests/balance_assertion_date/last_transaction/transactions.qfx.extract
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/libreader/tests/balance_assertion_date/last_transaction/transactions.qfx.file_account
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/libreader/tests/balance_assertion_date/last_transaction/transactions.qfx.file_date
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/libreader/tests/balance_assertion_date/last_transaction/transactions.qfx.file_name
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 07:41:27.970792 beancount_reds_importers-0.8.0/beancount_reds_importers/libreader/tests/balance_assertion_date/ofx_date/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/libreader/tests/balance_assertion_date/ofx_date/ofx_date_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/libreader/tests/balance_assertion_date/ofx_date/transactions.qfx
--rw-r--r--   0 runner    (1001) docker     (127)      222 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/libreader/tests/balance_assertion_date/ofx_date/transactions.qfx.extract
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/libreader/tests/balance_assertion_date/ofx_date/transactions.qfx.file_account
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/libreader/tests/balance_assertion_date/ofx_date/transactions.qfx.file_date
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/libreader/tests/balance_assertion_date/ofx_date/transactions.qfx.file_name
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 07:41:27.970792 beancount_reds_importers-0.8.0/beancount_reds_importers/libreader/tests/balance_assertion_date/smart/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/libreader/tests/balance_assertion_date/smart/smart_date_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/libreader/tests/balance_assertion_date/smart/transactions.qfx
--rw-r--r--   0 runner    (1001) docker     (127)      222 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/libreader/tests/balance_assertion_date/smart/transactions.qfx.extract
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/libreader/tests/balance_assertion_date/smart/transactions.qfx.file_account
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/libreader/tests/balance_assertion_date/smart/transactions.qfx.file_date
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/libreader/tests/balance_assertion_date/smart/transactions.qfx.file_name
--rw-r--r--   0 runner    (1001) docker     (127)      430 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/libreader/tsvreader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/libreader/xlsreader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/libreader/xlsx_multitable_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/libreader/xlsxreader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 07:41:27.970792 beancount_reds_importers-0.8.0/beancount_reds_importers/libtransactionbuilder/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/libtransactionbuilder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6275 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/libtransactionbuilder/banking.py
--rw-r--r--   0 runner    (1001) docker     (127)     3380 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/libtransactionbuilder/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    21874 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/libtransactionbuilder/investments.py
--rw-r--r--   0 runner    (1001) docker     (127)     5322 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/libtransactionbuilder/paycheck.py
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/libtransactionbuilder/transactionbuilder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 07:41:27.970792 beancount_reds_importers-0.8.0/beancount_reds_importers/util/
--rwxr-xr-x   0 runner    (1001) docker     (127)     6203 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/util/bean_download.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6794 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/util/needs_update.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3589 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/util/ofx_summarize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/beancount_reds_importers/util/template.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 07:41:27.970792 beancount_reds_importers-0.8.0/beancount_reds_importers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10214 2023-11-25 07:41:27.000000 beancount_reds_importers-0.8.0/beancount_reds_importers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9720 2023-11-25 07:41:27.000000 beancount_reds_importers-0.8.0/beancount_reds_importers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-25 07:41:27.000000 beancount_reds_importers-0.8.0/beancount_reds_importers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      152 2023-11-25 07:41:27.000000 beancount_reds_importers-0.8.0/beancount_reds_importers.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-25 07:41:27.000000 beancount_reds_importers-0.8.0/beancount_reds_importers.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      137 2023-11-25 07:41:27.000000 beancount_reds_importers-0.8.0/beancount_reds_importers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-11-25 07:41:27.000000 beancount_reds_importers-0.8.0/beancount_reds_importers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      228 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-25 07:41:27.974792 beancount_reds_importers-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2023-11-25 07:41:16.000000 beancount_reds_importers-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:26.496137 beancount_reds_importers-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    10816 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/.gitchangelog.rc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:26.456137 beancount_reds_importers-0.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:26.464137 beancount_reds_importers-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/.github/workflows/conventionalcommits.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/.github/workflows/pythonpackage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    16597 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10574 2024-05-14 08:22:26.496137 beancount_reds_importers-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9294 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:26.464137 beancount_reds_importers-0.9.0/beancount_reds_importers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:26.468137 beancount_reds_importers-0.9.0/beancount_reds_importers/example/
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/example/OfxDownload.qfx
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/example/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1530 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/example/fund_info.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      275 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/example/import.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/example/my-smart.import
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/example/my.beancount
+-rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/example/my.import
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/example/transactions.qfx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:26.468137 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:26.468137 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/alliant/
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/alliant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:26.468137 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/ally/
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/ally/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:26.472137 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/ally/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/ally/tests/ally_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/ally/tests/transactions.qfx
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/ally/tests/transactions.qfx.extract
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/ally/tests/transactions.qfx.file_account
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/ally/tests/transactions.qfx.file_date
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/ally/tests/transactions.qfx.file_name
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:26.472137 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/amazongc/
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/amazongc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:26.472137 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/amex/
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/amex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:26.472137 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/bamboohr/
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/bamboohr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:26.472137 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/becu/
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/becu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:26.472137 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/capitalonebank/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/capitalonebank/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:26.472137 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/capitalonebank/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/capitalonebank/tests/360Checking.qfx
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/capitalonebank/tests/360Checking.qfx.extract
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/capitalonebank/tests/360Checking.qfx.file_account
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/capitalonebank/tests/360Checking.qfx.file_date
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/capitalonebank/tests/360Checking.qfx.file_name
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/capitalonebank/tests/capitalone_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:26.472137 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/chase/
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/chase/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:26.472137 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/citi/
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/citi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:26.472137 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/dcu/
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/dcu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:26.472137 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/dcu/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/dcu/tests/Main_Checking_Account_Transactions.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/dcu/tests/Main_Checking_Account_Transactions.csv.extract
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/dcu/tests/Main_Checking_Account_Transactions.csv.file_account
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/dcu/tests/Main_Checking_Account_Transactions.csv.file_date
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/dcu/tests/Main_Checking_Account_Transactions.csv.file_name
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/dcu/tests/dcu_csv_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:26.476137 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/discover/
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/discover/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/discover/discover_ofx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:26.476137 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/etrade/
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/etrade/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:26.476137 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/etrade/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/etrade/tests/etrade_09092023.QFX
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/etrade/tests/etrade_09092023.QFX.extract
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/etrade/tests/etrade_09092023.QFX.file_account
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/etrade/tests/etrade_09092023.QFX.file_date
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/etrade/tests/etrade_09092023.QFX.file_name
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/etrade/tests/etrade_qfx_brokerage_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:26.476137 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/fidelity/
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/fidelity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/fidelity/fidelity_cma_csv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:26.476137 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/fidelity/fidelity_cma_csv_examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/fidelity/fidelity_cma_csv_examples/History_for_Account_X8YYYYYYY.csv
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1016 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/fidelity/fidelity_cma_csv_examples/fidelity-cma-csv.import
+-rwxr-xr-x   0 runner    (1001) docker     (127)       71 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/fidelity/fidelity_cma_csv_examples/run_test.bash
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:26.476137 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/genericpdf/
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/genericpdf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:26.476137 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/genericpdf/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/genericpdf/tests/genericpdf_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49181 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/genericpdf/tests/paystub.sample.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/genericpdf/tests/paystub.sample.pdf.extract
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/genericpdf/tests/paystub.sample.pdf.file_account
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/genericpdf/tests/paystub.sample.pdf.file_date
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/genericpdf/tests/paystub.sample.pdf.file_name
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:26.476137 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/morganstanley/
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/morganstanley/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:26.480137 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/schwab/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/schwab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/schwab/schwab_csv_balances.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/schwab/schwab_csv_brokerage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/schwab/schwab_csv_checking.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/schwab/schwab_csv_creditline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/schwab/schwab_csv_positions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/schwab/schwab_json_brokerage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/schwab/schwab_ofx_bank_ofx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/schwab/schwab_ofx_brokerage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:26.460137 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/schwab/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:26.480137 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/schwab/tests/schwab_csv_brokerage/
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/schwab/tests/schwab_csv_brokerage/schwab_csv_brokerage_XX876_Transactions_20220731.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/schwab/tests/schwab_csv_brokerage/schwab_csv_brokerage_XX876_Transactions_20220731.csv.extract
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/schwab/tests/schwab_csv_brokerage/schwab_csv_brokerage_XX876_Transactions_20220731.csv.file_account
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/schwab/tests/schwab_csv_brokerage/schwab_csv_brokerage_XX876_Transactions_20220731.csv.file_date
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/schwab/tests/schwab_csv_brokerage/schwab_csv_brokerage_XX876_Transactions_20220731.csv.file_name
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/schwab/tests/schwab_csv_brokerage/schwab_csv_brokerage_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:26.480137 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/schwab/tests/schwab_csv_checking/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/schwab/tests/schwab_csv_checking/schwab_XXX234_Checking_Transactions_20220203.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/schwab/tests/schwab_csv_checking/schwab_XXX234_Checking_Transactions_20220203.csv.extract
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/schwab/tests/schwab_csv_checking/schwab_XXX234_Checking_Transactions_20220203.csv.file_account
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/schwab/tests/schwab_csv_checking/schwab_XXX234_Checking_Transactions_20220203.csv.file_date
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/schwab/tests/schwab_csv_checking/schwab_XXX234_Checking_Transactions_20220203.csv.file_name
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/schwab/tests/schwab_csv_checking/schwab_csv_checking_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:26.484137 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/stanchart/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/stanchart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/stanchart/scbbank.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/stanchart/scbcard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:26.484137 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/target/
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/target/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:26.484137 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/tdameritrade/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/tdameritrade/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:26.484137 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/techcubank/
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/techcubank/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:26.484137 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/unitedoverseas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/unitedoverseas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:26.484137 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/unitedoverseas/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    26112 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/unitedoverseas/tests/ACC_TXN_History_1234_clean.xls
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/unitedoverseas/tests/ACC_TXN_History_1234_clean.xls.extract
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/unitedoverseas/tests/ACC_TXN_History_1234_clean.xls.file_account
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/unitedoverseas/tests/ACC_TXN_History_1234_clean.xls.file_date
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/unitedoverseas/tests/ACC_TXN_History_1234_clean.xls.file_name
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/unitedoverseas/tests/uobbank_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/unitedoverseas/uobbank.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/unitedoverseas/uobcard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/unitedoverseas/uobsrs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:26.484137 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/vanguard/
+-rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/vanguard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:26.488137 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/vanguard/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6819 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/vanguard/tests/OfxDownload-401k.qfx
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/vanguard/tests/OfxDownload-401k.qfx.extract
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/vanguard/tests/OfxDownload-401k.qfx.file_account
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/vanguard/tests/OfxDownload-401k.qfx.file_date
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/vanguard/tests/OfxDownload-401k.qfx.file_name
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/vanguard/tests/vanguard_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/vanguard/vanguard_screenscrape.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:26.488137 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/workday/
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/importers/workday/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:26.488137 beancount_reds_importers-0.9.0/beancount_reds_importers/libreader/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/libreader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/libreader/csv_multitable_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10342 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/libreader/csvreader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/libreader/jsonreader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7756 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/libreader/ofxreader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8927 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/libreader/pdfreader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/libreader/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:26.464137 beancount_reds_importers-0.9.0/beancount_reds_importers/libreader/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:26.464137 beancount_reds_importers-0.9.0/beancount_reds_importers/libreader/tests/balance_assertion_date/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:26.488137 beancount_reds_importers-0.9.0/beancount_reds_importers/libreader/tests/balance_assertion_date/last_transaction/
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/libreader/tests/balance_assertion_date/last_transaction/last_transaction_date_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/libreader/tests/balance_assertion_date/last_transaction/transactions.qfx
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/libreader/tests/balance_assertion_date/last_transaction/transactions.qfx.extract
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/libreader/tests/balance_assertion_date/last_transaction/transactions.qfx.file_account
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/libreader/tests/balance_assertion_date/last_transaction/transactions.qfx.file_date
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/libreader/tests/balance_assertion_date/last_transaction/transactions.qfx.file_name
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:26.492137 beancount_reds_importers-0.9.0/beancount_reds_importers/libreader/tests/balance_assertion_date/ofx_date/
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/libreader/tests/balance_assertion_date/ofx_date/ofx_date_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/libreader/tests/balance_assertion_date/ofx_date/transactions.qfx
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/libreader/tests/balance_assertion_date/ofx_date/transactions.qfx.extract
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/libreader/tests/balance_assertion_date/ofx_date/transactions.qfx.file_account
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/libreader/tests/balance_assertion_date/ofx_date/transactions.qfx.file_date
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/libreader/tests/balance_assertion_date/ofx_date/transactions.qfx.file_name
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:26.492137 beancount_reds_importers-0.9.0/beancount_reds_importers/libreader/tests/balance_assertion_date/smart/
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/libreader/tests/balance_assertion_date/smart/smart_date_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/libreader/tests/balance_assertion_date/smart/transactions.qfx
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/libreader/tests/balance_assertion_date/smart/transactions.qfx.extract
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/libreader/tests/balance_assertion_date/smart/transactions.qfx.file_account
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/libreader/tests/balance_assertion_date/smart/transactions.qfx.file_date
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/libreader/tests/balance_assertion_date/smart/transactions.qfx.file_name
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/libreader/tsvreader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/libreader/xlsreader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/libreader/xlsx_multitable_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/libreader/xlsxreader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:26.492137 beancount_reds_importers-0.9.0/beancount_reds_importers/libtransactionbuilder/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/libtransactionbuilder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5977 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/libtransactionbuilder/banking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/libtransactionbuilder/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22824 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/libtransactionbuilder/investments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5784 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/libtransactionbuilder/paycheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/libtransactionbuilder/transactionbuilder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:26.492137 beancount_reds_importers-0.9.0/beancount_reds_importers/util/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6261 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/util/bean_download.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6872 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/util/needs_update.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3865 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/util/ofx_summarize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/beancount_reds_importers/util/template.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:26.492137 beancount_reds_importers-0.9.0/beancount_reds_importers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10574 2024-05-14 08:22:26.000000 beancount_reds_importers-0.9.0/beancount_reds_importers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11327 2024-05-14 08:22:26.000000 beancount_reds_importers-0.9.0/beancount_reds_importers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 08:22:26.000000 beancount_reds_importers-0.9.0/beancount_reds_importers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-14 08:22:26.000000 beancount_reds_importers-0.9.0/beancount_reds_importers.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 08:22:26.000000 beancount_reds_importers-0.9.0/beancount_reds_importers.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-14 08:22:26.000000 beancount_reds_importers-0.9.0/beancount_reds_importers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-14 08:22:26.000000 beancount_reds_importers-0.9.0/beancount_reds_importers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 08:22:26.496137 beancount_reds_importers-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-14 08:22:13.000000 beancount_reds_importers-0.9.0/setup.py
```

### Comparing `beancount_reds_importers-0.8.0/.gitchangelog.rc` & `beancount_reds_importers-0.9.0/.gitchangelog.rc`

 * *Files identical despite different names*

### Comparing `beancount_reds_importers-0.8.0/.github/workflows/pythonpackage.yml` & `beancount_reds_importers-0.9.0/.github/workflows/pythonpackage.yml`

 * *Files 18% similar despite different names*

```diff
@@ -4,36 +4,38 @@
 name: Python package
 
 on:
   push:
     branches: [ main ]
   pull_request:
     branches: [ main ]
+    types: [opened, reopened, edited]
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["3.8", "3.9", "3.10"]
+        python-version: ["3.11"]
 
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v3
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        python -m pip install flake8 pytest
-        if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
-    - name: Lint with flake8
+        python -m pip install -e .[dev] -r requirements.txt
+    - name: Lint with ruff
       run: |
-        # stop the build if there are Python syntax errors or undefined names
-        # flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
-        flake8 . --count --max-complexity=14 --max-line-length=127 --show-source --statistics
-    # - name: Test with pytest
-    #   run: |
-    #     pytest
+        ruff check . --statistics
+    - name: Test with pytest
+      run: |
+        pytest
+    - name: Check formatting is applied
+      run: |
+        ruff format --check
+        isort --profile black --check .
```

### Comparing `beancount_reds_importers-0.8.0/.github/workflows/pythonpublish.yml` & `beancount_reds_importers-0.9.0/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `beancount_reds_importers-0.8.0/.gitignore` & `beancount_reds_importers-0.9.0/.gitignore`

 * *Files 0% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 .cache
 nosetests.xml
 coverage.xml
 *.cover
 *.py,cover
 .hypothesis/
 .pytest_cache/
+.debug-*
 
 # Translations
 *.mo
 *.pot
 
 # Django stuff:
 *.log
```

### Comparing `beancount_reds_importers-0.8.0/CHANGELOG.md` & `beancount_reds_importers-0.9.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,52 @@
 # Changelog
 
-## (unreleased)
+## 0.9.0 (2024-05-14)
+
+### New Features
+
+- add genericpdf paycheck importer. [Ammon Sarver]
+- add bamboohr paycheck importer. [Ammon Sarver]
+- add pdfreader libreader importer. [Ammon Sarver]
+- minor: add 'show_configured' in paycheck transaction builder. [Red S]
+
+### New Importers
+- add CSV importer for Digital Credit Union (#89) [Harlan Lieberman-Berg]
+- add importer for Alliant Federal Credit Union (#88) [Harlan Lieberman-Berg]
+- add schwab csv credit line importer. [Red S]
+
+### Improvements
+
+- minor: add_custom_postings to banking.py. [Red S]
+- minor: add identification based on filename to schwab importers. [Red S]
+- minor: overridable add_custom_postings() [Red S]
+- minor: add tdameritrade to template.cfg. [Red S]
+
+
+### Fixes
+
+- update requirements to add back lost packages. [Ammon Sarver]
+- schwab_csv_creditline balance sign. [Red S]
+- add file encoding support to csvreader. [Ad Timmering]
+- only emit filing account metadata if configured #97. [Red S]
+- one-file-per-account broke with smart_importer #97. [Red S]
+- timestamp issue in balance assertions. [Red S]
+- balance date on test. [Red S]
+- schwab tests. [Red S]
+- schwab doesn't use a header in their csv any more. [Red S]
+- schwab_csv_checking format changed #91. [Red S]
+
+### Other
+- enforce formatting with ruff. [Rane Brown]
+- format with isort, use pyproject.toml. [Rane Brown]
+- switch to ruff for linting (#90) [Harlan Lieberman-Berg]
+- style: reformat to 99 col width (previously 88 col) [Red S]
+
+
+## 0.8.0 (2023-11-24)
 
 
 ### Improvements
 
 - Handle the INVEXPENSE field (#79) [Jacob Farkas]
   * Handle the INVEXPENSE field
   * Rename the 'expenses' property to 'invexpense' to match the OFX tag
```

### Comparing `beancount_reds_importers-0.8.0/LICENSE` & `beancount_reds_importers-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `beancount_reds_importers-0.8.0/PKG-INFO` & `beancount_reds_importers-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beancount_reds_importers
-Version: 0.8.0
+Version: 0.9.0
 Summary: Importers for various institutions for Beancount
 Home-page: https://github.com/redstreet/beancount_reds_importers
 Author: Red Street
 Author-email: redstreet@users.noreply.github.com
 License: GPL-3.0
 Keywords: importer ingestor beancount accounting
 Classifier: Development Status :: 4 - Beta
@@ -16,20 +16,25 @@
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Click>=7.0
 Requires-Dist: beancount>=2.3.5
 Requires-Dist: click_aliases>=1.0.1
+Requires-Dist: dateparser>=1.2.0
 Requires-Dist: ofxparse>=0.21
 Requires-Dist: openpyxl>=3.0.9
 Requires-Dist: packaging>=20.3
+Requires-Dist: pdfplumber>=0.11.0
 Requires-Dist: petl>=1.7.4
 Requires-Dist: tabulate>=0.8.9
 Requires-Dist: tqdm>=4.64.0
+Provides-Extra: dev
+Requires-Dist: ruff; extra == "dev"
+Requires-Dist: isort; extra == "dev"
 
 # Beancount Red's Importers
 
 Simple importers and tools for [Beancount](https://beancount.github.io/), software for
 [plain text](https://plaintextaccounting.org/), double entry bookkeeping. _More
 importantly, a framework to allow you to easily write your own importers._
 
@@ -158,16 +163,20 @@
 - `last_transaction`: max transaction date
 - `today`:            today's date
 
 If you want something else, simply override this method in individual importer
 
 `smart` dates: Banks and credit cards typically have pending transactions that are not
 included in downloads. When we download the next statement, new transactions may appear
-prior to the balance assertion date that we generate for this statement. To attempt to
-avoid this, we set the balance assertion date to either two days (fudge factor to
+prior to the balance assertion date that we generate for this statement, which renders
+this balance assertion invalid. This problem manifests occasionally as an existing
+balance statement breaking  when a new statement is downloaded and is an annoyance as it
+needs manual fixing.
+
+To minimize this, we set the balance assertion date to either two days (fudge factor to
 account for pending transactions) before the statement's end date or the last
 transaction's date, whichever is later. To choose a different fudge factor, simply set
 `balance_assertion_date_fudge` in your config.
 
 
 ### Note
```

### Comparing `beancount_reds_importers-0.8.0/README.md` & `beancount_reds_importers-0.9.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -129,16 +129,20 @@
 - `last_transaction`: max transaction date
 - `today`:            today's date
 
 If you want something else, simply override this method in individual importer
 
 `smart` dates: Banks and credit cards typically have pending transactions that are not
 included in downloads. When we download the next statement, new transactions may appear
-prior to the balance assertion date that we generate for this statement. To attempt to
-avoid this, we set the balance assertion date to either two days (fudge factor to
+prior to the balance assertion date that we generate for this statement, which renders
+this balance assertion invalid. This problem manifests occasionally as an existing
+balance statement breaking  when a new statement is downloaded and is an annoyance as it
+needs manual fixing.
+
+To minimize this, we set the balance assertion date to either two days (fudge factor to
 account for pending transactions) before the statement's end date or the last
 transaction's date, whichever is later. To choose a different fudge factor, simply set
 `balance_assertion_date_fudge` in your config.
 
 
 ### Note
```

### Comparing `beancount_reds_importers-0.8.0/beancount_reds_importers/example/OfxDownload.qfx` & `beancount_reds_importers-0.9.0/beancount_reds_importers/example/OfxDownload.qfx`

 * *Files identical despite different names*

### Comparing `beancount_reds_importers-0.8.0/beancount_reds_importers/example/fund_info.py` & `beancount_reds_importers-0.9.0/beancount_reds_importers/example/fund_info.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 # A site that has CUSIP info for "securities traded on the NYSE, NYSE Arca, NYSE Amex, Nasdaq, OTCBB and the
 # Pink Sheets" is here:
 # https://www.quantumonline.com/search.cfm
 # Note it wouldn't list VMFXX in the example below since that is a money market fund, nor would it list
 # mutual funds since those are brokerage specific.
 
 fund_data = [
- ('SCHF',   '808524805', 'Schwab International Equity ETF'),
- ('VGTEST', '012345678', 'Vanguard Test Fund'),
- ('VMFXX',  '922906300', 'Vanguard Federal Money Market Fund'),
+    ("SCHF", "808524805", "Schwab International Equity ETF"),
+    ("VGTEST", "012345678", "Vanguard Test Fund"),
+    ("VMFXX", "922906300", "Vanguard Federal Money Market Fund"),
 ]
 
 # list of money_market accounts. These will not be held at cost, and instead will use price conversions
-money_market = ['VMFXX']
+money_market = ["VMFXX"]
 
 fund_info = {
-        'fund_data': fund_data,
-        'money_market': money_market,
-        }
+    "fund_data": fund_data,
+    "money_market": money_market,
+}
```

### Comparing `beancount_reds_importers-0.8.0/beancount_reds_importers/example/my.beancount` & `beancount_reds_importers-0.9.0/beancount_reds_importers/example/my.beancount`

 * *Files identical despite different names*

### Comparing `beancount_reds_importers-0.8.0/beancount_reds_importers/example/my.import` & `beancount_reds_importers-0.9.0/beancount_reds_importers/example/my.import`

 * *Files 0% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 """Import configuration."""
 
 import sys
 from os import path
 
 sys.path.insert(0, path.join(path.dirname(__file__)))
 
+from fund_info import *
+
 from beancount_reds_importers.importers import vanguard
 from beancount_reds_importers.importers.schwab import schwab_csv_brokerage
-from fund_info import *
+
 # For a better solution for fund_info, see: https://reds-rants.netlify.app/personal-finance/tickers-and-identifiers/
 
 # Setting this variable provides a list of importer instances.
 CONFIG = [
 
     # Investments
     # --------------------------------------------------------------------------------------
```

### Comparing `beancount_reds_importers-0.8.0/beancount_reds_importers/example/transactions.qfx` & `beancount_reds_importers-0.9.0/beancount_reds_importers/example/transactions.qfx`

 * *Files identical despite different names*

### Comparing `beancount_reds_importers-0.8.0/beancount_reds_importers/importers/ally/tests/transactions.qfx` & `beancount_reds_importers-0.9.0/beancount_reds_importers/importers/ally/tests/transactions.qfx`

 * *Files identical despite different names*

### Comparing `beancount_reds_importers-0.8.0/beancount_reds_importers/importers/amazongc/__init__.py` & `beancount_reds_importers-0.9.0/beancount_reds_importers/importers/amazongc/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -19,64 +19,73 @@
     })
 
 """
 
 import datetime
 import itertools
 import ntpath
+
 from beancount.core import data
-from beancount.ingest import importer
 from beancount.core.number import D
+from beancount.ingest import importer
 
 # account flow                          ingest source
 # ----------------------------------------------------
 # credit_card -> amazon_purchases       credit card
 # gift_card   -> amazon_purchases       amazon account
 # amazon_purchases -> expenses          amazon account
 
 
 class Importer(importer.ImporterProtocol):
     def __init__(self, config):
         self.config = config
-        self.currency = self.config.get('currency', 'CURRENCY_NOT_CONFIGURED')
-        self.filename_pattern_def = 'amazon-gift-card.tsv'
+        self.currency = self.config.get("currency", "CURRENCY_NOT_CONFIGURED")
+        self.filename_pattern_def = "amazon-gift-card.tsv"
 
     def identify(self, file):
         return self.filename_pattern_def in file.name
 
     def file_name(self, file):
-        return '{}'.format(ntpath.basename(file.name))
+        return "{}".format(ntpath.basename(file.name))
 
     def file_account(self, _):
-        return self.config['main_account']
+        return self.config["main_account"]
 
     def file_date(self, file):
         "Get the maximum date from the file."
         maxdate = datetime.date.min
-        for line in open(file.name, 'r').readlines()[1:]:
-            f = line.split('\t')
+        for line in open(file.name, "r").readlines()[1:]:
+            f = line.split("\t")
             f = [i.strip() for i in f]
-            date = datetime.datetime.strptime(f[0], '%B %d, %Y').date()
+            date = datetime.datetime.strptime(f[0], "%B %d, %Y").date()
             maxdate = max(date, maxdate)
         return maxdate
 
     def extract(self, file, existing_entries=None):
         config = self.config
 
         new_entries = []
 
         counter = itertools.count()
-        for line in open(file.name, 'r').readlines()[1:]:
-            f = line.split('\t')
+        for line in open(file.name, "r").readlines()[1:]:
+            f = line.split("\t")
             f = [i.strip() for i in f]
-            date = datetime.datetime.strptime(f[0], '%B %d, %Y').date()
+            date = datetime.datetime.strptime(f[0], "%B %d, %Y").date()
             description = f[1].encode("ascii", "ignore").decode()
-            number = D(f[2].replace('$', ''))
+            number = D(f[2].replace("$", ""))
 
             metadata = data.new_metadata(file.name, next(counter))
-            entry = data.Transaction(metadata, date, self.FLAG,
-                                     None, description, data.EMPTY_SET, data.EMPTY_SET, [])
-            data.create_simple_posting(entry, config['main_account'], number, self.currency)
-            data.create_simple_posting(entry, config['target_account'], None, None)
+            entry = data.Transaction(
+                metadata,
+                date,
+                self.FLAG,
+                None,
+                description,
+                data.EMPTY_SET,
+                data.EMPTY_SET,
+                [],
+            )
+            data.create_simple_posting(entry, config["main_account"], number, self.currency)
+            data.create_simple_posting(entry, config["target_account"], None, None)
             new_entries.append(entry)
 
         return new_entries
```

### Comparing `beancount_reds_importers-0.8.0/beancount_reds_importers/importers/capitalonebank/tests/360Checking.qfx` & `beancount_reds_importers-0.9.0/beancount_reds_importers/importers/capitalonebank/tests/360Checking.qfx`

 * *Files identical despite different names*

### Comparing `beancount_reds_importers-0.8.0/beancount_reds_importers/importers/discover/__init__.py` & `beancount_reds_importers-0.9.0/beancount_reds_importers/importers/discover/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-""" Discover credit card .csv importer."""
+"""Discover credit card .csv importer."""
 
 from beancount_reds_importers.libreader import csvreader
 from beancount_reds_importers.libtransactionbuilder import banking
 
 
 class Importer(csvreader.Importer, banking.Importer):
     IMPORTER_NAME = """ Discover credit card .csv importer."""
 
     def custom_init(self):
         self.max_rounding_error = 0.04
-        self.filename_pattern_def = 'Discover.*'
-        self.header_identifier = 'Trans. Date,Post Date,Description,Amount,Category'
-        self.date_format = '%m/%d/%Y'
+        self.filename_pattern_def = "Discover.*"
+        self.header_identifier = "Trans. Date,Post Date,Description,Amount,Category"
+        self.date_format = "%m/%d/%Y"
+        # fmt: off
         self.header_map = {
-            "Category":    'payee',
-            "Description": 'memo',
-            "Trans. Date": 'date',
-            "Post Date":   'postDate',
-            "Amount":      'amount',
-            }
+            "Category":     "payee",
+            "Description":  "memo",
+            "Trans. Date":  "date",
+            "Post Date":    "postDate",
+            "Amount":       "amount",
+        }
+        # fmt: on
 
     def skip_transaction(self, ot):
         return False
 
     def prepare_processed_table(self, rdr):
         # Need to invert numbers supplied by Discover
-        rdr = rdr.convert('amount', lambda x: -1 * x)
+        rdr = rdr.convert("amount", lambda x: -1 * x)
         return rdr
```

### Comparing `beancount_reds_importers-0.8.0/beancount_reds_importers/importers/etrade/__init__.py` & `beancount_reds_importers-0.9.0/beancount_reds_importers/importers/etrade/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-""" ETrade Brokerage ofx importer."""
+"""ETrade Brokerage ofx importer."""
 
 from beancount_reds_importers.libreader import ofxreader
 from beancount_reds_importers.libtransactionbuilder import investments
 
 
 class Importer(investments.Importer, ofxreader.Importer):
-    IMPORTER_NAME = 'ETrade Brokerage OFX'
+    IMPORTER_NAME = "ETrade Brokerage OFX"
 
     def custom_init(self):
         self.max_rounding_error = 0.11
-        self.filename_pattern_def = '.*etrade'
+        self.filename_pattern_def = ".*etrade"
         self.get_ticker_info = self.get_ticker_info_from_id
 
     def skip_transaction(self, ot):
-        if 'JNL' in ot.memo:
+        if "JNL" in ot.memo:
             return True
         return False
```

### Comparing `beancount_reds_importers-0.8.0/beancount_reds_importers/importers/etrade/tests/etrade_09092023.QFX` & `beancount_reds_importers-0.9.0/beancount_reds_importers/importers/etrade/tests/etrade_09092023.QFX`

 * *Files identical despite different names*

### Comparing `beancount_reds_importers-0.8.0/beancount_reds_importers/importers/etrade/tests/etrade_09092023.QFX.extract` & `beancount_reds_importers-0.9.0/beancount_reds_importers/importers/etrade/tests/etrade_09092023.QFX.extract`

 * *Files identical despite different names*

### Comparing `beancount_reds_importers-0.8.0/beancount_reds_importers/importers/etrade/tests/etrade_qfx_brokerage_test.py` & `beancount_reds_importers-0.9.0/beancount_reds_importers/importers/schwab/tests/schwab_csv_brokerage/schwab_csv_brokerage_test.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,54 +1,52 @@
 # flake8: noqa
 
 from os import path
+
 from beancount.ingest import regression_pytest as regtest
-from beancount_reds_importers.importers import etrade
 
+from beancount_reds_importers.importers.schwab import schwab_csv_brokerage
 
 fund_data = [
- ('TSM', '874039100', 'Taiwan Semiconductor Mfg LTD'),
- ('VISA', '92826C839', 'Visa Inc'),
+    ("SWVXX", "123", "SCHWAB VALUE ADVANTAGE MONEY INV"),
+    ("GIS", "456", "GENERAL MILLS INC"),
+    ("BND", "789", "Vanguard Total Bond Market Index Fund"),
 ]
 
 # list of money_market accounts. These will not be held at cost, and instead will use price conversions
-money_market = ['VMFXX']
+money_market = ["VMFXX"]
 
 fund_info = {
-        'fund_data': fund_data,
-        'money_market': money_market,
-        }
+    "fund_data": fund_data,
+    "money_market": money_market,
+}
 
 
 def build_config():
-    acct = "Assets:Investments:Etrade"
-    root = 'Investments'
-    taxability = 'Taxable'
-    leaf = 'Etrade'
-    currency = 'USD'
+    acct = "Assets:Investments:Schwab"
+    root = "Investments"
+    taxability = "Taxable"
+    leaf = "Schwab"
+    currency = "USD"
     config = {
-        'account_number' : '555555555',
-        'main_account'   : acct + ':{ticker}',
-        'cash_account'   : f'{acct}:{{currency}}',
-        'transfer'       : 'Assets:Zero-Sum-Accounts:Transfers:Bank-Account',
-        'dividends'      : f'Income:{root}:{taxability}:Dividends:{leaf}:{{ticker}}',
-        'interest'       : f'Income:{root}:{taxability}:Interest:{leaf}:{{ticker}}',
-        'cg'             : f'Income:{root}:{taxability}:Capital-Gains:{leaf}:{{ticker}}',
-        'capgainsd_lt'   : f'Income:{root}:{taxability}:Capital-Gains-Distributions:Long:{leaf}:{{ticker}}',
-        'capgainsd_st'   : f'Income:{root}:{taxability}:Capital-Gains-Distributions:Short:{leaf}:{{ticker}}',
-        'fees'           : f'Expenses:Fees-and-Charges:Brokerage-Fees:{taxability}:{leaf}',
-        'invexpense'     : f'Expenses:Expenses:Investment-Expenses:{taxability}:{leaf}',
-        'rounding_error' : 'Equity:Rounding-Errors:Imports',
-        'fund_info'      : fund_info,
-        'currency'       : currency,
+        "account_number": "9876",
+        "main_account": acct + ":{ticker}",
+        "cash_account": f"{acct}:{{currency}}",
+        "transfer": "Assets:Zero-Sum-Accounts:Transfers:Bank-Account",
+        "dividends": f"Income:{root}:{taxability}:Dividends:{leaf}:{{ticker}}",
+        "interest": f"Income:{root}:{taxability}:Interest:{leaf}:{{ticker}}",
+        "cg": f"Income:{root}:{taxability}:Capital-Gains:{leaf}:{{ticker}}",
+        "capgainsd_lt": f"Income:{root}:{taxability}:Capital-Gains-Distributions:Long:{leaf}:{{ticker}}",
+        "capgainsd_st": f"Income:{root}:{taxability}:Capital-Gains-Distributions:Short:{leaf}:{{ticker}}",
+        "fees": f"Expenses:Fees-and-Charges:Brokerage-Fees:{taxability}:{leaf}",
+        "invexpense": f"Expenses:Expenses:Investment-Expenses:{taxability}:{leaf}",
+        "rounding_error": "Equity:Rounding-Errors:Imports",
+        "fund_info": fund_info,
+        "currency": currency,
     }
     return config
 
 
-@regtest.with_importer(
-    etrade.Importer(
-        build_config()
-    )
-)
+@regtest.with_importer(schwab_csv_brokerage.Importer(build_config()))
 @regtest.with_testdir(path.dirname(__file__))
-class TestEtradeQFX(regtest.ImporterTestBase):
+class TestSchwabBrokerage(regtest.ImporterTestBase):
     pass
```

### Comparing `beancount_reds_importers-0.8.0/beancount_reds_importers/importers/fidelity/__init__.py` & `beancount_reds_importers-0.9.0/beancount_reds_importers/importers/fidelity/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 """Fidelity Net Benefits and Fidelity Investments OFX importer."""
 
 import ntpath
+
 from beancount_reds_importers.libreader import ofxreader
 from beancount_reds_importers.libtransactionbuilder import investments
 
 
 class Importer(investments.Importer, ofxreader.Importer):
-    IMPORTER_NAME = 'Fidelity Net Benefits / Fidelity Investments OFX'
+    IMPORTER_NAME = "Fidelity Net Benefits / Fidelity Investments OFX"
 
     def custom_init(self):
         self.max_rounding_error = 0.18
-        self.filename_pattern_def = '.*fidelity'
+        self.filename_pattern_def = ".*fidelity"
         self.get_ticker_info = self.get_ticker_info_from_id
-        self.get_payee = lambda ot: ot.memo.split(";", 1)[0] if ';' in ot.memo else ot.memo
+        self.get_payee = lambda ot: ot.memo.split(";", 1)[0] if ";" in ot.memo else ot.memo
 
     def security_narration(self, ot):
         ticker, ticker_long_name = self.get_ticker_info(ot.security)
         return f"[{ticker}]"
 
     def file_name(self, file):
-        return 'fidelity-{}-{}'.format(self.config['account_number'], ntpath.basename(file.name))
+        return "fidelity-{}-{}".format(self.config["account_number"], ntpath.basename(file.name))
 
     def get_target_acct_custom(self, transaction, ticker=None):
         if transaction.memo.startswith("CONTRIBUTION"):
-            return self.config['transfer']
+            return self.config["transfer"]
         if transaction.memo.startswith("FEES"):
-            return self.config['fees']
+            return self.config["fees"]
         return None
 
     def get_available_cash(self, settlement_fund_balance=0):
-        return getattr(self.ofx_account.statement, 'available_cash', None)
+        return getattr(self.ofx_account.statement, "available_cash", None)
```

### Comparing `beancount_reds_importers-0.8.0/beancount_reds_importers/importers/fidelity/fidelity_cma_csv_examples/History_for_Account_X8YYYYYYY.csv` & `beancount_reds_importers-0.9.0/beancount_reds_importers/importers/fidelity/fidelity_cma_csv_examples/History_for_Account_X8YYYYYYY.csv`

 * *Files identical despite different names*

### Comparing `beancount_reds_importers-0.8.0/beancount_reds_importers/importers/fidelity/fidelity_cma_csv_examples/fidelity-cma-csv.import` & `beancount_reds_importers-0.9.0/beancount_reds_importers/importers/fidelity/fidelity_cma_csv_examples/fidelity-cma-csv.import`

 * *Files identical despite different names*

### Comparing `beancount_reds_importers-0.8.0/beancount_reds_importers/importers/schwab/schwab_csv_balances.py` & `beancount_reds_importers-0.9.0/beancount_reds_importers/importers/schwab/schwab_csv_balances.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,68 +1,73 @@
-""" Schwab csv importer."""
+"""Schwab csv importer."""
 
 import datetime
 import re
+
 from beancount.core.number import D
+
 from beancount_reds_importers.libreader import csv_multitable_reader
 from beancount_reds_importers.libtransactionbuilder import investments
 
 
 class Importer(investments.Importer, csv_multitable_reader.Importer):
-    IMPORTER_NAME = 'Schwab Brokerage Balances CSV'
+    IMPORTER_NAME = "Schwab Brokerage Balances CSV"
 
     def custom_init(self):
         self.max_rounding_error = 0.04
-        self.filename_pattern_def = '.*_Balances_'
-        self.header_identifier = 'Balances  for account'
+        self.filename_pattern_def = ".*_Balances_"
+        self.header_identifier = "Balances  for account"
         self.get_ticker_info = self.get_ticker_info_from_id
-        self.date_format = '%m/%d/%Y'
-        self.funds_db_txt = 'funds_by_ticker'
+        self.date_format = "%m/%d/%Y"
+        self.funds_db_txt = "funds_by_ticker"
+        # fmt: off
         self.header_map = {
-            "Description": 'memo',
-            "Symbol":      'security',
-            "Quantity":    'units',
-            "Price":       'unit_price',
-            }
+            "Description":  "memo",
+            "Symbol":       "security",
+            "Quantity":     "units",
+            "Price":        "unit_price",
+        }
+        # fmt: on
 
     def prepare_table(self, rdr):
         return rdr
 
     def convert_columns(self, rdr):
         # fixup decimals
-        decimals = ['units']
+        decimals = ["units"]
         for i in decimals:
             rdr = rdr.convert(i, D)
 
         # fixup currencies
         def remove_non_numeric(x):
-            return re.sub(r'[^0-9\.]', "", x)  # noqa: W605
-        currencies = ['unit_price']
+            return re.sub(r"[^0-9\.]", "", x)  # noqa: W605
+
+        currencies = ["unit_price"]
         for i in currencies:
             rdr = rdr.convert(i, remove_non_numeric)
             rdr = rdr.convert(i, D)
 
         return rdr
 
     def file_date(self, file):
         return self.date.date()
 
     def get_max_transaction_date(self):
         return self.date.date()
 
     def prepare_tables(self):
         # first row has date
-        d = self.raw_rdr[0][0].rsplit(' ', 1)[1]
+        d = self.raw_rdr[0][0].rsplit(" ", 1)[1]
         self.date = datetime.datetime.strptime(d, self.date_format)
 
         for section, table in self.alltables.items():
-            if section in self.config['section_headers']:
+            if section in self.config["section_headers"]:
                 table = table.rename(self.header_map)
                 table = self.convert_columns(table)
-                table = table.cut('memo', 'security', 'units', 'unit_price')
-                table = table.selectne('memo', '--')  # we don't need total rows
-                table = table.addfield('date', self.date)
+                table = table.cut("memo", "security", "units", "unit_price")
+                table = table.selectne("memo", "--")  # we don't need total rows
+                table = table.addfield("date", self.date)
                 self.alltables[section] = table
 
     def get_balance_positions(self):
-        for section in self.config['section_headers']:
+        for section in self.config["section_headers"]:
             yield from self.alltables[section].namedtuples()
```

### Comparing `beancount_reds_importers-0.8.0/beancount_reds_importers/importers/schwab/schwab_csv_checking.py` & `beancount_reds_importers-0.9.0/beancount_reds_importers/importers/stanchart/scbbank.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,80 @@
-""" Schwab Checking .csv importer."""
+"""SCB Banking .csv importer."""
+
+import re
+
+from beancount.core.number import D
 
 from beancount_reds_importers.libreader import csvreader
 from beancount_reds_importers.libtransactionbuilder import banking
 
 
 class Importer(csvreader.Importer, banking.Importer):
-    IMPORTER_NAME = 'Schwab Checking account CSV'
+    IMPORTER_NAME = "SCB Banking Account CSV"
 
     def custom_init(self):
         self.max_rounding_error = 0.04
-        self.filename_pattern_def = '.*_Checking_Transactions_'
-        self.header_identifier = '"Transactions  for Checking account.*'
-        self.column_labels_line = '"Date","Type","Check #","Description","Withdrawal (-)","Deposit (+)","RunningBalance"'
-        self.date_format = '%m/%d/%Y'
-        self.skip_comments = '# '
+        self.filename_pattern_def = "AccountTransactions[0-9]*"
+        self.header_identifier = self.config.get("custom_header", "Account transactions shown:")
+        self.column_labels_line = (
+            "Date,Transaction,Currency,Deposit,Withdrawal,Running Balance,SGD Equivalent Balance"
+        )
+        self.balance_column_labels_line = (
+            "Account Name,Account Number,Currency,Current Balance,Available Balance"
+        )
+        self.date_format = "%d/%m/%Y"
+        self.skip_tail_rows = 0
+        self.skip_comments = "# "
+        # fmt: off
         self.header_map = {
-            "Date":           "date",
-            "Type":           "type",
-            "Check #":        "checknum",
-            "Description":    "payee",
-            "Withdrawal (-)": "withdrawal",
-            "Deposit (+)":    "deposit",
-            "RunningBalance": "balance"
+            "Date":                     "date",
+            "Transaction":              "payee",
+            "Currency":                 "currency",
+            "Withdrawal":               "withdrawal",
+            "Deposit":                  "deposit",
+            "Running Balance":          "balance_running",
+            "SGD Equivalent Balance":   "balance",
         }
-        self.transaction_type_map = {
-            "INTADJUST": 'income',
-            "TRANSFER": 'transfer',
-            "ACH": 'transfer'
-        }
-        self.skip_transaction_types = ['Journal']
+        # fmt: on
+        self.transaction_type_map = {}
+        self.skip_transaction_types = []
+
+    def deep_identify(self, file):
+        account_number = self.config.get("account_number", "")
+        return re.match(self.header_identifier, file.head()) and account_number in file.head()
 
+    # TODO: move into utils, since this is probably a common operation
     def prepare_table(self, rdr):
-        if self.config.get('include_pending', False):
-            rows_to_remove = ['Pending Transactions', 'Posted Transactions', 'Total Pending Check']
-            rdr = rdr.select(lambda x: not any(x[0].startswith(i) for i in rows_to_remove))
-            # TODO: this doesn't work with generating balance assertions: pending transactions
-            # don't include balance assertion data. So what we need to do is generate a balance
-            # assertion at the end of posted transactions. This has not yet been done.
-        else:
-            # There are two sub-tables: pending and posted transactions. Skip pending transactions
-            rdr = self.skip_until_row_contains(rdr, "Posted Transactions")
-
-        rdr = rdr.addfield('amount',
-                           lambda x: "-" + x['Withdrawal (-)'] if x['Withdrawal (-)'] != '' else x['Deposit (+)'])
-        rdr = rdr.addfield('memo', lambda x: '')
+        rdr = rdr.addfield(
+            "amount",
+            lambda x: "-" + x["Withdrawal"] if x["Withdrawal"] != "" else x["Deposit"],
+        )
+        rdr = rdr.addfield("memo", lambda x: "")
+        return rdr
+
+    def prepare_raw_file(self, rdr):
+        # Strip tabs and spaces around each field in the entire file
+        rdr = rdr.convertall(lambda x: x.strip(" \t") if isinstance(x, str) else x)
+
         return rdr
 
     def get_balance_statement(self, file=None):
         """Return the balance on the first and last dates"""
-
         date = self.get_balance_assertion_date()
         if date:
-            yield banking.Balance(date, self.rdr.namedtuples()[0].balance, self.currency)
+            rdr = self.read_raw(file)
+            rdr = self.prepare_raw_file(rdr)
+            col_labels = self.balance_column_labels_line.split(",")
+            rdr = self.extract_table_with_header(rdr, col_labels)
+
+            header_map = {k: k.replace(" ", "_") for k in col_labels}
+            rdr = rdr.rename(header_map)
+
+            while "" in rdr.header():
+                rdr = rdr.cutout("")
+
+            row = rdr.namedtuples()[0]
+            amount = row.Current_Balance
+            units, debitcredit = amount.split()
+            if debitcredit != "CR":
+                units = "-" + units
+            yield banking.Balance(date, D(units), row.Currency)
```

### Comparing `beancount_reds_importers-0.8.0/beancount_reds_importers/importers/schwab/schwab_csv_positions.py` & `beancount_reds_importers-0.9.0/beancount_reds_importers/importers/schwab/schwab_csv_positions.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,47 +1,52 @@
-""" Schwab CSV Positions importer.
+"""Schwab CSV Positions importer.
 
 Note: Schwab "Positions" CSV is not the same as Schwab "Balances" CSV."""
 
 import datetime
 import re
+
 from beancount.core.number import D
+
 from beancount_reds_importers.libreader import csvreader
 from beancount_reds_importers.libtransactionbuilder import investments
 
 
 class Importer(investments.Importer, csvreader.Importer):
     IMPORTER_NAME = "Schwab Brokerage Positions CSV"
 
     def custom_init(self):
         self.max_rounding_error = 0.04
-        self.filename_pattern_def = '.*-Positions-'
+        self.filename_pattern_def = ".*-Positions-"
         self.header_identifier = '["]+Positions for account'
         self.get_ticker_info = self.get_ticker_info_from_id
-        self.date_format = '%Y/%m/%d'
-        self.funds_db_txt = 'funds_by_ticker'
+        self.date_format = "%Y/%m/%d"
+        self.funds_db_txt = "funds_by_ticker"
         self.column_labels_line = '"Symbol","Description","Quantity","Price","Price Change %","Price Change $","Market Value","Day Change %","Day Change $","Cost Basis","Gain/Loss %","Gain/Loss $","Ratings","Reinvest Dividends?","Capital Gains?","% Of Account","Security Type"'  # noqa: #501
+        # fmt: off
         self.header_map = {
-            "Description": 'memo',
-            "Symbol":      'security',
-            "Quantity":    'units',
-            "Price":       'unit_price',
-            }
+            "Description":  "memo",
+            "Symbol":       "security",
+            "Quantity":     "units",
+            "Price":        "unit_price",
+        }
+        # fmt: on
         self.skip_transaction_types = []
 
     def convert_columns(self, rdr):
         # fixup decimals
-        decimals = ['units']
+        decimals = ["units"]
         for i in decimals:
             rdr = rdr.convert(i, D)
 
         # fixup currencies
         def remove_non_numeric(x):
-            return re.sub(r'[^0-9\.]', "", x)  # noqa: W605
-        currencies = ['unit_price']
+            return re.sub(r"[^0-9\.]", "", x)  # noqa: W605
+
+        currencies = ["unit_price"]
         for i in currencies:
             rdr = rdr.convert(i, remove_non_numeric)
             rdr = rdr.convert(i, D)
 
         return rdr
 
     def file_date(self, file):
@@ -49,24 +54,24 @@
         return self.date.date()
 
     def get_max_transaction_date(self):
         return self.date.date()
 
     def prepare_raw_file(self, rdr):
         # first row has date
-        d = rdr[0][0].rsplit(' ', 1)[1]
+        d = rdr[0][0].rsplit(" ", 1)[1]
         self.date = datetime.datetime.strptime(d, self.date_format)
         return rdr
 
     def get_transactions(self):
         """No transactions, this is a file with positions only (balance positions)"""
         return []
 
     def prepare_table(self, rdr):
         # Delete uninteresting columns
         rdr = rdr.cut(list(self.header_map.keys()))
         return rdr
 
     def get_balance_positions(self):
         for pos in self.rdr.namedtuples():
-            if pos.memo != '--':
+            if pos.memo != "--":
                 yield pos
```

### Comparing `beancount_reds_importers-0.8.0/beancount_reds_importers/importers/schwab/tests/schwab_csv_brokerage/schwab_csv_brokerage_Transactions_123.csv` & `beancount_reds_importers-0.9.0/beancount_reds_importers/importers/schwab/tests/schwab_csv_brokerage/schwab_csv_brokerage_XX876_Transactions_20220731.csv`

 * *Files identical despite different names*

### Comparing `beancount_reds_importers-0.8.0/beancount_reds_importers/importers/schwab/tests/schwab_csv_brokerage/schwab_csv_brokerage_Transactions_123.csv.extract` & `beancount_reds_importers-0.9.0/beancount_reds_importers/importers/schwab/tests/schwab_csv_brokerage/schwab_csv_brokerage_XX876_Transactions_20220731.csv.extract`

 * *Files 12% similar despite different names*

```diff
@@ -25,16 +25,24 @@
 
 2023-04-17 * "Bank Interest" "income"
   Assets:Investments:Schwab:USD                    0.03 USD
   Income:Investments:Taxable:Interest:Schwab:USD  -0.03 USD
 
 2023-04-18 * "Sell" "[BND] Vanguard Total Bond Market Index Fund"
   todo: "TODO: this entry is incomplete until lots are selected (bean-doctor context <filename> <lineno>)"
-  Assets:Investments:Schwab:BND                              -10.065 BND {} @ 73.4049 USD
+  Assets:Investments:Schwab:BND                      -10.065 BND {} @ 73.4049 USD
   Income:Investments:Taxable:Capital-Gains:Schwab:BND
   Assets:Investments:Schwab:USD                               738.81 USD
-  Equity:Rounding-Errors:Imports                           0.0103185 USD
+  Equity:Rounding-Errors:Imports                                                   0.0103185 USD
   Expenses:Fees-and-Charges:Brokerage-Fees:Taxable:Schwab       0.01 USD
 
+2023-04-20 * "Journal" "cash"
+  Assets:Investments:Schwab:USD                                  -7461.72 USD
+  Assets:Zero-Sum-Accounts:Transfers:Bank-Account                 7461.72 USD
+
 2023-04-27 * "Buy" "[BND] Vanguard Total Bond Market Index Fund"
   Assets:Investments:Schwab:BND        45 BND {73.7789 USD}
   Assets:Investments:Schwab:USD  -3320.05 USD
+
+2023-04-27 * "Journal" "cash"
+  Assets:Investments:Schwab:USD                                   7461.72 USD
+  Assets:Zero-Sum-Accounts:Transfers:Bank-Account                -7461.72 USD
```

### Comparing `beancount_reds_importers-0.8.0/beancount_reds_importers/importers/schwab/tests/schwab_csv_brokerage/schwab_csv_brokerage_test.py` & `beancount_reds_importers-0.9.0/beancount_reds_importers/importers/etrade/tests/etrade_qfx_brokerage_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,51 @@
 # flake8: noqa
 
 from os import path
+
 from beancount.ingest import regression_pytest as regtest
-from beancount_reds_importers.importers.schwab import schwab_csv_brokerage
 
+from beancount_reds_importers.importers import etrade
 
 fund_data = [
- ('SWVXX', '123', 'SCHWAB VALUE ADVANTAGE MONEY INV'),
- ('GIS',   '456', 'GENERAL MILLS INC'),
- ('BND',   '789', 'Vanguard Total Bond Market Index Fund'),
+    ("TSM", "874039100", "Taiwan Semiconductor Mfg LTD"),
+    ("VISA", "92826C839", "Visa Inc"),
 ]
 
 # list of money_market accounts. These will not be held at cost, and instead will use price conversions
-money_market = ['VMFXX']
+money_market = ["VMFXX"]
 
 fund_info = {
-        'fund_data': fund_data,
-        'money_market': money_market,
-        }
+    "fund_data": fund_data,
+    "money_market": money_market,
+}
 
 
 def build_config():
-    acct = "Assets:Investments:Schwab"
-    root = 'Investments'
-    taxability = 'Taxable'
-    leaf = 'Schwab'
-    currency = 'USD'
+    acct = "Assets:Investments:Etrade"
+    root = "Investments"
+    taxability = "Taxable"
+    leaf = "Etrade"
+    currency = "USD"
     config = {
-        'account_number' : 9876,
-        'main_account'   : acct + ':{ticker}',
-        'cash_account'   : f'{acct}:{{currency}}',
-        'transfer'       : 'Assets:Zero-Sum-Accounts:Transfers:Bank-Account',
-        'dividends'      : f'Income:{root}:{taxability}:Dividends:{leaf}:{{ticker}}',
-        'interest'       : f'Income:{root}:{taxability}:Interest:{leaf}:{{ticker}}',
-        'cg'             : f'Income:{root}:{taxability}:Capital-Gains:{leaf}:{{ticker}}',
-        'capgainsd_lt'   : f'Income:{root}:{taxability}:Capital-Gains-Distributions:Long:{leaf}:{{ticker}}',
-        'capgainsd_st'   : f'Income:{root}:{taxability}:Capital-Gains-Distributions:Short:{leaf}:{{ticker}}',
-        'fees'           : f'Expenses:Fees-and-Charges:Brokerage-Fees:{taxability}:{leaf}',
-        'invexpense'     : f'Expenses:Expenses:Investment-Expenses:{taxability}:{leaf}',
-        'rounding_error' : 'Equity:Rounding-Errors:Imports',
-        'fund_info'      : fund_info,
-        'currency'       : currency,
+        "account_number": "555555555",
+        "main_account": acct + ":{ticker}",
+        "cash_account": f"{acct}:{{currency}}",
+        "transfer": "Assets:Zero-Sum-Accounts:Transfers:Bank-Account",
+        "dividends": f"Income:{root}:{taxability}:Dividends:{leaf}:{{ticker}}",
+        "interest": f"Income:{root}:{taxability}:Interest:{leaf}:{{ticker}}",
+        "cg": f"Income:{root}:{taxability}:Capital-Gains:{leaf}:{{ticker}}",
+        "capgainsd_lt": f"Income:{root}:{taxability}:Capital-Gains-Distributions:Long:{leaf}:{{ticker}}",
+        "capgainsd_st": f"Income:{root}:{taxability}:Capital-Gains-Distributions:Short:{leaf}:{{ticker}}",
+        "fees": f"Expenses:Fees-and-Charges:Brokerage-Fees:{taxability}:{leaf}",
+        "invexpense": f"Expenses:Expenses:Investment-Expenses:{taxability}:{leaf}",
+        "rounding_error": "Equity:Rounding-Errors:Imports",
+        "fund_info": fund_info,
+        "currency": currency,
     }
     return config
 
 
-@regtest.with_importer(
-    schwab_csv_brokerage.Importer(
-        build_config()
-    )
-)
+@regtest.with_importer(etrade.Importer(build_config()))
 @regtest.with_testdir(path.dirname(__file__))
-class TestSchwabCSV(regtest.ImporterTestBase):
+class TestEtradeQFX(regtest.ImporterTestBase):
     pass
```

### Comparing `beancount_reds_importers-0.8.0/beancount_reds_importers/importers/stanchart/scbbank.py` & `beancount_reds_importers-0.9.0/beancount_reds_importers/importers/unitedoverseas/uobbank.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-"""SCB Banking .csv importer."""
+"""United Overseas Bank, Bank account .csv importer."""
 
-from beancount_reds_importers.libreader import csvreader
-from beancount_reds_importers.libtransactionbuilder import banking
 import re
+
 from beancount.core.number import D
 
+from beancount_reds_importers.libreader import xlsreader
+from beancount_reds_importers.libtransactionbuilder import banking
+
 
-class Importer(csvreader.Importer, banking.Importer):
-    IMPORTER_NAME = 'SCB Banking Account CSV'
+class Importer(xlsreader.Importer, banking.Importer):
+    IMPORTER_NAME = __doc__
 
     def custom_init(self):
         self.max_rounding_error = 0.04
-        self.filename_pattern_def = 'AccountTransactions[0-9]*'
-        self.header_identifier = self.config.get('custom_header', 'Account transactions shown:')
-        self.column_labels_line = 'Date,Transaction,Currency,Deposit,Withdrawal,Running Balance,SGD Equivalent Balance'
-        self.balance_column_labels_line = 'Account Name,Account Number,Currency,Current Balance,Available Balance'
-        self.date_format = '%d/%m/%Y'
-        self.skip_tail_rows = 0
-        self.skip_comments = '# '
+        self.filename_pattern_def = "ACC_TXN_History[0-9]*"
+        self.header_identifier = self.config.get(
+            "custom_header",
+            "United Overseas Bank Limited.*Account Type:Uniplus Account",
+        )
+        self.column_labels_line = (
+            "Transaction Date,Transaction Description,Withdrawal,Deposit,Available Balance"
+        )
+        self.date_format = "%d %b %Y"
+        # fmt: off
         self.header_map = {
-            "Date":            "date",
-            "Transaction":     "payee",
-            "Currency":        "currency",
-            "Withdrawal":      "withdrawal",
-            "Deposit":         "deposit",
-            "Running Balance": "balance_running",
-            "SGD Equivalent Balance": "balance",
+            "Transaction Date":         "date",
+            "Transaction Description":  "payee",
+            "Available Balance":        "balance",
         }
+        # fmt: on
         self.transaction_type_map = {}
         self.skip_transaction_types = []
 
     def deep_identify(self, file):
-        account_number = self.config.get('account_number', '')
-        return re.match(self.header_identifier, file.head()) and \
-            account_number in file.head()
+        account_number = self.config.get("account_number", "")
+        return re.match(self.header_identifier, file.head()) and account_number in file.head()
 
-    # TODO: move into utils, since this is probably a common operation
+    # TODO: move these into utils, since this is probably a common operation
     def prepare_table(self, rdr):
-        rdr = rdr.addfield('amount',
-                           lambda x: "-" + x['Withdrawal'] if x['Withdrawal'] != '' else x['Deposit'])
-        rdr = rdr.addfield('memo', lambda x: '')
+        # Remove carriage returns in description
+        rdr = rdr.convert("Transaction Description", lambda x: x.replace("\n", " "))
+
+        def Ds(x):
+            return D(str(x))
+
+        rdr = rdr.addfield(
+            "amount",
+            lambda x: -1 * Ds(x["Withdrawal"]) if x["Withdrawal"] != 0 else Ds(x["Deposit"]),
+        )
+        rdr = rdr.addfield("memo", lambda x: "")
         return rdr
 
     def prepare_raw_file(self, rdr):
         # Strip tabs and spaces around each field in the entire file
-        rdr = rdr.convertall(lambda x: x.strip(' \t') if isinstance(x, str) else x)
+        rdr = rdr.convertall(lambda x: x.strip(" \t") if isinstance(x, str) else x)
+
+        # Delete empty rows
+        rdr = rdr.select(lambda x: any([i != "" for i in x]))
 
         return rdr
 
     def get_balance_statement(self, file=None):
         """Return the balance on the first and last dates"""
         date = self.get_balance_assertion_date()
         if date:
-            rdr = self.read_raw(file)
-            rdr = self.prepare_raw_file(rdr)
-            col_labels = self.balance_column_labels_line.split(',')
-            rdr = self.extract_table_with_header(rdr, col_labels)
-
-            header_map = {k: k.replace(' ', '_') for k in col_labels}
-            rdr = rdr.rename(header_map)
-
-            while '' in rdr.header():
-                rdr = rdr.cutout('')
-
-            row = rdr.namedtuples()[0]
-            amount = row.Current_Balance
-            units, debitcredit = amount.split()
-            if debitcredit != 'CR':
-                units = '-' + units
-            yield banking.Balance(date, D(units), row.Currency)
+            row = self.rdr.namedtuples()[0]
+            # Get currency from input file
+            currency = self.get_row_by_label(file, "Account Number:")[2]
+
+            yield banking.Balance(date, D(str(row.balance)), currency)
```

### Comparing `beancount_reds_importers-0.8.0/beancount_reds_importers/importers/stanchart/scbcard.py` & `beancount_reds_importers-0.9.0/beancount_reds_importers/importers/stanchart/scbcard.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,77 +1,86 @@
 """SCB Credit .csv importer."""
 
-from beancount_reds_importers.libreader import csvreader
-from beancount_reds_importers.libtransactionbuilder import banking
 import re
+
 from beancount.core.number import D
 
+from beancount_reds_importers.libreader import csvreader
+from beancount_reds_importers.libtransactionbuilder import banking
+
 
 class Importer(csvreader.Importer, banking.Importer):
-    IMPORTER_NAME = 'SCB Card CSV'
+    IMPORTER_NAME = "SCB Card CSV"
 
     def custom_init(self):
         self.max_rounding_error = 0.04
-        self.filename_pattern_def = 'CardTransactions[0-9]*'
-        self.header_identifier = self.config.get('custom_header', 'PRIORITY BANKING VISA INFINITE CARD')
-        self.column_labels_line = 'Date,DESCRIPTION,Foreign Currency Amount,SGD Amount'
-        self.date_format = '%d/%m/%Y'
+        self.filename_pattern_def = "CardTransactions[0-9]*"
+        self.header_identifier = self.config.get(
+            "custom_header", "PRIORITY BANKING VISA INFINITE CARD"
+        )
+        self.column_labels_line = "Date,DESCRIPTION,Foreign Currency Amount,SGD Amount"
+        self.date_format = "%d/%m/%Y"
         self.skip_tail_rows = 6
-        self.skip_comments = '# '
+        self.skip_comments = "# "
+        # fmt: off
         self.header_map = {
-            "Date":           "date",
-            "DESCRIPTION":    "payee",
+            "Date":         "date",
+            "DESCRIPTION":  "payee",
         }
+        # fmt: on
         self.transaction_type_map = {}
 
     def deep_identify(self, file):
-        account_number = self.config.get('account_number', '')
-        return re.match(self.header_identifier, file.head()) and \
-            account_number in file.head()
+        account_number = self.config.get("account_number", "")
+        return re.match(self.header_identifier, file.head()) and account_number in file.head()
 
     def skip_transaction(self, row):
-        return '[UNPOSTED]' in row.payee
+        return "[UNPOSTED]" in row.payee
 
     def prepare_table(self, rdr):
-        rdr = rdr.select(lambda r: 'UNPOSTED' not in r['DESCRIPTION'])
+        rdr = rdr.select(lambda r: "UNPOSTED" not in r["DESCRIPTION"])
 
         # parse foreign_currency amount: "YEN 74,000"
-        if self.config.get('convert_currencies', False):
+        if self.config.get("convert_currencies", False):
             # Currency conversions won't work as expected since Beancount v2
             # doesn't support adding @@ (total price conversions) via code.
             # See https://groups.google.com/g/beancount/c/nMvuoR4yOmM
             # This means the '@' generated by this code below needs to be replaced with an '@@'
 
-            rdr = rdr.capture('Foreign Currency Amount', '(.*) (.*)',
-                              ['foreign_currency', 'foreign_amount'],
-                              fill=' ', include_original=True)
-        rdr = rdr.cutout('Foreign Currency Amount')
+            rdr = rdr.capture(
+                "Foreign Currency Amount",
+                "(.*) (.*)",
+                ["foreign_currency", "foreign_amount"],
+                fill=" ",
+                include_original=True,
+            )
+        rdr = rdr.cutout("Foreign Currency Amount")
 
         # parse SGD Amount: "SGD 141.02 CR" into a single amount column
-        rdr = rdr.capture('SGD Amount', '(.*) (.*) (.*)', ['currency', 'amount', 'crdr'])
+        rdr = rdr.capture("SGD Amount", "(.*) (.*) (.*)", ["currency", "amount", "crdr"])
 
         # change DR into -ve. TODO: move this into csvreader or csvreader.utils
-        crdrdict = {'DR': '-', 'CR': ''}
-        rdr = rdr.convert('amount', lambda i, row: crdrdict[row.crdr] + i, pass_row=True)
+        crdrdict = {"DR": "-", "CR": ""}
+        rdr = rdr.convert("amount", lambda i, row: crdrdict[row.crdr] + i, pass_row=True)
 
-        rdr = rdr.addfield('memo', lambda x: '')  # TODO: make this non-mandatory in csvreader
+        rdr = rdr.addfield("memo", lambda x: "")  # TODO: make this non-mandatory in csvreader
         return rdr
 
     def prepare_raw_file(self, rdr):
         # Strip tabs and spaces around each field in the entire file
-        rdr = rdr.convertall(lambda x: x.strip(' \t') if isinstance(x, str) else x)
+        rdr = rdr.convertall(lambda x: x.strip(" \t") if isinstance(x, str) else x)
 
         # Delete empty rows
-        rdr = rdr.select(lambda x: any([i != '' for i in x]))
+        rdr = rdr.select(lambda x: any([i != "" for i in x]))
         return rdr
 
     def get_balance_statement(self, file=None):
         """Return the balance on the first and last dates"""
         date = self.get_balance_assertion_date()
         if date:
-            balance_row = self.get_row_by_label(file, 'Current Balance')
+            balance_row = self.get_row_by_label(file, "Current Balance")
             currency, amount = balance_row[1], balance_row[2]
             units, debitcredit = amount.split()
-            if debitcredit != 'CR':
-                units = '-' + units
+            if debitcredit != "CR":
+                units = "-" + units
 
             yield banking.Balance(date, D(units), currency)
```

### Comparing `beancount_reds_importers-0.8.0/beancount_reds_importers/importers/tdameritrade/__init__.py` & `beancount_reds_importers-0.9.0/beancount_reds_importers/importers/tdameritrade/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-
 from beancount_reds_importers.libreader import ofxreader
 from beancount_reds_importers.libtransactionbuilder import investments
 
 
 class Importer(investments.Importer, ofxreader.Importer):
-    IMPORTER_NAME = 'TDAmeritrade'
+    IMPORTER_NAME = "TDAmeritrade"
 
     def custom_init(self):
         super(Importer, self).custom_init()
         self.max_rounding_error = 0.07
-        self.filename_pattern_def = '.*tdameritrade'
+        self.filename_pattern_def = ".*tdameritrade"
         self.get_ticker_info = self.get_ticker_info_from_id
 
     def get_ticker_info(self, security):
-        ticker = self.config['fund_info']['cusip_map'][security]
-        return ticker, ''
+        ticker = self.config["fund_info"]["cusip_map"][security]
+        return ticker, ""
```

### Comparing `beancount_reds_importers-0.8.0/beancount_reds_importers/importers/unitedoverseas/tests/ACC_TXN_History_1234_clean.xls` & `beancount_reds_importers-0.9.0/beancount_reds_importers/importers/unitedoverseas/tests/ACC_TXN_History_1234_clean.xls`

 * *Files identical despite different names*

### Comparing `beancount_reds_importers-0.8.0/beancount_reds_importers/importers/unitedoverseas/tests/ACC_TXN_History_1234_clean.xls.extract` & `beancount_reds_importers-0.9.0/beancount_reds_importers/importers/unitedoverseas/tests/ACC_TXN_History_1234_clean.xls.extract`

 * *Files identical despite different names*

### Comparing `beancount_reds_importers-0.8.0/beancount_reds_importers/importers/unitedoverseas/uobbank.py` & `beancount_reds_importers-0.9.0/beancount_reds_importers/importers/unitedoverseas/uobsrs.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,60 +1,56 @@
-"""United Overseas Bank, Bank account .csv importer."""
+"""UOB SRS importer."""
 
-from beancount_reds_importers.libreader import xlsreader
-from beancount_reds_importers.libtransactionbuilder import banking
 import re
+
 from beancount.core.number import D
 
+from beancount_reds_importers.libreader import xlsreader
+from beancount_reds_importers.libtransactionbuilder import banking
+
 
 class Importer(xlsreader.Importer, banking.Importer):
-    IMPORTER_NAME = __doc__
+    IMPORTER_NAME = "UOB SRS"
 
     def custom_init(self):
         self.max_rounding_error = 0.04
-        self.filename_pattern_def = 'ACC_TXN_History[0-9]*'
-        self.header_identifier = self.config.get('custom_header', 'United Overseas Bank Limited.*Account Type:Uniplus Account')
-        self.column_labels_line = 'Transaction Date,Transaction Description,Withdrawal,Deposit,Available Balance'
-        self.date_format = '%d %b %Y'
+        self.filename_pattern_def = "SRS_TXN_History[0-9]*"
+        self.header_identifier = self.config.get(
+            "custom_header", "United Overseas Bank Limited.*Account Type:SRS Account"
+        )
+        self.column_labels_line = "Transaction Date,Transaction Description,Withdrawal,Deposit"
+        self.date_format = "%Y%m%d"
+        # fmt: off
         self.header_map = {
-            'Transaction Date': 'date',
-            'Transaction Description': 'payee',
-            'Available Balance': 'balance'
+            "Transaction Date":         "date",
+            "Transaction Description":  "payee",
         }
+        # fmt: on
         self.transaction_type_map = {}
         self.skip_transaction_types = []
 
     def deep_identify(self, file):
-        account_number = self.config.get('account_number', '')
-        return re.match(self.header_identifier, file.head()) and \
-            account_number in file.head()
+        account_number = self.config.get("account_number", "")
+        return re.match(self.header_identifier, file.head()) and account_number in file.head()
 
-    # TODO: move these into utils, since this is probably a common operation
     def prepare_table(self, rdr):
         # Remove carriage returns in description
-        rdr = rdr.convert('Transaction Description', lambda x: x.replace('\n', ' '))
+        rdr = rdr.convert("Transaction Description", lambda x: x.replace("\n", " "))
 
         def Ds(x):
             return D(str(x))
-        rdr = rdr.addfield('amount',
-                           lambda x: -1 * Ds(x['Withdrawal']) if x['Withdrawal'] != 0 else Ds(x['Deposit']))
-        rdr = rdr.addfield('memo', lambda x: '')
+
+        rdr = rdr.addfield(
+            "amount",
+            lambda x: -1 * Ds(x["Withdrawal"]) if x["Withdrawal"] != "" else Ds(x["Deposit"]),
+        )
+        rdr = rdr.addfield("memo", lambda x: "")
         return rdr
 
     def prepare_raw_file(self, rdr):
         # Strip tabs and spaces around each field in the entire file
-        rdr = rdr.convertall(lambda x: x.strip(' \t') if isinstance(x, str) else x)
+        rdr = rdr.convertall(lambda x: x.strip(" \t") if isinstance(x, str) else x)
 
         # Delete empty rows
-        rdr = rdr.select(lambda x: any([i != '' for i in x]))
+        rdr = rdr.select(lambda x: any([i != "" for i in x]))
 
         return rdr
-
-    def get_balance_statement(self, file=None):
-        """Return the balance on the first and last dates"""
-        date = self.get_balance_assertion_date()
-        if date:
-            row = self.rdr.namedtuples()[0]
-            # Get currency from input file
-            currency = self.get_row_by_label(file, 'Account Number:')[2]
-
-            yield banking.Balance(date, D(str(row.balance)), currency)
```

### Comparing `beancount_reds_importers-0.8.0/beancount_reds_importers/importers/unitedoverseas/uobcard.py` & `beancount_reds_importers-0.9.0/beancount_reds_importers/importers/unitedoverseas/uobcard.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,75 +1,80 @@
 """SCB Credit .csv importer."""
 
-from beancount_reds_importers.libreader import xlsreader
-from beancount_reds_importers.libtransactionbuilder import banking
 import re
+
 from beancount.core.number import D
 
+from beancount_reds_importers.libreader import xlsreader
+from beancount_reds_importers.libtransactionbuilder import banking
+
 
 class Importer(xlsreader.Importer, banking.Importer):
-    IMPORTER_NAME = 'SCB Card CSV'
+    IMPORTER_NAME = "SCB Card CSV"
 
     def custom_init(self):
         self.max_rounding_error = 0.04
-        self.filename_pattern_def = '^CC_TXN_History[0-9]*'
-        self.header_identifier = self.config.get('custom_header', 'United Overseas Bank Limited.*Account Type:VISA SIGNATURE')
-        self.column_labels_line = 'Transaction Date,Posting Date,Description,Foreign Currency Type,Transaction Amount(Foreign),Local Currency Type,Transaction Amount(Local)'  # noqa: E501
-        self.date_format = '%d %b %Y'
+        self.filename_pattern_def = "^CC_TXN_History[0-9]*"
+        self.header_identifier = self.config.get(
+            "custom_header", "United Overseas Bank Limited.*Account Type:VISA SIGNATURE"
+        )
+        self.column_labels_line = "Transaction Date,Posting Date,Description,Foreign Currency Type,Transaction Amount(Foreign),Local Currency Type,Transaction Amount(Local)"  # noqa: E501
+        self.date_format = "%d %b %Y"
 
         # Remove _DISABLED below to include currency conversions. This won't work as expected since
         # Beancount v2 doesn't support adding @@ (total price conversions) via code. See
         # https://groups.google.com/g/beancount/c/nMvuoR4yOmM This means the '@' generated by this
         # code below needs to be replaced with an '@@'
 
-        foreign_currency = 'foreign_currency_DISABLED'
-        foreign_amount = 'foreign_amount_DISABLED'
-        if self.config.get('convert_currencies', False):
-            foreign_currency = 'foreign_currency'
-            foreign_amount = 'foreign_amount'
+        foreign_currency = "foreign_currency_DISABLED"
+        foreign_amount = "foreign_amount_DISABLED"
+        if self.config.get("convert_currencies", False):
+            foreign_currency = "foreign_currency"
+            foreign_amount = "foreign_amount"
 
+        # fmt: off
         self.header_map = {
-                'Transaction Date': 'date',
-                'Posting Date': 'date_posting',
-                'Description': 'payee',
-                'Foreign Currency Type': foreign_currency,
-                'Transaction Amount(Foreign)': foreign_amount,
-                'Local Currency Type': 'currency',
-                'Transaction Amount(Local)': 'amount'
+            "Transaction Date":             "date",
+            "Posting Date":                 "date_posting",
+            "Description":                  "payee",
+            "Foreign Currency Type":        foreign_currency,
+            "Transaction Amount(Foreign)":  foreign_amount,
+            "Local Currency Type":          "currency",
+            "Transaction Amount(Local)":    "amount",
         }
+        # fmt: on
         self.transaction_type_map = {}
         self.skip_transaction_types = []
 
     def deep_identify(self, file):
-        account_number = self.config.get('account_number', '')
-        return re.match(self.header_identifier, file.head()) and \
-            account_number in file.head()
+        account_number = self.config.get("account_number", "")
+        return re.match(self.header_identifier, file.head()) and account_number in file.head()
 
     # TODO: move into utils, since this is probably a common operation
     def prepare_table(self, rdr):
         # Remove carriage returns in description
-        rdr = rdr.convert('Description', lambda x: x.replace('\n', ' '))
-        rdr = rdr.addfield('memo', lambda x: '')
+        rdr = rdr.convert("Description", lambda x: x.replace("\n", " "))
+        rdr = rdr.addfield("memo", lambda x: "")
 
         # delete empty rows
-        rdr = rdr.select(lambda x: x['Transaction Date'] != '')
+        rdr = rdr.select(lambda x: x["Transaction Date"] != "")
         return rdr
 
     def prepare_processed_table(self, rdr):
-        return rdr.convert('amount', lambda x: -1 * D(str(x)))
+        return rdr.convert("amount", lambda x: -1 * D(str(x)))
 
     def prepare_raw_file(self, rdr):
         # Strip tabs and spaces around each field in the entire file
-        rdr = rdr.convertall(lambda x: x.strip(' \t') if isinstance(x, str) else x)
+        rdr = rdr.convertall(lambda x: x.strip(" \t") if isinstance(x, str) else x)
 
         # Delete empty rows
-        rdr = rdr.select(lambda x: any([i != '' for i in x]))
+        rdr = rdr.select(lambda x: any([i != "" for i in x]))
 
         return rdr
 
     def get_balance_statement(self, file=None):
         """Return the balance on the first and last dates"""
         date = self.get_balance_assertion_date()
         if date:
-            balance_row = self.get_row_by_label(file, 'Statement Balance:')
+            balance_row = self.get_row_by_label(file, "Statement Balance:")
             units, currency = balance_row[1], balance_row[2]
             yield banking.Balance(date, -1 * D(str(units)), currency)
```

### Comparing `beancount_reds_importers-0.8.0/beancount_reds_importers/importers/unitedoverseas/uobsrs.py` & `beancount_reds_importers-0.9.0/beancount_reds_importers/importers/schwab/schwab_csv_checking.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,48 +1,52 @@
-"""UOB SRS importer."""
+"""Schwab Checking .csv importer."""
 
-import re
-from beancount_reds_importers.libreader import xlsreader
+from beancount_reds_importers.libreader import csvreader
 from beancount_reds_importers.libtransactionbuilder import banking
-from beancount.core.number import D
 
 
-class Importer(xlsreader.Importer, banking.Importer):
-    IMPORTER_NAME = 'UOB SRS'
+class Importer(csvreader.Importer, banking.Importer):
+    IMPORTER_NAME = "Schwab Checking account CSV"
 
     def custom_init(self):
         self.max_rounding_error = 0.04
-        self.filename_pattern_def = 'SRS_TXN_History[0-9]*'
-        self.header_identifier = self.config.get('custom_header', 'United Overseas Bank Limited.*Account Type:SRS Account')
-        self.column_labels_line = 'Transaction Date,Transaction Description,Withdrawal,Deposit'
-        self.date_format = '%Y%m%d'
+        self.filename_pattern_def = ".*_Checking_Transactions_"
+        self.header_identifier = ""
+        self.column_labels_line = '"Date","Status","Type","CheckNumber","Description","Withdrawal","Deposit","RunningBalance"'
+        self.date_format = "%m/%d/%Y"
+        self.skip_comments = "# "
+        # fmt: off
         self.header_map = {
-            'Transaction Date': 'date',
-            'Transaction Description': 'payee',
+            "Date":             "date",
+            "Type":             "type",
+            "CheckNumber":      "checknum",
+            "Description":      "payee",
+            "Withdrawal":       "withdrawal",
+            "Deposit":          "deposit",
+            "RunningBalance":   "balance",
         }
-        self.transaction_type_map = {}
-        self.skip_transaction_types = []
+        self.transaction_type_map = {
+            "INTADJUST":    "income",
+            "TRANSFER":     "transfer",
+            "ACH":          "transfer",
+        }
+        # fmt: on
+        self.skip_transaction_types = ["Journal"]
 
     def deep_identify(self, file):
-        account_number = self.config.get('account_number', '')
-        return re.match(self.header_identifier, file.head()) and \
-            account_number in file.head()
+        last_three = self.config.get("account_number", "")[-3:]
+        return self.column_labels_line in file.head() and f"XX{last_three}" in file.name
 
     def prepare_table(self, rdr):
-        # Remove carriage returns in description
-        rdr = rdr.convert('Transaction Description', lambda x: x.replace('\n', ' '))
-
-        def Ds(x):
-            return D(str(x))
-        rdr = rdr.addfield('amount',
-                           lambda x: -1 * Ds(x['Withdrawal']) if x['Withdrawal'] != '' else Ds(x['Deposit']))
-        rdr = rdr.addfield('memo', lambda x: '')
+        rdr = rdr.addfield(
+            "amount",
+            lambda x: "-" + x["Withdrawal"] if x["Withdrawal"] != "" else x["Deposit"],
+        )
+        rdr = rdr.addfield("memo", lambda x: "")
         return rdr
 
-    def prepare_raw_file(self, rdr):
-        # Strip tabs and spaces around each field in the entire file
-        rdr = rdr.convertall(lambda x: x.strip(' \t') if isinstance(x, str) else x)
+    def get_balance_statement(self, file=None):
+        """Return the balance on the first and last dates"""
 
-        # Delete empty rows
-        rdr = rdr.select(lambda x: any([i != '' for i in x]))
-
-        return rdr
+        date = self.get_balance_assertion_date()
+        if date:
+            yield banking.Balance(date, self.rdr.namedtuples()[0].balance, self.currency)
```

### Comparing `beancount_reds_importers-0.8.0/beancount_reds_importers/importers/vanguard/__init__.py` & `beancount_reds_importers-0.9.0/beancount_reds_importers/importers/vanguard/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,55 +1,56 @@
-""" Vanguard Brokerage ofx importer."""
+"""Vanguard Brokerage ofx importer."""
 
 import ntpath
+
 from beancount_reds_importers.libreader import ofxreader
 from beancount_reds_importers.libtransactionbuilder import investments
 
 
 class Importer(investments.Importer, ofxreader.Importer):
-    IMPORTER_NAME = 'Vanguard'
+    IMPORTER_NAME = "Vanguard"
 
     # Any memo in the source OFX that's in this set is not carried forward.
     # Vanguard sets memos that aren't very useful and would create noise in the
     # generated ledger transactions.
     SKIP_MEMOS = {
         "Price as of date based on closing price",
     }
 
     def custom_init(self):
         self.max_rounding_error = 0.11
-        self.filename_pattern_def = '.*OfxDownload'
+        self.filename_pattern_def = ".*OfxDownload"
         self.get_ticker_info = self.get_ticker_info_from_id
         self.get_payee = self.cleanup_memo
 
         # See https://github.com/redstreet/beancount_reds_importers/issues/15: occasionally, Vanguard qfx
         # files contain a transaction with untiprice set to zero. Probably an internal bug at their end. We
         # set this handler to "do nothing", which will result in the below, which can be fixed manually:
         # 2021-01-01 * "DIVIDEND REINVEST" "[TICKER] Vanguard Ticker"
         #    Assets:Vanguard:TICKER  234.56 TICKER
         #    Income:Dividends:TICKER  -78 USD
 
         self.price_cost_both_zero_handler = lambda *args: None
 
     def file_name(self, file):
-        return 'vanguard-all-{}'.format(ntpath.basename(file.name))
+        return "vanguard-all-{}".format(ntpath.basename(file.name))
 
     def get_target_acct_custom(self, transaction, ticker=None):
-        if 'LT CAP GAIN' in transaction.memo:
-            return self.config['capgainsd_lt']
-        elif 'ST CAP GAIN' in transaction.memo:
-            return self.config['capgainsd_st']
+        if "LT CAP GAIN" in transaction.memo:
+            return self.config["capgainsd_lt"]
+        elif "ST CAP GAIN" in transaction.memo:
+            return self.config["capgainsd_st"]
         return None
 
     def cleanup_memo(self, ot):
         # some vanguard files have memos repeated like this:
         # 'DIVIDEND REINVESTMENTDIVIDEND REINVESTMENT'
         retval = ot.memo
-        if ot.memo[:int(len(ot.memo)/2)] == ot.memo[int(len(ot.memo)/2):]:
-            retval = ot.memo[:int(len(ot.memo)/2)]
+        if ot.memo[: int(len(ot.memo) / 2)] == ot.memo[int(len(ot.memo) / 2) :]:
+            retval = ot.memo[: int(len(ot.memo) / 2)]
         return retval
 
         # For users to comment out in their local file if they so prefer
         # parts = [ot.type]
         # if ot.memo not in self.SKIP_MEMOS:
         #     parts.append(ot.memo)
         # return ' - '.join(parts)
```

### Comparing `beancount_reds_importers-0.8.0/beancount_reds_importers/importers/vanguard/tests/OfxDownload-401k.qfx` & `beancount_reds_importers-0.9.0/beancount_reds_importers/importers/vanguard/tests/OfxDownload-401k.qfx`

 * *Files identical despite different names*

### Comparing `beancount_reds_importers-0.8.0/beancount_reds_importers/importers/vanguard/tests/OfxDownload-401k.qfx.extract` & `beancount_reds_importers-0.9.0/beancount_reds_importers/importers/vanguard/tests/OfxDownload-401k.qfx.extract`

 * *Files identical despite different names*

### Comparing `beancount_reds_importers-0.8.0/beancount_reds_importers/importers/vanguard/tests/vanguard_test.py` & `beancount_reds_importers-0.9.0/beancount_reds_importers/importers/vanguard/tests/vanguard_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from os import path
+
 from beancount.ingest import regression_pytest as regtest
+
 from beancount_reds_importers.importers import vanguard
 
 
 @regtest.with_importer(
     vanguard.Importer(
         {
             "account_number": "444555",
```

### Comparing `beancount_reds_importers-0.8.0/beancount_reds_importers/importers/vanguard/vanguard_screenscrape.py` & `beancount_reds_importers-0.9.0/beancount_reds_importers/importers/vanguard/vanguard_screenscrape.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,59 +1,79 @@
-""" Vanguard screenscrape importer. Unsettled trades are not available in Vanguard's qfx and need to be
+"""Vanguard screenscrape importer. Unsettled trades are not available in Vanguard's qfx and need to be
 screenscrapped into a tsv"""
 
 from beancount_reds_importers.libreader import tsvreader
 from beancount_reds_importers.libtransactionbuilder import investments
 
 
 class Importer(investments.Importer, tsvreader.Importer):
-    IMPORTER_NAME = 'Vanguard screenscrape tsv'
+    IMPORTER_NAME = "Vanguard screenscrape tsv"
 
     def custom_init(self):
         self.max_rounding_error = 0.04
-        self.filename_pattern_def = '.*vanguardss.*'
-        self.header_identifier = ''
+        self.filename_pattern_def = ".*vanguardss.*"
+        self.header_identifier = ""
         self.get_ticker_info = self.get_ticker_info_from_id
-        self.date_format = '%m/%d/%Y'
-        self.funds_db_txt = 'funds_by_ticker'
+        self.date_format = "%m/%d/%Y"
+        self.funds_db_txt = "funds_by_ticker"
+        # fmt: off
         self.header_map = {
-            "date":        'date',
-            "settledate":   'tradeDate',
-            "symbol":      'security',
-            "description": 'memo',
-            "action":      'type',
-            "quantity":    'units',
-            "price":       'unit_price',
-            "fees":        'fees',
-            "amount":      'amount',
-            "total":       'total',
-            }
+            "date":         "date",
+            "settledate":   "tradeDate",
+            "symbol":       "security",
+            "description":  "memo",
+            "action":       "type",
+            "quantity":     "units",
+            "price":        "unit_price",
+            "fees":         "fees",
+            "amount":       "amount",
+            "total":        "total",
+        }
         self.transaction_type_map = {
-            'Buy':                          'buystock',
-            'Sell':                         'sellstock',
-            }
-        self.skip_transaction_types = ['']
+            "Buy":  "buystock",
+            "Sell": "sellstock",
+        }
+        # fmt: on
+        self.skip_transaction_types = [""]
 
     def prepare_table(self, rdr):
         def extract_numbers(x):
-            replacements = {'– ': '-',
-                            '$': '',
-                            ',': '',
-                            'Free': '0',
-                            }
+            replacements = {
+                "– ": "-",
+                "$": "",
+                ",": "",
+                "Free": "0",
+            }
             for k, v in replacements.items():
                 x = x.replace(k, v)
             return x
 
-        header = ('date', 'settledate', 'symbol', 'description', 'quantity', 'price', 'fees', 'amount')
+        header = (
+            "date",
+            "settledate",
+            "symbol",
+            "description",
+            "quantity",
+            "price",
+            "fees",
+            "amount",
+        )
         rdr = rdr.pushheader(header)
 
-        rdr = rdr.addfield('action', lambda x: x['description'].rsplit(' ', 2)[1].strip())
+        rdr = rdr.addfield("action", lambda x: x["description"].rsplit(" ", 2)[1].strip())
 
-        for field in ["date", "settledate", "symbol", "description", "quantity", "price", "fees"]:
+        for field in [
+            "date",
+            "settledate",
+            "symbol",
+            "description",
+            "quantity",
+            "price",
+            "fees",
+        ]:
             rdr = rdr.convert(field, lambda x: x.strip())
         for field in ["quantity", "amount", "price", "fees"]:
             rdr = rdr.convert(field, extract_numbers)
 
-        rdr = rdr.addfield('total', lambda x: x['amount'])
+        rdr = rdr.addfield("total", lambda x: x["amount"])
 
         return rdr
```

### Comparing `beancount_reds_importers-0.8.0/beancount_reds_importers/importers/workday/__init__.py` & `beancount_reds_importers-0.9.0/beancount_reds_importers/importers/workday/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,52 +1,56 @@
-""" Workday paycheck importer."""
+"""Workday paycheck importer."""
 
 import datetime
+
 from beancount_reds_importers.libreader import xlsx_multitable_reader
 from beancount_reds_importers.libtransactionbuilder import paycheck
 
 # Workday exports paycheck stubs to a .xlsx, one paycheck per .xlsx, with multiple tables on a single sheet,
 # that this importer imports. Call this importer with a config that looks like:
 #
 # workday.Importer({'desc': "Paycheck (Acme Company)",
 #      'main_account' : 'Income:Employment',
 #      'paycheck_template': '{}' # See beancount_reds_importers/libtransactionbuilder/paycheck.py for sample template
 #      'currency' : 'PENNIES',
 #     }),
 
 
 class Importer(paycheck.Importer, xlsx_multitable_reader.Importer):
-    IMPORTER_NAME = 'Workday Paycheck'
+    IMPORTER_NAME = "Workday Paycheck"
 
     def custom_init(self):
         self.max_rounding_error = 0.04
-        self.filename_pattern_def = '.*_Complete'
-        self.header_identifier = '- Complete' + self.config.get('custom_header', '')
-        self.date_format = '%m/%d/%Y'
+        self.filename_pattern_def = ".*_Complete"
+        self.header_identifier = "- Complete" + self.config.get("custom_header", "")
+        self.date_format = "%m/%d/%Y"
         self.skip_head_rows = 1
         # TODO: need to be smarter about this, and skip only when needed
         self.skip_tail_rows = 0
-        self.funds_db_txt = 'funds_by_ticker'
+        self.funds_db_txt = "funds_by_ticker"
+        # fmt: off
         self.header_map = {
-            "Description": 'memo',
-            "Symbol":      'security',
-            "Quantity":    'units',
-            "Price":       'unit_price',
-            }
+            "Description":  "memo",
+            "Symbol":       "security",
+            "Quantity":     "units",
+            "Price":        "unit_price",
+        }
+        # fmt: on
 
     def paycheck_date(self, input_file):
         self.read_file(input_file)
-        d = self.alltables['Payslip Information'].namedtuples()[0].check_date
+        d = self.alltables["Payslip Information"].namedtuples()[0].check_date
         self.date = datetime.datetime.strptime(d, self.date_format)
         return self.date.date()
 
     def prepare_tables(self):
         def valid_header_label(label):
-            return label.lower().replace(' ', '_')
+            return label.lower().replace(" ", "_")
 
         for section, table in self.alltables.items():
             for header in table.header():
                 table = table.rename(header, valid_header_label(header))
             self.alltables[section] = table
 
     def build_metadata(self, file, metatype=None, data={}):
-        return {'filing_account': self.config['main_account']}
+        acct = self.config.get("filing_account", self.config.get("main_account", None))
+        return {"filing_account": acct}
```

### Comparing `beancount_reds_importers-0.8.0/beancount_reds_importers/libreader/csv_multitable_reader.py` & `beancount_reds_importers-0.9.0/beancount_reds_importers/libreader/csv_multitable_reader.py`

 * *Files 10% similar despite different names*

```diff
@@ -55,30 +55,34 @@
         # output is in self.alltables
 
         if self.file_read_done:
             return
 
         self.raw_rdr = rdr = self.read_raw(file)
 
-        rdr = rdr.skip(getattr(self, 'skip_head_rows', 0))                 # chop unwanted file header rows
-        rdr = rdr.head(len(rdr) - getattr(self, 'skip_tail_rows', 0) - 1)  # chop unwanted file footer rows
+        rdr = rdr.skip(getattr(self, "skip_head_rows", 0))  # chop unwanted file header rows
+        rdr = rdr.head(
+            len(rdr) - getattr(self, "skip_tail_rows", 0) - 1
+        )  # chop unwanted file footer rows
 
         #     [0, 2, 10] <-- starts
         # [-1, 1, 9]     <-- ends
-        table_starts = [i for (i, row) in enumerate(rdr) if self.is_section_title(row)] + [len(rdr)]
-        table_ends = [r-1 for r in table_starts][1:]
+        table_starts = [i for (i, row) in enumerate(rdr) if self.is_section_title(row)] + [
+            len(rdr)
+        ]
+        table_ends = [r - 1 for r in table_starts][1:]
         table_indexes = zip(table_starts, table_ends)
 
         # build the dictionary of tables
         self.alltables = {}
-        for (s, e) in table_indexes:
+        for s, e in table_indexes:
             if s == e:
                 continue
-            table = rdr.skip(s+1)      # skip past start index and header row
-            table = table.head(e-s-1)  # chop lines after table section data
+            table = rdr.skip(s + 1)  # skip past start index and header row
+            table = table.head(e - s - 1)  # chop lines after table section data
             self.alltables[rdr[s][0]] = table
 
         for section, table in self.alltables.items():
             table = table.rowlenselect(0, complement=True)  # clean up empty rows
             table = table.cut(*[h for h in table.header() if h])  # clean up empty columns
             self.alltables[section] = table
```

### Comparing `beancount_reds_importers-0.8.0/beancount_reds_importers/libreader/csvreader.py` & `beancount_reds_importers-0.9.0/beancount_reds_importers/libreader/csvreader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """csv importer module for beancount to be used along with investment/banking/other importer modules in
 beancount_reds_importers."""
 
 import datetime
 import re
+import sys
 import traceback
-from beancount.ingest import importer
-from beancount.core.number import D
+
 import petl as etl
+from beancount.core.number import D
+from beancount.ingest import importer
+
 from beancount_reds_importers.libreader import reader
-import sys
 
-# This csv reader uses petl to read a .csv into a table for maniupulation. The output of this reader is a list
+# This csv reader uses petl to read a .csv into a table for manipulation. The output of this reader is a list
 # of namedtuples corresponding roughly to ofx transactions. The following steps achieve this. When writing
 # your own importer, you only should need to:
 # - override prepare_table()
 #   - provide the following mappings, which correspond to the input file format of a given institution:
 #       - header_map
 #       - transaction_type_map
 #       - skip_transaction_types
@@ -55,28 +57,31 @@
 #
 #   - numbers are parsed from string and convered into Decimal type. Non-numeric characters like '$' are removed.
 #   - dates are parsed and converted into datetime type.
 # - The table is now ready for use by the importer. petl makes each row available via namedtuples
 
 
 class Importer(reader.Reader, importer.ImporterProtocol):
-    FILE_EXTS = ['csv']
+    FILE_EXTS = ["csv"]
 
     def initialize_reader(self, file):
-        if getattr(self, 'file', None) != file:
+        if getattr(self, "file", None) != file:
             self.file = file
             self.reader_ready = self.deep_identify(file)
             if self.reader_ready:
                 self.file_read_done = False
             # else:
             #     print("header_identifier failed---------------:")
             #     print(self.header_identifier, file.head())
 
     def deep_identify(self, file):
-        return re.match(self.header_identifier, file.head())
+        return re.match(
+            self.header_identifier,
+            file.head(encoding=getattr(self, "file_encoding", None)),
+        )
 
     def file_date(self, file):
         "Get the maximum date from the file."
         self.initialize(file)  # self.date_format gets set via this
         self.read_file(file)
         return max(ot.date for ot in self.get_transactions()).date()
 
@@ -92,51 +97,59 @@
         return rdr
 
     def prepare_processed_table(self, rdr):
         return rdr
 
     def convert_columns(self, rdr):
         # convert data in transaction types column
-        if 'type' in rdr.header():
-            rdr = rdr.convert('type', self.transaction_type_map)
+        if "type" in rdr.header():
+            rdr = rdr.convert("type", self.transaction_type_map)
 
         # fixup decimals
-        decimals = ['units']
+        decimals = ["units"]
         for i in decimals:
             if i in rdr.header():
                 rdr = rdr.convert(i, D)
 
         # fixup currencies
         def remove_non_numeric(x):
-            return re.sub(r'[^0-9\.-]', "", str(x).strip())  # noqa: W605
-        currencies = getattr(self, 'currency_fields', []) + ['unit_price', 'fees', 'total', 'amount', 'balance']
+            return re.sub(r"[^0-9\.-]", "", str(x).strip())  # noqa: W605
+
+        currencies = getattr(self, "currency_fields", []) + [
+            "unit_price",
+            "fees",
+            "total",
+            "amount",
+            "balance",
+        ]
         for i in currencies:
             if i in rdr.header():
                 rdr = rdr.convert(i, remove_non_numeric)
                 rdr = rdr.convert(i, D)
 
         # fixup dates
         def convert_date(d):
             return datetime.datetime.strptime(d, self.date_format)
-        dates = getattr(self, 'date_fields', []) + ['date', 'tradeDate', 'settleDate']
+
+        dates = getattr(self, "date_fields", []) + ["date", "tradeDate", "settleDate"]
         for i in dates:
             if i in rdr.header():
                 rdr = rdr.convert(i, convert_date)
 
         return rdr
 
     def read_raw(self, file):
-        return etl.fromcsv(file.name)
+        return etl.fromcsv(file.name, encoding=getattr(self, "file_encoding", None))
 
     def skip_until_main_table(self, rdr, col_labels=None):
         """Skip csv lines until the header line is found."""
         # TODO: convert this into an 'extract_table()' method that handles the tail as well
         if not col_labels:
-            if hasattr(self, 'column_labels_line'):
-                col_labels = self.column_labels_line.replace('"', '').split(',')
+            if hasattr(self, "column_labels_line"):
+                col_labels = self.column_labels_line.replace('"', "").split(",")
             else:
                 return rdr
         skip = None
         for n, r in enumerate(rdr):
             # We only check if each element in col_labels shows up in the line in the file, and not
             # the other way around. This allows additional fields to show up anywhere, case the csv
             # format changes
@@ -147,16 +160,16 @@
             print(col_labels)
             sys.exit(1)
         return rdr.skip(skip)
 
     def extract_table_with_header(self, rdr, col_labels=None):
         rdr = self.skip_until_main_table(rdr, col_labels)
         nrows = len(rdr)
-        for (n, r) in enumerate(rdr):
-            if not r or all(i == '' for i in r):
+        for n, r in enumerate(rdr):
+            if not r or all(i == "" for i in r):
                 # blank line, terminate
                 nrows = n - 1
                 break
         rdr = rdr.head(nrows)
         return rdr
 
     def skip_until_row_contains(self, rdr, value):
@@ -166,27 +179,28 @@
                 start = n
         if start is None:
             print(f'Error: table is not as expected. "{value}" row not found.')
             sys.exit(1)
         return rdr.rowslice(start, len(rdr))
 
     def read_file(self, file):
-        if not self.file_read_done:
-
+        if not getattr(self, "file_read_done", False):
             # read file
             rdr = self.read_raw(file)
             rdr = self.prepare_raw_file(rdr)
 
             # extract main table
-            rdr = rdr.skip(getattr(self, 'skip_head_rows', 0))                 # chop unwanted header rows
-            rdr = rdr.head(len(rdr) - getattr(self, 'skip_tail_rows', 0) - 1)  # chop unwanted footer rows
+            rdr = rdr.skip(getattr(self, "skip_head_rows", 0))  # chop unwanted header rows
+            rdr = rdr.head(
+                len(rdr) - getattr(self, "skip_tail_rows", 0) - 1
+            )  # chop unwanted footer rows
             rdr = self.extract_table_with_header(rdr)
-            if hasattr(self, 'skip_comments'):
+            if hasattr(self, "skip_comments"):
                 rdr = rdr.skipcomments(self.skip_comments)
-            rdr = rdr.rowslice(getattr(self, 'skip_data_rows', 0), None)
+            rdr = rdr.rowslice(getattr(self, "skip_data_rows", 0), None)
             rdr = self.prepare_table(rdr)
 
             # process table
             rdr = rdr.rename(self.header_map)
             rdr = self.convert_columns(rdr)
             rdr = self.fix_column_names(rdr)
             rdr = self.prepare_processed_table(rdr)
@@ -196,20 +210,17 @@
 
     def get_transactions(self):
         for ot in self.rdr.namedtuples():
             if self.skip_transaction(ot):
                 continue
             yield ot
 
-    def get_available_cash(self, settlement_fund_balance=0):
-        return None
-
     # TOOD: custom, overridable
     def skip_transaction(self, row):
-        return getattr(row, 'type', 'NO_TYPE') in self.skip_transaction_types
+        return getattr(row, "type", "NO_TYPE") in self.skip_transaction_types
 
     def get_balance_assertion_date(self):
         """
         We add an additional day to get_max_transaction_date(), since Beancount balance
         assertions are defined to occur on the beginning of the assertion date.
         """
         return self.get_max_transaction_date() + datetime.timedelta(days=1)
@@ -220,16 +231,18 @@
             # we find the last transaction's date. If we use the ofx download date (if our source is ofx), we
             # could end up with a gap in time between the last transaction's date and balance assertion.
             # Pending (but not yet downloaded) transactions in this gap will get downloaded the next time we
             # do a download in the future, and cause the balance assertions to be invalid.
 
             # TODO: clean this up. this probably suffices:
             # return max(ot.date for ot in self.get_transactions()).date()
-            date = max(ot.tradeDate if hasattr(ot, 'tradeDate') else ot.date
-                       for ot in self.get_transactions()).date()
+            date = max(
+                ot.tradeDate if hasattr(ot, "tradeDate") else ot.date
+                for ot in self.get_transactions()
+            ).date()
         except Exception as err:
             print("ERROR: no end_date. SKIPPING input.")
             traceback.print_tb(err.__traceback__)
             return None
 
         return date
```

### Comparing `beancount_reds_importers-0.8.0/beancount_reds_importers/libreader/ofxreader.py` & `beancount_reds_importers-0.9.0/beancount_reds_importers/libreader/ofxreader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,99 +1,100 @@
 """Ofx importer module for beancount to be used along with investment/banking/other importer modules in
 beancount_reds_importers."""
 
 import datetime
-import ofxparse
+import warnings
 from collections import namedtuple
+
+import ofxparse
 from beancount.ingest import importer
-from beancount_reds_importers.libreader import reader
 from bs4.builder import XMLParsedAsHTMLWarning
-import warnings
+
+from beancount_reds_importers.libreader import reader
+
 warnings.filterwarnings("ignore", category=XMLParsedAsHTMLWarning)
 
 
 class Importer(reader.Reader, importer.ImporterProtocol):
-    FILE_EXTS = ['ofx', 'qfx']
+    FILE_EXTS = ["ofx", "qfx"]
 
     def initialize_reader(self, file):
-        if getattr(self, 'file', None) != file:
+        if getattr(self, "file", None) != file:
             self.file = file
             self.ofx_account = None
             self.reader_ready = False
             try:
                 self.ofx = self.read_file(file)
             except ofxparse.OfxParserException:
                 return
             for acc in self.ofx.accounts:
                 # account identifying info fieldname varies across institutions
                 # self.acc_num_field can be overridden in self.custom_init() if needed
-                acc_num_field = getattr(self, 'account_number_field', 'account_id')
-                if self.match_account_number(getattr(acc, acc_num_field),
-                                             self.config['account_number']):
+                acc_num_field = getattr(self, "account_number_field", "account_id")
+                if self.match_account_number(
+                    getattr(acc, acc_num_field), self.config["account_number"]
+                ):
                     self.ofx_account = acc
                     self.reader_ready = True
             if self.reader_ready:
                 self.currency = self.ofx_account.statement.currency.upper()
 
     def match_account_number(self, file_account, config_account):
         """We many not want to store entire credit card numbers in our config. Or a given ofx may not contain
         the full account number. Override this method to handle these cases."""
         return file_account == config_account
 
     def file_date(self, file):
         """Get the ending date of the statement."""
-        if not getattr(self, 'ofx_account', None):
+        if not getattr(self, "ofx_account", None):
             self.initialize(file)
         try:
             return self.ofx_account.statement.end_date
         except AttributeError:
             return None
 
     def read_file(self, file):
         with open(file.name) as fh:
             return ofxparse.OfxParser.parse(fh)
 
     def get_transactions(self):
         yield from self.ofx_account.statement.transactions
 
     def get_balance_statement(self, file=None):
-        if not hasattr(self.ofx_account.statement, 'balance'):
+        if not hasattr(self.ofx_account.statement, "balance"):
             return []
         date = self.get_balance_assertion_date()
         if date:
-            Balance = namedtuple('Balance', ['date', 'amount'])
+            Balance = namedtuple("Balance", ["date", "amount"])
             yield Balance(date, self.ofx_account.statement.balance)
 
     def get_balance_positions(self):
-        if not hasattr(self.ofx_account.statement, 'positions'):
+        if not hasattr(self.ofx_account.statement, "positions"):
             return []
         yield from self.ofx_account.statement.positions
 
     def get_available_cash(self, settlement_fund_balance=0):
-        available_cash = getattr(self.ofx_account.statement, 'available_cash', None)
+        available_cash = getattr(self.ofx_account.statement, "available_cash", None)
         if available_cash is not None:
             # Some institutions compute available_cash this way. For others, override this method
             # in the importer
             return available_cash - settlement_fund_balance
         return None
 
-    def get_ofx_end_date(self, field='end_date'):
+    def get_ofx_end_date(self, field="end_date"):
         end_date = getattr(self.ofx_account.statement, field, None)
 
-        # Convert end_date from utc to local timezone if needed and return
-        # This is needed only if there is an actual timestamp other than time(0, 0)
         if end_date:
-            if end_date.time() != datetime.time(0, 0):
-                end_date = end_date.replace(tzinfo=datetime.timezone.utc).astimezone()
+            # We don't care about timestamps, remove them so they don't affect date calculations
             return end_date.date()
 
         return None
 
     def get_smart_date(self):
-        """ We want the latest date we can assert balance on. Let's consider all the dates we have:
+        """We want the latest date we can assert balance on. Let's consider all the dates we have:
         b--------e-------(s-2)----(s)----(d)
 
         - b: date of first transaction in this ofx file (end_date)
         - e: date of last  transaction in this ofx file (max_transaction_date)
         - s: statement's end date as claimed by the ofx import fileinput (acc.statement.available_balance_date)
         - d: date of download
 
@@ -104,53 +105,68 @@
         (s-2), where 2 is the fudge factor (the time where pending transactions not seen in this
         statement might occur in the next statement).
 
         Not all ofx files have all these dates. Hence we compute this date with the best info we
         have.
         """
 
-        ofx_max_transation_date = self.get_ofx_end_date('end_date')
-        ofx_balance_date1 = self.get_ofx_end_date('available_balance_date')
-        ofx_balance_date2 = self.get_ofx_end_date('balance_date')
+        ofx_max_transation_date = self.get_ofx_end_date("end_date")
+        ofx_balance_date1 = self.get_ofx_end_date("available_balance_date")
+        ofx_balance_date2 = self.get_ofx_end_date("balance_date")
         max_transaction_date = self.get_max_transaction_date()
 
         if ofx_balance_date1:
-            ofx_balance_date1 -= datetime.timedelta(days=self.config.get('balance_assertion_date_fudge', 2))
+            ofx_balance_date1 -= datetime.timedelta(
+                days=self.config.get("balance_assertion_date_fudge", 2)
+            )
         if ofx_balance_date2:
-            ofx_balance_date2 -= datetime.timedelta(days=self.config.get('balance_assertion_date_fudge', 2))
-
-        dates = [ofx_max_transation_date, max_transaction_date, ofx_balance_date1, ofx_balance_date2]
-        if all(v is None for v in dates[:2]):  # because ofx_balance_date appears even for closed accounts
+            ofx_balance_date2 -= datetime.timedelta(
+                days=self.config.get("balance_assertion_date_fudge", 2)
+            )
+
+        dates = [
+            ofx_max_transation_date,
+            max_transaction_date,
+            ofx_balance_date1,
+            ofx_balance_date2,
+        ]
+        if all(
+            v is None for v in dates[:2]
+        ):  # because ofx_balance_date appears even for closed accounts
             return None
 
-        def vd(x): return x if x else datetime.date.min
+        def vd(x):
+            return x if x else datetime.date.min
+
         return_date = max(*[vd(x) for x in dates])
         # print("Smart date computation. Dates were: ", dates)
 
         return return_date
 
     def get_balance_assertion_date(self):
-        """ Choices for the date of the generated balance assertion can be specified in
+        """Choices for the date of the generated balance assertion can be specified in
         self.config['balance_assertion_date_type'], which can be:
         - 'smart':            smart date (default)
         - 'ofx_date':         date specified in ofx file
         - 'last_transaction': max transaction date
         - 'today':            today's date
 
         If you want something else, simply override this method in individual importer
 
         Finally, we add an additional day, since Beancount balance assertions are defined to occur
         on the beginning of the assertion date.
         """
 
-        date_type_map = {'smart': self.get_smart_date,
-                         'ofx_date': self.get_ofx_end_date,
-                         'last_transaction': self.get_max_transaction_date,
-                         'today': datetime.date.today}
-        date_type = self.config.get('balance_assertion_date_type', 'smart')
+        date_type_map = {
+            "smart": self.get_smart_date,
+            "ofx_date": self.get_ofx_end_date,
+            "last_transaction": self.get_max_transaction_date,
+            "today": datetime.date.today,
+        }
+        date_type = self.config.get("balance_assertion_date_type", "smart")
         return_date = date_type_map[date_type]()
 
         if not return_date:
             return None
         return return_date + datetime.timedelta(days=1)  # Next day, as defined by Beancount
 
     def get_max_transaction_date(self):
@@ -159,15 +175,16 @@
         could end up with a gap in time between the last transaction's date and balance assertion.
         Pending (but not yet downloaded) transactions in this gap will get downloaded the next time we
         do a download in the future, and cause the balance assertions to be invalid. This is
         a problem particularly with credit card accounts and bank accounts.
 
         """
         try:
-
-            date = max(ot.tradeDate if hasattr(ot, 'tradeDate') else ot.date
-                       for ot in self.get_transactions()).date()
+            date = max(
+                ot.tradeDate if hasattr(ot, "tradeDate") else ot.date
+                for ot in self.get_transactions()
+            ).date()
         except TypeError:
             return None
         except ValueError:
             return None
         return date
```

### Comparing `beancount_reds_importers-0.8.0/beancount_reds_importers/libreader/reader.py` & `beancount_reds_importers-0.9.0/beancount_reds_importers/libreader/reader.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,56 +1,57 @@
 """Reader module base class for beancount_reds_importers. ofx, csv, etc. readers inherit this."""
 
 import ntpath
-from os import path
 import re
+from os import path
 
 
-class Reader():
-    FILE_EXTS = ['']
-    IMPORTER_NAME = 'NOT SET'
+class Reader:
+    FILE_EXTS = [""]
+    IMPORTER_NAME = "NOT SET"
 
     def identify(self, file):
         # quick check to filter out files that are not the right format
         # print()
         # print('------------------', self.IMPORTER_NAME, '(' + self.FILE_EXT + ')')
         # print(file.name.lower())
         if not any(file.name.lower().endswith(ext) for ext in self.FILE_EXTS):
             # print("No match on extension")
             return False
         self.custom_init()
-        self.filename_pattern = self.config.get('filename_pattern', self.filename_pattern_def)
+        self.filename_pattern = self.config.get("filename_pattern", self.filename_pattern_def)
         if not re.match(self.filename_pattern, path.basename(file.name)):
             # print("No match on filename_pattern", self.filename_pattern, path.basename(file.name))
             return False
-        self.currency = self.config.get('currency', 'CURRENCY_NOT_CONFIGURED')
+        self.currency = self.config.get("currency", "CURRENCY_NOT_CONFIGURED")
         self.initialize_reader(file)
         # print("reader_ready:", self.reader_ready)
         return self.reader_ready
 
     def file_name(self, file):
-        return '{}'.format(ntpath.basename(file.name))
+        return "{}".format(ntpath.basename(file.name))
 
     def file_account(self, file):
         # Ugly hack to handle an interaction with smart_importer. See:
         # https://github.com/redstreet/beancount_reds_importers/issues/41
         # https://github.com/beancount/smart_importer/issues/122
         # https://github.com/beancount/smart_importer/issues/30
         import inspect
+
         curframe = inspect.currentframe()
         calframe = inspect.getouterframes(curframe, 2)
-        if any('predictor' in i.filename for i in calframe):
-            if 'smart_importer_hack' in self.config:
-                return self.config['smart_importer_hack']
+        if any("predictor" in i.filename for i in calframe):
+            if "smart_importer_hack" in self.config:
+                return self.config["smart_importer_hack"]
 
         # Otherwise handle a typical bean-file call
         self.initialize(file)
-        if 'filing_account' in self.config:
-            return self.config['filing_account']
-        return self.config['main_account']
+        if "filing_account" in self.config:
+            return self.config["filing_account"]
+        return self.config["main_account"]
 
     def get_balance_statement(self, file=None):
         return []
 
     def get_balance_positions(self):
         return []
```

### Comparing `beancount_reds_importers-0.8.0/beancount_reds_importers/libreader/tests/balance_assertion_date/last_transaction/transactions.qfx` & `beancount_reds_importers-0.9.0/beancount_reds_importers/libreader/tests/balance_assertion_date/last_transaction/transactions.qfx`

 * *Files identical despite different names*

### Comparing `beancount_reds_importers-0.8.0/beancount_reds_importers/libreader/tests/balance_assertion_date/ofx_date/transactions.qfx` & `beancount_reds_importers-0.9.0/beancount_reds_importers/libreader/tests/balance_assertion_date/ofx_date/transactions.qfx`

 * *Files identical despite different names*

### Comparing `beancount_reds_importers-0.8.0/beancount_reds_importers/libreader/tests/balance_assertion_date/smart/transactions.qfx` & `beancount_reds_importers-0.9.0/beancount_reds_importers/libreader/tests/balance_assertion_date/smart/transactions.qfx`

 * *Files identical despite different names*

### Comparing `beancount_reds_importers-0.8.0/beancount_reds_importers/libreader/xlsreader.py` & `beancount_reds_importers-0.9.0/beancount_reds_importers/libreader/xlsreader.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 """xlsx importer module for beancount to be used along with investment/banking/other importer modules in
 beancount_reds_importers."""
 
-import petl as etl
 import re
-from beancount_reds_importers.libreader import csvreader
 from os import devnull
 
+import petl as etl
+
+from beancount_reds_importers.libreader import csvreader
+
 
 class Importer(csvreader.Importer):
-    FILE_EXTS = ['xls']
+    FILE_EXTS = ["xls"]
 
     def initialize_reader(self, file):
-        if getattr(self, 'file', None) != file:
+        if getattr(self, "file", None) != file:
             self.file = file
             self.file_read_done = False
             self.reader_ready = False
 
             # TODO: this reads the entire file. Chop off after perhaps 2k or n lines
             rdr = self.read_raw(file)
-            header = ''
+            header = ""
             for r in rdr:
-                line = ''.join(str(x) for x in r)
+                line = "".join(str(x) for x in r)
                 header += line
 
             # TODO
             # account_number = self.config.get('account_number', '')
             # self.reader_ready = re.match(self.header_identifier, file.head()) and \
             #                     account_number in file.head()
 
             if re.match(self.header_identifier, header):
                 self.reader_ready = True
 
     def read_raw(self, file):
         # set logfile to ignore WARNING *** file size (92598) not 512 + multiple of sector size (512)
-        return etl.fromxls(file.name, logfile=open(devnull, 'w'))
+        return etl.fromxls(file.name, logfile=open(devnull, "w"))
```

### Comparing `beancount_reds_importers-0.8.0/beancount_reds_importers/libreader/xlsx_multitable_reader.py` & `beancount_reds_importers-0.9.0/beancount_reds_importers/libreader/xlsx_multitable_reader.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 """xlsx importer module for beancount to be used along with investment/banking/other importer modules in
 beancount_reds_importers."""
 
-import petl as etl
-from io import StringIO
 import csv
-import openpyxl
 import warnings
+from io import StringIO
+
+import openpyxl
+import petl as etl
+
 from beancount_reds_importers.libreader import csv_multitable_reader
 
 # This xlsx reader uses petl to read a .csv with multiple tables into a dictionary of petl tables. The section
 # title is the key. See csv_multitable_reader for more.
 
 
 class Importer(csv_multitable_reader.Importer):
-    FILE_EXTS = ['xlsx']
+    FILE_EXTS = ["xlsx"]
 
     def initialize_reader(self, file):
-        if getattr(self, 'file', None) != file:
+        if getattr(self, "file", None) != file:
             self.file = file
             self.file_read_done = False
             self.reader_ready = True
 
     def read_raw(self, file):
         # return etl.fromcsv(file.name)
 
@@ -39,8 +41,8 @@
         raw = etl.MemorySource(rawlines)
         rdr = etl.fromcsv(raw)
         return rdr
 
     def is_section_title(self, row):
         if len(row) == 1:
             return True
-        return all(i == '' or i is None for i in row[1:])
+        return all(i == "" or i is None for i in row[1:])
```

### Comparing `beancount_reds_importers-0.8.0/beancount_reds_importers/libreader/xlsxreader.py` & `beancount_reds_importers-0.9.0/beancount_reds_importers/libreader/xlsxreader.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """xlsx importer module for beancount to be used along with investment/banking/other importer modules in
 beancount_reds_importers."""
 
 import petl as etl
+
 from beancount_reds_importers.libreader import xlsreader
 
 
 class Importer(xlsreader.Importer):
-    FILE_EXTS = ['xlsx']
+    FILE_EXTS = ["xlsx"]
 
     def read_raw(self, file):
         rdr = etl.fromxlsx(file.name)
         # openpyxl gives us typed columns from the xlsx files (e.g. `float` for numeric
         # values, `datetime.datetime` for dates). Since xlsxreader currently inherits from csvreader,
         # converting these to be plain strings. Consider building a new xlsxreader that doesn't have to
         return rdr.convertall(str)
```

### Comparing `beancount_reds_importers-0.8.0/beancount_reds_importers/libtransactionbuilder/banking.py` & `beancount_reds_importers-0.9.0/beancount_reds_importers/libtransactionbuilder/banking.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Generic banking importer for beancount."""
 
 import itertools
 from collections import namedtuple
-from beancount.core import data
-from beancount.core import amount
+
+from beancount.core import amount, data
 from beancount.ingest import importer
-from beancount_reds_importers.libtransactionbuilder import common, transactionbuilder
 
+from beancount_reds_importers.libtransactionbuilder import common, transactionbuilder
 
-Balance = namedtuple('Balance', ['date', 'amount', 'currency'])
+Balance = namedtuple("Balance", ["date", "amount", "currency"])
 
 
 class Importer(importer.ImporterProtocol, transactionbuilder.TransactionBuilder):
     def __init__(self, config):
         self.config = config
         self.initialized = False
         self.reader_ready = False
@@ -39,57 +39,56 @@
         # self.target_account_map = {
         #         "directdep": 'TODO',
         #         "credit":    'TODO',
         #         "debit":     'TODO',
         # }
         pass
 
-    def build_metadata(self, file, metatype=None, data={}):
-        """This method is for importers to override. The overridden method can
-        look at the metatype ('transaction', 'balance', 'account', 'commodity', etc.)
-        and the data dictionary to return additional metadata"""
-        return {}
-
     def match_account_number(self, file_account, config_account):
         return file_account.endswith(config_account)
 
     def custom_init(self):
         if not self.custom_init_run:
             self.max_rounding_error = 0.04
-            self.filename_pattern_def = '.*bank_specific_filename.*'
+            self.filename_pattern_def = ".*bank_specific_filename.*"
             self.custom_init_run = True
 
     # def get_target_acct(self, transaction):
     #     # Not needed for accounts using smart_importer
     #     return self.target_account_map.get(transaction.type, None)
 
     @staticmethod
     def fields_contain_data(ot, fields):
         return all(hasattr(ot, f) and getattr(ot, f) for f in fields)
 
     def get_main_account(self, ot):
         """Can be overridden by importer"""
-        return self.config['main_account']
+        return self.config["main_account"]
 
     def get_target_account(self, ot):
         """Can be overridden by importer"""
-        return self.config.get('target_account')
+        return self.config.get("target_account")
 
     # --------------------------------------------------------------------------------
 
     def extract_balance(self, file, counter):
         entries = []
 
         for bal in self.get_balance_statement(file=file):
             if bal:
                 metadata = data.new_metadata(file.name, next(counter))
-                metadata.update(self.build_metadata(file, metatype='balance'))
-                balance_entry = data.Balance(metadata, bal.date, self.config['main_account'],
-                                             amount.Amount(bal.amount, self.get_currency(bal)),
-                                             None, None)
+                metadata.update(self.build_metadata(file, metatype="balance"))
+                balance_entry = data.Balance(
+                    metadata,
+                    bal.date,
+                    self.config["main_account"],
+                    amount.Amount(bal.amount, self.get_currency(bal)),
+                    None,
+                    None,
+                )
                 entries.append(balance_entry)
         return entries
 
     def extract_custom_entries(self, file, counter):
         """For custom importers to override"""
         return []
 
@@ -106,52 +105,59 @@
 
         self.read_file(file)
         for ot in self.get_transactions():
             if self.skip_transaction(ot):
                 continue
             metadata = data.new_metadata(file.name, next(counter))
             # metadata['type'] = ot.type # Optional metadata, useful for debugging #TODO
-            metadata.update(self.build_metadata(file,
-                                                metatype='transaction',
-                                                data={'transaction': ot}))
+            metadata.update(
+                self.build_metadata(file, metatype="transaction", data={"transaction": ot})
+            )
 
             # description fields: With OFX, ot.payee tends to be the "main" description field,
             # while ot.memo is optional
             #
             # With Beancount, the grammar is (payee, narration). payee is optional, narration is
             # mandatory. This is a bit unintuitive. In addition, smart_importer relies on
             # narration, so keeping the order unchanged in the call below is important.
 
             # Build transaction entry
             # Banking transactions might include foreign currency transactions. TODO: figure out
             # how ofx handles this and use the same interface for csv and other files
             entry = data.Transaction(
-                    meta=metadata,
-                    date=ot.date.date(),
-                    flag=self.FLAG,
-                    # payee and narration are switched. See the preceding note
-                    payee=self.get_narration(ot),
-                    narration=self.get_payee(ot),
-                    tags=self.get_tags(ot),
-                    links=data.EMPTY_SET,
-                    postings=[])
+                meta=metadata,
+                date=ot.date.date(),
+                flag=self.FLAG,
+                # payee and narration are switched. See the preceding note
+                payee=self.get_narration(ot),
+                narration=self.get_payee(ot),
+                tags=self.get_tags(ot),
+                links=data.EMPTY_SET,
+                postings=[],
+            )
 
             main_account = self.get_main_account(ot)
 
-            if self.fields_contain_data(ot, ['foreign_amount', 'foreign_currency']):
-                common.create_simple_posting_with_price(entry, main_account,
-                                                        ot.amount, self.get_currency(ot),
-                                                        ot.foreign_amount, ot.foreign_currency)
+            if self.fields_contain_data(ot, ["foreign_amount", "foreign_currency"]):
+                common.create_simple_posting_with_price(
+                    entry,
+                    main_account,
+                    ot.amount,
+                    self.get_currency(ot),
+                    ot.foreign_amount,
+                    ot.foreign_currency,
+                )
             else:
                 data.create_simple_posting(entry, main_account, ot.amount, self.get_currency(ot))
 
             # smart_importer can fill this in if the importer doesn't override self.get_target_acct()
             target_acct = self.get_target_account(ot)
             if target_acct:
                 data.create_simple_posting(entry, target_acct, None, None)
 
+            self.add_custom_postings(entry, ot)
             new_entries.append(entry)
 
         new_entries += self.extract_balance(file, counter)
         new_entries += self.extract_custom_entries(file, counter)
 
         return new_entries
```

### Comparing `beancount_reds_importers-0.8.0/beancount_reds_importers/libtransactionbuilder/common.py` & `beancount_reds_importers-0.9.0/beancount_reds_importers/libtransactionbuilder/common.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,66 @@
 #!/usr/bin/env python3
 
 from beancount.core import data
 from beancount.core.amount import Amount
+from beancount.core.number import D, Decimal
 from beancount.core.position import Cost
-from beancount.core.number import Decimal
-from beancount.core.number import D
 
 
 class PriceCostBothZeroException(Exception):
     """Raised when the input value is too small"""
+
     pass
 
 
-def create_simple_posting_with_price(entry, account,
-                                     number, currency,
-                                     price_number, price_currency):
-    return create_simple_posting_with_cost_or_price(entry, account,
-                                                    number, currency,
-                                                    price_number=price_number, price_currency=price_currency)
-
-
-def create_simple_posting_with_cost(entry, account,
-                                    number, currency,
-                                    cost_number, cost_currency, price_cost_both_zero_handler=None):
-    return create_simple_posting_with_cost_or_price(entry, account,
-                                                    number, currency,
-                                                    cost_number=cost_number, cost_currency=cost_currency,
-                                                    price_cost_both_zero_handler=price_cost_both_zero_handler)
-
-
-def create_simple_posting_with_cost_or_price(entry, account,
-                                             number, currency,
-                                             price_number=None, price_currency=None,
-                                             cost_number=None, cost_currency=None, costspec=None,
-                                             price_cost_both_zero_handler=None):
+def create_simple_posting_with_price(
+    entry, account, number, currency, price_number, price_currency
+):
+    return create_simple_posting_with_cost_or_price(
+        entry,
+        account,
+        number,
+        currency,
+        price_number=price_number,
+        price_currency=price_currency,
+    )
+
+
+def create_simple_posting_with_cost(
+    entry,
+    account,
+    number,
+    currency,
+    cost_number,
+    cost_currency,
+    price_cost_both_zero_handler=None,
+):
+    return create_simple_posting_with_cost_or_price(
+        entry,
+        account,
+        number,
+        currency,
+        cost_number=cost_number,
+        cost_currency=cost_currency,
+        price_cost_both_zero_handler=price_cost_both_zero_handler,
+    )
+
+
+def create_simple_posting_with_cost_or_price(
+    entry,
+    account,
+    number,
+    currency,
+    price_number=None,
+    price_currency=None,
+    cost_number=None,
+    cost_currency=None,
+    costspec=None,
+    price_cost_both_zero_handler=None,
+):
     """Create a simple posting on the entry, with a cost (for purchases) or price (for sell transactions).
 
     Args:
       entry: The entry instance to add the posting to.
       account: A string, the account to use on the posting.
       number: A Decimal number or string to use in the posting's Amount.
       currency: A string, the currency for the Amount.
@@ -55,15 +78,19 @@
         number = D(number)
     units = Amount(number, currency)
 
     if not (price_number or cost_number):
         if price_cost_both_zero_handler:
             price_cost_both_zero_handler()
         else:
-            print("WARNING: Either price ({}) or cost ({}) must be specified ({})".format(price_number, cost_number, entry))
+            print(
+                "WARNING: Either price ({}) or cost ({}) must be specified ({})".format(
+                    price_number, cost_number, entry
+                )
+            )
             raise PriceCostBothZeroException
             # import pdb; pdb.set_trace()
 
     price = Amount(D(price_number), price_currency) if price_number else None
     cost = Cost(cost_number, cost_currency, None, None) if cost_number else None
     cost = costspec if costspec else cost
     posting = data.Posting(account, units, cost, price, None, None)
```

### Comparing `beancount_reds_importers-0.8.0/beancount_reds_importers/libtransactionbuilder/investments.py` & `beancount_reds_importers-0.9.0/beancount_reds_importers/libtransactionbuilder/investments.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Generic investment importer module for beancount. Needs a reader module (eg: ofx, csv, etc.) from
 beancount_reads_importers to work."""
 
 import itertools
 import sys
-from beancount.core import data
-from beancount.core import amount
-from beancount.ingest import importer
+
+from beancount.core import amount, data
 from beancount.core.position import CostSpec
+from beancount.ingest import importer
+
 from beancount_reds_importers.libtransactionbuilder import common, transactionbuilder
 
 
 class Importer(importer.ImporterProtocol, transactionbuilder.TransactionBuilder):
     def __init__(self, config):
         """Initializes the importer.
 
@@ -79,83 +80,90 @@
         if self.initialized:
             return
 
         self.custom_init()
         self.initialize_reader(file)
 
         if self.reader_ready:
-            config_subst_vars = {'currency': self.currency,
-                                 # Leave the other values as is
-                                 'ticker': '{ticker}',
-                                 'source401k': '{source401k}',
-                                 }
+            config_subst_vars = {
+                "currency": self.currency,
+                # Leave the other values as is
+                "ticker": "{ticker}",
+                "source401k": "{source401k}",
+            }
             self.set_config_variables(config_subst_vars)
-            self.money_market_funds = self.config['fund_info']['money_market']
-            self.fund_data = self.config['fund_info']['fund_data']  # [(ticker, id, long_name), ...]
+            self.money_market_funds = self.config["fund_info"]["money_market"]
+            self.fund_data = self.config["fund_info"][
+                "fund_data"
+            ]  # [(ticker, id, long_name), ...]
             self.funds_by_id = {i: (ticker, desc) for ticker, i, desc in self.fund_data}
             self.funds_by_ticker = {ticker: (ticker, desc) for ticker, _, desc in self.fund_data}
 
             # Most ofx/csv files refer to funds by id (cusip/isin etc.) Some use tickers instead
-            self.funds_db = getattr(self, getattr(self, 'funds_db_txt', 'funds_by_id'))
+            self.funds_db = getattr(self, getattr(self, "funds_db_txt", "funds_by_id"))
             self.build_account_map()
 
         self.initialized = True
 
     def build_account_map(self):
+        # fmt: off
         # map transaction types to target posting accounts
         self.target_account_map = {
-            "buymf":        self.config['cash_account'],
-            "sellmf":       self.config['cash_account'],
-            "buystock":     self.config['cash_account'],
-            "sellstock":    self.config['cash_account'],
-            "buyother":     self.config['cash_account'],
-            "sellother":    self.config['cash_account'],
-            "buydebt":      self.config['cash_account'],
-            "reinvest":     self.config['dividends'],
-            "dividends":    self.config['dividends'],
-            "capgainsd_lt": self.config['capgainsd_lt'],
-            "capgainsd_st": self.config['capgainsd_st'],
-            "income":       self.config['interest'],
-            "fee":          self.config['fees'],
-            "invexpense":   self.config.get('invexpense', "ACCOUNT_NOT_CONFIGURED:INVEXPENSE"),
+            "buymf":        self.config["cash_account"],
+            "sellmf":       self.config["cash_account"],
+            "buystock":     self.config["cash_account"],
+            "sellstock":    self.config["cash_account"],
+            "buyother":     self.config["cash_account"],
+            "sellother":    self.config["cash_account"],
+            "buydebt":      self.config["cash_account"],
+            "reinvest":     self.config["dividends"],
+            "dividends":    self.config["dividends"],
+            "capgainsd_lt": self.config["capgainsd_lt"],
+            "capgainsd_st": self.config["capgainsd_st"],
+            "income":       self.config["interest"],
+            "fee":          self.config["fees"],
+            "invexpense":   self.config.get("invexpense", "ACCOUNT_NOT_CONFIGURED:INVEXPENSE"),
         }
+        # fmt: on
 
-        if 'transfer' in self.config:
-            self.target_account_map.update({
-                "other":    self.config['transfer'],
-                "credit":   self.config['transfer'],
-                "debit":    self.config['transfer'],
-                "transfer": self.config['transfer'],
-                "cash":     self.config['transfer'],
-                "dep":      self.config['transfer'],
-            })
-
-    def build_metadata(self, file, metatype=None, data={}):
-        """This method is for importers to override. The overridden method can
-        look at the metatype ('transaction', 'balance', 'account', 'commodity', etc.)
-        and the data dictionary to return additional metadata"""
-        return {}
+        if "transfer" in self.config:
+            # fmt: off
+            self.target_account_map.update(
+                {
+                    "other":    self.config["transfer"],
+                    "credit":   self.config["transfer"],
+                    "debit":    self.config["transfer"],
+                    "transfer": self.config["transfer"],
+                    "cash":     self.config["transfer"],
+                    "dep":      self.config["transfer"],
+                }
+            )
+            # fmt: on
 
     def custom_init(self):
         if not self.custom_init_run:
             self.max_rounding_error = 0.04
-            self.filename_pattern_def = '.*bank_specific_filename.*'
+            self.filename_pattern_def = ".*bank_specific_filename.*"
             self.custom_init_run = True
 
     def get_ticker_info(self, security_id):
-        return security_id, 'UNKNOWN'
+        return security_id, "UNKNOWN"
 
     def get_ticker_info_from_id(self, security_id):
         try:
             # isin might look like "US293409829" while the ofx use only a substring like "29340982"
             ticker = None
             try:  # first try a full match, fall back to substring
-                ticker, ticker_long_name = [v for k, v in self.funds_db.items() if security_id == k][0]
+                ticker, ticker_long_name = [
+                    v for k, v in self.funds_db.items() if security_id == k
+                ][0]
             except IndexError:
-                ticker, ticker_long_name = [v for k, v in self.funds_db.items() if security_id in k][0]
+                ticker, ticker_long_name = [
+                    v for k, v in self.funds_db.items() if security_id in k
+                ][0]
         except IndexError:
             print(f"Error: fund info not found for {security_id}", file=sys.stderr)
             securities = self.get_security_list()
             securities_missing = [s for s in securities]
             for s in securities:
                 for k in self.funds_db:
                     if s in k:
@@ -185,168 +193,227 @@
         special cases, or return None, which will let get_target_acct() decide the target account"""
         return None
 
     def get_target_acct(self, transaction, ticker):
         target = self.get_target_acct_custom(transaction, ticker)
         if target:
             return target
-        if transaction.type == 'income' and getattr(transaction, 'income_type', None) == 'DIV':
-            return self.target_account_map.get('dividends', None)
+        if transaction.type == "income" and getattr(transaction, "income_type", None) == "DIV":
+            return self.target_account_map.get("dividends", None)
         return self.target_account_map.get(transaction.type, None)
 
     def security_narration(self, ot):
         ticker, ticker_long_name = self.get_ticker_info(ot.security)
         return f"[{ticker}] {ticker_long_name}"
 
     def get_security_list(self):
         tickers = set()
         for ot in self.get_transactions():
-            if hasattr(ot, 'security'):
+            if hasattr(ot, "security"):
                 tickers.add(ot.security)
         return tickers
 
     def subst_acct_vars(self, raw_acct, ot, ticker):
-        """Resolve variables within an account like {ticker}.
-        """
+        """Resolve variables within an account like {ticker}."""
         ot = ot if ot else {}
         # inv401ksource is an ofx field that is 'PRETAX', 'AFTERTAX', etc.
-        kwargs = {'ticker': ticker, 'source401k': getattr(ot, 'inv401ksource', '').title()}
+        kwargs = {
+            "ticker": ticker,
+            "source401k": getattr(ot, "inv401ksource", "").title(),
+        }
         acct = raw_acct.format(**kwargs)
         return self.remove_empty_subaccounts(acct)  # if 'inv401ksource' was unavailable
 
     def get_acct(self, acct, ot, ticker):
-        """Get an account from self.config, resolve variables, and return
-        """
+        """Get an account from self.config, resolve variables, and return"""
         template = self.config.get(acct)
         if not template:
-            raise KeyError(f'{acct} not set in importer configuration. Config: {self.config}')
+            raise KeyError(f"{acct} not set in importer configuration. Config: {self.config}")
         return self.subst_acct_vars(template, ot, ticker)
 
     # extract() and supporting methods
     # --------------------------------------------------------------------------------
 
     def generate_trade_entry(self, ot, file, counter):
-        """ Involves a commodity. One of: ['buymf', 'sellmf', 'buystock', 'sellstock', 'buyother',
+        """Involves a commodity. One of: ['buymf', 'sellmf', 'buystock', 'sellstock', 'buyother',
         'sellother', 'reinvest']"""
 
         config = self.config
         ticker, ticker_long_name = self.get_ticker_info(ot.security)
         is_money_market = ticker in self.money_market_funds
 
         # Build metadata
         metadata = data.new_metadata(file.name, next(counter))
-        metadata.update(self.build_metadata(file, metatype='transaction_trade', data={'transaction': ot}))
-        if getattr(ot, 'settleDate', None) is not None and ot.settleDate != ot.tradeDate:
-            metadata['settlement_date'] = str(ot.settleDate.date())
+        metadata.update(
+            self.build_metadata(file, metatype="transaction_trade", data={"transaction": ot})
+        )
+        if getattr(ot, "settleDate", None) is not None and ot.settleDate != ot.tradeDate:
+            metadata["settlement_date"] = str(ot.settleDate.date())
 
         narration = self.security_narration(ot)
         raw_target_acct = self.get_target_acct(ot, ticker)
         units = ot.units
         total = ot.total
 
         # special cases
-        if 'sell' in ot.type:
+        if "sell" in ot.type:
             units = -1 * abs(ot.units)
             if not is_money_market:
-                metadata['todo'] = 'TODO: this entry is incomplete until lots are selected (bean-doctor context <filename> <lineno>)'  # noqa: E501
-        if ot.type in ['reinvest']:  # dividends are booked to commodity_leaf. Eg: Income:Dividends:HOOLI
+                metadata["todo"] = (
+                    "TODO: this entry is incomplete until lots are selected (bean-doctor context <filename> <lineno>)"  # noqa: E501
+                )
+        if ot.type in [
+            "reinvest"
+        ]:  # dividends are booked to commodity_leaf. Eg: Income:Dividends:HOOLI
             ticker_val = ticker
         else:
             ticker_val = self.currency
         target_acct = self.subst_acct_vars(raw_target_acct, ot, ticker_val)
 
         # Build transaction entry
-        entry = data.Transaction(metadata, ot.tradeDate.date(), self.FLAG,
-                                 self.get_payee(ot), narration,
-                                 self.get_tags(ot), data.EMPTY_SET, [])
+        entry = data.Transaction(
+            metadata,
+            ot.tradeDate.date(),
+            self.FLAG,
+            self.get_payee(ot),
+            narration,
+            self.get_tags(ot),
+            data.EMPTY_SET,
+            [],
+        )
 
         # Main posting(s):
-        main_acct = self.get_acct('main_account', ot, ticker)
+        main_acct = self.get_acct("main_account", ot, ticker)
 
         if is_money_market:  # Use price conversions instead of holding these at cost
-            common.create_simple_posting_with_price(entry, main_acct,
-                                                    units, ticker, ot.unit_price, self.currency)
-        elif 'sell' in ot.type:
-            common.create_simple_posting_with_cost_or_price(entry, main_acct,
-                                                            units, ticker, price_number=ot.unit_price,
-                                                            price_currency=self.currency,
-                                                            costspec=CostSpec(None, None, None, None, None, None))
-            cg_acct = self.get_acct('cg', ot, ticker)
+            common.create_simple_posting_with_price(
+                entry, main_acct, units, ticker, ot.unit_price, self.currency
+            )
+        elif "sell" in ot.type:
+            common.create_simple_posting_with_cost_or_price(
+                entry,
+                main_acct,
+                units,
+                ticker,
+                price_number=ot.unit_price,
+                price_currency=self.currency,
+                costspec=CostSpec(None, None, None, None, None, None),
+            )
+            cg_acct = self.get_acct("cg", ot, ticker)
             data.create_simple_posting(entry, cg_acct, None, None)
         else:  # buy stock/fund
-            unit_price = getattr(ot, 'unit_price', 0)
+            unit_price = getattr(ot, "unit_price", 0)
             # annoyingly, vanguard reinvests have ot.unit_price set to zero. so manually compute it
-            if (hasattr(ot, 'security') and ot.security) and ot.units and not ot.unit_price:
+            if (hasattr(ot, "security") and ot.security) and ot.units and not ot.unit_price:
                 unit_price = round(abs(ot.total) / ot.units, 4)
-            common.create_simple_posting_with_cost(entry, main_acct, units, ticker, unit_price,
-                                                   self.currency, self.price_cost_both_zero_handler)
+            common.create_simple_posting_with_cost(
+                entry,
+                main_acct,
+                units,
+                ticker,
+                unit_price,
+                self.currency,
+                self.price_cost_both_zero_handler,
+            )
 
         # "Other" account posting
         reverser = 1
-        if units > 0 and total > 0:  # (ugly) hack for some brokerages with incorrect signs (TODO: remove)
+        if (
+            units > 0 and total > 0
+        ):  # (ugly) hack for some brokerages with incorrect signs (TODO: remove)
             reverser = -1
         data.create_simple_posting(entry, target_acct, reverser * total, self.currency)
 
         # Rounding errors posting
         rounding_error = (reverser * total) + (ot.unit_price * units)
         if 0.0005 <= abs(rounding_error) <= self.max_rounding_error:
             data.create_simple_posting(
-                entry, config['rounding_error'], -1 * rounding_error, self.currency)
+                entry, config["rounding_error"], -1 * rounding_error, self.currency
+            )
         # if abs(rounding_error) > self.max_rounding_error:
         #     print("Transactions legs do not sum up! Difference: {}. Entry: {}, ot: {}".format(
         #         rounding_error, entry, ot))
 
         return entry
 
     def generate_transfer_entry(self, ot, file, counter):
-        """ Cash transactions, or in-kind transfers. One of:
-            [credit, debit, dep, transfer, income, dividends, capgainsd_lt, capgainsd_st, other]"""
+        """Cash transactions, or in-kind transfers. One of:
+        [credit, debit, dep, transfer, income, dividends, capgainsd_lt, capgainsd_st, other]"""
         config = self.config
         metadata = data.new_metadata(file.name, next(counter))
-        metadata.update(self.build_metadata(file, metatype='transaction_transfer', data={'transaction': ot}))
+        metadata.update(
+            self.build_metadata(file, metatype="transaction_transfer", data={"transaction": ot})
+        )
         ticker = None
-        date = getattr(ot, 'tradeDate', None)
+        date = getattr(ot, "tradeDate", None)
         if not date:
             date = ot.date
         date = date.date()
 
         try:
-            if ot.type in ['transfer']:
+            if ot.type in ["transfer"]:
                 units = ot.units
-            elif ot.type in ['other', 'credit', 'debit', 'dep', 'cash', 'payment', 'check', 'xfer']:
+            elif ot.type in [
+                "other",
+                "credit",
+                "debit",
+                "dep",
+                "cash",
+                "payment",
+                "check",
+                "xfer",
+            ]:
                 units = ot.amount
             else:
                 units = ot.total
         except AttributeError:
             print("Could not determine field for transaction amount")
             # import pdb; pdb.set_trace()
 
         main_acct = None
-        if ot.type in ['income', 'dividends', 'capgainsd_lt',
-                       'capgainsd_st', 'transfer'] and (hasattr(ot, 'security') and ot.security):
+        if ot.type in [
+            "income",
+            "dividends",
+            "capgainsd_lt",
+            "capgainsd_st",
+            "transfer",
+        ] and (hasattr(ot, "security") and ot.security):
             ticker, ticker_long_name = self.get_ticker_info(ot.security)
             narration = self.security_narration(ot)
-            main_acct = self.get_acct('main_account', ot, ticker)
+            main_acct = self.get_acct("main_account", ot, ticker)
         else:  # cash transaction
             narration = ot.type
             ticker = self.currency
-            main_acct = config['cash_account']
+            main_acct = config["cash_account"]
 
         # Build transaction entry
-        entry = data.Transaction(metadata, date, self.FLAG,
-                                 self.get_payee(ot), narration,
-                                 self.get_tags(ot), data.EMPTY_SET, [])
+        entry = data.Transaction(
+            metadata,
+            date,
+            self.FLAG,
+            self.get_payee(ot),
+            narration,
+            self.get_tags(ot),
+            data.EMPTY_SET,
+            [],
+        )
         target_acct = self.get_target_acct(ot, ticker)
         if target_acct:
             target_acct = self.subst_acct_vars(target_acct, ot, ticker)
 
         # Build postings
-        if ot.type in ['income', 'dividends', 'capgainsd_st', 'capgainsd_lt', 'fee']:  # cash
-            amount = ot.total if hasattr(ot, 'total') else ot.amount
-            data.create_simple_posting(entry, config['cash_account'], amount, self.currency)
+        if ot.type in [
+            "income",
+            "dividends",
+            "capgainsd_st",
+            "capgainsd_lt",
+            "fee",
+        ]:  # cash
+            amount = ot.total if hasattr(ot, "total") else ot.amount
+            data.create_simple_posting(entry, config["cash_account"], amount, self.currency)
             data.create_simple_posting(entry, target_acct, -1 * amount, self.currency)
         else:
             data.create_simple_posting(entry, main_acct, units, ticker)
             if target_acct:
                 data.create_simple_posting(entry, target_acct, -1 * units, ticker)
         return entry
 
@@ -367,78 +434,119 @@
         # 'fees': Decimal('0'),
 
         new_entries = []
         self.read_file(file)
         for ot in self.get_transactions():
             if self.skip_transaction(ot):
                 continue
-            if ot.type in ['buymf', 'sellmf', 'buystock', 'buydebt', 'sellstock', 'buyother', 'sellother', 'reinvest']:
+            if ot.type in [
+                "buymf",
+                "sellmf",
+                "buystock",
+                "buydebt",
+                "sellstock",
+                "buyother",
+                "sellother",
+                "reinvest",
+            ]:
                 entry = self.generate_trade_entry(ot, file, counter)
-            elif ot.type in ['other', 'credit', 'debit', 'transfer', 'xfer', 'dep', 'income', 'fee',
-                             'dividends', 'capgainsd_st', 'capgainsd_lt', 'cash', 'payment', 'check', 'invexpense']:
+            elif ot.type in [
+                "other",
+                "credit",
+                "debit",
+                "transfer",
+                "xfer",
+                "dep",
+                "income",
+                "fee",
+                "dividends",
+                "capgainsd_st",
+                "capgainsd_lt",
+                "cash",
+                "payment",
+                "check",
+                "invexpense",
+            ]:
                 entry = self.generate_transfer_entry(ot, file, counter)
             else:
                 print("ERROR: unknown entry type:", ot.type)
-                raise Exception('Unknown entry type')
+                raise Exception("Unknown entry type")
             self.add_fee_postings(entry, ot)
+            self.add_custom_postings(entry, ot)
             new_entries.append(entry)
         return new_entries
 
     def extract_balances_and_prices(self, file, counter):
         new_entries = []
         date = self.get_balance_assertion_date()
 
         settlement_fund_balance = 0
         for pos in self.get_balance_positions():
             ticker, ticker_long_name = self.get_ticker_info(pos.security)
             metadata = data.new_metadata(file.name, next(counter))
-            metadata.update(self.build_metadata(file, metatype='balance', data={'pos': pos}))
+            metadata.update(self.build_metadata(file, metatype="balance", data={"pos": pos}))
 
             # if there are no transactions, use the date in the source file for the balance. This gives us the
             # bonus of an updated, recent balance assertion
             bal_date = date if date else pos.date.date()
-            main_acct = self.get_acct('main_account', None, ticker)
-            balance_entry = data.Balance(metadata, bal_date, main_acct,
-                                         amount.Amount(pos.units, ticker),
-                                         None, None)
+            main_acct = self.get_acct("main_account", None, ticker)
+            balance_entry = data.Balance(
+                metadata,
+                bal_date,
+                main_acct,
+                amount.Amount(pos.units, ticker),
+                None,
+                None,
+            )
             new_entries.append(balance_entry)
             if ticker in self.money_market_funds:
                 settlement_fund_balance = pos.units
 
             # extract price info if available
-            if hasattr(pos, 'unit_price') and hasattr(pos, 'date'):
+            if hasattr(pos, "unit_price") and hasattr(pos, "date"):
                 metadata = data.new_metadata(file.name, next(counter))
-                metadata.update(self.build_metadata(file, metatype='price', data={'pos': pos}))
-                price_entry = data.Price(metadata, pos.date.date(), ticker,
-                                         amount.Amount(pos.unit_price, self.currency))
+                metadata.update(self.build_metadata(file, metatype="price", data={"pos": pos}))
+                price_entry = data.Price(
+                    metadata,
+                    pos.date.date(),
+                    ticker,
+                    amount.Amount(pos.unit_price, self.currency),
+                )
                 new_entries.append(price_entry)
 
         # ----------------- available cash
         available_cash = self.get_available_cash(settlement_fund_balance)
         if available_cash is not None:
             metadata = data.new_metadata(file.name, next(counter))
-            metadata.update(self.build_metadata(file, metatype='balance_cash'))
+            metadata.update(self.build_metadata(file, metatype="balance_cash"))
             try:
-                bal_date = date if date else self.file_date(file).date()  # unavailable file_date raises AttributeError
-                balance_entry = data.Balance(metadata, bal_date, self.config['cash_account'],
-                                             amount.Amount(available_cash, self.currency),
-                                             None, None)
+                bal_date = (
+                    date if date else self.file_date(file).date()
+                )  # unavailable file_date raises AttributeError
+                balance_entry = data.Balance(
+                    metadata,
+                    bal_date,
+                    self.config["cash_account"],
+                    amount.Amount(available_cash, self.currency),
+                    None,
+                    None,
+                )
                 new_entries.append(balance_entry)
             except AttributeError:
                 pass
 
         return new_entries
 
     def add_fee_postings(self, entry, ot):
         config = self.config
-        if hasattr(ot, 'fees') or hasattr(ot, 'commission'):
-            if getattr(ot, 'fees', 0) != 0:
-                data.create_simple_posting(entry, config['fees'], ot.fees, self.currency)
-            if getattr(ot, 'commission', 0) != 0:
-                data.create_simple_posting(entry, config['fees'], ot.commission, self.currency)
+        if hasattr(ot, "fees") or hasattr(ot, "commission"):
+            if getattr(ot, "fees", 0) != 0:
+                data.create_simple_posting(entry, config["fees"], ot.fees, self.currency)
+            if getattr(ot, "commission", 0) != 0:
+                data.create_simple_posting(entry, config["fees"], ot.commission, self.currency)
 
     def extract_custom_entries(self, file, counter):
         """For custom importers to override"""
         return []
 
     def extract(self, file, existing_entries=None):
         self.initialize(file)
```

### Comparing `beancount_reds_importers-0.8.0/beancount_reds_importers/libtransactionbuilder/paycheck.py` & `beancount_reds_importers-0.9.0/beancount_reds_importers/libtransactionbuilder/paycheck.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """Generic banking ofx importer for beancount."""
 
+from collections import defaultdict
+
 from beancount.core import data
 from beancount.core.number import D
-from beancount_reds_importers.libtransactionbuilder import banking
 
+from beancount_reds_importers.libtransactionbuilder import banking
 
 # paychecks are typically transaction with many (10-40) postings including several each of income, taxes,
 # pre-tax and post-tax deductions, transfers, reimbursements, etc. This importer enables importing a single
 # paycheck, resulting in a single transaction. The source can be a pdf that has been turned to text, or a .csv
 # or .xlsx, or another format. The input specification is a dictionary corresponding to various sections of a
 # paycheck and the text in them to match. For example:
 
@@ -46,74 +48,98 @@
 #         },
 #
 #         'Deductions': {
 #             "..." : "...",
 #         },
 # }
 
+
 def flip_if_needed(amount, account):
-    if amount >= 0 and any(account.startswith(prefix) for prefix in ['Income:', 'Equity:', 'Liabilities:']):
+    if amount >= 0 and any(
+        account.startswith(prefix) for prefix in ["Income:", "Equity:", "Liabilities:"]
+    ):
         amount *= -1
-    if amount < 0 and any(account.startswith(prefix) for prefix in ['Expenses:', 'Assets:']):
+    if amount < 0 and any(account.startswith(prefix) for prefix in ["Expenses:", "Assets:"]):
         amount *= -1
     return amount
 
 
 class Importer(banking.Importer):
     def file_date(self, input_file):
         return self.paycheck_date(input_file)
 
     def build_postings(self, entry):
-        template = self.config['paycheck_template']
-        currency = self.config['currency']
+        template = self.config["paycheck_template"]
+        currency = self.config["currency"]
         total = 0
+        template_missing = defaultdict(set)
 
         for section, table in self.alltables.items():
             if section not in template:
+                template_missing[section] = set()
                 continue
             for row in table.namedtuples():
                 # TODO: 'bank' is workday specific; move it there
-                row_description = getattr(row, 'description', getattr(row, 'bank', None))
-                row_pattern = next(filter(lambda ts: row_description.startswith(ts), template[section]), None)
-                if row_pattern:
+                row_description = getattr(row, "description", getattr(row, "bank", None))
+                row_pattern = next(
+                    filter(lambda ts: row_description.startswith(ts), template[section]),
+                    None,
+                )
+                if not row_pattern:
+                    template_missing[section].add(row_description)
+                else:
                     accounts = template[section][row_pattern]
                     accounts = [accounts] if not isinstance(accounts, list) else accounts
                     for account in accounts:
                         # TODO: 'amount_in_pay_group_currency' is workday specific; move it there
-                        amount = getattr(row, 'amount', getattr(row, 'amount_in_pay_group_currency', None))
+                        amount = getattr(
+                            row,
+                            "amount",
+                            getattr(row, "amount_in_pay_group_currency", None),
+                        )
                         # import pdb; pdb.set_trace()
 
                         if not amount:
                             continue
                         amount = D(amount)
                         amount = flip_if_needed(amount, account)
                         total += amount
                         if amount:
                             data.create_simple_posting(entry, account, amount, currency)
+
+        if self.config.get("show_unconfigured", False):
+            for section in template_missing:
+                print(section)
+                if template_missing[section]:
+                    print("  " + "\n  ".join(i for i in template_missing[section]))
+                print()
+
         if total != 0:
             data.create_simple_posting(entry, "TOTAL:NONZERO", total, currency)
 
-        if self.config.get('sort_postings', True):
+        if self.config.get("sort_postings", True):
             postings = sorted(entry.postings)
         else:
             postings = entry.postings
         newentry = entry._replace(postings=postings)
         return newentry
 
-    def build_metadata(self, file, metatype=None, data={}):
-        """This method is for importers to override. The overridden method can
-        look at the metatype ('transaction', 'balance', 'account', 'commodity', etc.)
-        and the data dictionary to return additional metadata"""
-        return {}
-
     def extract(self, file, existing_entries=None):
         self.initialize(file)
         config = self.config
 
         self.read_file(file)
         metadata = data.new_metadata(file.name, 0)
-        metadata.update(self.build_metadata(file, metatype='transaction'))
-        entry = data.Transaction(metadata, self.paycheck_date(file), self.FLAG,
-                                 None, config['desc'], self.get_tags(), data.EMPTY_SET, [])
+        metadata.update(self.build_metadata(file, metatype="transaction"))
+        entry = data.Transaction(
+            metadata,
+            self.paycheck_date(file),
+            self.FLAG,
+            None,
+            config["desc"],
+            self.get_tags(),
+            data.EMPTY_SET,
+            [],
+        )
 
         entry = self.build_postings(entry)
         return [entry]
```

### Comparing `beancount_reds_importers-0.8.0/beancount_reds_importers/libtransactionbuilder/transactionbuilder.py` & `beancount_reds_importers-0.9.0/beancount_reds_importers/libtransactionbuilder/transactionbuilder.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,41 +1,60 @@
 """Transaction builder module base class Transaction builders such as the investment, banking, and
 paycheck inherit this."""
 
 from beancount.core import data
 
 
-class TransactionBuilder():
+class TransactionBuilder:
     def skip_transaction(self, ot):
         """For custom importers to override"""
         return False
 
     def get_tags(self, ot=None):
         """For custom importers to override"""
         return data.EMPTY_SET
 
     @staticmethod
     def remove_empty_subaccounts(acct):
         """Translates 'Assets:Foo::Bar' to 'Assets:Foo:Bar'."""
-        return ':'.join(x for x in acct.split(':') if x)
+        return ":".join(x for x in acct.split(":") if x)
 
     def set_config_variables(self, substs):
         """
         Replaces {} strings in config with substitutions specified in a dictionary (substs)
 
         Eg: replaces 'Assets:Broker:{currency}' with 'Assets:Broker:USD'
 
         substs is the substitution dictionary. For example:
         substs = { 'currency': self.currency,
                   # Leave the other values as is
                   'ticker': '{ticker}',
                   'source401k': '{source401k}',
                   }
         """
-        self.config = {k: v.format(**substs) if isinstance(v, str) else v for k, v in self.config.items()}
+        self.config = {
+            k: v.format(**substs) if isinstance(v, str) else v for k, v in self.config.items()
+        }
 
         # Prevent the replacement fields from appearing in the output of
         # the file_account method
-        if 'filing_account' not in self.config:
-            kwargs = {k: '' for k in substs}
-            filing_account = self.config['main_account'].format(**kwargs)
-            self.config['filing_account'] = self.remove_empty_subaccounts(filing_account)
+        if "filing_account" not in self.config:
+            kwargs = {k: "" for k in substs}
+            filing_account = self.config["main_account"].format(**kwargs)
+            self.config["filing_account"] = self.remove_empty_subaccounts(filing_account)
+
+    def add_custom_postings(self, entry, ot):
+        """This method is for importers to override. Add arbitrary posting to each entry."""
+        pass
+
+    def build_metadata(self, file, metatype=None, data={}):
+        """This method is for importers to override. The overridden method can
+        look at the metatype ('transaction', 'balance', 'account', 'commodity', etc.)
+        and the data dictionary to return additional metadata"""
+
+        # This 'filing_account' is read by a patch to bean-extract so it can output transactions to
+        # a file that corresponds with filing_account, when the one-file-per-account feature is
+        # used.
+        if self.config.get("emit_filing_account_metadata"):
+            acct = self.config.get("filing_account", self.config.get("main_account", None))
+            return {"filing_account": acct}
+        return {}
```

### Comparing `beancount_reds_importers-0.8.0/beancount_reds_importers/util/bean_download.py` & `beancount_reds_importers-0.9.0/beancount_reds_importers/util/bean_download.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 #!/usr/bin/env python3
 """Download account statements automatically when possible, or display a reminder of how to download them.
 Multi-threaded."""
 
-from click_aliases import ClickAliasedGroup
 import asyncio
-import click
 import configparser
 import os
+
+import click
 import tabulate
 import tqdm
+from click_aliases import ClickAliasedGroup
+
 import beancount_reds_importers.util.needs_update as needs_update
 
 
 @click.group(cls=ClickAliasedGroup)
 def cli():
     """Download account statements automatically when possible, or display a reminder of how to download them.
     Multi-threaded."""
@@ -26,116 +28,137 @@
     config = configparser.ConfigParser()
     # config.optionxform = str # makes config file case sensitive
     config.read(os.path.expandvars(configfile))
     return config
 
 
 def get_sites(sites, t, config):
-    return [s for s in sites if config[s]['type'] == t]
+    return [s for s in sites if config[s]["type"] == t]
 
 
-@cli.command(aliases=['list'])
-@click.option('-c', '--config-file', envvar='BEAN_DOWNLOAD_CONFIG', required=True,
-              help='Config file. The environment variable BEAN_DOWNLOAD_CONFIG can also be used to specify this',
-              type=click.Path(exists=True))
-@click.option('-s', '--sort', is_flag=True, help='Sort output')
+@cli.command(aliases=["list"])
+@click.option(
+    "-c",
+    "--config-file",
+    envvar="BEAN_DOWNLOAD_CONFIG",
+    required=True,
+    help="Config file. The environment variable BEAN_DOWNLOAD_CONFIG can also be used to specify this",
+    type=click.Path(exists=True),
+)
+@click.option("-s", "--sort", is_flag=True, help="Sort output")
 def list_institutions(config_file, sort):
     """List institutions (sites) currently configured."""
     config = readConfigFile(config_file)
     all_sites = config.sections()
-    types = set([config[s]['type'] for s in all_sites])
+    types = set([config[s]["type"] for s in all_sites])
     for t in sorted(types):
         sites = get_sites(all_sites, t, config)
         if sort:
             sites = sorted(sites)
         name = f"{t} ({len(sites)})".ljust(14)
-        print(f"{name}:", end='')
-        print(*sites, sep=', ')
+        print(f"{name}:", end="")
+        print(*sites, sep=", ")
         print()
 
 
 def get_sites_and_sections(config_file):
     if config_file and os.path.exists(config_file):
         config = readConfigFile(config_file)
         all_sites = config.sections()
-        types = set([config[s]['type'] for s in all_sites])
+        types = set([config[s]["type"] for s in all_sites])
     return all_sites, types
 
 
 def complete_sites(ctx, param, incomplete):
-    config_file = ctx.params['config_file']
+    config_file = ctx.params["config_file"]
     all_sites, _ = get_sites_and_sections(config_file)
     return [s for s in all_sites if s.startswith(incomplete)]
 
 
 def complete_site_types(ctx, param, incomplete):
-    config_file = ctx.params['config_file']
+    config_file = ctx.params["config_file"]
     _, types = get_sites_and_sections(config_file)
     return [s for s in types if s.startswith(incomplete)]
 
 
 @cli.command()
-@click.option('-c', '--config-file', envvar='BEAN_DOWNLOAD_CONFIG', required=True, help='Config file')
-@click.option('-i', '--sites', '--institutions', help="Institutions to download (comma separated); unspecified means all",
-              default='', shell_complete=complete_sites)
-@click.option('-t', '--site-types', '--institution-types',
-              help="Download all institutions of specified types (comma separated)",
-              default='', shell_complete=complete_site_types)
-@click.option('--dry-run', is_flag=True, help="Do not actually download", default=False)
-@click.option('--verbose', is_flag=True, help="Verbose", default=False)
+@click.option(
+    "-c",
+    "--config-file",
+    envvar="BEAN_DOWNLOAD_CONFIG",
+    required=True,
+    help="Config file",
+)
+@click.option(
+    "-i",
+    "--sites",
+    "--institutions",
+    help="Institutions to download (comma separated); unspecified means all",
+    default="",
+    shell_complete=complete_sites,
+)
+@click.option(
+    "-t",
+    "--site-types",
+    "--institution-types",
+    help="Download all institutions of specified types (comma separated)",
+    default="",
+    shell_complete=complete_site_types,
+)
+@click.option("--dry-run", is_flag=True, help="Do not actually download", default=False)
+@click.option("--verbose", is_flag=True, help="Verbose", default=False)
 def download(config_file, sites, site_types, dry_run, verbose):  # noqa: C901
     """Download statements for the specified institutions (sites)."""
 
     def pverbose(*args, **kwargs):
         if verbose:
             print(*args, **kwargs)
 
     config = readConfigFile(config_file)
     if sites:
-        sites = sites.split(',')
+        sites = sites.split(",")
     else:
         sites = config.sections()
         if site_types:
-            site_types = site_types.split(',')
+            site_types = site_types.split(",")
             sites_lists = [get_sites(sites, site_type, config) for site_type in site_types]
             sites = [j for i in sites_lists for j in i]
 
     errors = []
     success = []
     numsites = len(sites)
     displays = []
     print(f"Processing {numsites} institutions.")
 
     async def download_site(i, site):
-        tid = f'[{i+1}/{numsites} {site}]'
-        pverbose(f'{tid}: Begin')
+        tid = f"[{i+1}/{numsites} {site}]"
+        pverbose(f"{tid}: Begin")
         try:
             options = config[site]
         except KeyError:
             errors.append(site)
             displays.append([site, f"Couldn't find {site} in {config_file}"])
             return
 
         # We support cmd and display, and type to filter
-        if 'display' in options:
+        if "display" in options:
             displays.append([site, f"{options['display']}"])
             success.append(site)
-        if 'cmd' in options:
-            cmd = os.path.expandvars(options['cmd'])
+        if "cmd" in options:
+            cmd = os.path.expandvars(options["cmd"])
             pverbose(f"{tid}: Executing: {cmd}")
             if dry_run:
                 await asyncio.sleep(2)
                 success.append(site)
                 pverbose(f"{tid}: Success")
             else:
                 # https://docs.python.org/3.8/library/asyncio-subprocess.html#asyncio.create_subprocess_exec
                 proc = await asyncio.create_subprocess_shell(
-                    cmd,
-                    stdout=asyncio.subprocess.PIPE,
-                    stderr=asyncio.subprocess.PIPE)
+                    cmd, stdout=asyncio.subprocess.PIPE, stderr=asyncio.subprocess.PIPE
+                )
                 stdout, stderr = await proc.communicate()
 
                 if proc.returncode:
                     errors.append(site)
                 else:
                     success.append(site)
                     pverbose(f"{tid}: Success")
@@ -146,30 +169,34 @@
             await t
 
     asyncio.run(perform_downloads(sites))
 
     if displays:
         print()
         displays = [[i + 1, *row] for i, row in enumerate(displays)]
-        click.secho(tabulate.tabulate(displays,
-                    headers=["#", "Institution", "Instructions"], tablefmt="plain"), fg='blue')
+        click.secho(
+            tabulate.tabulate(
+                displays, headers=["#", "Institution", "Instructions"], tablefmt="plain"
+            ),
+            fg="blue",
+        )
         print()
 
     s = len(sites)
     if success:
         print(f"{len(success)}/{s} sites succeeded: {', '.join(success)}")
     if errors:
-        click.secho(f"{len(errors)}/{s} sites failed:    {', '.join(errors)}", fg='red')
+        click.secho(f"{len(errors)}/{s} sites failed:    {', '.join(errors)}", fg="red")
 
 
-@cli.command(aliases=['init'])
+@cli.command(aliases=["init"])
 def config_template():
     """Output a template for download.cfg that you can then use to build your own."""
 
     path = os.path.dirname(os.path.realpath(__file__))
-    with open(os.path.join(*[path, 'template.cfg'])) as f:
+    with open(os.path.join(*[path, "template.cfg"])) as f:
         for line in f:
-            print(line, end='')
+            print(line, end="")
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     cli()
```

### Comparing `beancount_reds_importers-0.8.0/beancount_reds_importers/util/needs_update.py` & `beancount_reds_importers-0.9.0/beancount_reds_importers/util/needs_update.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,61 +1,63 @@
 #!/usr/bin/env python3
 """Determine the list of accounts needing updates based on the last balance entry."""
 
-import click
+import ast
 import re
+from datetime import datetime
+
+import click
 import tabulate
 from beancount import loader
 from beancount.core import getters
 from beancount.core.data import Balance, Close, Custom
-from datetime import datetime
-import ast
 
-
-tbl_options = {'tablefmt': 'simple'}
+tbl_options = {"tablefmt": "simple"}
 
 
 def get_config(entries, args):
     """Get beancount config for the given plugin that can then be used on the command line"""
     global excluded_re, included_re
-    _extension_entries = [e for e in entries
-                          if isinstance(e, Custom) and e.type == 'reds-importers']
-    config_meta = {entry.values[0].value:
-                   (entry.values[1].value if (len(entry.values) == 2) else None)
-                   for entry in _extension_entries}
-
-    config = {k: ast.literal_eval(v) for k, v in config_meta.items() if 'needs-updates' in k}
-    config = config.get('needs-updates', {})
-    if args['all_accounts']:
-        config['included_account_pats'] = []
-        config['excluded_account_pats'] = ['$-^']
-    included_account_pats = config.get('included_account_pats', ['^Assets:', '^Liabilities:'])
-    excluded_account_pats = config.get('excluded_account_pats', ['$-^'])  # exclude nothing by default
-    excluded_re = re.compile('|'.join(excluded_account_pats))
-    included_re = re.compile('|'.join(included_account_pats))
+    _extension_entries = [
+        e for e in entries if isinstance(e, Custom) and e.type == "reds-importers"
+    ]
+    config_meta = {
+        entry.values[0].value: (entry.values[1].value if (len(entry.values) == 2) else None)
+        for entry in _extension_entries
+    }
+
+    config = {k: ast.literal_eval(v) for k, v in config_meta.items() if "needs-updates" in k}
+    config = config.get("needs-updates", {})
+    if args["all_accounts"]:
+        config["included_account_pats"] = []
+        config["excluded_account_pats"] = ["$-^"]
+    included_account_pats = config.get("included_account_pats", ["^Assets:", "^Liabilities:"])
+    excluded_account_pats = config.get(
+        "excluded_account_pats", ["$-^"]
+    )  # exclude nothing by default
+    excluded_re = re.compile("|".join(excluded_account_pats))
+    included_re = re.compile("|".join(included_account_pats))
 
 
 def is_interesting_account(account, closes):
-    return account not in closes and \
-           included_re.match(account) and \
-           not excluded_re.match(account)
+    return account not in closes and included_re.match(account) and not excluded_re.match(account)
 
 
 def handle_commodity_leaf_accounts(last_balance):
     """
     Handle commodity leaf accounts. If an account ends with all capital letters, it is a
     commodity leaf. Eg: Assets:Investments:Etrade:AAPL
 
     Commodity leaf accounts are ascribed to their parent. The parent's last updated date is
     considered to be the latest date of a balance assertion on any child.
     """
     d = {}
-    pat_ticker = re.compile(r'^[A-Z0-9]+$')
+    pat_ticker = re.compile(r"^[A-Z0-9]+$")
     for acc in last_balance:
-        parent, leaf = acc.rsplit(':', 1)
+        parent, leaf = acc.rsplit(":", 1)
         if pat_ticker.match(leaf):
             if parent in d:
                 if d[parent].date < last_balance[acc].date:
                     d[parent] = last_balance[acc]
             else:
                 d[parent] = last_balance[acc]
         else:
@@ -68,41 +70,52 @@
     accounts = getters.get_accounts(entries)
     asset_accounts = [a for a in accounts if is_interesting_account(a, closes)]
     accs_no_bal_raw = [a for a in asset_accounts if a not in last_balance]
 
     # Handle commodity leaf accounts
     accs_no_bal = []
 
-    pat_ticker = re.compile(r'^[A-Z0-9]+$')
+    pat_ticker = re.compile(r"^[A-Z0-9]+$")
 
     def acc_or_parent(acc):
-        parent, leaf = acc.rsplit(':', 1)
+        parent, leaf = acc.rsplit(":", 1)
         if pat_ticker.match(leaf):
             return parent
         return acc
+
     accs_no_bal = [acc_or_parent(i) for i in accs_no_bal_raw]
 
     # Remove accounts where one or more children do have a balance entry. Needed because of
     # commodity leaf accounts
-    accs_no_bal = [(i,) for i in set(accs_no_bal) if not any(j.startswith(i) for j in last_balance)]
+    accs_no_bal = [
+        (i,) for i in set(accs_no_bal) if not any(j.startswith(i) for j in last_balance)
+    ]
     return accs_no_bal
 
 
 def pretty_print_table(not_updated_accounts, sort_by_date):
     field = 0 if sort_by_date else 1
     output = sorted([(v.date, k) for k, v in not_updated_accounts.items()], key=lambda x: x[field])
-    headers = ['Last Updated', 'Account']
+    headers = ["Last Updated", "Account"]
     print(click.style(tabulate.tabulate(output, headers=headers, **tbl_options)))
 
 
-@click.command("needs-update", context_settings={'show_default': True})
-@click.argument('beancount-file', type=click.Path(exists=True), envvar='BEANCOUNT_FILE')
-@click.option('--recency', help='How many days ago should the last balance assertion be to be considered old', default=15)
-@click.option('--sort-by-date', help='Sort output by date (instead of account name)', is_flag=True)
-@click.option('--all-accounts', help='Show all account (ignore include/exclude in config)', is_flag=True)
+@click.command("needs-update", context_settings={"show_default": True})
+@click.argument("beancount-file", type=click.Path(exists=True), envvar="BEANCOUNT_FILE")
+@click.option(
+    "--recency",
+    help="How many days ago should the last balance assertion be to be considered old",
+    default=15,
+)
+@click.option("--sort-by-date", help="Sort output by date (instead of account name)", is_flag=True)
+@click.option(
+    "--all-accounts",
+    help="Show all account (ignore include/exclude in config)",
+    is_flag=True,
+)
 def accounts_needing_updates(beancount_file, recency, sort_by_date, all_accounts):
     """
     Show a list of accounts needing updates, and the date of the last update (which is defined as
     the date of the last balance assertion on the account).
 
     Only accounts in the included list which are not in the excluded list are considered. Both
     lists are specified as regular expressions. These can be used to include only accounts
@@ -137,25 +150,34 @@
        'excluded_account_pats' : []
      }}"
     """
 
     entries, _, _ = loader.load_file(beancount_file)
     get_config(entries, locals())
     closes = [a.account for a in entries if isinstance(a, Close)]
-    balance_entries = [a for a in entries if isinstance(a, Balance) and
-                       is_interesting_account(a.account, closes)]
+    balance_entries = [
+        a for a in entries if isinstance(a, Balance) and is_interesting_account(a.account, closes)
+    ]
     last_balance = {v.account: v for v in balance_entries}
     d = handle_commodity_leaf_accounts(last_balance)
 
     # find accounts with balance assertions older than N days
-    need_updates = {acc: bal for acc, bal in d.items() if ((datetime.now().date() - d[acc].date).days > recency)}
+    need_updates = {
+        acc: bal
+        for acc, bal in d.items()
+        if ((datetime.now().date() - d[acc].date).days > recency)
+    }
     pretty_print_table(need_updates, sort_by_date)
 
     # If there are accounts with zero balance entries, print them
     accs_no_bal = accounts_with_no_balance_entries(entries, closes, last_balance)
     if accs_no_bal:
-        headers = ['Accounts without balance entries:']
-        print(click.style('\n' + tabulate.tabulate(sorted(accs_no_bal), headers=headers, **tbl_options)))
+        headers = ["Accounts without balance entries:"]
+        print(
+            click.style(
+                "\n" + tabulate.tabulate(sorted(accs_no_bal), headers=headers, **tbl_options)
+            )
+        )
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     accounts_needing_updates()
```

### Comparing `beancount_reds_importers-0.8.0/beancount_reds_importers/util/ofx_summarize.py` & `beancount_reds_importers-0.9.0/beancount_reds_importers/util/ofx_summarize.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,43 @@
 #!/usr/bin/env python3
 """Quick and dirty way to summarize a .ofx file and peek inside it."""
 
-import click
 import os
 import sys
+import warnings
 from collections import defaultdict
-from ofxparse import OfxParser
+
+import click
 from bs4.builder import XMLParsedAsHTMLWarning
-import warnings
+from ofxparse import OfxParser
+
 warnings.filterwarnings("ignore", category=XMLParsedAsHTMLWarning)
 
 
-def analyze(filename, ttype='dividends', pdb_explore=False):
+def analyze(filename, ttype="dividends", pdb_explore=False):
     ts = defaultdict(list)
     ofx = OfxParser.parse(open(filename))
     for acc in ofx.accounts:
         for t in acc.statement.transactions:
             ts[t.type].append(t)
     if pdb_explore:
         import pdb
+
         pdb.set_trace()
 
 
 @click.command()
-@click.argument('filename', type=click.Path(exists=True))
-@click.option('-n', '--num-transactions', default=5, help='Number of transactions to show')
-@click.option('-e', '--pdb-explore', is_flag=True, help='Open a pdb shell to explore')
-@click.option('--stats-only', is_flag=True, help='Print total number of transactions contained in the file, and quit')
+@click.argument("filename", type=click.Path(exists=True))
+@click.option("-n", "--num-transactions", default=5, help="Number of transactions to show")
+@click.option("-e", "--pdb-explore", is_flag=True, help="Open a pdb shell to explore")
+@click.option(
+    "--stats-only",
+    is_flag=True,
+    help="Print total number of transactions contained in the file, and quit",
+)
 def summarize(filename, pdb_explore, num_transactions, stats_only):  # noqa: C901
     """Quick and dirty way to summarize a .ofx file and peek inside it."""
     if os.stat(filename).st_size == 0:
         if stats_only:
             print(0)
             sys.exit(0)
         else:
@@ -41,49 +48,66 @@
     if stats_only:
         total_txns = sum([len(acc.statement.transactions) for acc in ofx.accounts])
         # print("{{'num_accounts' : {}, 'total_transactions' : {}}}".format(len(ofx.accounts), total_txns))
         print(total_txns)
         sys.exit(0)
     print("Total number of accounts:", len(ofx.accounts))
     for acc in ofx.accounts:
-        print('----------------')
+        print("----------------")
         try:
-            print("Account info: ", acc.account_type, acc.account_id, acc.institution.organization)
+            print(
+                "Account info: ",
+                acc.account_type,
+                acc.account_id,
+                acc.institution.organization,
+            )
         except AttributeError:
             print("Account info: ", acc.account_type, acc.account_id)
             pass
 
         try:
-            print("Statement info: {} -- {}. Bal: {}".format(acc.statement.start_date,
-                  acc.statement.end_date, acc.statement.balance))
+            print(
+                "Statement info: {} -- {}. Bal: {}".format(
+                    acc.statement.start_date,
+                    acc.statement.end_date,
+                    acc.statement.balance,
+                )
+            )
         except AttributeError:
             try:
                 positions = [(p.units, p.security) for p in acc.statement.positions]
-                print("Statement info: {} -- {}. Bal: {}".format(acc.statement.start_date,
-                      acc.statement.end_date, positions))
+                print(
+                    "Statement info: {} -- {}. Bal: {}".format(
+                        acc.statement.start_date, acc.statement.end_date, positions
+                    )
+                )
             except AttributeError:
                 print("Statement info: UNABLE to get start_date and end_date")
 
         print("Types: ", set([t.type for t in acc.statement.transactions]))
 
         print()
-        txns = sorted(acc.statement.transactions, reverse=True,
-                      key=lambda t: t.date if hasattr(t, 'date') else t.tradeDate)
+        txns = sorted(
+            acc.statement.transactions,
+            reverse=True,
+            key=lambda t: t.date if hasattr(t, "date") else t.tradeDate,
+        )
         for t in txns[:num_transactions]:
-            date = t.date if hasattr(t, 'date') else t.tradeDate
-            description = t.payee + ' ' + t.memo if hasattr(t, 'payee') else t.memo
-            amount = t.amount if hasattr(t, 'amount') else t.total
+            date = t.date if hasattr(t, "date") else t.tradeDate
+            description = t.payee + " " + t.memo if hasattr(t, "payee") else t.memo
+            amount = t.amount if hasattr(t, "amount") else t.total
             print(date, t.type, description, amount)
         if pdb_explore:
             print("Hints:")
             print("- try dir(acc), dir(acc.statement.transactions)")
             print("- try the 'interact' command to start an interactive python interpreter")
             if len(ofx.accounts) > 1:
                 print("- type 'c' to explore the next account in this file")
             import pdb
+
             pdb.set_trace()
         print()
         print()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     summarize()
```

### Comparing `beancount_reds_importers-0.8.0/beancount_reds_importers/util/template.cfg` & `beancount_reds_importers-0.9.0/beancount_reds_importers/util/template.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 [DEFAULT]
 ofx_pre = pass show dummy > /dev/null; ofxget stmt --nokeyring -u
 downloads_dir = ~/Downloads
 
 [fidelity]
-type = ofxget
+type = investment
 cmd = %(ofx_pre)s <your_username>             \
        --useragent randomstring              \
        --password $(pass financial/fidelity) \
        fidelity                              \
        -i <accnum1>                          \
        -i <accnum2>                          \
        > %(downloads_dir)s/fidelity.ofx
 
 [fidelity_netbenefits]
-type = ofxget
+type = retirement
 cmd = %(ofx_pre)s <your_username> \
        --useragent randomstring     \
        --password $(pass financial/netbenefits) netbenefits -i <acc_num> \
        > %(downloads_dir)s/fidelity_netbenefits.ofx
 
 # chase requires same clientuid, unique to the account.
 [chase]
-type = ofxget
+type = creditcard
 cmd = %(ofx_pre)s <your_username> \
        --password $(pass financial/chase) \
        --clientuid DAB2934E-A112-2309-BCD2-ABCD12345678 chase --all \
        > %(downloads_dir)s/chase.ofx
 
 [etrade]
 type = investment
@@ -35,7 +35,13 @@
 
 # Setting type to 'manual' makes bean-download simply display the reminder message below
 # instead of actually downloading a .ofx
 [amazon_purchases]
 type = manual
 display = "Submit via: https://www.amazon.com/gp/privacycentral/dsar/preview.html"
 comment = "Internet-search for Request My Data, choose my orders. Last updated: 2022-02-22"
+
+[tdameritrade]
+type = investment
+cmd = %(ofx_pre)s <your_username> \
+     --password $(pass financial/tdameritrade) ameritrade -i <acc_num> \
+     > %(downloads_dir)s/tdameritrade.ofx
```

### Comparing `beancount_reds_importers-0.8.0/beancount_reds_importers.egg-info/PKG-INFO` & `beancount_reds_importers-0.9.0/beancount_reds_importers.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: beancount-reds-importers
-Version: 0.8.0
+Name: beancount_reds_importers
+Version: 0.9.0
 Summary: Importers for various institutions for Beancount
 Home-page: https://github.com/redstreet/beancount_reds_importers
 Author: Red Street
 Author-email: redstreet@users.noreply.github.com
 License: GPL-3.0
 Keywords: importer ingestor beancount accounting
 Classifier: Development Status :: 4 - Beta
@@ -16,20 +16,25 @@
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Click>=7.0
 Requires-Dist: beancount>=2.3.5
 Requires-Dist: click_aliases>=1.0.1
+Requires-Dist: dateparser>=1.2.0
 Requires-Dist: ofxparse>=0.21
 Requires-Dist: openpyxl>=3.0.9
 Requires-Dist: packaging>=20.3
+Requires-Dist: pdfplumber>=0.11.0
 Requires-Dist: petl>=1.7.4
 Requires-Dist: tabulate>=0.8.9
 Requires-Dist: tqdm>=4.64.0
+Provides-Extra: dev
+Requires-Dist: ruff; extra == "dev"
+Requires-Dist: isort; extra == "dev"
 
 # Beancount Red's Importers
 
 Simple importers and tools for [Beancount](https://beancount.github.io/), software for
 [plain text](https://plaintextaccounting.org/), double entry bookkeeping. _More
 importantly, a framework to allow you to easily write your own importers._
 
@@ -158,16 +163,20 @@
 - `last_transaction`: max transaction date
 - `today`:            today's date
 
 If you want something else, simply override this method in individual importer
 
 `smart` dates: Banks and credit cards typically have pending transactions that are not
 included in downloads. When we download the next statement, new transactions may appear
-prior to the balance assertion date that we generate for this statement. To attempt to
-avoid this, we set the balance assertion date to either two days (fudge factor to
+prior to the balance assertion date that we generate for this statement, which renders
+this balance assertion invalid. This problem manifests occasionally as an existing
+balance statement breaking  when a new statement is downloaded and is an annoyance as it
+needs manual fixing.
+
+To minimize this, we set the balance assertion date to either two days (fudge factor to
 account for pending transactions) before the statement's end date or the last
 transaction's date, whichever is later. To choose a different fudge factor, simply set
 `balance_assertion_date_fudge` in your config.
 
 
 ### Note
```

### Comparing `beancount_reds_importers-0.8.0/beancount_reds_importers.egg-info/SOURCES.txt` & `beancount_reds_importers-0.9.0/beancount_reds_importers.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 .gitignore
 CHANGELOG.md
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.md
 conftest.py
+pyproject.toml
 requirements.txt
 setup.py
+.github/workflows/conventionalcommits.yml
 .github/workflows/pythonpackage.yml
 .github/workflows/pythonpublish.yml
 beancount_reds_importers/__init__.py
 beancount_reds_importers.egg-info/PKG-INFO
 beancount_reds_importers.egg-info/SOURCES.txt
 beancount_reds_importers.egg-info/dependency_links.txt
 beancount_reds_importers.egg-info/entry_points.txt
@@ -23,66 +25,84 @@
 beancount_reds_importers/example/fund_info.py
 beancount_reds_importers/example/import.sh
 beancount_reds_importers/example/my-smart.import
 beancount_reds_importers/example/my.beancount
 beancount_reds_importers/example/my.import
 beancount_reds_importers/example/transactions.qfx
 beancount_reds_importers/importers/__init__.py
+beancount_reds_importers/importers/alliant/__init__.py
 beancount_reds_importers/importers/ally/__init__.py
 beancount_reds_importers/importers/ally/tests/ally_test.py
 beancount_reds_importers/importers/ally/tests/transactions.qfx
 beancount_reds_importers/importers/ally/tests/transactions.qfx.extract
 beancount_reds_importers/importers/ally/tests/transactions.qfx.file_account
 beancount_reds_importers/importers/ally/tests/transactions.qfx.file_date
 beancount_reds_importers/importers/ally/tests/transactions.qfx.file_name
 beancount_reds_importers/importers/amazongc/__init__.py
 beancount_reds_importers/importers/amex/__init__.py
+beancount_reds_importers/importers/bamboohr/__init__.py
 beancount_reds_importers/importers/becu/__init__.py
 beancount_reds_importers/importers/capitalonebank/__init__.py
 beancount_reds_importers/importers/capitalonebank/tests/360Checking.qfx
 beancount_reds_importers/importers/capitalonebank/tests/360Checking.qfx.extract
 beancount_reds_importers/importers/capitalonebank/tests/360Checking.qfx.file_account
 beancount_reds_importers/importers/capitalonebank/tests/360Checking.qfx.file_date
 beancount_reds_importers/importers/capitalonebank/tests/360Checking.qfx.file_name
 beancount_reds_importers/importers/capitalonebank/tests/capitalone_test.py
 beancount_reds_importers/importers/chase/__init__.py
 beancount_reds_importers/importers/citi/__init__.py
+beancount_reds_importers/importers/dcu/__init__.py
+beancount_reds_importers/importers/dcu/tests/Main_Checking_Account_Transactions.csv
+beancount_reds_importers/importers/dcu/tests/Main_Checking_Account_Transactions.csv.extract
+beancount_reds_importers/importers/dcu/tests/Main_Checking_Account_Transactions.csv.file_account
+beancount_reds_importers/importers/dcu/tests/Main_Checking_Account_Transactions.csv.file_date
+beancount_reds_importers/importers/dcu/tests/Main_Checking_Account_Transactions.csv.file_name
+beancount_reds_importers/importers/dcu/tests/dcu_csv_test.py
 beancount_reds_importers/importers/discover/__init__.py
 beancount_reds_importers/importers/discover/discover_ofx.py
 beancount_reds_importers/importers/etrade/__init__.py
 beancount_reds_importers/importers/etrade/tests/etrade_09092023.QFX
 beancount_reds_importers/importers/etrade/tests/etrade_09092023.QFX.extract
 beancount_reds_importers/importers/etrade/tests/etrade_09092023.QFX.file_account
 beancount_reds_importers/importers/etrade/tests/etrade_09092023.QFX.file_date
 beancount_reds_importers/importers/etrade/tests/etrade_09092023.QFX.file_name
 beancount_reds_importers/importers/etrade/tests/etrade_qfx_brokerage_test.py
 beancount_reds_importers/importers/fidelity/__init__.py
 beancount_reds_importers/importers/fidelity/fidelity_cma_csv.py
 beancount_reds_importers/importers/fidelity/fidelity_cma_csv_examples/History_for_Account_X8YYYYYYY.csv
 beancount_reds_importers/importers/fidelity/fidelity_cma_csv_examples/fidelity-cma-csv.import
 beancount_reds_importers/importers/fidelity/fidelity_cma_csv_examples/run_test.bash
+beancount_reds_importers/importers/genericpdf/__init__.py
+beancount_reds_importers/importers/genericpdf/tests/genericpdf_test.py
+beancount_reds_importers/importers/genericpdf/tests/paystub.sample.pdf
+beancount_reds_importers/importers/genericpdf/tests/paystub.sample.pdf.extract
+beancount_reds_importers/importers/genericpdf/tests/paystub.sample.pdf.file_account
+beancount_reds_importers/importers/genericpdf/tests/paystub.sample.pdf.file_date
+beancount_reds_importers/importers/genericpdf/tests/paystub.sample.pdf.file_name
 beancount_reds_importers/importers/morganstanley/__init__.py
 beancount_reds_importers/importers/schwab/__init__.py
 beancount_reds_importers/importers/schwab/schwab_csv_balances.py
 beancount_reds_importers/importers/schwab/schwab_csv_brokerage.py
 beancount_reds_importers/importers/schwab/schwab_csv_checking.py
+beancount_reds_importers/importers/schwab/schwab_csv_creditline.py
 beancount_reds_importers/importers/schwab/schwab_csv_positions.py
+beancount_reds_importers/importers/schwab/schwab_json_brokerage.py
 beancount_reds_importers/importers/schwab/schwab_ofx_bank_ofx.py
 beancount_reds_importers/importers/schwab/schwab_ofx_brokerage.py
-beancount_reds_importers/importers/schwab/tests/schwab_csv_brokerage/schwab_csv_brokerage_Transactions_123.csv
-beancount_reds_importers/importers/schwab/tests/schwab_csv_brokerage/schwab_csv_brokerage_Transactions_123.csv.extract
-beancount_reds_importers/importers/schwab/tests/schwab_csv_brokerage/schwab_csv_brokerage_Transactions_123.csv.file_account
-beancount_reds_importers/importers/schwab/tests/schwab_csv_brokerage/schwab_csv_brokerage_Transactions_123.csv.file_date
-beancount_reds_importers/importers/schwab/tests/schwab_csv_brokerage/schwab_csv_brokerage_Transactions_123.csv.file_name
+beancount_reds_importers/importers/schwab/tests/schwab_csv_brokerage/schwab_csv_brokerage_XX876_Transactions_20220731.csv
+beancount_reds_importers/importers/schwab/tests/schwab_csv_brokerage/schwab_csv_brokerage_XX876_Transactions_20220731.csv.extract
+beancount_reds_importers/importers/schwab/tests/schwab_csv_brokerage/schwab_csv_brokerage_XX876_Transactions_20220731.csv.file_account
+beancount_reds_importers/importers/schwab/tests/schwab_csv_brokerage/schwab_csv_brokerage_XX876_Transactions_20220731.csv.file_date
+beancount_reds_importers/importers/schwab/tests/schwab_csv_brokerage/schwab_csv_brokerage_XX876_Transactions_20220731.csv.file_name
 beancount_reds_importers/importers/schwab/tests/schwab_csv_brokerage/schwab_csv_brokerage_test.py
-beancount_reds_importers/importers/schwab/tests/schwab_csv_checking/schwab_Checking_Transactions_1234.csv
-beancount_reds_importers/importers/schwab/tests/schwab_csv_checking/schwab_Checking_Transactions_1234.csv.extract
-beancount_reds_importers/importers/schwab/tests/schwab_csv_checking/schwab_Checking_Transactions_1234.csv.file_account
-beancount_reds_importers/importers/schwab/tests/schwab_csv_checking/schwab_Checking_Transactions_1234.csv.file_date
-beancount_reds_importers/importers/schwab/tests/schwab_csv_checking/schwab_Checking_Transactions_1234.csv.file_name
+beancount_reds_importers/importers/schwab/tests/schwab_csv_checking/schwab_XXX234_Checking_Transactions_20220203.csv
+beancount_reds_importers/importers/schwab/tests/schwab_csv_checking/schwab_XXX234_Checking_Transactions_20220203.csv.extract
+beancount_reds_importers/importers/schwab/tests/schwab_csv_checking/schwab_XXX234_Checking_Transactions_20220203.csv.file_account
+beancount_reds_importers/importers/schwab/tests/schwab_csv_checking/schwab_XXX234_Checking_Transactions_20220203.csv.file_date
+beancount_reds_importers/importers/schwab/tests/schwab_csv_checking/schwab_XXX234_Checking_Transactions_20220203.csv.file_name
 beancount_reds_importers/importers/schwab/tests/schwab_csv_checking/schwab_csv_checking_test.py
 beancount_reds_importers/importers/stanchart/__init__.py
 beancount_reds_importers/importers/stanchart/scbbank.py
 beancount_reds_importers/importers/stanchart/scbcard.py
 beancount_reds_importers/importers/target/__init__.py
 beancount_reds_importers/importers/tdameritrade/__init__.py
 beancount_reds_importers/importers/techcubank/__init__.py
@@ -104,15 +124,17 @@
 beancount_reds_importers/importers/vanguard/tests/OfxDownload-401k.qfx.file_date
 beancount_reds_importers/importers/vanguard/tests/OfxDownload-401k.qfx.file_name
 beancount_reds_importers/importers/vanguard/tests/vanguard_test.py
 beancount_reds_importers/importers/workday/__init__.py
 beancount_reds_importers/libreader/__init__.py
 beancount_reds_importers/libreader/csv_multitable_reader.py
 beancount_reds_importers/libreader/csvreader.py
+beancount_reds_importers/libreader/jsonreader.py
 beancount_reds_importers/libreader/ofxreader.py
+beancount_reds_importers/libreader/pdfreader.py
 beancount_reds_importers/libreader/reader.py
 beancount_reds_importers/libreader/tsvreader.py
 beancount_reds_importers/libreader/xlsreader.py
 beancount_reds_importers/libreader/xlsx_multitable_reader.py
 beancount_reds_importers/libreader/xlsxreader.py
 beancount_reds_importers/libreader/tests/balance_assertion_date/last_transaction/last_transaction_date_test.py
 beancount_reds_importers/libreader/tests/balance_assertion_date/last_transaction/transactions.qfx
```

### Comparing `beancount_reds_importers-0.8.0/setup.py` & `beancount_reds_importers-0.9.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,58 @@
 from os import path
+
 from setuptools import find_packages, setup
 
-with open(path.join(path.dirname(__file__), 'README.md')) as readme:
+with open(path.join(path.dirname(__file__), "README.md")) as readme:
     LONG_DESCRIPTION = readme.read()
 
 setup(
-    name='beancount_reds_importers',
+    name="beancount_reds_importers",
     use_scm_version=True,
-    setup_requires=['setuptools_scm'],
-    description='Importers for various institutions for Beancount',
+    setup_requires=["setuptools_scm"],
+    description="Importers for various institutions for Beancount",
     long_description=LONG_DESCRIPTION,
-    long_description_content_type='text/markdown',
-    url='https://github.com/redstreet/beancount_reds_importers',
-    author='Red Street',
-    author_email='redstreet@users.noreply.github.com',
-    keywords='importer ingestor beancount accounting',
-    license='GPL-3.0',
+    long_description_content_type="text/markdown",
+    url="https://github.com/redstreet/beancount_reds_importers",
+    author="Red Street",
+    author_email="redstreet@users.noreply.github.com",
+    keywords="importer ingestor beancount accounting",
+    license="GPL-3.0",
     packages=find_packages(),
     include_package_data=True,
+    extras_require={
+        "dev": [
+            "ruff",
+            "isort",
+        ]
+    },
     install_requires=[
-        'Click >= 7.0',
-        'beancount >= 2.3.5',
-        'click_aliases >= 1.0.1',
-        'ofxparse >= 0.21',
-        'openpyxl >= 3.0.9',
-        'packaging >= 20.3',
-        'petl >= 1.7.4',
-        'tabulate >= 0.8.9',
-        'tqdm >= 4.64.0',
+        "Click >= 7.0",
+        "beancount >= 2.3.5",
+        "click_aliases >= 1.0.1",
+        "dateparser >= 1.2.0",
+        "ofxparse >= 0.21",
+        "openpyxl >= 3.0.9",
+        "packaging >= 20.3",
+        "pdfplumber>=0.11.0",
+        "petl >= 1.7.4",
+        "tabulate >= 0.8.9",
+        "tqdm >= 4.64.0",
     ],
     entry_points={
-        'console_scripts': [
-            'ofx-summarize = beancount_reds_importers.util.ofx_summarize:summarize',
-            'bean-download = beancount_reds_importers.util.bean_download:cli',
+        "console_scripts": [
+            "ofx-summarize = beancount_reds_importers.util.ofx_summarize:summarize",
+            "bean-download = beancount_reds_importers.util.bean_download:cli",
         ]
     },
     zip_safe=False,
     classifiers=[
-        'Development Status :: 4 - Beta',
-        'Intended Audience :: Financial and Insurance Industry',
-        'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
-        'Natural Language :: English',
-        'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: Python :: 3.7',
-        'Topic :: Office/Business :: Financial :: Accounting',
-        'Topic :: Office/Business :: Financial :: Investment',
+        "Development Status :: 4 - Beta",
+        "Intended Audience :: Financial and Insurance Industry",
+        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+        "Natural Language :: English",
+        "Programming Language :: Python :: 3 :: Only",
+        "Programming Language :: Python :: 3.7",
+        "Topic :: Office/Business :: Financial :: Accounting",
+        "Topic :: Office/Business :: Financial :: Investment",
     ],
 )
```

