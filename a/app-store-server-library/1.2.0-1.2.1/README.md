# Comparing `tmp/app_store_server_library-1.2.0.tar.gz` & `tmp/app_store_server_library-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "app_store_server_library-1.2.0.tar", last modified: Tue May  7 05:12:03 2024, max compression
+gzip compressed data, was "app_store_server_library-1.2.1.tar", last modified: Tue May 14 03:34:46 2024, max compression
```

## Comparing `app_store_server_library-1.2.0.tar` & `app_store_server_library-1.2.1.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 05:12:03.635512 app_store_server_library-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    37755 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6036 2024-05-07 05:12:03.635512 app_store_server_library-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5518 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 05:12:03.635512 app_store_server_library-1.2.0/app_store_server_library.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6036 2024-05-07 05:12:03.000000 app_store_server_library-1.2.0/app_store_server_library.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-05-07 05:12:03.000000 app_store_server_library-1.2.0/app_store_server_library.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 05:12:03.000000 app_store_server_library-1.2.0/app_store_server_library.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-07 05:12:03.000000 app_store_server_library-1.2.0/app_store_server_library.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-07 05:12:03.000000 app_store_server_library-1.2.0/app_store_server_library.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 05:12:03.623512 app_store_server_library-1.2.0/appstoreserverlibrary/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31918 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 05:12:03.631512 app_store_server_library-1.2.0/appstoreserverlibrary/models/
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/AccountTenure.py
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/AppTransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/AutoRenewStatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/CheckTestNotificationResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/ConsumptionRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/ConsumptionRequestReason.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/ConsumptionStatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/Data.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/DeliveryStatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/Environment.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/ExpirationIntent.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/ExtendReasonCode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/ExtendRenewalDateRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/ExtendRenewalDateResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/ExternalPurchaseToken.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/FirstSendAttemptResult.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/HistoryResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/InAppOwnershipType.py
--rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/JWSRenewalInfoDecodedPayload.py
--rw-r--r--   0 runner    (1001) docker     (127)     8372 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/JWSTransactionDecodedPayload.py
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/LastTransactionsItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/LibraryUtility.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/LifetimeDollarsPurchased.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/LifetimeDollarsRefunded.py
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/MassExtendRenewalDateRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/MassExtendRenewalDateResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/MassExtendRenewalDateStatusResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/NotificationHistoryRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/NotificationHistoryResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/NotificationHistoryResponseItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/NotificationTypeV2.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/OfferDiscountType.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/OfferType.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/OrderLookupResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/OrderLookupStatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/Platform.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/PlayTime.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/PriceIncreaseStatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/RefundHistoryResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/RefundPreference.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/ResponseBodyV2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/ResponseBodyV2DecodedPayload.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/RevocationReason.py
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/SendAttemptItem.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/SendAttemptResult.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/SendTestNotificationResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/Status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/StatusResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/SubscriptionGroupIdentifierItem.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/Subtype.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/Summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/TransactionHistoryRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/TransactionInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/TransactionReason.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/Type.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/UserStatus.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/promotional_offer.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5412 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/receipt_utility.py
--rw-r--r--   0 runner    (1001) docker     (127)    17203 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/signed_data_verifier.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 05:12:03.635512 app_store_server_library-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 05:12:03.635512 app_store_server_library-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    28548 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/tests/test_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    16096 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/tests/test_decoded_payloads.py
--rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/tests/test_payload_verification.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/tests/test_promotional_offer_signature_creator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/tests/test_receipt_utility.py
--rw-r--r--   0 runner    (1001) docker     (127)    12131 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/tests/test_x509_verifiction.py
--rw-r--r--   0 runner    (1001) docker     (127)     5975 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/tests/test_xcode_signed_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 03:34:46.577896 app_store_server_library-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    37755 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6036 2024-05-14 03:34:46.577896 app_store_server_library-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5518 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 03:34:46.577896 app_store_server_library-1.2.1/app_store_server_library.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6036 2024-05-14 03:34:46.000000 app_store_server_library-1.2.1/app_store_server_library.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-05-14 03:34:46.000000 app_store_server_library-1.2.1/app_store_server_library.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 03:34:46.000000 app_store_server_library-1.2.1/app_store_server_library.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-14 03:34:46.000000 app_store_server_library-1.2.1/app_store_server_library.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-14 03:34:46.000000 app_store_server_library-1.2.1/app_store_server_library.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 03:34:46.565896 app_store_server_library-1.2.1/appstoreserverlibrary/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31918 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 03:34:46.573897 app_store_server_library-1.2.1/appstoreserverlibrary/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/models/AccountTenure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/models/AppTransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/models/AutoRenewStatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/models/CheckTestNotificationResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/models/ConsumptionRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/models/ConsumptionRequestReason.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/models/ConsumptionStatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/models/Data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/models/DeliveryStatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/models/Environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/models/ExpirationIntent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/models/ExtendReasonCode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/models/ExtendRenewalDateRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/models/ExtendRenewalDateResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/models/ExternalPurchaseToken.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/models/FirstSendAttemptResult.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/models/HistoryResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/models/InAppOwnershipType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/models/JWSRenewalInfoDecodedPayload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8365 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/models/JWSTransactionDecodedPayload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/models/LastTransactionsItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/models/LibraryUtility.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/models/LifetimeDollarsPurchased.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/models/LifetimeDollarsRefunded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/models/MassExtendRenewalDateRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/models/MassExtendRenewalDateResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/models/MassExtendRenewalDateStatusResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/models/NotificationHistoryRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/models/NotificationHistoryResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/models/NotificationHistoryResponseItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/models/NotificationTypeV2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/models/OfferDiscountType.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/models/OfferType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/models/OrderLookupResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/models/OrderLookupStatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/models/Platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/models/PlayTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/models/PriceIncreaseStatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/models/RefundHistoryResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/models/RefundPreference.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/models/ResponseBodyV2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/models/ResponseBodyV2DecodedPayload.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/models/RevocationReason.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/models/SendAttemptItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/models/SendAttemptResult.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/models/SendTestNotificationResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/models/Status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/models/StatusResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/models/SubscriptionGroupIdentifierItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/models/Subtype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/models/Summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/models/TransactionHistoryRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/models/TransactionInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/models/TransactionReason.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/models/Type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/models/UserStatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/promotional_offer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5412 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/receipt_utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17203 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/appstoreserverlibrary/signed_data_verifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 03:34:46.577896 app_store_server_library-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 03:34:46.577896 app_store_server_library-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    28548 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/tests/test_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16096 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/tests/test_decoded_payloads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/tests/test_payload_verification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/tests/test_promotional_offer_signature_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/tests/test_receipt_utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12131 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/tests/test_x509_verifiction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5975 2024-05-14 03:34:43.000000 app_store_server_library-1.2.1/tests/test_xcode_signed_data.py
```

### Comparing `app_store_server_library-1.2.0/LICENSE.txt` & `app_store_server_library-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `app_store_server_library-1.2.0/NOTICE.txt` & `app_store_server_library-1.2.1/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `app_store_server_library-1.2.0/PKG-INFO` & `app_store_server_library-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: app-store-server-library
-Version: 1.2.0
+Version: 1.2.1
 Summary: The App Store Server Library
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 License-File: NOTICE.txt
```

### Comparing `app_store_server_library-1.2.0/README.md` & `app_store_server_library-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `app_store_server_library-1.2.0/app_store_server_library.egg-info/PKG-INFO` & `app_store_server_library-1.2.1/app_store_server_library.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: app-store-server-library
-Version: 1.2.0
+Version: 1.2.1
 Summary: The App Store Server Library
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 License-File: NOTICE.txt
```

### Comparing `app_store_server_library-1.2.0/app_store_server_library.egg-info/SOURCES.txt` & `app_store_server_library-1.2.1/app_store_server_library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `app_store_server_library-1.2.0/appstoreserverlibrary/api_client.py` & `app_store_server_library-1.2.1/appstoreserverlibrary/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -480,15 +480,15 @@
         )
 
     def _make_request(self, path: str, method: str, queryParameters: Dict[str, Union[str, List[str]]], body, destination_class: Type[T]) -> T:
         url = self._base_url + path
         c = _get_cattrs_converter(type(body)) if body is not None else None
         json = c.unstructure(body) if body is not None else None
         headers = {
-            'User-Agent': "app-store-server-library/python/1.2.0",
+            'User-Agent': "app-store-server-library/python/1.2.1",
             'Authorization': 'Bearer ' + self._generate_token(),
             'Accept': 'application/json'
         }
         
         response = self._execute_request(method, url, queryParameters, headers, json)
         if 200 <= response.status_code < 300:
             if destination_class is None:
```

### Comparing `app_store_server_library-1.2.0/appstoreserverlibrary/models/AccountTenure.py` & `app_store_server_library-1.2.1/appstoreserverlibrary/models/AccountTenure.py`

 * *Files identical despite different names*

### Comparing `app_store_server_library-1.2.0/appstoreserverlibrary/models/AppTransaction.py` & `app_store_server_library-1.2.1/appstoreserverlibrary/models/AppTransaction.py`

 * *Files identical despite different names*

### Comparing `app_store_server_library-1.2.0/appstoreserverlibrary/models/CheckTestNotificationResponse.py` & `app_store_server_library-1.2.1/appstoreserverlibrary/models/CheckTestNotificationResponse.py`

 * *Files identical despite different names*

### Comparing `app_store_server_library-1.2.0/appstoreserverlibrary/models/ConsumptionRequest.py` & `app_store_server_library-1.2.1/appstoreserverlibrary/models/ConsumptionRequest.py`

 * *Files identical despite different names*

### Comparing `app_store_server_library-1.2.0/appstoreserverlibrary/models/ConsumptionRequestReason.py` & `app_store_server_library-1.2.1/appstoreserverlibrary/models/ConsumptionRequestReason.py`

 * *Files identical despite different names*

### Comparing `app_store_server_library-1.2.0/appstoreserverlibrary/models/Data.py` & `app_store_server_library-1.2.1/appstoreserverlibrary/models/Data.py`

 * *Files identical despite different names*

### Comparing `app_store_server_library-1.2.0/appstoreserverlibrary/models/DeliveryStatus.py` & `app_store_server_library-1.2.1/appstoreserverlibrary/models/DeliveryStatus.py`

 * *Files identical despite different names*

### Comparing `app_store_server_library-1.2.0/appstoreserverlibrary/models/ExpirationIntent.py` & `app_store_server_library-1.2.1/appstoreserverlibrary/models/ExpirationIntent.py`

 * *Files identical despite different names*

### Comparing `app_store_server_library-1.2.0/appstoreserverlibrary/models/ExtendRenewalDateRequest.py` & `app_store_server_library-1.2.1/appstoreserverlibrary/models/ExtendRenewalDateRequest.py`

 * *Files identical despite different names*

### Comparing `app_store_server_library-1.2.0/appstoreserverlibrary/models/ExtendRenewalDateResponse.py` & `app_store_server_library-1.2.1/appstoreserverlibrary/models/ExtendRenewalDateResponse.py`

 * *Files identical despite different names*

### Comparing `app_store_server_library-1.2.0/appstoreserverlibrary/models/ExternalPurchaseToken.py` & `app_store_server_library-1.2.1/appstoreserverlibrary/models/ExternalPurchaseToken.py`

 * *Files identical despite different names*

### Comparing `app_store_server_library-1.2.0/appstoreserverlibrary/models/FirstSendAttemptResult.py` & `app_store_server_library-1.2.1/appstoreserverlibrary/models/FirstSendAttemptResult.py`

 * *Files identical despite different names*

### Comparing `app_store_server_library-1.2.0/appstoreserverlibrary/models/HistoryResponse.py` & `app_store_server_library-1.2.1/appstoreserverlibrary/models/HistoryResponse.py`

 * *Files identical despite different names*

### Comparing `app_store_server_library-1.2.0/appstoreserverlibrary/models/JWSRenewalInfoDecodedPayload.py` & `app_store_server_library-1.2.1/appstoreserverlibrary/models/JWSRenewalInfoDecodedPayload.py`

 * *Files identical despite different names*

### Comparing `app_store_server_library-1.2.0/appstoreserverlibrary/models/JWSTransactionDecodedPayload.py` & `app_store_server_library-1.2.1/appstoreserverlibrary/models/JWSTransactionDecodedPayload.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,15 +152,15 @@
     isUpgraded: Optional[bool] = attr.ib(default=None)
     """
     The Boolean value that indicates whether the user upgraded to another subscription.
     
     https://developer.apple.com/documentation/appstoreserverapi/isupgraded
     """
 
-    offerType: Optional[OfferType] = RevocationReason.create_main_attr('rawOfferType')
+    offerType: Optional[OfferType] = OfferType.create_main_attr('rawOfferType')
     """
     A value that represents the promotional offer type.
     
     https://developer.apple.com/documentation/appstoreserverapi/offertype
     """
 
     rawOfferType: Optional[int] = OfferType.create_raw_attr('offerType')
```

### Comparing `app_store_server_library-1.2.0/appstoreserverlibrary/models/LastTransactionsItem.py` & `app_store_server_library-1.2.1/appstoreserverlibrary/models/LastTransactionsItem.py`

 * *Files identical despite different names*

### Comparing `app_store_server_library-1.2.0/appstoreserverlibrary/models/LibraryUtility.py` & `app_store_server_library-1.2.1/appstoreserverlibrary/models/LibraryUtility.py`

 * *Files identical despite different names*

### Comparing `app_store_server_library-1.2.0/appstoreserverlibrary/models/LifetimeDollarsPurchased.py` & `app_store_server_library-1.2.1/appstoreserverlibrary/models/LifetimeDollarsPurchased.py`

 * *Files identical despite different names*

### Comparing `app_store_server_library-1.2.0/appstoreserverlibrary/models/LifetimeDollarsRefunded.py` & `app_store_server_library-1.2.1/appstoreserverlibrary/models/LifetimeDollarsRefunded.py`

 * *Files identical despite different names*

### Comparing `app_store_server_library-1.2.0/appstoreserverlibrary/models/MassExtendRenewalDateRequest.py` & `app_store_server_library-1.2.1/appstoreserverlibrary/models/MassExtendRenewalDateRequest.py`

 * *Files identical despite different names*

### Comparing `app_store_server_library-1.2.0/appstoreserverlibrary/models/MassExtendRenewalDateResponse.py` & `app_store_server_library-1.2.1/appstoreserverlibrary/models/MassExtendRenewalDateResponse.py`

 * *Files identical despite different names*

### Comparing `app_store_server_library-1.2.0/appstoreserverlibrary/models/MassExtendRenewalDateStatusResponse.py` & `app_store_server_library-1.2.1/appstoreserverlibrary/models/MassExtendRenewalDateStatusResponse.py`

 * *Files identical despite different names*

### Comparing `app_store_server_library-1.2.0/appstoreserverlibrary/models/NotificationHistoryRequest.py` & `app_store_server_library-1.2.1/appstoreserverlibrary/models/NotificationHistoryRequest.py`

 * *Files identical despite different names*

### Comparing `app_store_server_library-1.2.0/appstoreserverlibrary/models/NotificationHistoryResponse.py` & `app_store_server_library-1.2.1/appstoreserverlibrary/models/NotificationHistoryResponse.py`

 * *Files identical despite different names*

### Comparing `app_store_server_library-1.2.0/appstoreserverlibrary/models/NotificationHistoryResponseItem.py` & `app_store_server_library-1.2.1/appstoreserverlibrary/models/NotificationHistoryResponseItem.py`

 * *Files identical despite different names*

### Comparing `app_store_server_library-1.2.0/appstoreserverlibrary/models/NotificationTypeV2.py` & `app_store_server_library-1.2.1/appstoreserverlibrary/models/NotificationTypeV2.py`

 * *Files identical despite different names*

### Comparing `app_store_server_library-1.2.0/appstoreserverlibrary/models/OfferDiscountType.py` & `app_store_server_library-1.2.1/appstoreserverlibrary/models/OfferDiscountType.py`

 * *Files identical despite different names*

### Comparing `app_store_server_library-1.2.0/appstoreserverlibrary/models/OrderLookupResponse.py` & `app_store_server_library-1.2.1/appstoreserverlibrary/models/OrderLookupResponse.py`

 * *Files identical despite different names*

### Comparing `app_store_server_library-1.2.0/appstoreserverlibrary/models/PlayTime.py` & `app_store_server_library-1.2.1/appstoreserverlibrary/models/PlayTime.py`

 * *Files identical despite different names*

### Comparing `app_store_server_library-1.2.0/appstoreserverlibrary/models/PriceIncreaseStatus.py` & `app_store_server_library-1.2.1/appstoreserverlibrary/models/PriceIncreaseStatus.py`

 * *Files identical despite different names*

### Comparing `app_store_server_library-1.2.0/appstoreserverlibrary/models/RefundHistoryResponse.py` & `app_store_server_library-1.2.1/appstoreserverlibrary/models/RefundHistoryResponse.py`

 * *Files identical despite different names*

### Comparing `app_store_server_library-1.2.0/appstoreserverlibrary/models/ResponseBodyV2.py` & `app_store_server_library-1.2.1/appstoreserverlibrary/models/ResponseBodyV2.py`

 * *Files identical despite different names*

### Comparing `app_store_server_library-1.2.0/appstoreserverlibrary/models/ResponseBodyV2DecodedPayload.py` & `app_store_server_library-1.2.1/appstoreserverlibrary/models/ResponseBodyV2DecodedPayload.py`

 * *Files identical despite different names*

### Comparing `app_store_server_library-1.2.0/appstoreserverlibrary/models/SendAttemptItem.py` & `app_store_server_library-1.2.1/appstoreserverlibrary/models/SendAttemptItem.py`

 * *Files identical despite different names*

### Comparing `app_store_server_library-1.2.0/appstoreserverlibrary/models/SendAttemptResult.py` & `app_store_server_library-1.2.1/appstoreserverlibrary/models/SendAttemptResult.py`

 * *Files identical despite different names*

### Comparing `app_store_server_library-1.2.0/appstoreserverlibrary/models/SendTestNotificationResponse.py` & `app_store_server_library-1.2.1/appstoreserverlibrary/models/SendTestNotificationResponse.py`

 * *Files identical despite different names*

### Comparing `app_store_server_library-1.2.0/appstoreserverlibrary/models/StatusResponse.py` & `app_store_server_library-1.2.1/appstoreserverlibrary/models/StatusResponse.py`

 * *Files identical despite different names*

### Comparing `app_store_server_library-1.2.0/appstoreserverlibrary/models/SubscriptionGroupIdentifierItem.py` & `app_store_server_library-1.2.1/appstoreserverlibrary/models/SubscriptionGroupIdentifierItem.py`

 * *Files identical despite different names*

### Comparing `app_store_server_library-1.2.0/appstoreserverlibrary/models/Subtype.py` & `app_store_server_library-1.2.1/appstoreserverlibrary/models/Subtype.py`

 * *Files identical despite different names*

### Comparing `app_store_server_library-1.2.0/appstoreserverlibrary/models/Summary.py` & `app_store_server_library-1.2.1/appstoreserverlibrary/models/Summary.py`

 * *Files identical despite different names*

### Comparing `app_store_server_library-1.2.0/appstoreserverlibrary/models/TransactionHistoryRequest.py` & `app_store_server_library-1.2.1/appstoreserverlibrary/models/TransactionHistoryRequest.py`

 * *Files identical despite different names*

### Comparing `app_store_server_library-1.2.0/appstoreserverlibrary/models/TransactionInfoResponse.py` & `app_store_server_library-1.2.1/appstoreserverlibrary/models/TransactionInfoResponse.py`

 * *Files identical despite different names*

### Comparing `app_store_server_library-1.2.0/appstoreserverlibrary/models/TransactionReason.py` & `app_store_server_library-1.2.1/appstoreserverlibrary/models/TransactionReason.py`

 * *Files identical despite different names*

### Comparing `app_store_server_library-1.2.0/appstoreserverlibrary/models/Type.py` & `app_store_server_library-1.2.1/appstoreserverlibrary/models/Type.py`

 * *Files identical despite different names*

### Comparing `app_store_server_library-1.2.0/appstoreserverlibrary/promotional_offer.py` & `app_store_server_library-1.2.1/appstoreserverlibrary/promotional_offer.py`

 * *Files identical despite different names*

### Comparing `app_store_server_library-1.2.0/appstoreserverlibrary/receipt_utility.py` & `app_store_server_library-1.2.1/appstoreserverlibrary/receipt_utility.py`

 * *Files identical despite different names*

### Comparing `app_store_server_library-1.2.0/appstoreserverlibrary/signed_data_verifier.py` & `app_store_server_library-1.2.1/appstoreserverlibrary/signed_data_verifier.py`

 * *Files identical despite different names*

### Comparing `app_store_server_library-1.2.0/setup.py` & `app_store_server_library-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools import find_packages, setup
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="app-store-server-library",
-    version="1.2.0",
+    version="1.2.1",
     description="The App Store Server Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(exclude=["tests"]),
     python_requires=">=3.7, <4",
     install_requires=["attrs >= 21.3.0", 'PyJWT >= 2.6.0, < 3', 'requests >= 2.28.0, < 3', 'cryptography >= 40.0.0, < 43', 'pyOpenSSL >= 23.1.1, < 25', 'asn1==2.7.0', 'cattrs==23.1.2'],
     package_data={"appstoreserverlibrary": ["py.typed"]},
```

### Comparing `app_store_server_library-1.2.0/tests/test_api_client.py` & `app_store_server_library-1.2.1/tests/test_api_client.py`

 * *Files identical despite different names*

### Comparing `app_store_server_library-1.2.0/tests/test_decoded_payloads.py` & `app_store_server_library-1.2.1/tests/test_decoded_payloads.py`

 * *Files identical despite different names*

### Comparing `app_store_server_library-1.2.0/tests/test_payload_verification.py` & `app_store_server_library-1.2.1/tests/test_payload_verification.py`

 * *Files identical despite different names*

### Comparing `app_store_server_library-1.2.0/tests/test_promotional_offer_signature_creator.py` & `app_store_server_library-1.2.1/tests/test_promotional_offer_signature_creator.py`

 * *Files identical despite different names*

### Comparing `app_store_server_library-1.2.0/tests/test_receipt_utility.py` & `app_store_server_library-1.2.1/tests/test_receipt_utility.py`

 * *Files identical despite different names*

### Comparing `app_store_server_library-1.2.0/tests/test_x509_verifiction.py` & `app_store_server_library-1.2.1/tests/test_x509_verifiction.py`

 * *Files identical despite different names*

### Comparing `app_store_server_library-1.2.0/tests/test_xcode_signed_data.py` & `app_store_server_library-1.2.1/tests/test_xcode_signed_data.py`

 * *Files identical despite different names*

