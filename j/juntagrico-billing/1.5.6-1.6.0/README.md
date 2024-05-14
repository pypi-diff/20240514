# Comparing `tmp/juntagrico-billing-1.5.6.tar.gz` & `tmp/juntagrico_billing-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "juntagrico-billing-1.5.6.tar", last modified: Tue Mar 26 10:20:37 2024, max compression
+gzip compressed data, was "juntagrico_billing-1.6.0.tar", last modified: Tue May 14 08:38:34 2024, max compression
```

## Comparing `juntagrico-billing-1.5.6.tar` & `juntagrico_billing-1.6.0.tar`

### file list

```diff
@@ -1,86 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:20:37.933021 juntagrico-billing-1.5.6/
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7632 2024-03-26 10:20:37.933021 juntagrico-billing-1.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6641 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:20:37.921021 juntagrico-billing-1.5.6/juntagrico_billing/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/juntagrico_billing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:20:37.925021 juntagrico-billing-1.5.6/juntagrico_billing/admin/
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/juntagrico_billing/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/juntagrico_billing/admin/bill.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/juntagrico_billing/admin/billitem_inline.py
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/juntagrico_billing/admin/businessyear.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/juntagrico_billing/admin/payment.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/juntagrico_billing/admin/payment_inline.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/juntagrico_billing/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/juntagrico_billing/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:20:37.925021 juntagrico-billing-1.5.6/juntagrico_billing/dao/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/juntagrico_billing/dao/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/juntagrico_billing/dao/billdao.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/juntagrico_billing/dao/paymentdao.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/juntagrico_billing/dao/subscription_parts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:20:37.925021 juntagrico-billing-1.5.6/juntagrico_billing/entity/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/juntagrico_billing/entity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/juntagrico_billing/entity/account.py
--rw-r--r--   0 runner    (1001) docker     (127)     7746 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/juntagrico_billing/entity/bill.py
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/juntagrico_billing/entity/payment.py
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/juntagrico_billing/entity/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/juntagrico_billing/juntagricoapp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:20:37.929021 juntagrico-billing-1.5.6/juntagrico_billing/lifecycle/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/juntagrico_billing/lifecycle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/juntagrico_billing/lifecycle/billitem.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/juntagrico_billing/lifecycle/payment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:20:37.917021 juntagrico-billing-1.5.6/juntagrico_billing/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:20:37.917021 juntagrico-billing-1.5.6/juntagrico_billing/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:20:37.929021 juntagrico-billing-1.5.6/juntagrico_billing/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     8227 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/juntagrico_billing/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    18853 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/juntagrico_billing/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/juntagrico_billing/mailer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:20:37.929021 juntagrico-billing-1.5.6/juntagrico_billing/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     8481 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/juntagrico_billing/migrations/0001_squashed_0012_post_1_4.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/juntagrico_billing/migrations/0002_bill_published.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/juntagrico_billing/migrations/0003_vat.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/juntagrico_billing/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/juntagrico_billing/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:20:37.921021 juntagrico-billing-1.5.6/juntagrico_billing/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:20:37.921021 juntagrico-billing-1.5.6/juntagrico_billing/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:20:37.921021 juntagrico-billing-1.5.6/juntagrico_billing/templates/admin/juntagrico_billing/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:20:37.929021 juntagrico-billing-1.5.6/juntagrico_billing/templates/admin/juntagrico_billing/bill/
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/juntagrico_billing/templates/admin/juntagrico_billing/bill/change_form.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:20:37.929021 juntagrico-billing-1.5.6/juntagrico_billing/templates/jb/
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/juntagrico_billing/templates/jb/billing_admin_menu.html
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/juntagrico_billing/templates/jb/billing_user_menu.html
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/juntagrico_billing/templates/jb/bills_notify.html
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/juntagrico_billing/templates/jb/bookings_export.html
--rw-r--r--   0 runner    (1001) docker     (127)     6409 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/juntagrico_billing/templates/jb/open_bills.html
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/juntagrico_billing/templates/jb/payments_upload.html
--rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/juntagrico_billing/templates/jb/pending_bills.html
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/juntagrico_billing/templates/jb/subscription_bookings.html
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/juntagrico_billing/templates/jb/unpublished_bills.html
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/juntagrico_billing/templates/jb/user_bill.html
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/juntagrico_billing/templates/jb/user_bills.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:20:37.929021 juntagrico-billing-1.5.6/juntagrico_billing/templates/mails/
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/juntagrico_billing/templates/mails/bill_notification.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:20:37.933021 juntagrico-billing-1.5.6/juntagrico_billing/templates/messages/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/juntagrico_billing/templates/messages/no_businessyear.html
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/juntagrico_billing/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:20:37.933021 juntagrico-billing-1.5.6/juntagrico_billing/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/juntagrico_billing/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7407 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/juntagrico_billing/util/billing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/juntagrico_billing/util/bookings.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/juntagrico_billing/util/esr.py
--rw-r--r--   0 runner    (1001) docker     (127)     5550 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/juntagrico_billing/util/payment_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/juntagrico_billing/util/payment_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     8602 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/juntagrico_billing/util/pdfbill.py
--rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/juntagrico_billing/util/qrbill.py
--rw-r--r--   0 runner    (1001) docker     (127)    11734 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/juntagrico_billing/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/juntagrico_billing/views_payment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:20:37.933021 juntagrico-billing-1.5.6/juntagrico_billing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7632 2024-03-26 10:20:37.000000 juntagrico-billing-1.5.6/juntagrico_billing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-03-26 10:20:37.000000 juntagrico-billing-1.5.6/juntagrico_billing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 10:20:37.000000 juntagrico-billing-1.5.6/juntagrico_billing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-26 10:20:37.000000 juntagrico-billing-1.5.6/juntagrico_billing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-26 10:20:37.000000 juntagrico-billing-1.5.6/juntagrico_billing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-26 10:20:37.933021 juntagrico-billing-1.5.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-03-26 10:20:34.000000 juntagrico-billing-1.5.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:34.647737 juntagrico_billing-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    17181 2024-05-14 08:38:34.647737 juntagrico_billing-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6977 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:34.631737 juntagrico_billing-1.6.0/juntagrico_billing/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:34.635737 juntagrico_billing-1.6.0/juntagrico_billing/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/admin/bill.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/admin/billitem_inline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/admin/businessyear.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/admin/payment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/admin/payment_inline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:34.635737 juntagrico_billing-1.6.0/juntagrico_billing/lifecycle/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/lifecycle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/lifecycle/billitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/lifecycle/payment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:34.627737 juntagrico_billing-1.6.0/juntagrico_billing/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:34.627737 juntagrico_billing-1.6.0/juntagrico_billing/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:34.635737 juntagrico_billing-1.6.0/juntagrico_billing/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     8227 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    18853 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/mailer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:34.635737 juntagrico_billing-1.6.0/juntagrico_billing/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     8481 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/migrations/0001_squashed_0012_post_1_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/migrations/0002_bill_published.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/migrations/0003_vat.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:34.639737 juntagrico_billing-1.6.0/juntagrico_billing/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/models/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7918 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/models/bill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/models/payment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/models/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:34.639737 juntagrico_billing-1.6.0/juntagrico_billing/querysets/
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/querysets/bill.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/querysets/payment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:34.627737 juntagrico_billing-1.6.0/juntagrico_billing/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:34.627737 juntagrico_billing-1.6.0/juntagrico_billing/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:34.627737 juntagrico_billing-1.6.0/juntagrico_billing/templates/admin/juntagrico_billing/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:34.639737 juntagrico_billing-1.6.0/juntagrico_billing/templates/admin/juntagrico_billing/bill/
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/templates/admin/juntagrico_billing/bill/change_form.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:34.639737 juntagrico_billing-1.6.0/juntagrico_billing/templates/jb/
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/templates/jb/bills_notify.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/templates/jb/bookings_export.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:34.639737 juntagrico_billing-1.6.0/juntagrico_billing/templates/jb/mails/
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/templates/jb/mails/bill_notification.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:34.639737 juntagrico_billing-1.6.0/juntagrico_billing/templates/jb/messages/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/templates/jb/messages/no_businessyear.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6409 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/templates/jb/open_bills.html
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/templates/jb/payments_upload.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/templates/jb/pending_bills.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/templates/jb/subscription_bookings.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/templates/jb/unpublished_bills.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/templates/jb/user_bill.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/templates/jb/user_bills.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:34.627737 juntagrico_billing-1.6.0/juntagrico_billing/templates/juntagrico/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:34.643736 juntagrico_billing-1.6.0/juntagrico_billing/templates/juntagrico/menu/
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/templates/juntagrico/menu/admin.html
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/templates/juntagrico/menu/user.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:34.643736 juntagrico_billing-1.6.0/juntagrico_billing/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5851 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/tests/test_billbookings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19644 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/tests/test_bills.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8206 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/tests/test_payment_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/tests/test_payment_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:34.643736 juntagrico_billing-1.6.0/juntagrico_billing/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7366 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/util/billing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/util/bookings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/util/esr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/util/payment_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/util/payment_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8602 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/util/pdfbill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/util/qrbill.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11684 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/views_payment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:34.643736 juntagrico_billing-1.6.0/juntagrico_billing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17181 2024-05-14 08:38:34.000000 juntagrico_billing-1.6.0/juntagrico_billing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-14 08:38:34.000000 juntagrico_billing-1.6.0/juntagrico_billing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 08:38:34.000000 juntagrico_billing-1.6.0/juntagrico_billing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-14 08:38:34.000000 juntagrico_billing-1.6.0/juntagrico_billing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-14 08:38:34.000000 juntagrico_billing-1.6.0/juntagrico_billing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-14 08:38:34.647737 juntagrico_billing-1.6.0/setup.cfg
```

### Comparing `juntagrico-billing-1.5.6/LICENSE` & `juntagrico_billing-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `juntagrico-billing-1.5.6/PKG-INFO` & `juntagrico_billing-1.6.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,7 @@
-Metadata-Version: 2.1
-Name: juntagrico-billing
-Version: 1.5.6
-Summary: Send and manage bills in juntagrico
-Home-page: https://juntagrico.org
-Author: juntagrico
-Author-email: info@juntagrico.org
-License: LPGLv3
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 4.0
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Other Audience
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: lxml==4.9.3
-Requires-Dist: python-stdnum==1.16
-Requires-Dist: qrbill==1.1.0
-Requires-Dist: svglib==1.0.1
-
 # juntagrico-billing
 
 
 [![juntagrico-ci](https://github.com/juntagrico/juntagrico-billing/actions/workflows/juntagrico-ci.yml/badge.svg?branch=main&event=push)](https://github.com/juntagrico/juntagrico-billing/actions/workflows/juntagrico-ci.yml)
 [![Maintainability](https://api.codeclimate.com/v1/badges/f1e8af41b78f052add70/maintainability)](https://codeclimate.com/github/juntagrico/juntagrico-billing/maintainability)
 [![Test Coverage](https://api.codeclimate.com/v1/badges/f1e8af41b78f052add70/test_coverage)](https://codeclimate.com/github/juntagrico/juntagrico-billing/test_coverage)
 [![image](https://img.shields.io/github/last-commit/juntagrico/juntagrico-billing.svg)](https://github.com/juntagrico/juntagrico-billing)
@@ -52,33 +25,47 @@
 
 or add it to your main django projects `requirements.txt`:
 `juntagrico-billing`
 
 You may also install from github source (or add it to `requirements.txt`):
 `pip install git+https://github.com/juntagrico/juntagrico-billing.git`
 
-In your `juntagrico.settings.py` add `juntagrico_billing`:
+In your `juntagrico.settings.py` add `juntagrico_billing` somewhere **above** `juntagrico`:
 ```python
 INSTALLED_APPS = (
+    'juntagrico_billing',
     'juntagrico',
     ...
-    'juntagrico_billing',
 ```
 
 In your urls.py you also need to add the new pattern:
 ```python
 urlpatterns = [
     ...
-    re_path(r'^',include('juntagrico_billing.urls')),
+    path('',include('juntagrico_billing.urls')),
 ]
 ```
 
 As the billing app introduces its own database tables, you need to apply migrations after installing.
 Execute `python manage.py migrate` in your main django project.
 
+## Configuration
+
+Set these in your `settings.py` to modify `juntagrico-billing`
+
+### BILLS_USERMENU
+  Set to True to add "bills" to the user menu.
+
+  default value: False
+
+### DUEDATE_NOTICE_URL
+  Set the url of a page that explains the due date policy of your bills, if you have any.
+
+  default value: ''
+
 ## Create settings object
 
 `juntagrico-billing` uses a singleton `Settings` object to store some setting.
 You need to create this settings object once in django admin.
 
 - Log in to juntagrico and go to the admin UI at `https://<my juntagrico site>/admin`.
 - You should see in admin a new section for juntagrico_billing
```

### Comparing `juntagrico-billing-1.5.6/juntagrico_billing/admin/bill.py` & `juntagrico_billing-1.6.0/juntagrico_billing/admin/bill.py`

 * *Files identical despite different names*

### Comparing `juntagrico-billing-1.5.6/juntagrico_billing/admin/billitem_inline.py` & `juntagrico_billing-1.6.0/juntagrico_billing/admin/billitem_inline.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from django.contrib import admin
 from django.urls import reverse
 from django.utils.html import escape, mark_safe
 from django.utils.translation import gettext as _
-from juntagrico_billing.entity.bill import BillItem
+from juntagrico_billing.models.bill import BillItem
 
 
 class BillItemInline(admin.TabularInline):
     model = BillItem
     readonly_fields = ('item_kind_link',)
     fields = ('item_kind_link', 'custom_item_type', 'description', 'amount')
     extra = 1
```

### Comparing `juntagrico-billing-1.5.6/juntagrico_billing/entity/account.py` & `juntagrico_billing-1.6.0/juntagrico_billing/models/account.py`

 * *Files identical despite different names*

### Comparing `juntagrico-billing-1.5.6/juntagrico_billing/entity/bill.py` & `juntagrico_billing-1.6.0/juntagrico_billing/models/bill.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 from django.core.exceptions import ValidationError
 from django.db import models
 from django.utils.translation import gettext as _
 from juntagrico.config import Config
 from juntagrico.entity import JuntagricoBaseModel
 from juntagrico.entity.member import Member
 from juntagrico.entity.subs import SubscriptionPart
+
+from juntagrico_billing.querysets.bill import BillQuerySet, BusinessYearQuerySet
 from juntagrico_billing.util.qrbill import calc_refnumber
 
 
 class BusinessYear(JuntagricoBaseModel):
     """
     Business Year for Billing.
     """
     start_date = models.DateField(_('start date'), unique=True)
     end_date = models.DateField(_('end date'))
     name = models.CharField(_('name'), max_length=20, null=True, blank=True, unique=True)
 
+    objects = BusinessYearQuerySet.as_manager()
+
     def __str__(self):
         return self.name or str(self.start_date)
 
     class Meta:
         verbose_name = _('Business Year')
         verbose_name_plural = _('Business Years')
 
@@ -53,14 +57,16 @@
     paid = models.BooleanField(_('Paid'), null=False, blank=False, default=False)
     public_notes = models.TextField(_('Notes visible to {}').format(Config.vocabulary('member_pl')), null=True, blank=True)
     private_notes = models.TextField(_('Notes not visible to {}').format(Config.vocabulary('member_pl')), null=True, blank=True)
     published = models.BooleanField(_('Published'), default=False)
     notification_sent = models.BooleanField(_('Notification sent'), null=False, blank=False, default=False)
     vat_rate = models.FloatField(_('VAT Rate'), null=False, blank=False, default=0.0)
 
+    objects = BillQuerySet.as_manager()
+
     # derived properties
     @property
     def amount_paid(self):
         return sum([p.amount for p in self.payments.all()])
 
     amount_paid.fget.short_description = _('Amount paid')
```

### Comparing `juntagrico-billing-1.5.6/juntagrico_billing/entity/payment.py` & `juntagrico_billing-1.6.0/juntagrico_billing/models/payment.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from django.db import models
 from juntagrico.entity import JuntagricoBaseModel
 from django.utils.translation import gettext as _
 from juntagrico.config import Config
 
+from juntagrico_billing.querysets.payment import PaymentQuerySet
+
 
 class Payment(JuntagricoBaseModel):
     """
     Payment for bill
     """
     bill = models.ForeignKey('Bill', related_name='payments',
                              null=False, blank=False,
@@ -22,14 +24,16 @@
     private_notes = models.TextField(
         _('Notes not visible to {}').format(Config.vocabulary('member_pl')),
         null=True, blank=True)
     unique_id = models.CharField(
         _('Unique Id'), max_length=50,
         null=True, blank=True, unique=True)
 
+    objects = PaymentQuerySet.as_manager()
+
     def __str__(self):
         return '{}'.format(self.bill.id)
 
     class Meta:
         verbose_name = _('Payment')
         verbose_name_plural = _('Payments')
```

### Comparing `juntagrico-billing-1.5.6/juntagrico_billing/entity/settings.py` & `juntagrico_billing-1.6.0/juntagrico_billing/models/settings.py`

 * *Files identical despite different names*

### Comparing `juntagrico-billing-1.5.6/juntagrico_billing/locale/de/LC_MESSAGES/django.mo` & `juntagrico_billing-1.6.0/juntagrico_billing/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `juntagrico-billing-1.5.6/juntagrico_billing/locale/de/LC_MESSAGES/django.po` & `juntagrico_billing-1.6.0/juntagrico_billing/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `juntagrico-billing-1.5.6/juntagrico_billing/mailer.py` & `juntagrico_billing-1.6.0/juntagrico_billing/mailer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from django.template.loader import get_template
 from django.utils.translation import gettext as _
 from juntagrico.config import Config
 from juntagrico.mailer import EmailSender, organisation_subject, base_dict
 
-from juntagrico_billing.entity.settings import Settings
+from juntagrico_billing.models.settings import Settings
 from juntagrico_billing.util.qrbill import is_qr_iban
 
 
 def send_bill_notification(bill):
     # prepare variables that are passed to
     # template using locals()
     settings = Settings.objects.first()
     payment_type = settings.default_paymenttype
     business_year = bill.business_year
     member = bill.member
     start_date = business_year.start_date
     end_date = business_year.end_date
     show_refnumber = is_qr_iban(payment_type.iban)
 
-    template = get_template('mails/bill_notification.txt')
+    template = get_template('jb/mails/bill_notification.txt')
     render_dict = base_dict(locals())
 
     # render template
     content = template.render(render_dict)
 
     subject = organisation_subject(_('{0} Bill').format(Config.vocabulary('subscription')))
```

### Comparing `juntagrico-billing-1.5.6/juntagrico_billing/migrations/0001_squashed_0012_post_1_4.py` & `juntagrico_billing-1.6.0/juntagrico_billing/migrations/0001_squashed_0012_post_1_4.py`

 * *Files identical despite different names*

### Comparing `juntagrico-billing-1.5.6/juntagrico_billing/migrations/0003_vat.py` & `juntagrico_billing-1.6.0/juntagrico_billing/migrations/0003_vat.py`

 * *Files identical despite different names*

### Comparing `juntagrico-billing-1.5.6/juntagrico_billing/templates/jb/billing_admin_menu.html` & `juntagrico_billing-1.6.0/juntagrico_billing/templates/juntagrico/menu/admin.html`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,32 @@
+{% extends "juntagrico/menu/admin.html" %}
 {% load i18n %}
-{% if perms.juntagrico.is_book_keeper %}
-<li class="nav-item">
-    <a class="nav-link" data-toggle="collapse" href="#jb">{% trans "Bills and Bookkeeping" %}<i class="fas fa-angle-right"></i></a>
-    <div class="collapse" id="jb">
-    <ul class="nav flex-column admin-menu subadmin-menu">
+{% block extend %}
+    {% if perms.juntagrico.is_book_keeper %}
         <li class="nav-item">
-            <a class="nav-link" href="{% url 'jb:pending-bills-list' %}">{% trans "Pending bills" %}</a>
-        </li>
-        <li class="nav-item">
-            <a class="nav-link" href="{% url 'jb:unpublished-bills-list' %}">{% trans "Unpublished bills" %}</a>
-        </li>
-        <li class="nav-item">
-            <a class="nav-link" href="{% url 'jb:open-bills-list' %}">{% trans "Open bills" %}</a>
-        </li>
-        <li class="nav-item">
-            <a class="nav-link" href="{% url 'jb:bills-notify' %}">{% trans "Send billing notifications" %}</a>
-        </li>
-        <li class="nav-item">
-            <a class="nav-link" href="{% url 'jb:payments-upload' %}">{% trans "Import payments" %}</a>
-        </li>
-        <li class="nav-item">
-            <a class="nav-link" href="/jb/bookings_export">{% trans "Export bookings" %}</a>
-        </li>
-    </ul>
-    </div>
-</li>
-{% endif %}
+            <a class="nav-link" data-toggle="collapse" href="#jb">{% trans "Bills and Bookkeeping" %}<i class="fas fa-angle-right"></i></a>
+            <div class="collapse" id="jb">
+            <ul class="nav flex-column admin-menu subadmin-menu">
+                <li class="nav-item">
+                    <a class="nav-link" href="{% url 'jb:pending-bills-list' %}">{% trans "Pending bills" %}</a>
+                </li>
+                <li class="nav-item">
+                    <a class="nav-link" href="{% url 'jb:unpublished-bills-list' %}">{% trans "Unpublished bills" %}</a>
+                </li>
+                <li class="nav-item">
+                    <a class="nav-link" href="{% url 'jb:open-bills-list' %}">{% trans "Open bills" %}</a>
+                </li>
+                <li class="nav-item">
+                    <a class="nav-link" href="{% url 'jb:bills-notify' %}">{% trans "Send billing notifications" %}</a>
+                </li>
+                <li class="nav-item">
+                    <a class="nav-link" href="{% url 'jb:payments-upload' %}">{% trans "Import payments" %}</a>
+                </li>
+                <li class="nav-item">
+                    <a class="nav-link" href="/jb/bookings_export">{% trans "Export bookings" %}</a>
+                </li>
+            </ul>
+            </div>
+        </li>
+    {% endif %}
+    {{ block.super }}
+{% endblock %}
```

### Comparing `juntagrico-billing-1.5.6/juntagrico_billing/templates/jb/bills_notify.html` & `juntagrico_billing-1.6.0/juntagrico_billing/templates/jb/bills_notify.html`

 * *Files identical despite different names*

### Comparing `juntagrico-billing-1.5.6/juntagrico_billing/templates/jb/bookings_export.html` & `juntagrico_billing-1.6.0/juntagrico_billing/templates/jb/bookings_export.html`

 * *Files identical despite different names*

### Comparing `juntagrico-billing-1.5.6/juntagrico_billing/templates/jb/open_bills.html` & `juntagrico_billing-1.6.0/juntagrico_billing/templates/jb/open_bills.html`

 * *Files identical despite different names*

### Comparing `juntagrico-billing-1.5.6/juntagrico_billing/templates/jb/payments_upload.html` & `juntagrico_billing-1.6.0/juntagrico_billing/templates/jb/payments_upload.html`

 * *Files identical despite different names*

### Comparing `juntagrico-billing-1.5.6/juntagrico_billing/templates/jb/pending_bills.html` & `juntagrico_billing-1.6.0/juntagrico_billing/templates/jb/pending_bills.html`

 * *Files identical despite different names*

### Comparing `juntagrico-billing-1.5.6/juntagrico_billing/templates/jb/subscription_bookings.html` & `juntagrico_billing-1.6.0/juntagrico_billing/templates/jb/subscription_bookings.html`

 * *Files identical despite different names*

### Comparing `juntagrico-billing-1.5.6/juntagrico_billing/templates/jb/unpublished_bills.html` & `juntagrico_billing-1.6.0/juntagrico_billing/templates/jb/unpublished_bills.html`

 * *Files identical despite different names*

### Comparing `juntagrico-billing-1.5.6/juntagrico_billing/templates/jb/user_bill.html` & `juntagrico_billing-1.6.0/juntagrico_billing/templates/jb/user_bill.html`

 * *Files identical despite different names*

### Comparing `juntagrico-billing-1.5.6/juntagrico_billing/templates/jb/user_bills.html` & `juntagrico_billing-1.6.0/juntagrico_billing/templates/jb/user_bills.html`

 * *Files identical despite different names*

### Comparing `juntagrico-billing-1.5.6/juntagrico_billing/templates/mails/bill_notification.txt` & `juntagrico_billing-1.6.0/juntagrico_billing/templates/jb/mails/bill_notification.txt`

 * *Files identical despite different names*

### Comparing `juntagrico-billing-1.5.6/juntagrico_billing/urls.py` & `juntagrico_billing-1.6.0/juntagrico_billing/urls.py`

 * *Files identical despite different names*

### Comparing `juntagrico-billing-1.5.6/juntagrico_billing/util/billing.py` & `juntagrico_billing-1.6.0/juntagrico_billing/util/billing.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from collections import defaultdict
 from datetime import date
 from decimal import Decimal
 
-from juntagrico_billing.dao.subscription_parts import\
-    subscription_parts_by_date, subscription_parts_member_date
-from juntagrico_billing.entity.bill import Bill, BillItem
-from juntagrico_billing.entity.settings import Settings
+from juntagrico.entity.subs import SubscriptionPart
+
+from juntagrico_billing.models.bill import Bill, BillItem
+from juntagrico_billing.models.settings import Settings
 
 
 def scale_subscriptionpart_price(part, fromdate, tilldate):
     """
     scale subscription part price for a certain date interval.
     """
 
-    if len(part.type.periods.all()):
+    if part.type.periods.count():
         # calculate price based on billing periods.
         # takes into account periods that overlap with the requested interval.
         period_prices = []
         for period in part.type.periods.all():
             period_start = date(fromdate.year, period.start_month, period.start_day)
             period_end = date(fromdate.year, period.end_month, period.end_day)
             if period_start <= tilldate and period_end >= fromdate:
@@ -58,15 +58,15 @@
 
     # prepare a dictionary with member, subscription_part tuples as keys
     # based on the bills of this year
     bill_items = BillItem.objects.filter(bill__business_year=business_year)
     bill_parts = [itm.subscription_part for itm in bill_items if itm.subscription_part]
 
     # get all active subscription parts for billing period
-    active_parts = subscription_parts_by_date(from_date, till_date)
+    active_parts = SubscriptionPart.objects.in_daterange(from_date, till_date)
 
     # get parts that are not billed yet
     billed_dict = dict([(part, None) for part in bill_parts])
 
     not_billed = [part for part in active_parts if part not in billed_dict]
 
     return not_billed
@@ -121,16 +121,15 @@
     """
     update an existing bill with all items that are not
     on another bill in the same businessyear.
     """
     # get all subscription parts for member and businessyear
     year = bill.business_year
     member = bill.member
-    parts_in_year = subscription_parts_member_date(
-        member, year.start_date, year.end_date)
+    parts_in_year = SubscriptionPart.objects.by_primary_member(member).in_daterange(year.start_date, year.end_date)
 
     # determine if part is on another bill in the same year
     def is_on_other_bill(part):
         items = part.bill_items.all()
         for itm in items:
             if itm.bill:
                 if itm.bill != bill:
```

### Comparing `juntagrico-billing-1.5.6/juntagrico_billing/util/bookings.py` & `juntagrico_billing-1.6.0/juntagrico_billing/util/bookings.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from django.utils.translation import gettext as _
 
-from juntagrico_billing.dao.billdao import BillDao
-from juntagrico_billing.dao.paymentdao import PaymentDao
-from juntagrico_billing.entity.settings import Settings
+from juntagrico_billing.models import Payment
+from juntagrico_billing.models.bill import Bill
+from juntagrico_billing.models.settings import Settings
 
 # Offset for generating Document numbers for bookings
 DOCNUMBER_OFFSET_BILL = 500000
 DOCNUMBER_OFFSET_PAYMENT = 600000
 
 
 class Booking(object):
     pass
 
 
 def get_bill_bookings(fromdate, tilldate):
     # get all bills by business-year start, end
 
-    bills = BillDao.bills_for_daterange(fromdate, tilldate)
+    bills = Bill.objects.in_daterange(fromdate, tilldate)
 
     # global debtor account on settings object
     debtor_account = Settings.objects.first().debtor_account
 
     bookings = []
 
     for bill in bills:
@@ -67,15 +67,15 @@
     else:
         booking.member_account = ""
 
     return booking
 
 
 def get_payment_bookings(fromdate, tilldate):
-    payments = PaymentDao.payments_for_daterange(fromdate, tilldate)
+    payments = Payment.objects.in_daterange(fromdate, tilldate)
 
     # global debtor account on settings object
     debtor_account = Settings.objects.first().debtor_account
 
     bookings = []
 
     for payment in payments:
```

### Comparing `juntagrico-billing-1.5.6/juntagrico_billing/util/esr.py` & `juntagrico_billing-1.6.0/juntagrico_billing/util/esr.py`

 * *Files identical despite different names*

### Comparing `juntagrico-billing-1.5.6/juntagrico_billing/util/payment_processor.py` & `juntagrico_billing-1.6.0/juntagrico_billing/util/payment_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from django.db import IntegrityError, transaction
 from django.utils.translation import gettext
 from juntagrico.entity.member import Member
-from juntagrico_billing.entity.bill import Bill
-from juntagrico_billing.entity.payment import Payment, PaymentType
+from juntagrico_billing.models.bill import Bill
+from juntagrico_billing.models.payment import Payment, PaymentType
 from juntagrico_billing.util.qrbill import bill_id_from_refnumber
 from juntagrico_billing.util.qrbill import member_id_from_refnumber
 from stdnum import iban
 
 
 class PaymentInfo(object):
     def __init__(self, date, credit_iban, amount, ref_type,
@@ -144,11 +144,10 @@
                     payment = Payment.objects.create(
                         bill=bill,
                         type=self.find_paymenttype(pinfo),
                         paid_date=pinfo.date,
                         amount=pinfo.amount,
                         unique_id=pinfo.unique_id)
                     payment.save()
-                except IntegrityError:
+                except IntegrityError as err:
                     msg = 'Payment with unique id %s has already been imported.'
-                    raise PaymentProcessorError(
-                        self._(msg) % pinfo.unique_id)
+                    raise PaymentProcessorError(self._(msg) % pinfo.unique_id) from err
```

### Comparing `juntagrico-billing-1.5.6/juntagrico_billing/util/payment_reader.py` & `juntagrico_billing-1.6.0/juntagrico_billing/util/payment_reader.py`

 * *Files identical despite different names*

### Comparing `juntagrico-billing-1.5.6/juntagrico_billing/util/pdfbill.py` & `juntagrico_billing-1.6.0/juntagrico_billing/util/pdfbill.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from reportlab.lib.styles import getSampleStyleSheet, ParagraphStyle
 from reportlab.lib.units import cm
 from django.utils.formats import get_format
 from django.utils.dateformat import format
 from django.utils.translation import gettext as _
 from juntagrico.config import Config
 from juntagrico_billing.config import Config as BillingConfig
-from juntagrico_billing.entity.settings import Settings
+from juntagrico_billing.models.settings import Settings
 from juntagrico_billing.util.qrbill import get_qrbill_svg
 from svglib.svglib import SvgRenderer
 from lxml import etree
 
 
 class PdfBillRenderer(object):
```

### Comparing `juntagrico-billing-1.5.6/juntagrico_billing/util/qrbill.py` & `juntagrico_billing-1.6.0/juntagrico_billing/util/qrbill.py`

 * *Files identical despite different names*

### Comparing `juntagrico-billing-1.5.6/juntagrico_billing/views.py` & `juntagrico_billing-1.6.0/juntagrico_billing/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,16 @@
 from django.urls import reverse
 from django.http import HttpResponse
 from django.views.decorators.http import require_POST
 from juntagrico.util import return_to_previous_location
 from juntagrico.util.temporal import start_of_business_year, \
     start_of_next_business_year
 from juntagrico.util.xls import generate_excel
-from juntagrico_billing.dao.billdao import BillDao
-from juntagrico_billing.entity.bill import BusinessYear, Bill
-from juntagrico_billing.entity.settings import Settings
+from juntagrico_billing.models.bill import BusinessYear, Bill
+from juntagrico_billing.models.settings import Settings
 from juntagrico_billing.mailer import send_bill_notification
 from juntagrico_billing.util.billing import get_billable_subscription_parts, \
     group_billables_by_member, create_bills_for_items, get_open_bills, \
     scale_subscriptionpart_price, recalc_bill, get_unpublished_bills, \
     publish_bills
 from juntagrico_billing.util.qrbill import get_qrbill_svg
 from juntagrico_billing.util.pdfbill import PdfBillRenderer
@@ -73,15 +72,15 @@
     return return_to_previous_location(request)
 
 
 @permission_required('juntagrico.is_book_keeper')
 def bills_generate(request):
     # generate bills for current business year
     year_name = request.session['bills_businessyear']
-    year = BusinessYear.objects.filter(name=year_name).first()
+    year = BusinessYear.objects.by_name(year_name)
 
     billable_items = get_billable_subscription_parts(year)
 
     create_bills_for_items(billable_items, year, date.today())
 
     return redirect(reverse('jb:unpublished-bills-list'))
 
@@ -264,15 +263,15 @@
 
 
 @login_required
 def user_bills(request):
     member = request.user.member
     settings = Settings.objects.first()
     renderdict = {
-        'bills': BillDao.bills_for_member(member).order_by("-bill_date"),
+        'bills': Bill.objects.of_member(member).published().order_by("-bill_date"),
         'paymenttype': settings.default_paymenttype,
         'menu': {'bills': 'active'},
     }
     return render(request, "jb/user_bills.html", renderdict)
 
 
 @login_required
@@ -354,15 +353,15 @@
     """
     # get all business years
     business_years = list(BusinessYear.objects.all().order_by('start_date'))
 
     if len(business_years) == 0:
         # add message 'no businessyear'
         messages = getattr(request, 'member_messages', []) or []
-        messages.append(get_template('messages/no_businessyear.html').render())
+        messages.append(get_template('jb/messages/no_businessyear.html').render())
         request.member_messages = messages
 
     # if no year set, choose most recent year
     selected_year = None
     selected_year_name = request.session.get('bills_businessyear', None)
     if selected_year_name:
         selected_year = [
```

### Comparing `juntagrico-billing-1.5.6/juntagrico_billing/views_payment.py` & `juntagrico_billing-1.6.0/juntagrico_billing/views_payment.py`

 * *Files identical despite different names*

### Comparing `juntagrico-billing-1.5.6/juntagrico_billing.egg-info/SOURCES.txt` & `juntagrico_billing-1.6.0/juntagrico_billing.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,65 +1,66 @@
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
 requirements.txt
 setup.cfg
-setup.py
 juntagrico_billing/__init__.py
 juntagrico_billing/apps.py
 juntagrico_billing/config.py
-juntagrico_billing/juntagricoapp.py
 juntagrico_billing/mailer.py
-juntagrico_billing/models.py
 juntagrico_billing/urls.py
 juntagrico_billing/views.py
 juntagrico_billing/views_payment.py
 juntagrico_billing.egg-info/PKG-INFO
 juntagrico_billing.egg-info/SOURCES.txt
 juntagrico_billing.egg-info/dependency_links.txt
 juntagrico_billing.egg-info/requires.txt
 juntagrico_billing.egg-info/top_level.txt
 juntagrico_billing/admin/__init__.py
 juntagrico_billing/admin/bill.py
 juntagrico_billing/admin/billitem_inline.py
 juntagrico_billing/admin/businessyear.py
 juntagrico_billing/admin/payment.py
 juntagrico_billing/admin/payment_inline.py
-juntagrico_billing/dao/__init__.py
-juntagrico_billing/dao/billdao.py
-juntagrico_billing/dao/paymentdao.py
-juntagrico_billing/dao/subscription_parts.py
-juntagrico_billing/entity/__init__.py
-juntagrico_billing/entity/account.py
-juntagrico_billing/entity/bill.py
-juntagrico_billing/entity/payment.py
-juntagrico_billing/entity/settings.py
 juntagrico_billing/lifecycle/__init__.py
 juntagrico_billing/lifecycle/billitem.py
 juntagrico_billing/lifecycle/payment.py
 juntagrico_billing/locale/de/LC_MESSAGES/django.mo
 juntagrico_billing/locale/de/LC_MESSAGES/django.po
 juntagrico_billing/migrations/0001_squashed_0012_post_1_4.py
 juntagrico_billing/migrations/0002_bill_published.py
 juntagrico_billing/migrations/0003_vat.py
 juntagrico_billing/migrations/__init__.py
+juntagrico_billing/models/__init__.py
+juntagrico_billing/models/account.py
+juntagrico_billing/models/bill.py
+juntagrico_billing/models/payment.py
+juntagrico_billing/models/settings.py
+juntagrico_billing/querysets/bill.py
+juntagrico_billing/querysets/payment.py
 juntagrico_billing/templates/admin/juntagrico_billing/bill/change_form.html
-juntagrico_billing/templates/jb/billing_admin_menu.html
-juntagrico_billing/templates/jb/billing_user_menu.html
 juntagrico_billing/templates/jb/bills_notify.html
 juntagrico_billing/templates/jb/bookings_export.html
 juntagrico_billing/templates/jb/open_bills.html
 juntagrico_billing/templates/jb/payments_upload.html
 juntagrico_billing/templates/jb/pending_bills.html
 juntagrico_billing/templates/jb/subscription_bookings.html
 juntagrico_billing/templates/jb/unpublished_bills.html
 juntagrico_billing/templates/jb/user_bill.html
 juntagrico_billing/templates/jb/user_bills.html
-juntagrico_billing/templates/mails/bill_notification.txt
-juntagrico_billing/templates/messages/no_businessyear.html
+juntagrico_billing/templates/jb/mails/bill_notification.txt
+juntagrico_billing/templates/jb/messages/no_businessyear.html
+juntagrico_billing/templates/juntagrico/menu/admin.html
+juntagrico_billing/templates/juntagrico/menu/user.html
+juntagrico_billing/tests/__init__.py
+juntagrico_billing/tests/test_billbookings.py
+juntagrico_billing/tests/test_bills.py
+juntagrico_billing/tests/test_payment_processor.py
+juntagrico_billing/tests/test_payment_reader.py
 juntagrico_billing/util/__init__.py
 juntagrico_billing/util/billing.py
 juntagrico_billing/util/bookings.py
 juntagrico_billing/util/esr.py
 juntagrico_billing/util/payment_processor.py
 juntagrico_billing/util/payment_reader.py
 juntagrico_billing/util/pdfbill.py
```

