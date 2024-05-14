# Comparing `tmp/lightspark-2.6.0.zip` & `tmp/lightspark-2.7.0.zip`

## zipinfo {}

```diff
@@ -1,223 +1,228 @@
-Zip file size: 219474 bytes, number of entries: 221
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-08 23:22 lightspark-2.6.0/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-08 23:22 lightspark-2.6.0/lightspark/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-08 23:22 lightspark-2.6.0/lightspark.egg-info/
--rwxr-xr-x  2.0 unx       87 b- defN 24-Mar-08 23:22 lightspark-2.6.0/setup.py
--rw-r--r--  2.0 unx    11352 b- defN 24-Mar-08 23:22 lightspark-2.6.0/LICENSE
--rw-r--r--  2.0 unx     1035 b- defN 24-Mar-08 23:22 lightspark-2.6.0/README.md
--rw-r--r--  2.0 unx       81 b- defN 24-Mar-08 23:22 lightspark-2.6.0/pyproject.toml
--rw-r--r--  2.0 unx      739 b- defN 24-Mar-08 23:22 lightspark-2.6.0/setup.cfg
--rw-r--r--  2.0 unx     1605 b- defN 24-Mar-08 23:22 lightspark-2.6.0/PKG-INFO
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-08 23:22 lightspark-2.6.0/lightspark/requests/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-08 23:22 lightspark-2.6.0/lightspark/utils/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-08 23:22 lightspark-2.6.0/lightspark/scripts/
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/py.typed
--rw-r--r--  2.0 unx     2354 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/webhooks.py
--rw-r--r--  2.0 unx       22 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/version.py
--rw-r--r--  2.0 unx     1038 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/remote_signing.py
--rw-r--r--  2.0 unx    33236 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/lightspark_client.py
--rw-r--r--  2.0 unx    12628 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/__init__.py
--rw-r--r--  2.0 unx      185 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/exceptions.py
--rw-r--r--  2.0 unx      416 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/requests/encoder.py
--rw-r--r--  2.0 unx       75 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/requests/__init__.py
--rw-r--r--  2.0 unx     4318 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/requests/requester.py
--rw-r--r--  2.0 unx     1587 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/utils/signing_key.py
--rw-r--r--  2.0 unx     3676 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/utils/crypto.py
--rw-r--r--  2.0 unx     1146 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/utils/enums.py
--rw-r--r--  2.0 unx     1151 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/utils/currency_amount.py
--rw-r--r--  2.0 unx      137 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/utils/__init__.py
--rw-r--r--  2.0 unx      924 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/ReleasePaymentPreimageOutput.py
--rw-r--r--  2.0 unx     6193 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/BlockchainBalance.py
--rw-r--r--  2.0 unx    38939 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/LightsparkNode.py
--rw-r--r--  2.0 unx     1341 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/CreateTestModeInvoiceInput.py
--rw-r--r--  2.0 unx     1807 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/NodeToAddressesConnection.py
--rw-r--r--  2.0 unx     1432 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/CurrencyUnit.py
--rw-r--r--  2.0 unx      892 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/RequestWithdrawalOutput.py
--rw-r--r--  2.0 unx     1927 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/HtlcAttemptFailureCode.py
--rw-r--r--  2.0 unx    48520 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/Transaction.py
--rw-r--r--  2.0 unx      711 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/UpdateNodeSharedSecretInput.py
--rw-r--r--  2.0 unx     1519 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/SendPaymentInput.py
--rw-r--r--  2.0 unx     2980 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/IncomingPaymentsForInvoiceQueryOutput.py
--rw-r--r--  2.0 unx    10338 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/OutgoingPaymentAttempt.py
--rw-r--r--  2.0 unx     1546 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/ChannelStatus.py
--rw-r--r--  2.0 unx    36020 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/LightningTransaction.py
--rw-r--r--  2.0 unx      948 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/CreateUmaInvitationOutput.py
--rw-r--r--  2.0 unx     1493 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/WithdrawalFeeEstimateOutput.py
--rw-r--r--  2.0 unx     3984 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/Balances.py
--rw-r--r--  2.0 unx     3198 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/SignablePayload.py
--rw-r--r--  2.0 unx     5785 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/AccountToTransactionsConnection.py
--rw-r--r--  2.0 unx    15709 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/Channel.py
--rw-r--r--  2.0 unx   125116 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/Account.py
--rw-r--r--  2.0 unx     9495 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/Connection.py
--rw-r--r--  2.0 unx     1646 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/CreateInvoiceInput.py
--rw-r--r--  2.0 unx      470 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/PaymentDirection.py
--rw-r--r--  2.0 unx      801 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/CreateInvoiceOutput.py
--rw-r--r--  2.0 unx      569 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/IncomingPaymentAttemptStatus.py
--rw-r--r--  2.0 unx     1491 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/CreateTestModePaymentoutput.py
--rw-r--r--  2.0 unx     1069 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/CreateInvitationWithIncentivesOutput.py
--rw-r--r--  2.0 unx     1004 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/CreateUmaInvoiceInput.py
--rw-r--r--  2.0 unx    16377 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/OnChainTransaction.py
--rw-r--r--  2.0 unx    20632 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/InvoiceData.py
--rw-r--r--  2.0 unx     2619 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/WalletToPaymentRequestsConnection.py
--rw-r--r--  2.0 unx      497 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/SignablePayloadStatus.py
--rw-r--r--  2.0 unx     1138 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/UpdateChannelPerCommitmentPointInput.py
--rw-r--r--  2.0 unx     1180 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/IncomingPaymentsForInvoiceQueryInput.py
--rw-r--r--  2.0 unx     1294 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/ReleaseChannelPerCommitmentSecretInput.py
--rw-r--r--  2.0 unx     6911 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/ChannelClosingTransaction.py
--rw-r--r--  2.0 unx      513 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/DeleteApiTokenInput.py
--rw-r--r--  2.0 unx     6067 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/CurrencyAmount.py
--rw-r--r--  2.0 unx      969 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/CreateTestModeInvoiceOutput.py
--rw-r--r--  2.0 unx      615 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/FundNodeInput.py
--rw-r--r--  2.0 unx     1090 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/ScreenNodeInput.py
--rw-r--r--  2.0 unx      543 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/InvoiceType.py
--rw-r--r--  2.0 unx     2793 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/AccountToWithdrawalRequestsConnection.py
--rw-r--r--  2.0 unx      935 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/SignInvoiceInput.py
--rw-r--r--  2.0 unx     6589 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/ChannelSnapshot.py
--rw-r--r--  2.0 unx      619 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/RiskRating.py
--rw-r--r--  2.0 unx      635 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/CancelInvoiceInput.py
--rw-r--r--  2.0 unx      990 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/UpdateChannelPerCommitmentPointOutput.py
--rw-r--r--  2.0 unx      849 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/BitcoinNetwork.py
--rw-r--r--  2.0 unx    18952 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/RegionCode.py
--rw-r--r--  2.0 unx      551 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/OutgoingPaymentAttemptStatus.py
--rw-r--r--  2.0 unx     2688 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/WalletToWithdrawalRequestsConnection.py
--rw-r--r--  2.0 unx     3325 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/LightsparkNodeToDailyLiquidityForecastsConnection.py
--rw-r--r--  2.0 unx     1195 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/SetInvoicePaymentHashInput.py
--rw-r--r--  2.0 unx      904 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/ClaimUmaInvitationOutput.py
--rw-r--r--  2.0 unx      964 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/Permission.py
--rw-r--r--  2.0 unx      823 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/SignInvoiceOutput.py
--rw-r--r--  2.0 unx     1579 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/RequestWithdrawalInput.py
--rw-r--r--  2.0 unx    87822 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/Entity.py
--rw-r--r--  2.0 unx     2756 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/OutgoingPaymentToAttemptsConnection.py
--rw-r--r--  2.0 unx    22165 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/Invoice.py
--rw-r--r--  2.0 unx      640 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/IdAndSignature.py
--rw-r--r--  2.0 unx      655 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/RoutingTransactionFailureReason.py
--rw-r--r--  2.0 unx     6914 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/ChannelOpeningTransaction.py
--rw-r--r--  2.0 unx    21325 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/PaymentRequestData.py
--rw-r--r--  2.0 unx     1613 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/WalletStatus.py
--rw-r--r--  2.0 unx      577 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/LightningPaymentDirection.py
--rw-r--r--  2.0 unx     2944 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/WithdrawalRequestToChannelOpeningTransactionsConnection.py
--rw-r--r--  2.0 unx      462 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/ComplianceProvider.py
--rw-r--r--  2.0 unx      864 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/UpdateNodeSharedSecretOutput.py
--rw-r--r--  2.0 unx     1080 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/ClaimUmaInvitationWithIncentivesOutput.py
--rw-r--r--  2.0 unx      604 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/WithdrawalRequestStatus.py
--rw-r--r--  2.0 unx     1119 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/WebhookEventType.py
--rw-r--r--  2.0 unx     3783 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/UmaInvitation.py
--rw-r--r--  2.0 unx      877 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/SetInvoicePaymentHashOutput.py
--rw-r--r--  2.0 unx     1172 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/PayUmaInvoiceInput.py
--rw-r--r--  2.0 unx     1377 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/WithdrawalFeeEstimateInput.py
--rw-r--r--  2.0 unx      900 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/PaymentFailureReason.py
--rw-r--r--  2.0 unx     2504 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/AuditLogActor.py
--rw-r--r--  2.0 unx     1206 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/CreateTestModePaymentInput.py
--rw-r--r--  2.0 unx      644 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/LightsparkNodeStatus.py
--rw-r--r--  2.0 unx     1836 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/ClaimUmaInvitationWithIncentivesInput.py
--rw-r--r--  2.0 unx      659 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/CreateUmaInvitationInput.py
--rw-r--r--  2.0 unx      900 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/ScreenNodeOutput.py
--rw-r--r--  2.0 unx     1483 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/LightningFeeEstimateOutput.py
--rw-r--r--  2.0 unx     2635 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/AccountToPaymentRequestsConnection.py
--rw-r--r--  2.0 unx    14407 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/all_entities.py
--rw-r--r--  2.0 unx     1268 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/FundNodeOutput.py
--rw-r--r--  2.0 unx     5177 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/LightsparkNodeOwner.py
--rw-r--r--  2.0 unx     2518 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/AccountToNodesConnection.py
--rw-r--r--  2.0 unx     1748 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/TransactionType.py
--rw-r--r--  2.0 unx    27195 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/LightsparkNodeWithRemoteSigning.py
--rw-r--r--  2.0 unx     1517 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/PageInfo.py
--rw-r--r--  2.0 unx     3961 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/IncomingPaymentAttempt.py
--rw-r--r--  2.0 unx     1668 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/ChannelFees.py
--rw-r--r--  2.0 unx    24929 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/OutgoingPaymentsForInvoiceQueryOutput.py
--rw-r--r--  2.0 unx      633 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/DeclineToSignMessagesInput.py
--rw-r--r--  2.0 unx     4273 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/ChannelToTransactionsConnection.py
--rw-r--r--  2.0 unx     2585 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/LightsparkNodeToChannelsConnection.py
--rw-r--r--  2.0 unx     1392 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/CreateLnurlInvoiceInput.py
--rw-r--r--  2.0 unx      647 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/RichText.py
--rw-r--r--  2.0 unx     5888 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/Withdrawal.py
--rw-r--r--  2.0 unx     9541 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/IncomingPayment.py
--rw-r--r--  2.0 unx      519 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/NodeAddressType.py
--rw-r--r--  2.0 unx      949 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/CreateApiTokenInput.py
--rw-r--r--  2.0 unx     2540 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/WalletToTransactionsConnection.py
--rw-r--r--  2.0 unx    84503 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/Wallet.py
--rw-r--r--  2.0 unx      937 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/ClaimUmaInvitationInput.py
--rw-r--r--  2.0 unx      527 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/WithdrawalMode.py
--rw-r--r--  2.0 unx     2464 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/AccountToChannelsConnection.py
--rw-r--r--  2.0 unx     2893 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/ApiToken.py
--rw-r--r--  2.0 unx     1293 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/OutgoingPaymentsForInvoiceQueryInput.py
--rw-r--r--  2.0 unx     1198 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/LightningFeeEstimateForNodeInput.py
--rw-r--r--  2.0 unx     2944 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/WithdrawalRequestToChannelClosingTransactionsConnection.py
--rw-r--r--  2.0 unx     1671 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/MultiSigAddressValidationParameters.py
--rw-r--r--  2.0 unx    27520 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/Node.py
--rw-r--r--  2.0 unx      811 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/IncentivesStatus.py
--rw-r--r--  2.0 unx     7110 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/RoutingTransaction.py
--rw-r--r--  2.0 unx     1086 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/ReleaseChannelPerCommitmentSecretOutput.py
--rw-r--r--  2.0 unx     1417 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/Signable.py
--rw-r--r--  2.0 unx      827 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/Secret.py
--rw-r--r--  2.0 unx      873 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/SignMessagesInput.py
--rw-r--r--  2.0 unx    14742 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/WithdrawalRequest.py
--rw-r--r--  2.0 unx     1967 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/RegisterPaymentInput.py
--rw-r--r--  2.0 unx     4269 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/Hop.py
--rw-r--r--  2.0 unx      827 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/SendPaymentOutput.py
--rw-r--r--  2.0 unx     1299 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/DeclineToSignMessagesOutput.py
--rw-r--r--  2.0 unx     2597 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/CreateNodeWalletAddressOutput.py
--rw-r--r--  2.0 unx     5187 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/GraphNode.py
--rw-r--r--  2.0 unx     1709 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/CreateApiTokenOutput.py
--rw-r--r--  2.0 unx      819 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/ReleasePaymentPreimageInput.py
--rw-r--r--  2.0 unx      999 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/TransactionStatus.py
--rw-r--r--  2.0 unx     2773 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/IncomingPaymentToAttemptsConnection.py
--rw-r--r--  2.0 unx      919 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/RemoteSigningSubEventType.py
--rw-r--r--  2.0 unx    23586 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/PaymentRequest.py
--rw-r--r--  2.0 unx       75 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/__init__.py
--rw-r--r--  2.0 unx     1477 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/CreateInvitationWithIncentivesInput.py
--rw-r--r--  2.0 unx      819 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/PayInvoiceOutput.py
--rw-r--r--  2.0 unx     1563 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/PayInvoiceInput.py
--rw-r--r--  2.0 unx      535 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/CreateNodeWalletAddressInput.py
--rw-r--r--  2.0 unx    32966 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/OutgoingPayment.py
--rw-r--r--  2.0 unx     2497 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/AccountToApiTokensConnection.py
--rw-r--r--  2.0 unx     1410 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/IncentivesIneligibilityReason.py
--rw-r--r--  2.0 unx     2310 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/DailyLiquidityForecast.py
--rw-r--r--  2.0 unx     2018 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/FeeEstimate.py
--rw-r--r--  2.0 unx     1240 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/SignMessagesOutput.py
--rw-r--r--  2.0 unx      511 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/PaymentRequestStatus.py
--rw-r--r--  2.0 unx      817 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/RegisterPaymentOutput.py
--rw-r--r--  2.0 unx     1543 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/TransactionFailures.py
--rw-r--r--  2.0 unx     2441 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/AccountToWalletsConnection.py
--rw-r--r--  2.0 unx     1310 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/LightningFeeEstimateForInvoiceInput.py
--rw-r--r--  2.0 unx     1204 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/NodeAddress.py
--rw-r--r--  2.0 unx     5774 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/Deposit.py
--rw-r--r--  2.0 unx     2777 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/OutgoingPaymentAttemptToHopsConnection.py
--rw-r--r--  2.0 unx      812 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/DeleteApiTokenOutput.py
--rw-r--r--  2.0 unx     1745 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/PostTransactionData.py
--rw-r--r--  2.0 unx    27343 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/LightsparkNodeWithOSK.py
--rw-r--r--  2.0 unx      912 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/objects/CancelInvoiceOutput.py
--rw-r--r--  2.0 unx     1068 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/scripts/claim_uma_invitation.py
--rw-r--r--  2.0 unx      475 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/scripts/decoded_payment_request.py
--rw-r--r--  2.0 unx      576 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/scripts/create_uma_invoice.py
--rw-r--r--  2.0 unx      701 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/scripts/send_payment.py
--rw-r--r--  2.0 unx      644 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/scripts/request_withdrawal.py
--rw-r--r--  2.0 unx      577 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/scripts/outgoing_payments_for_invoice.py
--rw-r--r--  2.0 unx      312 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/scripts/screen_node.py
--rw-r--r--  2.0 unx      626 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/scripts/lightning_fee_estimate_for_invoice.py
--rw-r--r--  2.0 unx      645 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/scripts/register_payment.py
--rw-r--r--  2.0 unx      266 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/scripts/delete_api_token.py
--rw-r--r--  2.0 unx      582 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/scripts/create_lnurl_invoice.py
--rw-r--r--  2.0 unx      283 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/scripts/current_account.py
--rw-r--r--  2.0 unx      477 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/scripts/create_api_token.py
--rw-r--r--  2.0 unx      433 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/scripts/fund_node.py
--rw-r--r--  2.0 unx      578 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/scripts/incoming_payments_for_invoice.py
--rw-r--r--  2.0 unx      929 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/scripts/create_uma_invitation.py
--rw-r--r--  2.0 unx      601 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/scripts/create_test_mode_payment.py
--rw-r--r--  2.0 unx      604 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/scripts/create_invoice.py
--rw-r--r--  2.0 unx      391 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/scripts/cancel_invoice.py
--rw-r--r--  2.0 unx      687 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/scripts/pay_uma_invoice.py
--rw-r--r--  2.0 unx      676 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/scripts/pay_invoice.py
--rw-r--r--  2.0 unx       75 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/scripts/__init__.py
--rw-r--r--  2.0 unx      630 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/scripts/lightning_fee_estimate_for_node.py
--rw-r--r--  2.0 unx      277 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/scripts/create_node_address.py
--rw-r--r--  2.0 unx      365 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/scripts/recover_node_signing_key.py
--rw-r--r--  2.0 unx      378 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/scripts/bitcoin_fee_estimate.py
--rw-r--r--  2.0 unx      471 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/scripts/create_test_mode_invoice.py
--rw-r--r--  2.0 unx      367 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark/scripts/fetch_uma_invitation.py
--rw-r--r--  2.0 unx        1 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx     8929 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx       11 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark.egg-info/top_level.txt
--rw-r--r--  2.0 unx     1605 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark.egg-info/PKG-INFO
--rw-r--r--  2.0 unx       53 b- defN 24-Mar-08 23:22 lightspark-2.6.0/lightspark.egg-info/requires.txt
-221 files, 1113601 bytes uncompressed, 177480 bytes compressed:  84.1%
+Zip file size: 223043 bytes, number of entries: 226
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-14 02:48 lightspark-2.7.0/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-14 02:48 lightspark-2.7.0/lightspark/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-14 02:48 lightspark-2.7.0/lightspark.egg-info/
+-rw-r--r--  2.0 unx    11352 b- defN 24-May-14 02:48 lightspark-2.7.0/LICENSE
+-rwxr-xr-x  2.0 unx       87 b- defN 24-May-14 02:48 lightspark-2.7.0/setup.py
+-rw-r--r--  2.0 unx     1035 b- defN 24-May-14 02:48 lightspark-2.7.0/README.md
+-rw-r--r--  2.0 unx       81 b- defN 24-May-14 02:48 lightspark-2.7.0/pyproject.toml
+-rw-r--r--  2.0 unx      750 b- defN 24-May-14 02:48 lightspark-2.7.0/setup.cfg
+-rw-r--r--  2.0 unx     1630 b- defN 24-May-14 02:48 lightspark-2.7.0/PKG-INFO
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-14 02:48 lightspark-2.7.0/lightspark/utils/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-14 02:48 lightspark-2.7.0/lightspark/requests/
+-rw-r--r--  2.0 unx        0 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/py.typed
+-rw-r--r--  2.0 unx       22 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/version.py
+-rw-r--r--  2.0 unx    35091 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/lightspark_client.py
+-rw-r--r--  2.0 unx    12874 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/__init__.py
+-rw-r--r--  2.0 unx      185 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/exceptions.py
+-rw-r--r--  2.0 unx     2354 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/webhooks.py
+-rw-r--r--  2.0 unx     1038 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/remote_signing.py
+-rw-r--r--  2.0 unx      912 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/CancelInvoiceOutput.py
+-rw-r--r--  2.0 unx     6800 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/ChannelClosingTransaction.py
+-rw-r--r--  2.0 unx    20571 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/InvoiceData.py
+-rw-r--r--  2.0 unx     3170 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/WithdrawalRequestToChannelOpeningTransactionsConnection.py
+-rw-r--r--  2.0 unx      999 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/TransactionStatus.py
+-rw-r--r--  2.0 unx    32826 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/OutgoingPayment.py
+-rw-r--r--  2.0 unx      949 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/CreateApiTokenInput.py
+-rw-r--r--  2.0 unx      635 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/CancelInvoiceInput.py
+-rw-r--r--  2.0 unx      543 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/InvoiceType.py
+-rw-r--r--  2.0 unx     2688 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/WalletToWithdrawalRequestsConnection.py
+-rw-r--r--  2.0 unx     1086 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/ReleaseChannelPerCommitmentSecretOutput.py
+-rw-r--r--  2.0 unx     2585 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/LightsparkNodeToChannelsConnection.py
+-rw-r--r--  2.0 unx      551 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/OutgoingPaymentAttemptStatus.py
+-rw-r--r--  2.0 unx      951 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/RemoteSigningSubEventType.py
+-rw-r--r--  2.0 unx     1824 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/RequestWithdrawalInput.py
+-rw-r--r--  2.0 unx      823 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/SignInvoiceOutput.py
+-rw-r--r--  2.0 unx      964 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/Permission.py
+-rw-r--r--  2.0 unx     1206 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/CreateTestModePaymentInput.py
+-rw-r--r--  2.0 unx     1080 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/ClaimUmaInvitationWithIncentivesOutput.py
+-rw-r--r--  2.0 unx      769 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/FailHtlcsOutput.py
+-rw-r--r--  2.0 unx     1519 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/SendPaymentInput.py
+-rw-r--r--  2.0 unx      633 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/DeclineToSignMessagesInput.py
+-rw-r--r--  2.0 unx      801 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/CreateInvoiceOutput.py
+-rw-r--r--  2.0 unx     5777 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/Withdrawal.py
+-rw-r--r--  2.0 unx     1299 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/DeclineToSignMessagesOutput.py
+-rw-r--r--  2.0 unx     1833 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/RegisterPaymentInput.py
+-rw-r--r--  2.0 unx     6010 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/CurrencyAmount.py
+-rw-r--r--  2.0 unx    48408 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/Transaction.py
+-rw-r--r--  2.0 unx      640 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/IdAndSignature.py
+-rw-r--r--  2.0 unx     1294 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/ReleaseChannelPerCommitmentSecretInput.py
+-rw-r--r--  2.0 unx     2773 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/IncomingPaymentToAttemptsConnection.py
+-rw-r--r--  2.0 unx     1613 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/WalletStatus.py
+-rw-r--r--  2.0 unx    10741 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/Connection.py
+-rw-r--r--  2.0 unx      847 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/ScreenNodeOutput.py
+-rw-r--r--  2.0 unx      527 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/WithdrawalMode.py
+-rw-r--r--  2.0 unx      659 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/CreateUmaInvitationInput.py
+-rw-r--r--  2.0 unx     1069 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/CreateInvitationWithIncentivesOutput.py
+-rw-r--r--  2.0 unx    27441 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/Node.py
+-rw-r--r--  2.0 unx     6193 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/BlockchainBalance.py
+-rw-r--r--  2.0 unx     3872 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/IncomingPaymentAttempt.py
+-rw-r--r--  2.0 unx     1563 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/PayInvoiceInput.py
+-rw-r--r--  2.0 unx     2777 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/OutgoingPaymentAttemptToHopsConnection.py
+-rw-r--r--  2.0 unx      655 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/RoutingTransactionFailureReason.py
+-rw-r--r--  2.0 unx     1138 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/UpdateChannelPerCommitmentPointInput.py
+-rw-r--r--  2.0 unx      497 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/SignablePayloadStatus.py
+-rw-r--r--  2.0 unx     1591 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/CreateInvoiceInput.py
+-rw-r--r--  2.0 unx    85008 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/Wallet.py
+-rw-r--r--  2.0 unx     3170 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/WithdrawalRequestToChannelClosingTransactionsConnection.py
+-rw-r--r--  2.0 unx      647 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/RichText.py
+-rw-r--r--  2.0 unx     1286 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/CreateTestModeInvoiceInput.py
+-rw-r--r--  2.0 unx    18534 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/WithdrawalRequest.py
+-rw-r--r--  2.0 unx     1293 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/OutgoingPaymentsForInvoiceQueryInput.py
+-rw-r--r--  2.0 unx     1119 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/WebhookEventType.py
+-rw-r--r--  2.0 unx     1745 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/PostTransactionData.py
+-rw-r--r--  2.0 unx     2635 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/AccountToPaymentRequestsConnection.py
+-rw-r--r--  2.0 unx      873 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/SignMessagesInput.py
+-rw-r--r--  2.0 unx     2464 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/AccountToChannelsConnection.py
+-rw-r--r--  2.0 unx     1240 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/SignMessagesOutput.py
+-rw-r--r--  2.0 unx     1417 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/Signable.py
+-rw-r--r--  2.0 unx      577 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/LightningPaymentDirection.py
+-rw-r--r--  2.0 unx     1268 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/FundNodeOutput.py
+-rw-r--r--  2.0 unx     2018 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/FeeEstimate.py
+-rw-r--r--  2.0 unx     5126 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/GraphNode.py
+-rw-r--r--  2.0 unx     9474 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/IncomingPayment.py
+-rw-r--r--  2.0 unx     2518 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/AccountToNodesConnection.py
+-rw-r--r--  2.0 unx      644 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/LightsparkNodeStatus.py
+-rw-r--r--  2.0 unx     1671 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/MultiSigAddressValidationParameters.py
+-rw-r--r--  2.0 unx      470 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/PaymentDirection.py
+-rw-r--r--  2.0 unx      864 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/UpdateNodeSharedSecretOutput.py
+-rw-r--r--  2.0 unx     1310 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/LightningFeeEstimateForInvoiceInput.py
+-rw-r--r--  2.0 unx    88288 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/Entity.py
+-rw-r--r--  2.0 unx      892 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/RequestWithdrawalOutput.py
+-rw-r--r--  2.0 unx      819 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/ReleasePaymentPreimageInput.py
+-rw-r--r--  2.0 unx     3242 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/LightsparkNodeToDailyLiquidityForecastsConnection.py
+-rw-r--r--  2.0 unx      849 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/BitcoinNetwork.py
+-rw-r--r--  2.0 unx     2227 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/DailyLiquidityForecast.py
+-rw-r--r--  2.0 unx     2893 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/ApiToken.py
+-rw-r--r--  2.0 unx     3618 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/UmaInvitation.py
+-rw-r--r--  2.0 unx   125678 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/Account.py
+-rw-r--r--  2.0 unx     2597 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/CreateNodeWalletAddressOutput.py
+-rw-r--r--  2.0 unx      812 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/DeleteApiTokenOutput.py
+-rw-r--r--  2.0 unx     6939 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/RoutingTransaction.py
+-rw-r--r--  2.0 unx     5785 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/AccountToTransactionsConnection.py
+-rw-r--r--  2.0 unx     5159 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/LightsparkNodeOwner.py
+-rw-r--r--  2.0 unx     1491 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/CreateTestModePaymentoutput.py
+-rw-r--r--  2.0 unx     1546 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/ChannelStatus.py
+-rw-r--r--  2.0 unx     1783 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/ClaimUmaInvitationWithIncentivesInput.py
+-rw-r--r--  2.0 unx      630 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/WithdrawalRequestStatus.py
+-rw-r--r--  2.0 unx     5663 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/Deposit.py
+-rw-r--r--  2.0 unx     1180 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/IncomingPaymentsForInvoiceQueryInput.py
+-rw-r--r--  2.0 unx     1927 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/HtlcAttemptFailureCode.py
+-rw-r--r--  2.0 unx    14407 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/all_entities.py
+-rw-r--r--  2.0 unx       75 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/__init__.py
+-rw-r--r--  2.0 unx    22092 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/Invoice.py
+-rw-r--r--  2.0 unx      511 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/PaymentRequestStatus.py
+-rw-r--r--  2.0 unx     1195 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/SetInvoicePaymentHashInput.py
+-rw-r--r--  2.0 unx    18952 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/RegionCode.py
+-rw-r--r--  2.0 unx      900 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/PaymentFailureReason.py
+-rw-r--r--  2.0 unx      935 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/SignInvoiceInput.py
+-rw-r--r--  2.0 unx     1392 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/CreateLnurlInvoiceInput.py
+-rw-r--r--  2.0 unx     1748 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/TransactionType.py
+-rw-r--r--  2.0 unx     1141 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/NodeAddress.py
+-rw-r--r--  2.0 unx     1668 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/ChannelFees.py
+-rw-r--r--  2.0 unx     4273 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/ChannelToTransactionsConnection.py
+-rw-r--r--  2.0 unx     3123 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/SignablePayload.py
+-rw-r--r--  2.0 unx      990 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/UpdateChannelPerCommitmentPointOutput.py
+-rw-r--r--  2.0 unx      844 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/FailHtlcsInput.py
+-rw-r--r--  2.0 unx     2793 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/AccountToWithdrawalRequestsConnection.py
+-rw-r--r--  2.0 unx      937 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/ClaimUmaInvitationInput.py
+-rw-r--r--  2.0 unx     4269 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/Hop.py
+-rw-r--r--  2.0 unx      904 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/ClaimUmaInvitationOutput.py
+-rw-r--r--  2.0 unx      827 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/SendPaymentOutput.py
+-rw-r--r--  2.0 unx    10172 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/OutgoingPaymentAttempt.py
+-rw-r--r--  2.0 unx      711 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/UpdateNodeSharedSecretInput.py
+-rw-r--r--  2.0 unx     2756 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/OutgoingPaymentToAttemptsConnection.py
+-rw-r--r--  2.0 unx      811 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/IncentivesStatus.py
+-rw-r--r--  2.0 unx    23513 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/PaymentRequest.py
+-rw-r--r--  2.0 unx    21264 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/PaymentRequestData.py
+-rw-r--r--  2.0 unx     1424 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/CreateInvitationWithIncentivesInput.py
+-rw-r--r--  2.0 unx     1004 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/CreateUmaInvoiceInput.py
+-rw-r--r--  2.0 unx     1432 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/CurrencyUnit.py
+-rw-r--r--  2.0 unx     3984 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/Balances.py
+-rw-r--r--  2.0 unx     2619 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/WalletToPaymentRequestsConnection.py
+-rw-r--r--  2.0 unx      827 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/Secret.py
+-rw-r--r--  2.0 unx     1172 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/PayUmaInvoiceInput.py
+-rw-r--r--  2.0 unx     6589 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/ChannelSnapshot.py
+-rw-r--r--  2.0 unx     2497 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/AccountToApiTokensConnection.py
+-rw-r--r--  2.0 unx     1807 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/NodeToAddressesConnection.py
+-rw-r--r--  2.0 unx      519 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/NodeAddressType.py
+-rw-r--r--  2.0 unx      969 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/CreateTestModeInvoiceOutput.py
+-rw-r--r--  2.0 unx     1483 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/LightningFeeEstimateOutput.py
+-rw-r--r--  2.0 unx      924 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/ReleasePaymentPreimageOutput.py
+-rw-r--r--  2.0 unx      877 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/SetInvoicePaymentHashOutput.py
+-rw-r--r--  2.0 unx     2504 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/AuditLogActor.py
+-rw-r--r--  2.0 unx     2441 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/AccountToWalletsConnection.py
+-rw-r--r--  2.0 unx     1198 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/LightningFeeEstimateForNodeInput.py
+-rw-r--r--  2.0 unx     1410 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/IncentivesIneligibilityReason.py
+-rw-r--r--  2.0 unx      513 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/DeleteApiTokenInput.py
+-rw-r--r--  2.0 unx    39085 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/LightsparkNode.py
+-rw-r--r--  2.0 unx      619 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/RiskRating.py
+-rw-r--r--  2.0 unx     1493 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/WithdrawalFeeEstimateOutput.py
+-rw-r--r--  2.0 unx    27341 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/LightsparkNodeWithRemoteSigning.py
+-rw-r--r--  2.0 unx     6803 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/ChannelOpeningTransaction.py
+-rw-r--r--  2.0 unx     1316 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/WithdrawalFeeEstimateInput.py
+-rw-r--r--  2.0 unx    24929 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/OutgoingPaymentsForInvoiceQueryOutput.py
+-rw-r--r--  2.0 unx     1021 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/ScreenNodeInput.py
+-rw-r--r--  2.0 unx     2980 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/IncomingPaymentsForInvoiceQueryOutput.py
+-rw-r--r--  2.0 unx     1789 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/WithdrawalRequestToWithdrawalsConnection.py
+-rw-r--r--  2.0 unx      535 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/CreateNodeWalletAddressInput.py
+-rw-r--r--  2.0 unx    27489 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/LightsparkNodeWithOSK.py
+-rw-r--r--  2.0 unx    15650 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/Channel.py
+-rw-r--r--  2.0 unx      615 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/FundNodeInput.py
+-rw-r--r--  2.0 unx     1543 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/TransactionFailures.py
+-rw-r--r--  2.0 unx     1709 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/CreateApiTokenOutput.py
+-rw-r--r--  2.0 unx      462 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/ComplianceProvider.py
+-rw-r--r--  2.0 unx     1517 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/PageInfo.py
+-rw-r--r--  2.0 unx      948 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/CreateUmaInvitationOutput.py
+-rw-r--r--  2.0 unx    16266 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/OnChainTransaction.py
+-rw-r--r--  2.0 unx      817 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/RegisterPaymentOutput.py
+-rw-r--r--  2.0 unx     2540 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/WalletToTransactionsConnection.py
+-rw-r--r--  2.0 unx    35908 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/LightningTransaction.py
+-rw-r--r--  2.0 unx      569 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/IncomingPaymentAttemptStatus.py
+-rw-r--r--  2.0 unx      819 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/objects/PayInvoiceOutput.py
+-rw-r--r--  2.0 unx     1151 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/utils/currency_amount.py
+-rw-r--r--  2.0 unx     3848 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/utils/crypto.py
+-rw-r--r--  2.0 unx     1587 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/utils/signing_key.py
+-rw-r--r--  2.0 unx      137 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/utils/__init__.py
+-rw-r--r--  2.0 unx     1146 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/utils/enums.py
+-rw-r--r--  2.0 unx      471 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/create_test_mode_invoice.py
+-rw-r--r--  2.0 unx      644 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/request_withdrawal.py
+-rw-r--r--  2.0 unx      601 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/create_test_mode_payment.py
+-rw-r--r--  2.0 unx      582 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/outgoing_payments_for_payment_hash.py
+-rw-r--r--  2.0 unx      630 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/lightning_fee_estimate_for_node.py
+-rw-r--r--  2.0 unx      365 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/recover_node_signing_key.py
+-rw-r--r--  2.0 unx      266 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/delete_api_token.py
+-rw-r--r--  2.0 unx      378 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/bitcoin_fee_estimate.py
+-rw-r--r--  2.0 unx      367 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/fetch_uma_invitation.py
+-rw-r--r--  2.0 unx      582 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/create_lnurl_invoice.py
+-rw-r--r--  2.0 unx      277 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/create_node_address.py
+-rw-r--r--  2.0 unx      312 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/screen_node.py
+-rw-r--r--  2.0 unx      645 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/register_payment.py
+-rw-r--r--  2.0 unx      626 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/lightning_fee_estimate_for_invoice.py
+-rw-r--r--  2.0 unx      578 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/incoming_payments_for_invoice.py
+-rw-r--r--  2.0 unx      433 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/fund_node.py
+-rw-r--r--  2.0 unx       75 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/__init__.py
+-rw-r--r--  2.0 unx      577 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/outgoing_payments_for_invoice.py
+-rw-r--r--  2.0 unx      687 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/pay_uma_invoice.py
+-rw-r--r--  2.0 unx      475 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/decoded_payment_request.py
+-rw-r--r--  2.0 unx     1068 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/claim_uma_invitation.py
+-rw-r--r--  2.0 unx      391 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/cancel_invoice.py
+-rw-r--r--  2.0 unx      283 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/current_account.py
+-rw-r--r--  2.0 unx      306 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/fail_htlcs.py
+-rw-r--r--  2.0 unx      929 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/create_uma_invitation.py
+-rw-r--r--  2.0 unx      701 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/send_payment.py
+-rw-r--r--  2.0 unx      676 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/pay_invoice.py
+-rw-r--r--  2.0 unx      477 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/create_api_token.py
+-rw-r--r--  2.0 unx      576 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/create_uma_invoice.py
+-rw-r--r--  2.0 unx      604 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/scripts/create_invoice.py
+-rw-r--r--  2.0 unx      416 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/requests/encoder.py
+-rw-r--r--  2.0 unx     4775 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/requests/requester.py
+-rw-r--r--  2.0 unx       75 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark/requests/__init__.py
+-rw-r--r--  2.0 unx        1 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx     9157 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx       11 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark.egg-info/top_level.txt
+-rw-r--r--  2.0 unx     1630 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx       63 b- defN 24-May-14 02:48 lightspark-2.7.0/lightspark.egg-info/requires.txt
+226 files, 1125728 bytes uncompressed, 180053 bytes compressed:  84.0%
```

## zipnote {}

```diff
@@ -1,664 +1,679 @@
-Filename: lightspark-2.6.0/
+Filename: lightspark-2.7.0/
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/
+Filename: lightspark-2.7.0/lightspark/
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark.egg-info/
+Filename: lightspark-2.7.0/lightspark.egg-info/
 Comment: 
 
-Filename: lightspark-2.6.0/setup.py
+Filename: lightspark-2.7.0/LICENSE
 Comment: 
 
-Filename: lightspark-2.6.0/LICENSE
+Filename: lightspark-2.7.0/setup.py
 Comment: 
 
-Filename: lightspark-2.6.0/README.md
+Filename: lightspark-2.7.0/README.md
 Comment: 
 
-Filename: lightspark-2.6.0/pyproject.toml
+Filename: lightspark-2.7.0/pyproject.toml
 Comment: 
 
-Filename: lightspark-2.6.0/setup.cfg
+Filename: lightspark-2.7.0/setup.cfg
 Comment: 
 
-Filename: lightspark-2.6.0/PKG-INFO
+Filename: lightspark-2.7.0/PKG-INFO
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/requests/
+Filename: lightspark-2.7.0/lightspark/objects/
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/utils/
+Filename: lightspark-2.7.0/lightspark/utils/
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/
+Filename: lightspark-2.7.0/lightspark/scripts/
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/scripts/
+Filename: lightspark-2.7.0/lightspark/requests/
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/py.typed
+Filename: lightspark-2.7.0/lightspark/py.typed
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/webhooks.py
+Filename: lightspark-2.7.0/lightspark/version.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/version.py
+Filename: lightspark-2.7.0/lightspark/lightspark_client.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/remote_signing.py
+Filename: lightspark-2.7.0/lightspark/__init__.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/lightspark_client.py
+Filename: lightspark-2.7.0/lightspark/exceptions.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/__init__.py
+Filename: lightspark-2.7.0/lightspark/webhooks.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/exceptions.py
+Filename: lightspark-2.7.0/lightspark/remote_signing.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/requests/encoder.py
+Filename: lightspark-2.7.0/lightspark/objects/CancelInvoiceOutput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/requests/__init__.py
+Filename: lightspark-2.7.0/lightspark/objects/ChannelClosingTransaction.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/requests/requester.py
+Filename: lightspark-2.7.0/lightspark/objects/InvoiceData.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/utils/signing_key.py
+Filename: lightspark-2.7.0/lightspark/objects/WithdrawalRequestToChannelOpeningTransactionsConnection.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/utils/crypto.py
+Filename: lightspark-2.7.0/lightspark/objects/TransactionStatus.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/utils/enums.py
+Filename: lightspark-2.7.0/lightspark/objects/OutgoingPayment.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/utils/currency_amount.py
+Filename: lightspark-2.7.0/lightspark/objects/CreateApiTokenInput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/utils/__init__.py
+Filename: lightspark-2.7.0/lightspark/objects/CancelInvoiceInput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/ReleasePaymentPreimageOutput.py
+Filename: lightspark-2.7.0/lightspark/objects/InvoiceType.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/BlockchainBalance.py
+Filename: lightspark-2.7.0/lightspark/objects/WalletToWithdrawalRequestsConnection.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/LightsparkNode.py
+Filename: lightspark-2.7.0/lightspark/objects/ReleaseChannelPerCommitmentSecretOutput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/CreateTestModeInvoiceInput.py
+Filename: lightspark-2.7.0/lightspark/objects/LightsparkNodeToChannelsConnection.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/NodeToAddressesConnection.py
+Filename: lightspark-2.7.0/lightspark/objects/OutgoingPaymentAttemptStatus.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/CurrencyUnit.py
+Filename: lightspark-2.7.0/lightspark/objects/RemoteSigningSubEventType.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/RequestWithdrawalOutput.py
+Filename: lightspark-2.7.0/lightspark/objects/RequestWithdrawalInput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/HtlcAttemptFailureCode.py
+Filename: lightspark-2.7.0/lightspark/objects/SignInvoiceOutput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/Transaction.py
+Filename: lightspark-2.7.0/lightspark/objects/Permission.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/UpdateNodeSharedSecretInput.py
+Filename: lightspark-2.7.0/lightspark/objects/CreateTestModePaymentInput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/SendPaymentInput.py
+Filename: lightspark-2.7.0/lightspark/objects/ClaimUmaInvitationWithIncentivesOutput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/IncomingPaymentsForInvoiceQueryOutput.py
+Filename: lightspark-2.7.0/lightspark/objects/FailHtlcsOutput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/OutgoingPaymentAttempt.py
+Filename: lightspark-2.7.0/lightspark/objects/SendPaymentInput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/ChannelStatus.py
+Filename: lightspark-2.7.0/lightspark/objects/DeclineToSignMessagesInput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/LightningTransaction.py
+Filename: lightspark-2.7.0/lightspark/objects/CreateInvoiceOutput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/CreateUmaInvitationOutput.py
+Filename: lightspark-2.7.0/lightspark/objects/Withdrawal.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/WithdrawalFeeEstimateOutput.py
+Filename: lightspark-2.7.0/lightspark/objects/DeclineToSignMessagesOutput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/Balances.py
+Filename: lightspark-2.7.0/lightspark/objects/RegisterPaymentInput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/SignablePayload.py
+Filename: lightspark-2.7.0/lightspark/objects/CurrencyAmount.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/AccountToTransactionsConnection.py
+Filename: lightspark-2.7.0/lightspark/objects/Transaction.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/Channel.py
+Filename: lightspark-2.7.0/lightspark/objects/IdAndSignature.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/Account.py
+Filename: lightspark-2.7.0/lightspark/objects/ReleaseChannelPerCommitmentSecretInput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/Connection.py
+Filename: lightspark-2.7.0/lightspark/objects/IncomingPaymentToAttemptsConnection.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/CreateInvoiceInput.py
+Filename: lightspark-2.7.0/lightspark/objects/WalletStatus.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/PaymentDirection.py
+Filename: lightspark-2.7.0/lightspark/objects/Connection.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/CreateInvoiceOutput.py
+Filename: lightspark-2.7.0/lightspark/objects/ScreenNodeOutput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/IncomingPaymentAttemptStatus.py
+Filename: lightspark-2.7.0/lightspark/objects/WithdrawalMode.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/CreateTestModePaymentoutput.py
+Filename: lightspark-2.7.0/lightspark/objects/CreateUmaInvitationInput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/CreateInvitationWithIncentivesOutput.py
+Filename: lightspark-2.7.0/lightspark/objects/CreateInvitationWithIncentivesOutput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/CreateUmaInvoiceInput.py
+Filename: lightspark-2.7.0/lightspark/objects/Node.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/OnChainTransaction.py
+Filename: lightspark-2.7.0/lightspark/objects/BlockchainBalance.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/InvoiceData.py
+Filename: lightspark-2.7.0/lightspark/objects/IncomingPaymentAttempt.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/WalletToPaymentRequestsConnection.py
+Filename: lightspark-2.7.0/lightspark/objects/PayInvoiceInput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/SignablePayloadStatus.py
+Filename: lightspark-2.7.0/lightspark/objects/OutgoingPaymentAttemptToHopsConnection.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/UpdateChannelPerCommitmentPointInput.py
+Filename: lightspark-2.7.0/lightspark/objects/RoutingTransactionFailureReason.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/IncomingPaymentsForInvoiceQueryInput.py
+Filename: lightspark-2.7.0/lightspark/objects/UpdateChannelPerCommitmentPointInput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/ReleaseChannelPerCommitmentSecretInput.py
+Filename: lightspark-2.7.0/lightspark/objects/SignablePayloadStatus.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/ChannelClosingTransaction.py
+Filename: lightspark-2.7.0/lightspark/objects/CreateInvoiceInput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/DeleteApiTokenInput.py
+Filename: lightspark-2.7.0/lightspark/objects/Wallet.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/CurrencyAmount.py
+Filename: lightspark-2.7.0/lightspark/objects/WithdrawalRequestToChannelClosingTransactionsConnection.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/CreateTestModeInvoiceOutput.py
+Filename: lightspark-2.7.0/lightspark/objects/RichText.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/FundNodeInput.py
+Filename: lightspark-2.7.0/lightspark/objects/CreateTestModeInvoiceInput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/ScreenNodeInput.py
+Filename: lightspark-2.7.0/lightspark/objects/WithdrawalRequest.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/InvoiceType.py
+Filename: lightspark-2.7.0/lightspark/objects/OutgoingPaymentsForInvoiceQueryInput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/AccountToWithdrawalRequestsConnection.py
+Filename: lightspark-2.7.0/lightspark/objects/WebhookEventType.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/SignInvoiceInput.py
+Filename: lightspark-2.7.0/lightspark/objects/PostTransactionData.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/ChannelSnapshot.py
+Filename: lightspark-2.7.0/lightspark/objects/AccountToPaymentRequestsConnection.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/RiskRating.py
+Filename: lightspark-2.7.0/lightspark/objects/SignMessagesInput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/CancelInvoiceInput.py
+Filename: lightspark-2.7.0/lightspark/objects/AccountToChannelsConnection.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/UpdateChannelPerCommitmentPointOutput.py
+Filename: lightspark-2.7.0/lightspark/objects/SignMessagesOutput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/BitcoinNetwork.py
+Filename: lightspark-2.7.0/lightspark/objects/Signable.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/RegionCode.py
+Filename: lightspark-2.7.0/lightspark/objects/LightningPaymentDirection.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/OutgoingPaymentAttemptStatus.py
+Filename: lightspark-2.7.0/lightspark/objects/FundNodeOutput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/WalletToWithdrawalRequestsConnection.py
+Filename: lightspark-2.7.0/lightspark/objects/FeeEstimate.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/LightsparkNodeToDailyLiquidityForecastsConnection.py
+Filename: lightspark-2.7.0/lightspark/objects/GraphNode.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/SetInvoicePaymentHashInput.py
+Filename: lightspark-2.7.0/lightspark/objects/IncomingPayment.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/ClaimUmaInvitationOutput.py
+Filename: lightspark-2.7.0/lightspark/objects/AccountToNodesConnection.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/Permission.py
+Filename: lightspark-2.7.0/lightspark/objects/LightsparkNodeStatus.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/SignInvoiceOutput.py
+Filename: lightspark-2.7.0/lightspark/objects/MultiSigAddressValidationParameters.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/RequestWithdrawalInput.py
+Filename: lightspark-2.7.0/lightspark/objects/PaymentDirection.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/Entity.py
+Filename: lightspark-2.7.0/lightspark/objects/UpdateNodeSharedSecretOutput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/OutgoingPaymentToAttemptsConnection.py
+Filename: lightspark-2.7.0/lightspark/objects/LightningFeeEstimateForInvoiceInput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/Invoice.py
+Filename: lightspark-2.7.0/lightspark/objects/Entity.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/IdAndSignature.py
+Filename: lightspark-2.7.0/lightspark/objects/RequestWithdrawalOutput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/RoutingTransactionFailureReason.py
+Filename: lightspark-2.7.0/lightspark/objects/ReleasePaymentPreimageInput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/ChannelOpeningTransaction.py
+Filename: lightspark-2.7.0/lightspark/objects/LightsparkNodeToDailyLiquidityForecastsConnection.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/PaymentRequestData.py
+Filename: lightspark-2.7.0/lightspark/objects/BitcoinNetwork.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/WalletStatus.py
+Filename: lightspark-2.7.0/lightspark/objects/DailyLiquidityForecast.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/LightningPaymentDirection.py
+Filename: lightspark-2.7.0/lightspark/objects/ApiToken.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/WithdrawalRequestToChannelOpeningTransactionsConnection.py
+Filename: lightspark-2.7.0/lightspark/objects/UmaInvitation.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/ComplianceProvider.py
+Filename: lightspark-2.7.0/lightspark/objects/Account.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/UpdateNodeSharedSecretOutput.py
+Filename: lightspark-2.7.0/lightspark/objects/CreateNodeWalletAddressOutput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/ClaimUmaInvitationWithIncentivesOutput.py
+Filename: lightspark-2.7.0/lightspark/objects/DeleteApiTokenOutput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/WithdrawalRequestStatus.py
+Filename: lightspark-2.7.0/lightspark/objects/RoutingTransaction.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/WebhookEventType.py
+Filename: lightspark-2.7.0/lightspark/objects/AccountToTransactionsConnection.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/UmaInvitation.py
+Filename: lightspark-2.7.0/lightspark/objects/LightsparkNodeOwner.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/SetInvoicePaymentHashOutput.py
+Filename: lightspark-2.7.0/lightspark/objects/CreateTestModePaymentoutput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/PayUmaInvoiceInput.py
+Filename: lightspark-2.7.0/lightspark/objects/ChannelStatus.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/WithdrawalFeeEstimateInput.py
+Filename: lightspark-2.7.0/lightspark/objects/ClaimUmaInvitationWithIncentivesInput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/PaymentFailureReason.py
+Filename: lightspark-2.7.0/lightspark/objects/WithdrawalRequestStatus.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/AuditLogActor.py
+Filename: lightspark-2.7.0/lightspark/objects/Deposit.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/CreateTestModePaymentInput.py
+Filename: lightspark-2.7.0/lightspark/objects/IncomingPaymentsForInvoiceQueryInput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/LightsparkNodeStatus.py
+Filename: lightspark-2.7.0/lightspark/objects/HtlcAttemptFailureCode.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/ClaimUmaInvitationWithIncentivesInput.py
+Filename: lightspark-2.7.0/lightspark/objects/all_entities.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/CreateUmaInvitationInput.py
+Filename: lightspark-2.7.0/lightspark/objects/__init__.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/ScreenNodeOutput.py
+Filename: lightspark-2.7.0/lightspark/objects/Invoice.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/LightningFeeEstimateOutput.py
+Filename: lightspark-2.7.0/lightspark/objects/PaymentRequestStatus.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/AccountToPaymentRequestsConnection.py
+Filename: lightspark-2.7.0/lightspark/objects/SetInvoicePaymentHashInput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/all_entities.py
+Filename: lightspark-2.7.0/lightspark/objects/RegionCode.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/FundNodeOutput.py
+Filename: lightspark-2.7.0/lightspark/objects/PaymentFailureReason.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/LightsparkNodeOwner.py
+Filename: lightspark-2.7.0/lightspark/objects/SignInvoiceInput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/AccountToNodesConnection.py
+Filename: lightspark-2.7.0/lightspark/objects/CreateLnurlInvoiceInput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/TransactionType.py
+Filename: lightspark-2.7.0/lightspark/objects/TransactionType.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/LightsparkNodeWithRemoteSigning.py
+Filename: lightspark-2.7.0/lightspark/objects/NodeAddress.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/PageInfo.py
+Filename: lightspark-2.7.0/lightspark/objects/ChannelFees.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/IncomingPaymentAttempt.py
+Filename: lightspark-2.7.0/lightspark/objects/ChannelToTransactionsConnection.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/ChannelFees.py
+Filename: lightspark-2.7.0/lightspark/objects/SignablePayload.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/OutgoingPaymentsForInvoiceQueryOutput.py
+Filename: lightspark-2.7.0/lightspark/objects/UpdateChannelPerCommitmentPointOutput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/DeclineToSignMessagesInput.py
+Filename: lightspark-2.7.0/lightspark/objects/FailHtlcsInput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/ChannelToTransactionsConnection.py
+Filename: lightspark-2.7.0/lightspark/objects/AccountToWithdrawalRequestsConnection.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/LightsparkNodeToChannelsConnection.py
+Filename: lightspark-2.7.0/lightspark/objects/ClaimUmaInvitationInput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/CreateLnurlInvoiceInput.py
+Filename: lightspark-2.7.0/lightspark/objects/Hop.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/RichText.py
+Filename: lightspark-2.7.0/lightspark/objects/ClaimUmaInvitationOutput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/Withdrawal.py
+Filename: lightspark-2.7.0/lightspark/objects/SendPaymentOutput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/IncomingPayment.py
+Filename: lightspark-2.7.0/lightspark/objects/OutgoingPaymentAttempt.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/NodeAddressType.py
+Filename: lightspark-2.7.0/lightspark/objects/UpdateNodeSharedSecretInput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/CreateApiTokenInput.py
+Filename: lightspark-2.7.0/lightspark/objects/OutgoingPaymentToAttemptsConnection.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/WalletToTransactionsConnection.py
+Filename: lightspark-2.7.0/lightspark/objects/IncentivesStatus.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/Wallet.py
+Filename: lightspark-2.7.0/lightspark/objects/PaymentRequest.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/ClaimUmaInvitationInput.py
+Filename: lightspark-2.7.0/lightspark/objects/PaymentRequestData.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/WithdrawalMode.py
+Filename: lightspark-2.7.0/lightspark/objects/CreateInvitationWithIncentivesInput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/AccountToChannelsConnection.py
+Filename: lightspark-2.7.0/lightspark/objects/CreateUmaInvoiceInput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/ApiToken.py
+Filename: lightspark-2.7.0/lightspark/objects/CurrencyUnit.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/OutgoingPaymentsForInvoiceQueryInput.py
+Filename: lightspark-2.7.0/lightspark/objects/Balances.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/LightningFeeEstimateForNodeInput.py
+Filename: lightspark-2.7.0/lightspark/objects/WalletToPaymentRequestsConnection.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/WithdrawalRequestToChannelClosingTransactionsConnection.py
+Filename: lightspark-2.7.0/lightspark/objects/Secret.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/MultiSigAddressValidationParameters.py
+Filename: lightspark-2.7.0/lightspark/objects/PayUmaInvoiceInput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/Node.py
+Filename: lightspark-2.7.0/lightspark/objects/ChannelSnapshot.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/IncentivesStatus.py
+Filename: lightspark-2.7.0/lightspark/objects/AccountToApiTokensConnection.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/RoutingTransaction.py
+Filename: lightspark-2.7.0/lightspark/objects/NodeToAddressesConnection.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/ReleaseChannelPerCommitmentSecretOutput.py
+Filename: lightspark-2.7.0/lightspark/objects/NodeAddressType.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/Signable.py
+Filename: lightspark-2.7.0/lightspark/objects/CreateTestModeInvoiceOutput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/Secret.py
+Filename: lightspark-2.7.0/lightspark/objects/LightningFeeEstimateOutput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/SignMessagesInput.py
+Filename: lightspark-2.7.0/lightspark/objects/ReleasePaymentPreimageOutput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/WithdrawalRequest.py
+Filename: lightspark-2.7.0/lightspark/objects/SetInvoicePaymentHashOutput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/RegisterPaymentInput.py
+Filename: lightspark-2.7.0/lightspark/objects/AuditLogActor.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/Hop.py
+Filename: lightspark-2.7.0/lightspark/objects/AccountToWalletsConnection.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/SendPaymentOutput.py
+Filename: lightspark-2.7.0/lightspark/objects/LightningFeeEstimateForNodeInput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/DeclineToSignMessagesOutput.py
+Filename: lightspark-2.7.0/lightspark/objects/IncentivesIneligibilityReason.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/CreateNodeWalletAddressOutput.py
+Filename: lightspark-2.7.0/lightspark/objects/DeleteApiTokenInput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/GraphNode.py
+Filename: lightspark-2.7.0/lightspark/objects/LightsparkNode.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/CreateApiTokenOutput.py
+Filename: lightspark-2.7.0/lightspark/objects/RiskRating.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/ReleasePaymentPreimageInput.py
+Filename: lightspark-2.7.0/lightspark/objects/WithdrawalFeeEstimateOutput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/TransactionStatus.py
+Filename: lightspark-2.7.0/lightspark/objects/LightsparkNodeWithRemoteSigning.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/IncomingPaymentToAttemptsConnection.py
+Filename: lightspark-2.7.0/lightspark/objects/ChannelOpeningTransaction.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/RemoteSigningSubEventType.py
+Filename: lightspark-2.7.0/lightspark/objects/WithdrawalFeeEstimateInput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/PaymentRequest.py
+Filename: lightspark-2.7.0/lightspark/objects/OutgoingPaymentsForInvoiceQueryOutput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/__init__.py
+Filename: lightspark-2.7.0/lightspark/objects/ScreenNodeInput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/CreateInvitationWithIncentivesInput.py
+Filename: lightspark-2.7.0/lightspark/objects/IncomingPaymentsForInvoiceQueryOutput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/PayInvoiceOutput.py
+Filename: lightspark-2.7.0/lightspark/objects/WithdrawalRequestToWithdrawalsConnection.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/PayInvoiceInput.py
+Filename: lightspark-2.7.0/lightspark/objects/CreateNodeWalletAddressInput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/CreateNodeWalletAddressInput.py
+Filename: lightspark-2.7.0/lightspark/objects/LightsparkNodeWithOSK.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/OutgoingPayment.py
+Filename: lightspark-2.7.0/lightspark/objects/Channel.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/AccountToApiTokensConnection.py
+Filename: lightspark-2.7.0/lightspark/objects/FundNodeInput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/IncentivesIneligibilityReason.py
+Filename: lightspark-2.7.0/lightspark/objects/TransactionFailures.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/DailyLiquidityForecast.py
+Filename: lightspark-2.7.0/lightspark/objects/CreateApiTokenOutput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/FeeEstimate.py
+Filename: lightspark-2.7.0/lightspark/objects/ComplianceProvider.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/SignMessagesOutput.py
+Filename: lightspark-2.7.0/lightspark/objects/PageInfo.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/PaymentRequestStatus.py
+Filename: lightspark-2.7.0/lightspark/objects/CreateUmaInvitationOutput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/RegisterPaymentOutput.py
+Filename: lightspark-2.7.0/lightspark/objects/OnChainTransaction.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/TransactionFailures.py
+Filename: lightspark-2.7.0/lightspark/objects/RegisterPaymentOutput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/AccountToWalletsConnection.py
+Filename: lightspark-2.7.0/lightspark/objects/WalletToTransactionsConnection.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/LightningFeeEstimateForInvoiceInput.py
+Filename: lightspark-2.7.0/lightspark/objects/LightningTransaction.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/NodeAddress.py
+Filename: lightspark-2.7.0/lightspark/objects/IncomingPaymentAttemptStatus.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/Deposit.py
+Filename: lightspark-2.7.0/lightspark/objects/PayInvoiceOutput.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/OutgoingPaymentAttemptToHopsConnection.py
+Filename: lightspark-2.7.0/lightspark/utils/currency_amount.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/DeleteApiTokenOutput.py
+Filename: lightspark-2.7.0/lightspark/utils/crypto.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/PostTransactionData.py
+Filename: lightspark-2.7.0/lightspark/utils/signing_key.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/LightsparkNodeWithOSK.py
+Filename: lightspark-2.7.0/lightspark/utils/__init__.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/objects/CancelInvoiceOutput.py
+Filename: lightspark-2.7.0/lightspark/utils/enums.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/scripts/claim_uma_invitation.py
+Filename: lightspark-2.7.0/lightspark/scripts/create_test_mode_invoice.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/scripts/decoded_payment_request.py
+Filename: lightspark-2.7.0/lightspark/scripts/request_withdrawal.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/scripts/create_uma_invoice.py
+Filename: lightspark-2.7.0/lightspark/scripts/create_test_mode_payment.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/scripts/send_payment.py
+Filename: lightspark-2.7.0/lightspark/scripts/outgoing_payments_for_payment_hash.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/scripts/request_withdrawal.py
+Filename: lightspark-2.7.0/lightspark/scripts/lightning_fee_estimate_for_node.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/scripts/outgoing_payments_for_invoice.py
+Filename: lightspark-2.7.0/lightspark/scripts/recover_node_signing_key.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/scripts/screen_node.py
+Filename: lightspark-2.7.0/lightspark/scripts/delete_api_token.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/scripts/lightning_fee_estimate_for_invoice.py
+Filename: lightspark-2.7.0/lightspark/scripts/bitcoin_fee_estimate.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/scripts/register_payment.py
+Filename: lightspark-2.7.0/lightspark/scripts/fetch_uma_invitation.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/scripts/delete_api_token.py
+Filename: lightspark-2.7.0/lightspark/scripts/create_lnurl_invoice.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/scripts/create_lnurl_invoice.py
+Filename: lightspark-2.7.0/lightspark/scripts/create_node_address.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/scripts/current_account.py
+Filename: lightspark-2.7.0/lightspark/scripts/screen_node.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/scripts/create_api_token.py
+Filename: lightspark-2.7.0/lightspark/scripts/register_payment.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/scripts/fund_node.py
+Filename: lightspark-2.7.0/lightspark/scripts/lightning_fee_estimate_for_invoice.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/scripts/incoming_payments_for_invoice.py
+Filename: lightspark-2.7.0/lightspark/scripts/incoming_payments_for_invoice.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/scripts/create_uma_invitation.py
+Filename: lightspark-2.7.0/lightspark/scripts/fund_node.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/scripts/create_test_mode_payment.py
+Filename: lightspark-2.7.0/lightspark/scripts/__init__.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/scripts/create_invoice.py
+Filename: lightspark-2.7.0/lightspark/scripts/outgoing_payments_for_invoice.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/scripts/cancel_invoice.py
+Filename: lightspark-2.7.0/lightspark/scripts/pay_uma_invoice.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/scripts/pay_uma_invoice.py
+Filename: lightspark-2.7.0/lightspark/scripts/decoded_payment_request.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/scripts/pay_invoice.py
+Filename: lightspark-2.7.0/lightspark/scripts/claim_uma_invitation.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/scripts/__init__.py
+Filename: lightspark-2.7.0/lightspark/scripts/cancel_invoice.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/scripts/lightning_fee_estimate_for_node.py
+Filename: lightspark-2.7.0/lightspark/scripts/current_account.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/scripts/create_node_address.py
+Filename: lightspark-2.7.0/lightspark/scripts/fail_htlcs.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/scripts/recover_node_signing_key.py
+Filename: lightspark-2.7.0/lightspark/scripts/create_uma_invitation.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/scripts/bitcoin_fee_estimate.py
+Filename: lightspark-2.7.0/lightspark/scripts/send_payment.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/scripts/create_test_mode_invoice.py
+Filename: lightspark-2.7.0/lightspark/scripts/pay_invoice.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark/scripts/fetch_uma_invitation.py
+Filename: lightspark-2.7.0/lightspark/scripts/create_api_token.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark.egg-info/dependency_links.txt
+Filename: lightspark-2.7.0/lightspark/scripts/create_uma_invoice.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark.egg-info/SOURCES.txt
+Filename: lightspark-2.7.0/lightspark/scripts/create_invoice.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark.egg-info/top_level.txt
+Filename: lightspark-2.7.0/lightspark/requests/encoder.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark.egg-info/PKG-INFO
+Filename: lightspark-2.7.0/lightspark/requests/requester.py
 Comment: 
 
-Filename: lightspark-2.6.0/lightspark.egg-info/requires.txt
+Filename: lightspark-2.7.0/lightspark/requests/__init__.py
+Comment: 
+
+Filename: lightspark-2.7.0/lightspark.egg-info/dependency_links.txt
+Comment: 
+
+Filename: lightspark-2.7.0/lightspark.egg-info/SOURCES.txt
+Comment: 
+
+Filename: lightspark-2.7.0/lightspark.egg-info/top_level.txt
+Comment: 
+
+Filename: lightspark-2.7.0/lightspark.egg-info/PKG-INFO
+Comment: 
+
+Filename: lightspark-2.7.0/lightspark.egg-info/requires.txt
 Comment: 
 
 Zip file comment:
```

## Comparing `lightspark-2.6.0/LICENSE` & `lightspark-2.7.0/LICENSE`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/README.md` & `lightspark-2.7.0/README.md`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/setup.cfg` & `lightspark-2.7.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 packages = find:
 include_package_data = True
 install_requires = 
 	cryptography
 	pyjwt
 	requests
 	lightspark-crypto-python
+	zstandard
 
 [options.packages.find]
 include = 
 	lightspark*
 
 [egg_info]
 tag_build =
```

## Comparing `lightspark-2.6.0/PKG-INFO` & `lightspark-2.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: lightspark
-Version: 2.6.0
+Version: 2.7.0
 Summary: Python SDK for the Lightspark API
 Home-page: https://www.lightspark.com/
 Author: Lightspark Group, Inc.
 Author-email: info@lightspark.com
 License: Apache-2.0
 Project-URL: Documentation, https://docs.lightspark.com/lightspark-sdk/getting-started?language=Python
 Project-URL: Source Code, https://github.com/lightsparkdev/python-sdk
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cryptography
 Requires-Dist: pyjwt
 Requires-Dist: requests
 Requires-Dist: lightspark-crypto-python
+Requires-Dist: zstandard
 
 # Lightspark Python SDK
 
 The Lightspark Python SDK provides a convenient way to interact with the Lightspark services from applications written in the Python language.
 
 ## Installation
```

## Comparing `lightspark-2.6.0/lightspark/webhooks.py` & `lightspark-2.7.0/lightspark/webhooks.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/remote_signing.py` & `lightspark-2.7.0/lightspark/remote_signing.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/lightspark_client.py` & `lightspark-2.7.0/lightspark/lightspark_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,28 +80,32 @@
     CREATE_UMA_INVITATION_MUTATION,
     CREATE_UMA_INVITATION_WITH_INCENTIVES_MUTATION,
 )
 from lightspark.scripts.create_uma_invoice import CREATE_UMA_INVOICE_MUTATION
 from lightspark.scripts.current_account import CURRENT_ACCOUNT_QUERY
 from lightspark.scripts.decoded_payment_request import DECODED_PAYMENT_REQUEST_QUERY
 from lightspark.scripts.delete_api_token import DELETE_API_TOKEN_MUTATION
+from lightspark.scripts.fail_htlcs import FAIL_HTLCS_MUTATION
 from lightspark.scripts.fetch_uma_invitation import FETCH_UMA_INVITATION_QUERY
 from lightspark.scripts.fund_node import FUND_NODE_MUTATION
 from lightspark.scripts.incoming_payments_for_invoice import (
     INCOMING_PAYMENTS_FOR_INVOICE_QUERY,
 )
 from lightspark.scripts.lightning_fee_estimate_for_invoice import (
     LIGHTNING_FEE_ESTIMATE_FOR_INVOICE_QUERY,
 )
 from lightspark.scripts.lightning_fee_estimate_for_node import (
     LIGHTNING_FEE_ESTIMATE_FOR_NODE_QUERY,
 )
 from lightspark.scripts.outgoing_payments_for_invoice import (
     OUTGOING_PAYMENTS_FOR_INVOICE_QUERY,
 )
+from lightspark.scripts.outgoing_payments_for_payment_hash import (
+    OUTGOING_PAYMENTS_FOR_PAYMENT_HASH_QUERY,
+)
 from lightspark.scripts.pay_invoice import PAY_INVOICE_MUTATION
 from lightspark.scripts.pay_uma_invoice import PAY_UMA_INVOICE_MUTATION
 from lightspark.scripts.recover_node_signing_key import RECOVER_NODE_SIGNING_KEY_QUERY
 from lightspark.scripts.register_payment import REGISTER_PAYMENT_MUTATION
 from lightspark.scripts.request_withdrawal import REQUEST_WITHDRAWAL_MUTATION
 from lightspark.scripts.screen_node import SCREEN_NODE_MUTATION
 from lightspark.scripts.send_payment import SEND_PAYMENT_MUTATION
@@ -280,15 +284,14 @@
         }
         if amount_msats is not None:
             variables["amount_msats"] = amount_msats
 
         json = self._requester.execute_graphql(
             CREATE_TEST_MODE_PAYMENT_MUTATION,
             variables,
-            self.get_signing_key(local_node_id),
         )
         return IncomingPayment_from_json(
             self._requester, json["create_test_mode_payment"]["incoming_payment"]
         )
 
     def create_uma_invoice(
         self,
@@ -688,14 +691,42 @@
         if "payments" not in json["outgoing_payments_for_invoice"]:
             return []
         return [
             OutgoingPayment_from_json(self._requester, payment)
             for payment in json["outgoing_payments_for_invoice"]["payments"]
         ]
 
+    def outgoing_payments_for_payment_hash(
+        self,
+        payment_hash: str,
+        transaction_statuses: Optional[List[TransactionStatus]] = None,
+    ) -> List[OutgoingPayment]:
+        """
+        Fetches the outgoing payments (if any) which have been made for a given payment hash.
+
+        Args:
+            payment_hash: The payment hash for which to fetch the outgoing payments.
+            transaction_statuses: The statuses of the transactions to fetch. If not specified, all transactions will be fetched.
+        """
+
+        variables: Dict[str, Any] = {"payment_hash": payment_hash}
+        if transaction_statuses is not None:
+            variables["transaction_statuses"] = transaction_statuses
+        json = self._requester.execute_graphql(
+            OUTGOING_PAYMENTS_FOR_PAYMENT_HASH_QUERY, variables
+        )
+        if "outgoing_payments_for_payment_hash" not in json:
+            return []
+        if "payments" not in json["outgoing_payments_for_payment_hash"]:
+            return []
+        return [
+            OutgoingPayment_from_json(self._requester, payment)
+            for payment in json["outgoing_payments_for_payment_hash"]["payments"]
+        ]
+
     def incoming_payments_for_invoice(
         self,
         invoice_id: str,
         transaction_statuses: Optional[List[TransactionStatus]] = None,
     ) -> List[IncomingPayment]:
         """
         Fetches the incoming payments (if any) which have been made for a given invoice.
@@ -845,10 +876,25 @@
         match = E614_REGEX.search(phone_number_e164_format)
         if not match:
             raise LightsparkException(
                 "InvalidPhoneNumber", "The phone number must follow the E.164 format."
             )
         return sha256(phone_number_e164_format.encode()).hexdigest()
 
+    def fail_htlcs(self, invoice_id: str, cancel_invoice: bool = True) -> str:
+        """
+        Fails all pending HTLCs associated with an invoice.
+
+        Args:
+            invoice_id: The ID of the invoice to fail.
+            cancel_invoice: Whether to cancel the invoice after failing the HTLCs.
+        """
+        json = self._requester.execute_graphql(
+            FAIL_HTLCS_MUTATION,
+            {"invoice_id": invoice_id, "cancel_invoice": cancel_invoice},
+        )
+
+        return json["fail_htlcs"]["invoice"]["id"]
+
 
 # pylint: disable=anomalous-backslash-in-string
 E614_REGEX = re.compile("^\+?[1-9]\d{1,14}$")
```

## Comparing `lightspark-2.6.0/lightspark/__init__.py` & `lightspark-2.7.0/lightspark/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,16 @@
 from lightspark.objects.DailyLiquidityForecast import DailyLiquidityForecast
 from lightspark.objects.DeclineToSignMessagesInput import DeclineToSignMessagesInput
 from lightspark.objects.DeclineToSignMessagesOutput import DeclineToSignMessagesOutput
 from lightspark.objects.DeleteApiTokenInput import DeleteApiTokenInput
 from lightspark.objects.DeleteApiTokenOutput import DeleteApiTokenOutput
 from lightspark.objects.Deposit import Deposit
 from lightspark.objects.Entity import Entity
+from lightspark.objects.FailHtlcsInput import FailHtlcsInput
+from lightspark.objects.FailHtlcsOutput import FailHtlcsOutput
 from lightspark.objects.FeeEstimate import FeeEstimate
 from lightspark.objects.FundNodeInput import FundNodeInput
 from lightspark.objects.FundNodeOutput import FundNodeOutput
 from lightspark.objects.GraphNode import GraphNode
 from lightspark.objects.Hop import Hop
 from lightspark.objects.HtlcAttemptFailureCode import HtlcAttemptFailureCode
 from lightspark.objects.IdAndSignature import IdAndSignature
@@ -222,10 +224,13 @@
 from lightspark.objects.WithdrawalRequestStatus import WithdrawalRequestStatus
 from lightspark.objects.WithdrawalRequestToChannelClosingTransactionsConnection import (
     WithdrawalRequestToChannelClosingTransactionsConnection,
 )
 from lightspark.objects.WithdrawalRequestToChannelOpeningTransactionsConnection import (
     WithdrawalRequestToChannelOpeningTransactionsConnection,
 )
+from lightspark.objects.WithdrawalRequestToWithdrawalsConnection import (
+    WithdrawalRequestToWithdrawalsConnection,
+)
 from lightspark.remote_signing import *
 from lightspark.version import __version__
 from lightspark.webhooks import SIGNATURE_HEADER, WebhookEvent
```

## Comparing `lightspark-2.6.0/lightspark/requests/requester.py` & `lightspark-2.7.0/lightspark/requests/requester.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 # Copyright ©, 2022-present, Lightspark Group, Inc. - All Rights Reserved
 
 import json
 import logging
 import re
 import secrets
+import zlib
 from datetime import datetime, timedelta, timezone
 from platform import python_version, release, system
 from typing import Any, Mapping, Optional
 from urllib.parse import urlparse
 
+try:
+    from zstandard import ZstdCompressor
+
+    zstd: Optional[ZstdCompressor] = ZstdCompressor()
+except ImportError:
+    zstd = None
+
 import requests
 from requests.auth import HTTPBasicAuth
 from requests.utils import default_user_agent
 
 from lightspark.exceptions import LightsparkException
 from lightspark.requests.encoder import Encoder
 from lightspark.utils.signing_key import SigningKey
@@ -65,24 +73,34 @@
 
         signing = signing_key.sign_payload(payload) if signing_key else None
 
         user_agent = self.user_agent_string()
         logger.debug(
             "Sending request to GraphQL with query = %s, payload = %s}", query, payload
         )
+
+        headers = {
+            "Content-Type": "application/json",
+            "X-GraphQL-Operation": operation.group(1) if operation else None,
+            "X-Lightspark-Signing": signing,
+            "User-Agent": user_agent + f" {default_user_agent()}",
+            "X-Lightspark-SDK": user_agent,
+        }
+        if len(payload) > 1024:
+            if zstd:
+                payload = zstd.compress(payload)
+                headers["Content-Encoding"] = "zstd"
+            else:
+                payload = zlib.compress(payload, level=zlib.Z_BEST_SPEED)
+                headers["Content-Encoding"] = "deflate"
+
         r = self.graphql_session.post(
             url=self.base_url,
             data=payload,
-            headers={
-                "Content-Type": "application/json",
-                "X-GraphQL-Operation": operation.group(1) if operation else None,
-                "X-Lightspark-Signing": signing,
-                "User-Agent": user_agent + f" {default_user_agent()}",
-                "X-Lightspark-SDK": user_agent,
-            },
+            headers=headers,
         )
         try:
             r.raise_for_status()
             result = r.json()
             if "errors" in result:
                 errors = result["errors"]
                 raise LightsparkException(
```

## Comparing `lightspark-2.6.0/lightspark/utils/signing_key.py` & `lightspark-2.7.0/lightspark/utils/signing_key.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/utils/crypto.py` & `lightspark-2.7.0/lightspark/utils/crypto.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from base64 import b64decode, b64encode
 from hashlib import pbkdf2_hmac
 from secrets import token_bytes
 from typing import Tuple
 
 from cryptography.hazmat.primitives import hashes, padding, serialization
 from cryptography.hazmat.primitives.asymmetric import padding as asymmetric_padding
+from cryptography.hazmat.primitives.asymmetric.rsa import RSAPrivateKey
 from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
 from cryptography.hazmat.primitives.ciphers.aead import AESGCM
 from lightspark.exceptions import LightsparkException
 
 IV_LEN = 12
 KEY_LEN = 32
 SALT_LEN = 16
@@ -94,14 +95,16 @@
     return plaintext
 
 
 def sign_payload(payload: bytes, signing_key: bytes) -> str:
     if signing_key[0] != 48:
         signing_key = b64decode(signing_key)
     key = serialization.load_der_private_key(signing_key, password=None)
+    if not isinstance(key, RSAPrivateKey):
+        raise ValueError("Unsupported signing key type")
 
     signature = key.sign(
         payload,
         asymmetric_padding.PSS(
             mgf=asymmetric_padding.MGF1(hashes.SHA256()),
             salt_length=asymmetric_padding.PSS.DIGEST_LENGTH,
         ),
```

## Comparing `lightspark-2.6.0/lightspark/utils/enums.py` & `lightspark-2.7.0/lightspark/utils/enums.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/utils/currency_amount.py` & `lightspark-2.7.0/lightspark/utils/currency_amount.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/ReleasePaymentPreimageOutput.py` & `lightspark-2.7.0/lightspark/objects/ReleasePaymentPreimageOutput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/BlockchainBalance.py` & `lightspark-2.7.0/lightspark/objects/BlockchainBalance.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/LightsparkNode.py` & `lightspark-2.7.0/lightspark/objects/LightsparkNode.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 # Copyright ©, 2022-present, Lightspark Group, Inc. - All Rights Reserved
 
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Any, List, Mapping, Optional
 
 from lightspark.exceptions import LightsparkException
-from lightspark.objects.BitcoinNetwork import BitcoinNetwork
-from lightspark.objects.LightsparkNodeStatus import LightsparkNodeStatus
 from lightspark.requests.requester import Requester
 from lightspark.utils.enums import parse_enum, parse_enum_optional
 
 from .Balances import Balances
 from .Balances import from_json as Balances_from_json
 from .BitcoinNetwork import BitcoinNetwork
 from .BlockchainBalance import BlockchainBalance
@@ -124,23 +122,25 @@
         )
         connection = json["entity"]["addresses"]
         return NodeToAddressesConnection_from_json(self.requester, connection)
 
     def get_channels(
         self,
         first: Optional[int] = None,
-        statuses: Optional[List[ChannelStatus]] = None,
         after: Optional[str] = None,
+        before_date: Optional[datetime] = None,
+        after_date: Optional[datetime] = None,
+        statuses: Optional[List[ChannelStatus]] = None,
     ) -> LightsparkNodeToChannelsConnection:
         json = self.requester.execute_graphql(
             """
-query FetchLightsparkNodeToChannelsConnection($entity_id: ID!, $first: Int, $statuses: [ChannelStatus!], $after: String) {
+query FetchLightsparkNodeToChannelsConnection($entity_id: ID!, $first: Int, $after: String, $before_date: DateTime, $after_date: DateTime, $statuses: [ChannelStatus!]) {
     entity(id: $entity_id) {
         ... on LightsparkNode {
-            channels(, first: $first, statuses: $statuses, after: $after) {
+            channels(, first: $first, after: $after, before_date: $before_date, after_date: $after_date, statuses: $statuses) {
                 __typename
                 lightspark_node_to_channels_connection_count: count
                 lightspark_node_to_channels_connection_page_info: page_info {
                     __typename
                     page_info_has_next_page: has_next_page
                     page_info_has_previous_page: has_previous_page
                     page_info_start_cursor: start_cursor
@@ -244,16 +244,18 @@
         }
     }
 }
             """,
             {
                 "entity_id": self.id,
                 "first": first,
-                "statuses": statuses,
                 "after": after,
+                "before_date": before_date,
+                "after_date": after_date,
+                "statuses": statuses,
             },
         )
         connection = json["entity"]["channels"]
         return LightsparkNodeToChannelsConnection_from_json(self.requester, connection)
 
     def get_daily_liquidity_forecasts(
         self,
```

## Comparing `lightspark-2.6.0/lightspark/objects/CreateTestModeInvoiceInput.py` & `lightspark-2.7.0/lightspark/objects/CreateTestModeInvoiceInput.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # Copyright ©, 2022-present, Lightspark Group, Inc. - All Rights Reserved
 
 from dataclasses import dataclass
 from typing import Any, Mapping, Optional
 
-from lightspark.objects.InvoiceType import InvoiceType
 from lightspark.utils.enums import parse_enum_optional
 
 from .InvoiceType import InvoiceType
 
 
 @dataclass
 class CreateTestModeInvoiceInput:
```

## Comparing `lightspark-2.6.0/lightspark/objects/NodeToAddressesConnection.py` & `lightspark-2.7.0/lightspark/objects/NodeToAddressesConnection.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/CurrencyUnit.py` & `lightspark-2.7.0/lightspark/objects/CurrencyUnit.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/RequestWithdrawalOutput.py` & `lightspark-2.7.0/lightspark/objects/RequestWithdrawalOutput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/HtlcAttemptFailureCode.py` & `lightspark-2.7.0/lightspark/objects/HtlcAttemptFailureCode.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/Transaction.py` & `lightspark-2.7.0/lightspark/objects/Transaction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 # Copyright ©, 2022-present, Lightspark Group, Inc. - All Rights Reserved
 
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Any, Mapping, Optional
 
 from lightspark.exceptions import LightsparkException
-from lightspark.objects.PaymentFailureReason import PaymentFailureReason
-from lightspark.objects.RoutingTransactionFailureReason import (
-    RoutingTransactionFailureReason,
-)
-from lightspark.objects.TransactionStatus import TransactionStatus
 from lightspark.requests.requester import Requester
 from lightspark.utils.enums import parse_enum, parse_enum_optional
 
 from .CurrencyAmount import CurrencyAmount
 from .CurrencyAmount import from_json as CurrencyAmount_from_json
 from .Entity import Entity
+from .PaymentFailureReason import PaymentFailureReason
 from .PaymentRequestData import from_json as PaymentRequestData_from_json
 from .PostTransactionData import from_json as PostTransactionData_from_json
 from .RichText import from_json as RichText_from_json
+from .RoutingTransactionFailureReason import RoutingTransactionFailureReason
 from .TransactionStatus import TransactionStatus
 
 
 @dataclass
 class Transaction(Entity):
     """This object represents a payment transaction. The transaction can occur either on a Bitcoin Network, or over the Lightning Network. You can retrieve this object to receive specific information about a particular transaction tied to your Lightspark Node."""
```

## Comparing `lightspark-2.6.0/lightspark/objects/UpdateNodeSharedSecretInput.py` & `lightspark-2.7.0/lightspark/objects/UpdateNodeSharedSecretInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/SendPaymentInput.py` & `lightspark-2.7.0/lightspark/objects/SendPaymentInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/IncomingPaymentsForInvoiceQueryOutput.py` & `lightspark-2.7.0/lightspark/objects/IncomingPaymentsForInvoiceQueryOutput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/OutgoingPaymentAttempt.py` & `lightspark-2.7.0/lightspark/objects/OutgoingPaymentAttempt.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # Copyright ©, 2022-present, Lightspark Group, Inc. - All Rights Reserved
 
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Any, Mapping, Optional
 
-from lightspark.objects.HtlcAttemptFailureCode import HtlcAttemptFailureCode
-from lightspark.objects.OutgoingPaymentAttemptStatus import OutgoingPaymentAttemptStatus
 from lightspark.requests.requester import Requester
 from lightspark.utils.enums import parse_enum, parse_enum_optional
 
 from .CurrencyAmount import CurrencyAmount
 from .CurrencyAmount import from_json as CurrencyAmount_from_json
 from .Entity import Entity
 from .HtlcAttemptFailureCode import HtlcAttemptFailureCode
```

## Comparing `lightspark-2.6.0/lightspark/objects/ChannelStatus.py` & `lightspark-2.7.0/lightspark/objects/ChannelStatus.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/LightningTransaction.py` & `lightspark-2.7.0/lightspark/objects/LightningTransaction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 # Copyright ©, 2022-present, Lightspark Group, Inc. - All Rights Reserved
 
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Any, Mapping, Optional
 
 from lightspark.exceptions import LightsparkException
-from lightspark.objects.PaymentFailureReason import PaymentFailureReason
-from lightspark.objects.RoutingTransactionFailureReason import (
-    RoutingTransactionFailureReason,
-)
-from lightspark.objects.TransactionStatus import TransactionStatus
 from lightspark.requests.requester import Requester
 from lightspark.utils.enums import parse_enum, parse_enum_optional
 
 from .CurrencyAmount import CurrencyAmount
 from .CurrencyAmount import from_json as CurrencyAmount_from_json
 from .Entity import Entity
+from .PaymentFailureReason import PaymentFailureReason
 from .PaymentRequestData import from_json as PaymentRequestData_from_json
 from .PostTransactionData import from_json as PostTransactionData_from_json
 from .RichText import from_json as RichText_from_json
+from .RoutingTransactionFailureReason import RoutingTransactionFailureReason
 from .Transaction import Transaction
 from .TransactionStatus import TransactionStatus
 
 
 @dataclass
 class LightningTransaction(Transaction, Entity):
     """This is an object representing a transaction made over the Lightning Network. You can retrieve this object to receive information about a specific transaction made over Lightning for a Lightspark node."""
```

## Comparing `lightspark-2.6.0/lightspark/objects/CreateUmaInvitationOutput.py` & `lightspark-2.7.0/lightspark/objects/CreateUmaInvitationOutput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/WithdrawalFeeEstimateOutput.py` & `lightspark-2.7.0/lightspark/objects/WithdrawalFeeEstimateOutput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/Balances.py` & `lightspark-2.7.0/lightspark/objects/Balances.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/SignablePayload.py` & `lightspark-2.7.0/lightspark/objects/SignablePayload.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Copyright ©, 2022-present, Lightspark Group, Inc. - All Rights Reserved
 
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Any, Mapping, Optional
 
-from lightspark.objects.SignablePayloadStatus import SignablePayloadStatus
 from lightspark.requests.requester import Requester
 from lightspark.utils.enums import parse_enum
 
 from .Entity import Entity
 from .SignablePayloadStatus import SignablePayloadStatus
```

## Comparing `lightspark-2.6.0/lightspark/objects/AccountToTransactionsConnection.py` & `lightspark-2.7.0/lightspark/objects/AccountToTransactionsConnection.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/Channel.py` & `lightspark-2.7.0/lightspark/objects/Channel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Copyright ©, 2022-present, Lightspark Group, Inc. - All Rights Reserved
 
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Any, List, Mapping, Optional
 
-from lightspark.objects.ChannelStatus import ChannelStatus
 from lightspark.requests.requester import Requester
 from lightspark.utils.enums import parse_enum_optional
 
 from .ChannelFees import ChannelFees
 from .ChannelFees import from_json as ChannelFees_from_json
 from .ChannelStatus import ChannelStatus
 from .ChannelToTransactionsConnection import ChannelToTransactionsConnection
```

## Comparing `lightspark-2.6.0/lightspark/objects/Account.py` & `lightspark-2.7.0/lightspark/objects/Account.py`

 * *Files 0% similar despite different names*

```diff
@@ -1764,14 +1764,22 @@
                         __typename
                         currency_amount_original_value: original_value
                         currency_amount_original_unit: original_unit
                         currency_amount_preferred_currency_unit: preferred_currency_unit
                         currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
                         currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
                     }
+                    withdrawal_request_total_fees: total_fees {
+                        __typename
+                        currency_amount_original_value: original_value
+                        currency_amount_original_unit: original_unit
+                        currency_amount_preferred_currency_unit: preferred_currency_unit
+                        currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
+                        currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
+                    }
                     withdrawal_request_bitcoin_address: bitcoin_address
                     withdrawal_request_withdrawal_mode: withdrawal_mode
                     withdrawal_request_status: status
                     withdrawal_request_completed_at: completed_at
                     withdrawal_request_withdrawal: withdrawal {
                         id
                     }
```

## Comparing `lightspark-2.6.0/lightspark/objects/Connection.py` & `lightspark-2.7.0/lightspark/objects/Connection.py`

 * *Files 8% similar despite different names*

```diff
@@ -238,9 +238,37 @@
             page_info_start_cursor: start_cursor
             page_info_end_cursor: end_cursor
         }
         wallet_to_withdrawal_requests_connection_entities: entities {
             id
         }
     }
+    ... on WithdrawalRequestToChannelClosingTransactionsConnection {
+        __typename
+        withdrawal_request_to_channel_closing_transactions_connection_count: count
+        withdrawal_request_to_channel_closing_transactions_connection_page_info: page_info {
+            __typename
+            page_info_has_next_page: has_next_page
+            page_info_has_previous_page: has_previous_page
+            page_info_start_cursor: start_cursor
+            page_info_end_cursor: end_cursor
+        }
+        withdrawal_request_to_channel_closing_transactions_connection_entities: entities {
+            id
+        }
+    }
+    ... on WithdrawalRequestToChannelOpeningTransactionsConnection {
+        __typename
+        withdrawal_request_to_channel_opening_transactions_connection_count: count
+        withdrawal_request_to_channel_opening_transactions_connection_page_info: page_info {
+            __typename
+            page_info_has_next_page: has_next_page
+            page_info_has_previous_page: has_previous_page
+            page_info_start_cursor: start_cursor
+            page_info_end_cursor: end_cursor
+        }
+        withdrawal_request_to_channel_opening_transactions_connection_entities: entities {
+            id
+        }
+    }
 }
 """
```

## Comparing `lightspark-2.6.0/lightspark/objects/CreateInvoiceInput.py` & `lightspark-2.7.0/lightspark/objects/CreateInvoiceInput.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # Copyright ©, 2022-present, Lightspark Group, Inc. - All Rights Reserved
 
 from dataclasses import dataclass
 from typing import Any, Mapping, Optional
 
-from lightspark.objects.InvoiceType import InvoiceType
 from lightspark.utils.enums import parse_enum_optional
 
 from .InvoiceType import InvoiceType
 
 
 @dataclass
 class CreateInvoiceInput:
```

## Comparing `lightspark-2.6.0/lightspark/objects/CreateInvoiceOutput.py` & `lightspark-2.7.0/lightspark/objects/CreateInvoiceOutput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/IncomingPaymentAttemptStatus.py` & `lightspark-2.7.0/lightspark/objects/IncomingPaymentAttemptStatus.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/CreateTestModePaymentoutput.py` & `lightspark-2.7.0/lightspark/objects/CreateTestModePaymentoutput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/CreateInvitationWithIncentivesOutput.py` & `lightspark-2.7.0/lightspark/objects/CreateInvitationWithIncentivesOutput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/CreateUmaInvoiceInput.py` & `lightspark-2.7.0/lightspark/objects/CreateUmaInvoiceInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/OnChainTransaction.py` & `lightspark-2.7.0/lightspark/objects/OnChainTransaction.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Copyright ©, 2022-present, Lightspark Group, Inc. - All Rights Reserved
 
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Any, List, Mapping, Optional
 
 from lightspark.exceptions import LightsparkException
-from lightspark.objects.TransactionStatus import TransactionStatus
 from lightspark.requests.requester import Requester
 from lightspark.utils.enums import parse_enum
 
 from .CurrencyAmount import CurrencyAmount
 from .CurrencyAmount import from_json as CurrencyAmount_from_json
 from .Entity import Entity
 from .Transaction import Transaction
@@ -40,15 +39,15 @@
     amount: CurrencyAmount
     """The amount of money involved in this transaction."""
 
     transaction_hash: Optional[str]
     """The hash of this transaction, so it can be uniquely identified on the Lightning Network."""
 
     fees: Optional[CurrencyAmount]
-    """The fees that were paid by the wallet sending the transaction to commit it to the Bitcoin blockchain."""
+    """The fees that were paid by the node for this transaction."""
 
     block_hash: Optional[str]
     """The hash of the block that included this transaction. This will be null for unconfirmed transactions."""
 
     block_height: int
     """The height of the block that included this transaction. This will be zero for unconfirmed transactions."""
```

## Comparing `lightspark-2.6.0/lightspark/objects/InvoiceData.py` & `lightspark-2.7.0/lightspark/objects/InvoiceData.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Copyright ©, 2022-present, Lightspark Group, Inc. - All Rights Reserved
 
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Any, Mapping, Optional
 
-from lightspark.objects.BitcoinNetwork import BitcoinNetwork
 from lightspark.requests.requester import Requester
 from lightspark.utils.enums import parse_enum
 
 from .BitcoinNetwork import BitcoinNetwork
 from .CurrencyAmount import CurrencyAmount
 from .CurrencyAmount import from_json as CurrencyAmount_from_json
 from .Node import Node
```

## Comparing `lightspark-2.6.0/lightspark/objects/WalletToPaymentRequestsConnection.py` & `lightspark-2.7.0/lightspark/objects/WalletToPaymentRequestsConnection.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/UpdateChannelPerCommitmentPointInput.py` & `lightspark-2.7.0/lightspark/objects/UpdateChannelPerCommitmentPointInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/IncomingPaymentsForInvoiceQueryInput.py` & `lightspark-2.7.0/lightspark/objects/IncomingPaymentsForInvoiceQueryInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/ReleaseChannelPerCommitmentSecretInput.py` & `lightspark-2.7.0/lightspark/objects/ReleaseChannelPerCommitmentSecretInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/ChannelClosingTransaction.py` & `lightspark-2.7.0/lightspark/objects/ChannelClosingTransaction.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Copyright ©, 2022-present, Lightspark Group, Inc. - All Rights Reserved
 
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Any, List, Mapping, Optional
 
-from lightspark.objects.TransactionStatus import TransactionStatus
 from lightspark.requests.requester import Requester
 from lightspark.utils.enums import parse_enum
 
 from .CurrencyAmount import CurrencyAmount
 from .CurrencyAmount import from_json as CurrencyAmount_from_json
 from .Entity import Entity
 from .OnChainTransaction import OnChainTransaction
@@ -40,15 +39,15 @@
     amount: CurrencyAmount
     """The amount of money involved in this transaction."""
 
     transaction_hash: Optional[str]
     """The hash of this transaction, so it can be uniquely identified on the Lightning Network."""
 
     fees: Optional[CurrencyAmount]
-    """The fees that were paid by the wallet sending the transaction to commit it to the Bitcoin blockchain."""
+    """The fees that were paid by the node for this transaction."""
 
     block_hash: Optional[str]
     """The hash of the block that included this transaction. This will be null for unconfirmed transactions."""
 
     block_height: int
     """The height of the block that included this transaction. This will be zero for unconfirmed transactions."""
```

## Comparing `lightspark-2.6.0/lightspark/objects/DeleteApiTokenInput.py` & `lightspark-2.7.0/lightspark/objects/DeleteApiTokenInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/CurrencyAmount.py` & `lightspark-2.7.0/lightspark/objects/CurrencyAmount.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Copyright ©, 2022-present, Lightspark Group, Inc. - All Rights Reserved
 
 from dataclasses import dataclass
 from typing import Any, Mapping
 
 from lightspark.exceptions import LightsparkException
-from lightspark.objects.CurrencyUnit import CurrencyUnit
 from lightspark.requests.requester import Requester
 from lightspark.utils.enums import parse_enum
 
 from .CurrencyUnit import CurrencyUnit
 
 
 @dataclass
```

## Comparing `lightspark-2.6.0/lightspark/objects/CreateTestModeInvoiceOutput.py` & `lightspark-2.7.0/lightspark/objects/CreateTestModeInvoiceOutput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/FundNodeInput.py` & `lightspark-2.7.0/lightspark/objects/FundNodeInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/ScreenNodeInput.py` & `lightspark-2.7.0/lightspark/objects/ScreenNodeInput.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # Copyright ©, 2022-present, Lightspark Group, Inc. - All Rights Reserved
 
 from dataclasses import dataclass
 from typing import Any, Mapping
 
-from lightspark.objects.ComplianceProvider import ComplianceProvider
 from lightspark.utils.enums import parse_enum
 
 from .ComplianceProvider import ComplianceProvider
 
 
 @dataclass
 class ScreenNodeInput:
```

## Comparing `lightspark-2.6.0/lightspark/objects/InvoiceType.py` & `lightspark-2.7.0/lightspark/objects/InvoiceType.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/AccountToWithdrawalRequestsConnection.py` & `lightspark-2.7.0/lightspark/objects/AccountToWithdrawalRequestsConnection.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/SignInvoiceInput.py` & `lightspark-2.7.0/lightspark/objects/SignInvoiceInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/ChannelSnapshot.py` & `lightspark-2.7.0/lightspark/objects/ChannelSnapshot.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/RiskRating.py` & `lightspark-2.7.0/lightspark/objects/RiskRating.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/CancelInvoiceInput.py` & `lightspark-2.7.0/lightspark/objects/CancelInvoiceInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/UpdateChannelPerCommitmentPointOutput.py` & `lightspark-2.7.0/lightspark/objects/UpdateChannelPerCommitmentPointOutput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/BitcoinNetwork.py` & `lightspark-2.7.0/lightspark/objects/BitcoinNetwork.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/RegionCode.py` & `lightspark-2.7.0/lightspark/objects/RegionCode.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/OutgoingPaymentAttemptStatus.py` & `lightspark-2.7.0/lightspark/objects/OutgoingPaymentAttemptStatus.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/WalletToWithdrawalRequestsConnection.py` & `lightspark-2.7.0/lightspark/objects/WalletToWithdrawalRequestsConnection.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/LightsparkNodeToDailyLiquidityForecastsConnection.py` & `lightspark-2.7.0/lightspark/objects/LightsparkNodeToDailyLiquidityForecastsConnection.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Copyright ©, 2022-present, Lightspark Group, Inc. - All Rights Reserved
 
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Any, List, Mapping
 
-from lightspark.objects.LightningPaymentDirection import LightningPaymentDirection
 from lightspark.requests.requester import Requester
 from lightspark.utils.enums import parse_enum
 
 from .DailyLiquidityForecast import DailyLiquidityForecast
 from .DailyLiquidityForecast import from_json as DailyLiquidityForecast_from_json
 from .LightningPaymentDirection import LightningPaymentDirection
```

## Comparing `lightspark-2.6.0/lightspark/objects/SetInvoicePaymentHashInput.py` & `lightspark-2.7.0/lightspark/objects/SetInvoicePaymentHashInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/ClaimUmaInvitationOutput.py` & `lightspark-2.7.0/lightspark/objects/ClaimUmaInvitationOutput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/Permission.py` & `lightspark-2.7.0/lightspark/objects/Permission.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/SignInvoiceOutput.py` & `lightspark-2.7.0/lightspark/objects/SignInvoiceOutput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/RequestWithdrawalInput.py` & `lightspark-2.7.0/lightspark/objects/WithdrawalFeeEstimateInput.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,37 @@
 # Copyright ©, 2022-present, Lightspark Group, Inc. - All Rights Reserved
 
 from dataclasses import dataclass
 from typing import Any, Mapping
 
-from lightspark.objects.WithdrawalMode import WithdrawalMode
 from lightspark.utils.enums import parse_enum
 
 from .WithdrawalMode import WithdrawalMode
 
 
 @dataclass
-class RequestWithdrawalInput:
+class WithdrawalFeeEstimateInput:
     node_id: str
     """The node from which you'd like to make the withdrawal."""
 
-    bitcoin_address: str
-    """The bitcoin address where the withdrawal should be sent."""
-
     amount_sats: int
     """The amount you want to withdraw from this node in Satoshis. Use the special value -1 to withdrawal all funds from this node."""
 
     withdrawal_mode: WithdrawalMode
     """The strategy that should be used to withdraw the funds from this node."""
 
     def to_json(self) -> Mapping[str, Any]:
         return {
-            "request_withdrawal_input_node_id": self.node_id,
-            "request_withdrawal_input_bitcoin_address": self.bitcoin_address,
-            "request_withdrawal_input_amount_sats": self.amount_sats,
-            "request_withdrawal_input_withdrawal_mode": self.withdrawal_mode.value,
+            "withdrawal_fee_estimate_input_node_id": self.node_id,
+            "withdrawal_fee_estimate_input_amount_sats": self.amount_sats,
+            "withdrawal_fee_estimate_input_withdrawal_mode": self.withdrawal_mode.value,
         }
 
 
-def from_json(obj: Mapping[str, Any]) -> RequestWithdrawalInput:
-    return RequestWithdrawalInput(
-        node_id=obj["request_withdrawal_input_node_id"],
-        bitcoin_address=obj["request_withdrawal_input_bitcoin_address"],
-        amount_sats=obj["request_withdrawal_input_amount_sats"],
+def from_json(obj: Mapping[str, Any]) -> WithdrawalFeeEstimateInput:
+    return WithdrawalFeeEstimateInput(
+        node_id=obj["withdrawal_fee_estimate_input_node_id"],
+        amount_sats=obj["withdrawal_fee_estimate_input_amount_sats"],
         withdrawal_mode=parse_enum(
-            WithdrawalMode, obj["request_withdrawal_input_withdrawal_mode"]
+            WithdrawalMode, obj["withdrawal_fee_estimate_input_withdrawal_mode"]
         ),
     )
```

## Comparing `lightspark-2.6.0/lightspark/objects/Entity.py` & `lightspark-2.7.0/lightspark/objects/Entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1495,14 +1495,22 @@
             __typename
             currency_amount_original_value: original_value
             currency_amount_original_unit: original_unit
             currency_amount_preferred_currency_unit: preferred_currency_unit
             currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
             currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
         }
+        withdrawal_request_total_fees: total_fees {
+            __typename
+            currency_amount_original_value: original_value
+            currency_amount_original_unit: original_unit
+            currency_amount_preferred_currency_unit: preferred_currency_unit
+            currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
+            currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
+        }
         withdrawal_request_bitcoin_address: bitcoin_address
         withdrawal_request_withdrawal_mode: withdrawal_mode
         withdrawal_request_status: status
         withdrawal_request_completed_at: completed_at
         withdrawal_request_withdrawal: withdrawal {
             id
         }
```

## Comparing `lightspark-2.6.0/lightspark/objects/OutgoingPaymentToAttemptsConnection.py` & `lightspark-2.7.0/lightspark/objects/OutgoingPaymentToAttemptsConnection.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/Invoice.py` & `lightspark-2.7.0/lightspark/objects/Invoice.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Copyright ©, 2022-present, Lightspark Group, Inc. - All Rights Reserved
 
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Any, Mapping, Optional
 
-from lightspark.objects.PaymentRequestStatus import PaymentRequestStatus
 from lightspark.requests.requester import Requester
 from lightspark.utils.enums import parse_enum
 
 from .CurrencyAmount import CurrencyAmount
 from .CurrencyAmount import from_json as CurrencyAmount_from_json
 from .Entity import Entity
 from .InvoiceData import InvoiceData
```

## Comparing `lightspark-2.6.0/lightspark/objects/IdAndSignature.py` & `lightspark-2.7.0/lightspark/objects/IdAndSignature.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/RoutingTransactionFailureReason.py` & `lightspark-2.7.0/lightspark/objects/RoutingTransactionFailureReason.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/ChannelOpeningTransaction.py` & `lightspark-2.7.0/lightspark/objects/ChannelOpeningTransaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Copyright ©, 2022-present, Lightspark Group, Inc. - All Rights Reserved
 
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Any, List, Mapping, Optional
 
-from lightspark.objects.TransactionStatus import TransactionStatus
 from lightspark.requests.requester import Requester
 from lightspark.utils.enums import parse_enum
 
 from .CurrencyAmount import CurrencyAmount
 from .CurrencyAmount import from_json as CurrencyAmount_from_json
 from .Entity import Entity
 from .OnChainTransaction import OnChainTransaction
@@ -40,15 +39,15 @@
     amount: CurrencyAmount
     """The amount of money involved in this transaction."""
 
     transaction_hash: Optional[str]
     """The hash of this transaction, so it can be uniquely identified on the Lightning Network."""
 
     fees: Optional[CurrencyAmount]
-    """The fees that were paid by the wallet sending the transaction to commit it to the Bitcoin blockchain."""
+    """The fees that were paid by the node for this transaction."""
 
     block_hash: Optional[str]
     """The hash of the block that included this transaction. This will be null for unconfirmed transactions."""
 
     block_height: int
     """The height of the block that included this transaction. This will be zero for unconfirmed transactions."""
```

## Comparing `lightspark-2.6.0/lightspark/objects/PaymentRequestData.py` & `lightspark-2.7.0/lightspark/objects/PaymentRequestData.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Copyright ©, 2022-present, Lightspark Group, Inc. - All Rights Reserved
 
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Any, Mapping
 
 from lightspark.exceptions import LightsparkException
-from lightspark.objects.BitcoinNetwork import BitcoinNetwork
 from lightspark.requests.requester import Requester
 from lightspark.utils.enums import parse_enum
 
 from .BitcoinNetwork import BitcoinNetwork
 from .CurrencyAmount import from_json as CurrencyAmount_from_json
 from .Node import from_json as Node_from_json
```

## Comparing `lightspark-2.6.0/lightspark/objects/WalletStatus.py` & `lightspark-2.7.0/lightspark/objects/WalletStatus.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/LightningPaymentDirection.py` & `lightspark-2.7.0/lightspark/objects/LightningPaymentDirection.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/WithdrawalRequestToChannelOpeningTransactionsConnection.py` & `lightspark-2.7.0/lightspark/objects/WithdrawalRequestToChannelOpeningTransactionsConnection.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,73 +3,77 @@
 from dataclasses import dataclass
 from typing import Any, List, Mapping
 
 from lightspark.requests.requester import Requester
 
 from .ChannelOpeningTransaction import ChannelOpeningTransaction
 from .ChannelOpeningTransaction import from_json as ChannelOpeningTransaction_from_json
+from .Connection import Connection
 from .PageInfo import PageInfo
 from .PageInfo import from_json as PageInfo_from_json
 
 
 @dataclass
-class WithdrawalRequestToChannelOpeningTransactionsConnection:
+class WithdrawalRequestToChannelOpeningTransactionsConnection(Connection):
     requester: Requester
 
-    page_info: PageInfo
-    """An object that holds pagination information about the objects in this connection."""
-
     count: int
     """The total count of objects in this connection, using the current filters. It is different from the number of objects returned in the current page (in the `entities` field)."""
 
+    page_info: PageInfo
+    """An object that holds pagination information about the objects in this connection."""
+
     entities: List[ChannelOpeningTransaction]
     """The channel opening transactions for the current page of this connection."""
+    typename: str
 
     def to_json(self) -> Mapping[str, Any]:
         return {
-            "withdrawal_request_to_channel_opening_transactions_connection_page_info": self.page_info.to_json(),
+            "__typename": "WithdrawalRequestToChannelOpeningTransactionsConnection",
             "withdrawal_request_to_channel_opening_transactions_connection_count": self.count,
+            "withdrawal_request_to_channel_opening_transactions_connection_page_info": self.page_info.to_json(),
             "withdrawal_request_to_channel_opening_transactions_connection_entities": [
                 e.to_json() for e in self.entities
             ],
         }
 
 
 FRAGMENT = """
 fragment WithdrawalRequestToChannelOpeningTransactionsConnectionFragment on WithdrawalRequestToChannelOpeningTransactionsConnection {
     __typename
+    withdrawal_request_to_channel_opening_transactions_connection_count: count
     withdrawal_request_to_channel_opening_transactions_connection_page_info: page_info {
         __typename
         page_info_has_next_page: has_next_page
         page_info_has_previous_page: has_previous_page
         page_info_start_cursor: start_cursor
         page_info_end_cursor: end_cursor
     }
-    withdrawal_request_to_channel_opening_transactions_connection_count: count
     withdrawal_request_to_channel_opening_transactions_connection_entities: entities {
         id
     }
 }
 """
 
 
 def from_json(
     requester: Requester, obj: Mapping[str, Any]
 ) -> WithdrawalRequestToChannelOpeningTransactionsConnection:
     return WithdrawalRequestToChannelOpeningTransactionsConnection(
         requester=requester,
+        typename="WithdrawalRequestToChannelOpeningTransactionsConnection",
+        count=obj[
+            "withdrawal_request_to_channel_opening_transactions_connection_count"
+        ],
         page_info=PageInfo_from_json(
             requester,
             obj[
                 "withdrawal_request_to_channel_opening_transactions_connection_page_info"
             ],
         ),
-        count=obj[
-            "withdrawal_request_to_channel_opening_transactions_connection_count"
-        ],
         entities=list(
             map(
                 # pylint: disable=unnecessary-lambda
                 lambda e: ChannelOpeningTransaction_from_json(requester, e),
                 obj[
                     "withdrawal_request_to_channel_opening_transactions_connection_entities"
                 ],
```

## Comparing `lightspark-2.6.0/lightspark/objects/UpdateNodeSharedSecretOutput.py` & `lightspark-2.7.0/lightspark/objects/UpdateNodeSharedSecretOutput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/ClaimUmaInvitationWithIncentivesOutput.py` & `lightspark-2.7.0/lightspark/objects/ClaimUmaInvitationWithIncentivesOutput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/WithdrawalRequestStatus.py` & `lightspark-2.7.0/lightspark/objects/WithdrawalRequestStatus.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,12 +4,13 @@
 
 
 class WithdrawalRequestStatus(Enum):
     """This is an enum of the potential statuses that a Withdrawal can take."""
 
     ___FUTURE_VALUE___ = "___FUTURE_VALUE___"
     """This is an enum value that represents future values that could be added in the future. Clients should support unknown values as more of them could be added without notice."""
+    CREATING = "CREATING"
     CREATED = "CREATED"
     FAILED = "FAILED"
     IN_PROGRESS = "IN_PROGRESS"
     SUCCESSFUL = "SUCCESSFUL"
     PARTIALLY_SUCCESSFUL = "PARTIALLY_SUCCESSFUL"
```

## Comparing `lightspark-2.6.0/lightspark/objects/WebhookEventType.py` & `lightspark-2.7.0/lightspark/objects/WebhookEventType.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/UmaInvitation.py` & `lightspark-2.7.0/lightspark/objects/UmaInvitation.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 # Copyright ©, 2022-present, Lightspark Group, Inc. - All Rights Reserved
 
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Any, Mapping, Optional
 
-from lightspark.objects.IncentivesIneligibilityReason import (
-    IncentivesIneligibilityReason,
-)
-from lightspark.objects.IncentivesStatus import IncentivesStatus
 from lightspark.requests.requester import Requester
 from lightspark.utils.enums import parse_enum, parse_enum_optional
 
 from .Entity import Entity
 from .IncentivesIneligibilityReason import IncentivesIneligibilityReason
 from .IncentivesStatus import IncentivesStatus
```

## Comparing `lightspark-2.6.0/lightspark/objects/SetInvoicePaymentHashOutput.py` & `lightspark-2.7.0/lightspark/objects/SetInvoicePaymentHashOutput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/PayUmaInvoiceInput.py` & `lightspark-2.7.0/lightspark/objects/PayUmaInvoiceInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/PaymentFailureReason.py` & `lightspark-2.7.0/lightspark/objects/PaymentFailureReason.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/AuditLogActor.py` & `lightspark-2.7.0/lightspark/objects/AuditLogActor.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/CreateTestModePaymentInput.py` & `lightspark-2.7.0/lightspark/objects/CreateTestModePaymentInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/LightsparkNodeStatus.py` & `lightspark-2.7.0/lightspark/objects/LightsparkNodeStatus.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/ClaimUmaInvitationWithIncentivesInput.py` & `lightspark-2.7.0/lightspark/objects/ClaimUmaInvitationWithIncentivesInput.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # Copyright ©, 2022-present, Lightspark Group, Inc. - All Rights Reserved
 
 from dataclasses import dataclass
 from typing import Any, Mapping
 
-from lightspark.objects.RegionCode import RegionCode
 from lightspark.utils.enums import parse_enum
 
 from .RegionCode import RegionCode
 
 
 @dataclass
 class ClaimUmaInvitationWithIncentivesInput:
```

## Comparing `lightspark-2.6.0/lightspark/objects/CreateUmaInvitationInput.py` & `lightspark-2.7.0/lightspark/objects/CreateUmaInvitationInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/ScreenNodeOutput.py` & `lightspark-2.7.0/lightspark/objects/ScreenNodeOutput.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # Copyright ©, 2022-present, Lightspark Group, Inc. - All Rights Reserved
 
 from dataclasses import dataclass
 from typing import Any, Mapping
 
-from lightspark.objects.RiskRating import RiskRating
 from lightspark.requests.requester import Requester
 from lightspark.utils.enums import parse_enum
 
 from .RiskRating import RiskRating
 
 
 @dataclass
```

## Comparing `lightspark-2.6.0/lightspark/objects/LightningFeeEstimateOutput.py` & `lightspark-2.7.0/lightspark/objects/LightningFeeEstimateOutput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/AccountToPaymentRequestsConnection.py` & `lightspark-2.7.0/lightspark/objects/AccountToPaymentRequestsConnection.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/all_entities.py` & `lightspark-2.7.0/lightspark/objects/all_entities.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/FundNodeOutput.py` & `lightspark-2.7.0/lightspark/objects/FundNodeOutput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/LightsparkNodeOwner.py` & `lightspark-2.7.0/lightspark/objects/LightsparkNodeOwner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # Copyright ©, 2022-present, Lightspark Group, Inc. - All Rights Reserved
 
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Any, Mapping
 
 from lightspark.exceptions import LightsparkException
-from lightspark.objects.WalletStatus import WalletStatus
 from lightspark.requests.requester import Requester
 from lightspark.utils.enums import parse_enum
 
 from .Balances import from_json as Balances_from_json
 from .Entity import Entity
+from .WalletStatus import WalletStatus
 
 
 @dataclass
 class LightsparkNodeOwner(Entity):
     """This is an object representing the owner of a LightsparkNode."""
 
     requester: Requester
```

## Comparing `lightspark-2.6.0/lightspark/objects/AccountToNodesConnection.py` & `lightspark-2.7.0/lightspark/objects/AccountToNodesConnection.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/TransactionType.py` & `lightspark-2.7.0/lightspark/objects/TransactionType.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/LightsparkNodeWithRemoteSigning.py` & `lightspark-2.7.0/lightspark/objects/LightsparkNodeWithRemoteSigning.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # Copyright ©, 2022-present, Lightspark Group, Inc. - All Rights Reserved
 
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Any, List, Mapping, Optional
 
-from lightspark.objects.BitcoinNetwork import BitcoinNetwork
-from lightspark.objects.LightsparkNodeStatus import LightsparkNodeStatus
 from lightspark.requests.requester import Requester
 from lightspark.utils.enums import parse_enum, parse_enum_optional
 
 from .Balances import Balances
 from .Balances import from_json as Balances_from_json
 from .BitcoinNetwork import BitcoinNetwork
 from .BlockchainBalance import BlockchainBalance
@@ -123,23 +121,25 @@
         )
         connection = json["entity"]["addresses"]
         return NodeToAddressesConnection_from_json(self.requester, connection)
 
     def get_channels(
         self,
         first: Optional[int] = None,
-        statuses: Optional[List[ChannelStatus]] = None,
         after: Optional[str] = None,
+        before_date: Optional[datetime] = None,
+        after_date: Optional[datetime] = None,
+        statuses: Optional[List[ChannelStatus]] = None,
     ) -> LightsparkNodeToChannelsConnection:
         json = self.requester.execute_graphql(
             """
-query FetchLightsparkNodeToChannelsConnection($entity_id: ID!, $first: Int, $statuses: [ChannelStatus!], $after: String) {
+query FetchLightsparkNodeToChannelsConnection($entity_id: ID!, $first: Int, $after: String, $before_date: DateTime, $after_date: DateTime, $statuses: [ChannelStatus!]) {
     entity(id: $entity_id) {
         ... on LightsparkNodeWithRemoteSigning {
-            channels(, first: $first, statuses: $statuses, after: $after) {
+            channels(, first: $first, after: $after, before_date: $before_date, after_date: $after_date, statuses: $statuses) {
                 __typename
                 lightspark_node_to_channels_connection_count: count
                 lightspark_node_to_channels_connection_page_info: page_info {
                     __typename
                     page_info_has_next_page: has_next_page
                     page_info_has_previous_page: has_previous_page
                     page_info_start_cursor: start_cursor
@@ -243,16 +243,18 @@
         }
     }
 }
             """,
             {
                 "entity_id": self.id,
                 "first": first,
-                "statuses": statuses,
                 "after": after,
+                "before_date": before_date,
+                "after_date": after_date,
+                "statuses": statuses,
             },
         )
         connection = json["entity"]["channels"]
         return LightsparkNodeToChannelsConnection_from_json(self.requester, connection)
 
     def get_daily_liquidity_forecasts(
         self,
```

## Comparing `lightspark-2.6.0/lightspark/objects/PageInfo.py` & `lightspark-2.7.0/lightspark/objects/PageInfo.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/IncomingPaymentAttempt.py` & `lightspark-2.7.0/lightspark/objects/IncomingPaymentAttempt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Copyright ©, 2022-present, Lightspark Group, Inc. - All Rights Reserved
 
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Any, Mapping, Optional
 
-from lightspark.objects.IncomingPaymentAttemptStatus import IncomingPaymentAttemptStatus
 from lightspark.requests.requester import Requester
 from lightspark.utils.enums import parse_enum
 
 from .CurrencyAmount import CurrencyAmount
 from .CurrencyAmount import from_json as CurrencyAmount_from_json
 from .Entity import Entity
 from .IncomingPaymentAttemptStatus import IncomingPaymentAttemptStatus
```

## Comparing `lightspark-2.6.0/lightspark/objects/ChannelFees.py` & `lightspark-2.7.0/lightspark/objects/ChannelFees.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/OutgoingPaymentsForInvoiceQueryOutput.py` & `lightspark-2.7.0/lightspark/objects/OutgoingPaymentsForInvoiceQueryOutput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/DeclineToSignMessagesInput.py` & `lightspark-2.7.0/lightspark/objects/DeclineToSignMessagesInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/ChannelToTransactionsConnection.py` & `lightspark-2.7.0/lightspark/objects/ChannelToTransactionsConnection.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/LightsparkNodeToChannelsConnection.py` & `lightspark-2.7.0/lightspark/objects/LightsparkNodeToChannelsConnection.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/CreateLnurlInvoiceInput.py` & `lightspark-2.7.0/lightspark/objects/CreateLnurlInvoiceInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/RichText.py` & `lightspark-2.7.0/lightspark/objects/RichText.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/Withdrawal.py` & `lightspark-2.7.0/lightspark/objects/Withdrawal.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Copyright ©, 2022-present, Lightspark Group, Inc. - All Rights Reserved
 
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Any, List, Mapping, Optional
 
-from lightspark.objects.TransactionStatus import TransactionStatus
 from lightspark.requests.requester import Requester
 from lightspark.utils.enums import parse_enum
 
 from .CurrencyAmount import CurrencyAmount
 from .CurrencyAmount import from_json as CurrencyAmount_from_json
 from .Entity import Entity
 from .OnChainTransaction import OnChainTransaction
@@ -40,15 +39,15 @@
     amount: CurrencyAmount
     """The amount of money involved in this transaction."""
 
     transaction_hash: Optional[str]
     """The hash of this transaction, so it can be uniquely identified on the Lightning Network."""
 
     fees: Optional[CurrencyAmount]
-    """The fees that were paid by the wallet sending the transaction to commit it to the Bitcoin blockchain."""
+    """The fees that were paid by the node for this transaction."""
 
     block_hash: Optional[str]
     """The hash of the block that included this transaction. This will be null for unconfirmed transactions."""
 
     block_height: int
     """The height of the block that included this transaction. This will be zero for unconfirmed transactions."""
```

## Comparing `lightspark-2.6.0/lightspark/objects/IncomingPayment.py` & `lightspark-2.7.0/lightspark/objects/IncomingPayment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Copyright ©, 2022-present, Lightspark Group, Inc. - All Rights Reserved
 
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Any, List, Mapping, Optional
 
-from lightspark.objects.TransactionStatus import TransactionStatus
 from lightspark.requests.requester import Requester
 from lightspark.utils.enums import parse_enum
 
 from .CurrencyAmount import CurrencyAmount
 from .CurrencyAmount import from_json as CurrencyAmount_from_json
 from .Entity import Entity
 from .IncomingPaymentAttemptStatus import IncomingPaymentAttemptStatus
```

## Comparing `lightspark-2.6.0/lightspark/objects/NodeAddressType.py` & `lightspark-2.7.0/lightspark/objects/NodeAddressType.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/CreateApiTokenInput.py` & `lightspark-2.7.0/lightspark/objects/CreateApiTokenInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/WalletToTransactionsConnection.py` & `lightspark-2.7.0/lightspark/objects/WalletToTransactionsConnection.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/Wallet.py` & `lightspark-2.7.0/lightspark/objects/Wallet.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Copyright ©, 2022-present, Lightspark Group, Inc. - All Rights Reserved
 
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Any, List, Mapping, Optional
 
-from lightspark.objects.WalletStatus import WalletStatus
 from lightspark.requests.requester import Requester
 from lightspark.utils.enums import parse_enum
 
 from .Balances import Balances
 from .Balances import from_json as Balances_from_json
 from .CurrencyAmount import CurrencyAmount
 from .CurrencyAmount import from_json as CurrencyAmount_from_json
@@ -1088,14 +1087,22 @@
                         __typename
                         currency_amount_original_value: original_value
                         currency_amount_original_unit: original_unit
                         currency_amount_preferred_currency_unit: preferred_currency_unit
                         currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
                         currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
                     }
+                    withdrawal_request_total_fees: total_fees {
+                        __typename
+                        currency_amount_original_value: original_value
+                        currency_amount_original_unit: original_unit
+                        currency_amount_preferred_currency_unit: preferred_currency_unit
+                        currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
+                        currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
+                    }
                     withdrawal_request_bitcoin_address: bitcoin_address
                     withdrawal_request_withdrawal_mode: withdrawal_mode
                     withdrawal_request_status: status
                     withdrawal_request_completed_at: completed_at
                     withdrawal_request_withdrawal: withdrawal {
                         id
                     }
```

## Comparing `lightspark-2.6.0/lightspark/objects/ClaimUmaInvitationInput.py` & `lightspark-2.7.0/lightspark/objects/ClaimUmaInvitationInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/WithdrawalMode.py` & `lightspark-2.7.0/lightspark/objects/WithdrawalMode.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/AccountToChannelsConnection.py` & `lightspark-2.7.0/lightspark/objects/AccountToChannelsConnection.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/ApiToken.py` & `lightspark-2.7.0/lightspark/objects/ApiToken.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/OutgoingPaymentsForInvoiceQueryInput.py` & `lightspark-2.7.0/lightspark/objects/OutgoingPaymentsForInvoiceQueryInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/LightningFeeEstimateForNodeInput.py` & `lightspark-2.7.0/lightspark/objects/LightningFeeEstimateForNodeInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/WithdrawalRequestToChannelClosingTransactionsConnection.py` & `lightspark-2.7.0/lightspark/objects/WithdrawalRequestToChannelClosingTransactionsConnection.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,73 +3,77 @@
 from dataclasses import dataclass
 from typing import Any, List, Mapping
 
 from lightspark.requests.requester import Requester
 
 from .ChannelClosingTransaction import ChannelClosingTransaction
 from .ChannelClosingTransaction import from_json as ChannelClosingTransaction_from_json
+from .Connection import Connection
 from .PageInfo import PageInfo
 from .PageInfo import from_json as PageInfo_from_json
 
 
 @dataclass
-class WithdrawalRequestToChannelClosingTransactionsConnection:
+class WithdrawalRequestToChannelClosingTransactionsConnection(Connection):
     requester: Requester
 
-    page_info: PageInfo
-    """An object that holds pagination information about the objects in this connection."""
-
     count: int
     """The total count of objects in this connection, using the current filters. It is different from the number of objects returned in the current page (in the `entities` field)."""
 
+    page_info: PageInfo
+    """An object that holds pagination information about the objects in this connection."""
+
     entities: List[ChannelClosingTransaction]
     """The channel closing transactions for the current page of this connection."""
+    typename: str
 
     def to_json(self) -> Mapping[str, Any]:
         return {
-            "withdrawal_request_to_channel_closing_transactions_connection_page_info": self.page_info.to_json(),
+            "__typename": "WithdrawalRequestToChannelClosingTransactionsConnection",
             "withdrawal_request_to_channel_closing_transactions_connection_count": self.count,
+            "withdrawal_request_to_channel_closing_transactions_connection_page_info": self.page_info.to_json(),
             "withdrawal_request_to_channel_closing_transactions_connection_entities": [
                 e.to_json() for e in self.entities
             ],
         }
 
 
 FRAGMENT = """
 fragment WithdrawalRequestToChannelClosingTransactionsConnectionFragment on WithdrawalRequestToChannelClosingTransactionsConnection {
     __typename
+    withdrawal_request_to_channel_closing_transactions_connection_count: count
     withdrawal_request_to_channel_closing_transactions_connection_page_info: page_info {
         __typename
         page_info_has_next_page: has_next_page
         page_info_has_previous_page: has_previous_page
         page_info_start_cursor: start_cursor
         page_info_end_cursor: end_cursor
     }
-    withdrawal_request_to_channel_closing_transactions_connection_count: count
     withdrawal_request_to_channel_closing_transactions_connection_entities: entities {
         id
     }
 }
 """
 
 
 def from_json(
     requester: Requester, obj: Mapping[str, Any]
 ) -> WithdrawalRequestToChannelClosingTransactionsConnection:
     return WithdrawalRequestToChannelClosingTransactionsConnection(
         requester=requester,
+        typename="WithdrawalRequestToChannelClosingTransactionsConnection",
+        count=obj[
+            "withdrawal_request_to_channel_closing_transactions_connection_count"
+        ],
         page_info=PageInfo_from_json(
             requester,
             obj[
                 "withdrawal_request_to_channel_closing_transactions_connection_page_info"
             ],
         ),
-        count=obj[
-            "withdrawal_request_to_channel_closing_transactions_connection_count"
-        ],
         entities=list(
             map(
                 # pylint: disable=unnecessary-lambda
                 lambda e: ChannelClosingTransaction_from_json(requester, e),
                 obj[
                     "withdrawal_request_to_channel_closing_transactions_connection_entities"
                 ],
```

## Comparing `lightspark-2.6.0/lightspark/objects/MultiSigAddressValidationParameters.py` & `lightspark-2.7.0/lightspark/objects/MultiSigAddressValidationParameters.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/Node.py` & `lightspark-2.7.0/lightspark/objects/Node.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # Copyright ©, 2022-present, Lightspark Group, Inc. - All Rights Reserved
 
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Any, List, Mapping, Optional
 
 from lightspark.exceptions import LightsparkException
-from lightspark.objects.BitcoinNetwork import BitcoinNetwork
-from lightspark.objects.LightsparkNodeStatus import LightsparkNodeStatus
 from lightspark.requests.requester import Requester
 from lightspark.utils.enums import parse_enum, parse_enum_optional
 
 from .Balances import from_json as Balances_from_json
 from .BitcoinNetwork import BitcoinNetwork
 from .BlockchainBalance import from_json as BlockchainBalance_from_json
 from .CurrencyAmount import from_json as CurrencyAmount_from_json
 from .Entity import Entity
+from .LightsparkNodeStatus import LightsparkNodeStatus
 from .NodeAddressType import NodeAddressType
 from .NodeToAddressesConnection import NodeToAddressesConnection
 from .NodeToAddressesConnection import from_json as NodeToAddressesConnection_from_json
 from .Secret import from_json as Secret_from_json
 
 
 @dataclass
```

## Comparing `lightspark-2.6.0/lightspark/objects/IncentivesStatus.py` & `lightspark-2.7.0/lightspark/objects/IncentivesStatus.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/RoutingTransaction.py` & `lightspark-2.7.0/lightspark/objects/RoutingTransaction.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 # Copyright ©, 2022-present, Lightspark Group, Inc. - All Rights Reserved
 
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Any, Mapping, Optional
 
-from lightspark.objects.RoutingTransactionFailureReason import (
-    RoutingTransactionFailureReason,
-)
-from lightspark.objects.TransactionStatus import TransactionStatus
 from lightspark.requests.requester import Requester
 from lightspark.utils.enums import parse_enum, parse_enum_optional
 
 from .CurrencyAmount import CurrencyAmount
 from .CurrencyAmount import from_json as CurrencyAmount_from_json
 from .Entity import Entity
 from .LightningTransaction import LightningTransaction
```

## Comparing `lightspark-2.6.0/lightspark/objects/ReleaseChannelPerCommitmentSecretOutput.py` & `lightspark-2.7.0/lightspark/objects/ReleaseChannelPerCommitmentSecretOutput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/Signable.py` & `lightspark-2.7.0/lightspark/objects/Signable.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/Secret.py` & `lightspark-2.7.0/lightspark/objects/Secret.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/SignMessagesInput.py` & `lightspark-2.7.0/lightspark/objects/SignMessagesInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/WithdrawalRequest.py` & `lightspark-2.7.0/lightspark/objects/WithdrawalRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # Copyright ©, 2022-present, Lightspark Group, Inc. - All Rights Reserved
 
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Any, Mapping, Optional
 
-from lightspark.objects.WithdrawalMode import WithdrawalMode
-from lightspark.objects.WithdrawalRequestStatus import WithdrawalRequestStatus
 from lightspark.requests.requester import Requester
 from lightspark.utils.enums import parse_enum
 
 from .CurrencyAmount import CurrencyAmount
 from .CurrencyAmount import from_json as CurrencyAmount_from_json
 from .Entity import Entity
 from .WithdrawalMode import WithdrawalMode
@@ -22,14 +20,20 @@
 )
 from .WithdrawalRequestToChannelOpeningTransactionsConnection import (
     WithdrawalRequestToChannelOpeningTransactionsConnection,
 )
 from .WithdrawalRequestToChannelOpeningTransactionsConnection import (
     from_json as WithdrawalRequestToChannelOpeningTransactionsConnection_from_json,
 )
+from .WithdrawalRequestToWithdrawalsConnection import (
+    WithdrawalRequestToWithdrawalsConnection,
+)
+from .WithdrawalRequestToWithdrawalsConnection import (
+    from_json as WithdrawalRequestToWithdrawalsConnection_from_json,
+)
 
 
 @dataclass
 class WithdrawalRequest(Entity):
     """This object represents a request made for an L1 withdrawal from your Lightspark Node to any Bitcoin wallet. You can retrieve this object to receive detailed information about any withdrawal request made from your Lightspark account."""
 
     requester: Requester
@@ -49,15 +53,18 @@
     amount: CurrencyAmount
     """The amount of money that should be withdrawn in this request."""
 
     estimated_amount: Optional[CurrencyAmount]
     """If the requested amount is `-1` (i.e. everything), this field may contain an estimate of the amount for the withdrawal."""
 
     amount_withdrawn: Optional[CurrencyAmount]
-    """The actual amount that is withdrawn. It will be set once the request is completed."""
+    """The actual amount that is withdrawn to the bitcoin address. It will be set once the request is completed."""
+
+    total_fees: Optional[CurrencyAmount]
+    """The total fees the node paid for the withdrawal. It will be set once the request is completed."""
 
     bitcoin_address: str
     """The bitcoin address where the funds should be sent."""
 
     withdrawal_mode: WithdrawalMode
     """The strategy that should be used to withdraw the funds from the account."""
 
@@ -68,31 +75,31 @@
     """The time at which this request was completed."""
 
     withdrawal_id: Optional[str]
     """The withdrawal transaction that has been generated by this request."""
     typename: str
 
     def get_channel_closing_transactions(
-        self, first: Optional[int] = None
+        self, first: Optional[int] = None, after: Optional[str] = None
     ) -> WithdrawalRequestToChannelClosingTransactionsConnection:
         json = self.requester.execute_graphql(
             """
-query FetchWithdrawalRequestToChannelClosingTransactionsConnection($entity_id: ID!, $first: Int) {
+query FetchWithdrawalRequestToChannelClosingTransactionsConnection($entity_id: ID!, $first: Int, $after: String) {
     entity(id: $entity_id) {
         ... on WithdrawalRequest {
-            channel_closing_transactions(, first: $first) {
+            channel_closing_transactions(, first: $first, after: $after) {
                 __typename
+                withdrawal_request_to_channel_closing_transactions_connection_count: count
                 withdrawal_request_to_channel_closing_transactions_connection_page_info: page_info {
                     __typename
                     page_info_has_next_page: has_next_page
                     page_info_has_previous_page: has_previous_page
                     page_info_start_cursor: start_cursor
                     page_info_end_cursor: end_cursor
                 }
-                withdrawal_request_to_channel_closing_transactions_connection_count: count
                 withdrawal_request_to_channel_closing_transactions_connection_entities: entities {
                     __typename
                     channel_closing_transaction_id: id
                     channel_closing_transaction_created_at: created_at
                     channel_closing_transaction_updated_at: updated_at
                     channel_closing_transaction_status: status
                     channel_closing_transaction_resolved_at: resolved_at
@@ -122,39 +129,39 @@
                     }
                 }
             }
         }
     }
 }
             """,
-            {"entity_id": self.id, "first": first},
+            {"entity_id": self.id, "first": first, "after": after},
         )
         connection = json["entity"]["channel_closing_transactions"]
         return WithdrawalRequestToChannelClosingTransactionsConnection_from_json(
             self.requester, connection
         )
 
     def get_channel_opening_transactions(
-        self, first: Optional[int] = None
+        self, first: Optional[int] = None, after: Optional[str] = None
     ) -> WithdrawalRequestToChannelOpeningTransactionsConnection:
         json = self.requester.execute_graphql(
             """
-query FetchWithdrawalRequestToChannelOpeningTransactionsConnection($entity_id: ID!, $first: Int) {
+query FetchWithdrawalRequestToChannelOpeningTransactionsConnection($entity_id: ID!, $first: Int, $after: String) {
     entity(id: $entity_id) {
         ... on WithdrawalRequest {
-            channel_opening_transactions(, first: $first) {
+            channel_opening_transactions(, first: $first, after: $after) {
                 __typename
+                withdrawal_request_to_channel_opening_transactions_connection_count: count
                 withdrawal_request_to_channel_opening_transactions_connection_page_info: page_info {
                     __typename
                     page_info_has_next_page: has_next_page
                     page_info_has_previous_page: has_previous_page
                     page_info_start_cursor: start_cursor
                     page_info_end_cursor: end_cursor
                 }
-                withdrawal_request_to_channel_opening_transactions_connection_count: count
                 withdrawal_request_to_channel_opening_transactions_connection_entities: entities {
                     __typename
                     channel_opening_transaction_id: id
                     channel_opening_transaction_created_at: created_at
                     channel_opening_transaction_updated_at: updated_at
                     channel_opening_transaction_status: status
                     channel_opening_transaction_resolved_at: resolved_at
@@ -184,35 +191,93 @@
                     }
                 }
             }
         }
     }
 }
             """,
-            {"entity_id": self.id, "first": first},
+            {"entity_id": self.id, "first": first, "after": after},
         )
         connection = json["entity"]["channel_opening_transactions"]
         return WithdrawalRequestToChannelOpeningTransactionsConnection_from_json(
             self.requester, connection
         )
 
+    def get_withdrawals(
+        self, first: Optional[int] = None
+    ) -> WithdrawalRequestToWithdrawalsConnection:
+        json = self.requester.execute_graphql(
+            """
+query FetchWithdrawalRequestToWithdrawalsConnection($entity_id: ID!, $first: Int) {
+    entity(id: $entity_id) {
+        ... on WithdrawalRequest {
+            withdrawals(, first: $first) {
+                __typename
+                withdrawal_request_to_withdrawals_connection_count: count
+                withdrawal_request_to_withdrawals_connection_entities: entities {
+                    __typename
+                    withdrawal_id: id
+                    withdrawal_created_at: created_at
+                    withdrawal_updated_at: updated_at
+                    withdrawal_status: status
+                    withdrawal_resolved_at: resolved_at
+                    withdrawal_amount: amount {
+                        __typename
+                        currency_amount_original_value: original_value
+                        currency_amount_original_unit: original_unit
+                        currency_amount_preferred_currency_unit: preferred_currency_unit
+                        currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
+                        currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
+                    }
+                    withdrawal_transaction_hash: transaction_hash
+                    withdrawal_fees: fees {
+                        __typename
+                        currency_amount_original_value: original_value
+                        currency_amount_original_unit: original_unit
+                        currency_amount_preferred_currency_unit: preferred_currency_unit
+                        currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
+                        currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
+                    }
+                    withdrawal_block_hash: block_hash
+                    withdrawal_block_height: block_height
+                    withdrawal_destination_addresses: destination_addresses
+                    withdrawal_num_confirmations: num_confirmations
+                    withdrawal_origin: origin {
+                        id
+                    }
+                }
+            }
+        }
+    }
+}
+            """,
+            {"entity_id": self.id, "first": first},
+        )
+        connection = json["entity"]["withdrawals"]
+        return WithdrawalRequestToWithdrawalsConnection_from_json(
+            self.requester, connection
+        )
+
     def to_json(self) -> Mapping[str, Any]:
         return {
             "__typename": "WithdrawalRequest",
             "withdrawal_request_id": self.id,
             "withdrawal_request_created_at": self.created_at.isoformat(),
             "withdrawal_request_updated_at": self.updated_at.isoformat(),
             "withdrawal_request_requested_amount": self.requested_amount.to_json(),
             "withdrawal_request_amount": self.amount.to_json(),
             "withdrawal_request_estimated_amount": self.estimated_amount.to_json()
             if self.estimated_amount
             else None,
             "withdrawal_request_amount_withdrawn": self.amount_withdrawn.to_json()
             if self.amount_withdrawn
             else None,
+            "withdrawal_request_total_fees": self.total_fees.to_json()
+            if self.total_fees
+            else None,
             "withdrawal_request_bitcoin_address": self.bitcoin_address,
             "withdrawal_request_withdrawal_mode": self.withdrawal_mode.value,
             "withdrawal_request_status": self.status.value,
             "withdrawal_request_completed_at": self.completed_at.isoformat()
             if self.completed_at
             else None,
             "withdrawal_request_withdrawal": {"id": self.withdrawal_id}
@@ -255,14 +320,22 @@
         __typename
         currency_amount_original_value: original_value
         currency_amount_original_unit: original_unit
         currency_amount_preferred_currency_unit: preferred_currency_unit
         currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
         currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
     }
+    withdrawal_request_total_fees: total_fees {
+        __typename
+        currency_amount_original_value: original_value
+        currency_amount_original_unit: original_unit
+        currency_amount_preferred_currency_unit: preferred_currency_unit
+        currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
+        currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
+    }
     withdrawal_request_bitcoin_address: bitcoin_address
     withdrawal_request_withdrawal_mode: withdrawal_mode
     withdrawal_request_status: status
     withdrawal_request_completed_at: completed_at
     withdrawal_request_withdrawal: withdrawal {
         id
     }
@@ -287,14 +360,19 @@
         if obj["withdrawal_request_estimated_amount"]
         else None,
         amount_withdrawn=CurrencyAmount_from_json(
             requester, obj["withdrawal_request_amount_withdrawn"]
         )
         if obj["withdrawal_request_amount_withdrawn"]
         else None,
+        total_fees=CurrencyAmount_from_json(
+            requester, obj["withdrawal_request_total_fees"]
+        )
+        if obj["withdrawal_request_total_fees"]
+        else None,
         bitcoin_address=obj["withdrawal_request_bitcoin_address"],
         withdrawal_mode=parse_enum(
             WithdrawalMode, obj["withdrawal_request_withdrawal_mode"]
         ),
         status=parse_enum(WithdrawalRequestStatus, obj["withdrawal_request_status"]),
         completed_at=datetime.fromisoformat(obj["withdrawal_request_completed_at"])
         if obj["withdrawal_request_completed_at"]
```

## Comparing `lightspark-2.6.0/lightspark/objects/RegisterPaymentInput.py` & `lightspark-2.7.0/lightspark/objects/RegisterPaymentInput.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 # Copyright ©, 2022-present, Lightspark Group, Inc. - All Rights Reserved
 
 from dataclasses import dataclass
 from typing import Any, Mapping
 
-from lightspark.objects.ComplianceProvider import ComplianceProvider
-from lightspark.objects.PaymentDirection import PaymentDirection
 from lightspark.utils.enums import parse_enum
 
 from .ComplianceProvider import ComplianceProvider
 from .PaymentDirection import PaymentDirection
 
 
 @dataclass
```

## Comparing `lightspark-2.6.0/lightspark/objects/Hop.py` & `lightspark-2.7.0/lightspark/objects/Hop.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/SendPaymentOutput.py` & `lightspark-2.7.0/lightspark/objects/SendPaymentOutput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/DeclineToSignMessagesOutput.py` & `lightspark-2.7.0/lightspark/objects/DeclineToSignMessagesOutput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/CreateNodeWalletAddressOutput.py` & `lightspark-2.7.0/lightspark/objects/CreateNodeWalletAddressOutput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/GraphNode.py` & `lightspark-2.7.0/lightspark/objects/GraphNode.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Copyright ©, 2022-present, Lightspark Group, Inc. - All Rights Reserved
 
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Any, List, Mapping, Optional
 
-from lightspark.objects.BitcoinNetwork import BitcoinNetwork
 from lightspark.requests.requester import Requester
 from lightspark.utils.enums import parse_enum
 
 from .BitcoinNetwork import BitcoinNetwork
 from .Entity import Entity
 from .Node import Node
 from .NodeAddressType import NodeAddressType
```

## Comparing `lightspark-2.6.0/lightspark/objects/CreateApiTokenOutput.py` & `lightspark-2.7.0/lightspark/objects/CreateApiTokenOutput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/ReleasePaymentPreimageInput.py` & `lightspark-2.7.0/lightspark/objects/ReleasePaymentPreimageInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/TransactionStatus.py` & `lightspark-2.7.0/lightspark/objects/TransactionStatus.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/IncomingPaymentToAttemptsConnection.py` & `lightspark-2.7.0/lightspark/objects/IncomingPaymentToAttemptsConnection.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/RemoteSigningSubEventType.py` & `lightspark-2.7.0/lightspark/objects/RemoteSigningSubEventType.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,7 +14,8 @@
     SIGN_INVOICE = "SIGN_INVOICE"
     DERIVE_KEY_AND_SIGN = "DERIVE_KEY_AND_SIGN"
     RELEASE_PAYMENT_PREIMAGE = "RELEASE_PAYMENT_PREIMAGE"
     REQUEST_INVOICE_PAYMENT_HASH = "REQUEST_INVOICE_PAYMENT_HASH"
     REVEAL_COUNTERPARTY_PER_COMMITMENT_SECRET = (
         "REVEAL_COUNTERPARTY_PER_COMMITMENT_SECRET"
     )
+    VLS_MESSAGE = "VLS_MESSAGE"
```

## Comparing `lightspark-2.6.0/lightspark/objects/PaymentRequest.py` & `lightspark-2.7.0/lightspark/objects/PaymentRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Copyright ©, 2022-present, Lightspark Group, Inc. - All Rights Reserved
 
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Any, Mapping
 
 from lightspark.exceptions import LightsparkException
-from lightspark.objects.PaymentRequestStatus import PaymentRequestStatus
 from lightspark.requests.requester import Requester
 from lightspark.utils.enums import parse_enum
 
 from .CurrencyAmount import from_json as CurrencyAmount_from_json
 from .Entity import Entity
 from .InvoiceData import from_json as InvoiceData_from_json
 from .PaymentRequestData import PaymentRequestData
```

## Comparing `lightspark-2.6.0/lightspark/objects/CreateInvitationWithIncentivesInput.py` & `lightspark-2.7.0/lightspark/objects/CreateInvitationWithIncentivesInput.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # Copyright ©, 2022-present, Lightspark Group, Inc. - All Rights Reserved
 
 from dataclasses import dataclass
 from typing import Any, Mapping
 
-from lightspark.objects.RegionCode import RegionCode
 from lightspark.utils.enums import parse_enum
 
 from .RegionCode import RegionCode
 
 
 @dataclass
 class CreateInvitationWithIncentivesInput:
```

## Comparing `lightspark-2.6.0/lightspark/objects/PayInvoiceOutput.py` & `lightspark-2.7.0/lightspark/objects/PayInvoiceOutput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/PayInvoiceInput.py` & `lightspark-2.7.0/lightspark/objects/PayInvoiceInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/CreateNodeWalletAddressInput.py` & `lightspark-2.7.0/lightspark/objects/CreateNodeWalletAddressInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/OutgoingPayment.py` & `lightspark-2.7.0/lightspark/objects/OutgoingPayment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # Copyright ©, 2022-present, Lightspark Group, Inc. - All Rights Reserved
 
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Any, List, Mapping, Optional
 
-from lightspark.objects.PaymentFailureReason import PaymentFailureReason
-from lightspark.objects.TransactionStatus import TransactionStatus
 from lightspark.requests.requester import Requester
 from lightspark.utils.enums import parse_enum, parse_enum_optional
 
 from .CurrencyAmount import CurrencyAmount
 from .CurrencyAmount import from_json as CurrencyAmount_from_json
 from .Entity import Entity
 from .LightningTransaction import LightningTransaction
```

## Comparing `lightspark-2.6.0/lightspark/objects/AccountToApiTokensConnection.py` & `lightspark-2.7.0/lightspark/objects/AccountToApiTokensConnection.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/IncentivesIneligibilityReason.py` & `lightspark-2.7.0/lightspark/objects/IncentivesIneligibilityReason.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/DailyLiquidityForecast.py` & `lightspark-2.7.0/lightspark/objects/DailyLiquidityForecast.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Copyright ©, 2022-present, Lightspark Group, Inc. - All Rights Reserved
 
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Any, Mapping
 
-from lightspark.objects.LightningPaymentDirection import LightningPaymentDirection
 from lightspark.requests.requester import Requester
 from lightspark.utils.enums import parse_enum
 
 from .CurrencyAmount import CurrencyAmount
 from .CurrencyAmount import from_json as CurrencyAmount_from_json
 from .LightningPaymentDirection import LightningPaymentDirection
```

## Comparing `lightspark-2.6.0/lightspark/objects/FeeEstimate.py` & `lightspark-2.7.0/lightspark/objects/FeeEstimate.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/SignMessagesOutput.py` & `lightspark-2.7.0/lightspark/objects/SignMessagesOutput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/RegisterPaymentOutput.py` & `lightspark-2.7.0/lightspark/objects/RegisterPaymentOutput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/TransactionFailures.py` & `lightspark-2.7.0/lightspark/objects/TransactionFailures.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/AccountToWalletsConnection.py` & `lightspark-2.7.0/lightspark/objects/AccountToWalletsConnection.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/LightningFeeEstimateForInvoiceInput.py` & `lightspark-2.7.0/lightspark/objects/LightningFeeEstimateForInvoiceInput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/NodeAddress.py` & `lightspark-2.7.0/lightspark/objects/NodeAddress.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # Copyright ©, 2022-present, Lightspark Group, Inc. - All Rights Reserved
 
 from dataclasses import dataclass
 from typing import Any, Mapping
 
-from lightspark.objects.NodeAddressType import NodeAddressType
 from lightspark.requests.requester import Requester
 from lightspark.utils.enums import parse_enum
 
 from .NodeAddressType import NodeAddressType
 
 
 @dataclass
```

## Comparing `lightspark-2.6.0/lightspark/objects/Deposit.py` & `lightspark-2.7.0/lightspark/objects/Deposit.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Copyright ©, 2022-present, Lightspark Group, Inc. - All Rights Reserved
 
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Any, List, Mapping, Optional
 
-from lightspark.objects.TransactionStatus import TransactionStatus
 from lightspark.requests.requester import Requester
 from lightspark.utils.enums import parse_enum
 
 from .CurrencyAmount import CurrencyAmount
 from .CurrencyAmount import from_json as CurrencyAmount_from_json
 from .Entity import Entity
 from .OnChainTransaction import OnChainTransaction
@@ -40,15 +39,15 @@
     amount: CurrencyAmount
     """The amount of money involved in this transaction."""
 
     transaction_hash: Optional[str]
     """The hash of this transaction, so it can be uniquely identified on the Lightning Network."""
 
     fees: Optional[CurrencyAmount]
-    """The fees that were paid by the wallet sending the transaction to commit it to the Bitcoin blockchain."""
+    """The fees that were paid by the node for this transaction."""
 
     block_hash: Optional[str]
     """The hash of the block that included this transaction. This will be null for unconfirmed transactions."""
 
     block_height: int
     """The height of the block that included this transaction. This will be zero for unconfirmed transactions."""
```

## Comparing `lightspark-2.6.0/lightspark/objects/OutgoingPaymentAttemptToHopsConnection.py` & `lightspark-2.7.0/lightspark/objects/OutgoingPaymentAttemptToHopsConnection.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/DeleteApiTokenOutput.py` & `lightspark-2.7.0/lightspark/objects/DeleteApiTokenOutput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/PostTransactionData.py` & `lightspark-2.7.0/lightspark/objects/PostTransactionData.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/objects/LightsparkNodeWithOSK.py` & `lightspark-2.7.0/lightspark/objects/LightsparkNodeWithOSK.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # Copyright ©, 2022-present, Lightspark Group, Inc. - All Rights Reserved
 
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Any, List, Mapping, Optional
 
-from lightspark.objects.BitcoinNetwork import BitcoinNetwork
-from lightspark.objects.LightsparkNodeStatus import LightsparkNodeStatus
 from lightspark.requests.requester import Requester
 from lightspark.utils.enums import parse_enum, parse_enum_optional
 
 from .Balances import Balances
 from .Balances import from_json as Balances_from_json
 from .BitcoinNetwork import BitcoinNetwork
 from .BlockchainBalance import BlockchainBalance
@@ -128,23 +126,25 @@
         )
         connection = json["entity"]["addresses"]
         return NodeToAddressesConnection_from_json(self.requester, connection)
 
     def get_channels(
         self,
         first: Optional[int] = None,
-        statuses: Optional[List[ChannelStatus]] = None,
         after: Optional[str] = None,
+        before_date: Optional[datetime] = None,
+        after_date: Optional[datetime] = None,
+        statuses: Optional[List[ChannelStatus]] = None,
     ) -> LightsparkNodeToChannelsConnection:
         json = self.requester.execute_graphql(
             """
-query FetchLightsparkNodeToChannelsConnection($entity_id: ID!, $first: Int, $statuses: [ChannelStatus!], $after: String) {
+query FetchLightsparkNodeToChannelsConnection($entity_id: ID!, $first: Int, $after: String, $before_date: DateTime, $after_date: DateTime, $statuses: [ChannelStatus!]) {
     entity(id: $entity_id) {
         ... on LightsparkNodeWithOSK {
-            channels(, first: $first, statuses: $statuses, after: $after) {
+            channels(, first: $first, after: $after, before_date: $before_date, after_date: $after_date, statuses: $statuses) {
                 __typename
                 lightspark_node_to_channels_connection_count: count
                 lightspark_node_to_channels_connection_page_info: page_info {
                     __typename
                     page_info_has_next_page: has_next_page
                     page_info_has_previous_page: has_previous_page
                     page_info_start_cursor: start_cursor
@@ -248,16 +248,18 @@
         }
     }
 }
             """,
             {
                 "entity_id": self.id,
                 "first": first,
-                "statuses": statuses,
                 "after": after,
+                "before_date": before_date,
+                "after_date": after_date,
+                "statuses": statuses,
             },
         )
         connection = json["entity"]["channels"]
         return LightsparkNodeToChannelsConnection_from_json(self.requester, connection)
 
     def get_daily_liquidity_forecasts(
         self,
```

## Comparing `lightspark-2.6.0/lightspark/objects/CancelInvoiceOutput.py` & `lightspark-2.7.0/lightspark/objects/CancelInvoiceOutput.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/scripts/claim_uma_invitation.py` & `lightspark-2.7.0/lightspark/scripts/claim_uma_invitation.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/scripts/create_uma_invoice.py` & `lightspark-2.7.0/lightspark/scripts/create_uma_invoice.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/scripts/send_payment.py` & `lightspark-2.7.0/lightspark/scripts/send_payment.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/scripts/request_withdrawal.py` & `lightspark-2.7.0/lightspark/scripts/request_withdrawal.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/scripts/outgoing_payments_for_invoice.py` & `lightspark-2.7.0/lightspark/scripts/outgoing_payments_for_invoice.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/scripts/lightning_fee_estimate_for_invoice.py` & `lightspark-2.7.0/lightspark/scripts/lightning_fee_estimate_for_invoice.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/scripts/register_payment.py` & `lightspark-2.7.0/lightspark/scripts/register_payment.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/scripts/create_lnurl_invoice.py` & `lightspark-2.7.0/lightspark/scripts/create_lnurl_invoice.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/scripts/incoming_payments_for_invoice.py` & `lightspark-2.7.0/lightspark/scripts/incoming_payments_for_invoice.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/scripts/create_uma_invitation.py` & `lightspark-2.7.0/lightspark/scripts/create_uma_invitation.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/scripts/create_test_mode_payment.py` & `lightspark-2.7.0/lightspark/scripts/create_test_mode_payment.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/scripts/create_invoice.py` & `lightspark-2.7.0/lightspark/scripts/create_invoice.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/scripts/pay_uma_invoice.py` & `lightspark-2.7.0/lightspark/scripts/pay_uma_invoice.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/scripts/pay_invoice.py` & `lightspark-2.7.0/lightspark/scripts/pay_invoice.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark/scripts/lightning_fee_estimate_for_node.py` & `lightspark-2.7.0/lightspark/scripts/lightning_fee_estimate_for_node.py`

 * *Files identical despite different names*

## Comparing `lightspark-2.6.0/lightspark.egg-info/SOURCES.txt` & `lightspark-2.7.0/lightspark.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -64,14 +64,16 @@
 lightspark/objects/DailyLiquidityForecast.py
 lightspark/objects/DeclineToSignMessagesInput.py
 lightspark/objects/DeclineToSignMessagesOutput.py
 lightspark/objects/DeleteApiTokenInput.py
 lightspark/objects/DeleteApiTokenOutput.py
 lightspark/objects/Deposit.py
 lightspark/objects/Entity.py
+lightspark/objects/FailHtlcsInput.py
+lightspark/objects/FailHtlcsOutput.py
 lightspark/objects/FeeEstimate.py
 lightspark/objects/FundNodeInput.py
 lightspark/objects/FundNodeOutput.py
 lightspark/objects/GraphNode.py
 lightspark/objects/Hop.py
 lightspark/objects/HtlcAttemptFailureCode.py
 lightspark/objects/IdAndSignature.py
@@ -169,14 +171,15 @@
 lightspark/objects/WithdrawalFeeEstimateInput.py
 lightspark/objects/WithdrawalFeeEstimateOutput.py
 lightspark/objects/WithdrawalMode.py
 lightspark/objects/WithdrawalRequest.py
 lightspark/objects/WithdrawalRequestStatus.py
 lightspark/objects/WithdrawalRequestToChannelClosingTransactionsConnection.py
 lightspark/objects/WithdrawalRequestToChannelOpeningTransactionsConnection.py
+lightspark/objects/WithdrawalRequestToWithdrawalsConnection.py
 lightspark/objects/__init__.py
 lightspark/objects/all_entities.py
 lightspark/requests/__init__.py
 lightspark/requests/encoder.py
 lightspark/requests/requester.py
 lightspark/scripts/__init__.py
 lightspark/scripts/bitcoin_fee_estimate.py
@@ -189,20 +192,22 @@
 lightspark/scripts/create_test_mode_invoice.py
 lightspark/scripts/create_test_mode_payment.py
 lightspark/scripts/create_uma_invitation.py
 lightspark/scripts/create_uma_invoice.py
 lightspark/scripts/current_account.py
 lightspark/scripts/decoded_payment_request.py
 lightspark/scripts/delete_api_token.py
+lightspark/scripts/fail_htlcs.py
 lightspark/scripts/fetch_uma_invitation.py
 lightspark/scripts/fund_node.py
 lightspark/scripts/incoming_payments_for_invoice.py
 lightspark/scripts/lightning_fee_estimate_for_invoice.py
 lightspark/scripts/lightning_fee_estimate_for_node.py
 lightspark/scripts/outgoing_payments_for_invoice.py
+lightspark/scripts/outgoing_payments_for_payment_hash.py
 lightspark/scripts/pay_invoice.py
 lightspark/scripts/pay_uma_invoice.py
 lightspark/scripts/recover_node_signing_key.py
 lightspark/scripts/register_payment.py
 lightspark/scripts/request_withdrawal.py
 lightspark/scripts/screen_node.py
 lightspark/scripts/send_payment.py
```

## Comparing `lightspark-2.6.0/lightspark.egg-info/PKG-INFO` & `lightspark-2.7.0/lightspark.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: lightspark
-Version: 2.6.0
+Version: 2.7.0
 Summary: Python SDK for the Lightspark API
 Home-page: https://www.lightspark.com/
 Author: Lightspark Group, Inc.
 Author-email: info@lightspark.com
 License: Apache-2.0
 Project-URL: Documentation, https://docs.lightspark.com/lightspark-sdk/getting-started?language=Python
 Project-URL: Source Code, https://github.com/lightsparkdev/python-sdk
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cryptography
 Requires-Dist: pyjwt
 Requires-Dist: requests
 Requires-Dist: lightspark-crypto-python
+Requires-Dist: zstandard
 
 # Lightspark Python SDK
 
 The Lightspark Python SDK provides a convenient way to interact with the Lightspark services from applications written in the Python language.
 
 ## Installation
```

