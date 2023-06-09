# Comparing `tmp/increase-0.6.0.tar.gz` & `tmp/increase-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "increase-0.6.0.tar", max compression
+gzip compressed data, was "increase-0.6.1.tar", max compression
```

## Comparing `increase-0.6.0.tar` & `increase-0.6.1.tar`

### file list

```diff
@@ -1,205 +1,210 @@
--rw-r--r--   0        0        0    11338 2023-05-31 10:09:43.188289 increase-0.6.0/LICENSE
--rw-r--r--   0        0        0     8443 2023-05-31 10:09:43.188289 increase-0.6.0/README.md
--rw-r--r--   0        0        0     1883 2023-05-31 10:09:43.188289 increase-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     2587 2023-05-31 10:09:43.188289 increase-0.6.0/src/increase/__init__.py
--rw-r--r--   0        0        0    46447 2023-05-31 10:09:43.188289 increase-0.6.0/src/increase/_base_client.py
--rw-r--r--   0        0        0     3889 2023-05-31 10:09:43.188289 increase-0.6.0/src/increase/_base_exceptions.py
--rw-r--r--   0        0        0    26766 2023-05-31 10:09:43.188289 increase-0.6.0/src/increase/_client.py
--rw-r--r--   0        0        0    10875 2023-05-31 10:09:43.188289 increase-0.6.0/src/increase/_exceptions.py
--rw-r--r--   0        0        0     7343 2023-05-31 10:09:43.188289 increase-0.6.0/src/increase/_models.py
--rw-r--r--   0        0        0     4781 2023-05-31 10:09:43.188289 increase-0.6.0/src/increase/_qs.py
--rw-r--r--   0        0        0      890 2023-05-31 10:09:43.188289 increase-0.6.0/src/increase/_resource.py
--rw-r--r--   0        0        0     3979 2023-05-31 10:09:43.188289 increase-0.6.0/src/increase/_types.py
--rw-r--r--   0        0        0     1277 2023-05-31 10:09:43.188289 increase-0.6.0/src/increase/_utils/__init__.py
--rw-r--r--   0        0        0     6710 2023-05-31 10:09:43.188289 increase-0.6.0/src/increase/_utils/_transform.py
--rw-r--r--   0        0        0     9411 2023-05-31 10:09:43.188289 increase-0.6.0/src/increase/_utils/_utils.py
--rw-r--r--   0        0        0      127 2023-05-31 10:09:43.188289 increase-0.6.0/src/increase/_version.py
--rw-r--r--   0        0        0     1109 2023-05-31 10:09:43.188289 increase-0.6.0/src/increase/pagination.py
--rw-r--r--   0        0        0        0 2023-05-31 10:09:43.188289 increase-0.6.0/src/increase/py.typed
--rw-r--r--   0        0        0     4478 2023-05-31 10:09:43.188289 increase-0.6.0/src/increase/resources/__init__.py
--rw-r--r--   0        0        0    14153 2023-05-31 10:09:43.188289 increase-0.6.0/src/increase/resources/account_numbers.py
--rw-r--r--   0        0        0     6612 2023-05-31 10:09:43.188289 increase-0.6.0/src/increase/resources/account_statements.py
--rw-r--r--   0        0        0    15452 2023-05-31 10:09:43.188289 increase-0.6.0/src/increase/resources/account_transfers.py
--rw-r--r--   0        0        0    16078 2023-05-31 10:09:43.188289 increase-0.6.0/src/increase/resources/accounts.py
--rw-r--r--   0        0        0    14804 2023-05-31 10:09:43.188289 increase-0.6.0/src/increase/resources/ach_prenotifications.py
--rw-r--r--   0        0        0    23469 2023-05-31 10:09:43.188289 increase-0.6.0/src/increase/resources/ach_transfers.py
--rw-r--r--   0        0        0     4285 2023-05-31 10:09:43.188289 increase-0.6.0/src/increase/resources/balance_lookups.py
--rw-r--r--   0        0        0     8651 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/bookkeeping_accounts.py
--rw-r--r--   0        0        0     4122 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/bookkeeping_entries.py
--rw-r--r--   0        0        0     4842 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/bookkeeping_entry_sets.py
--rw-r--r--   0        0        0     9963 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/card_disputes.py
--rw-r--r--   0        0        0     9853 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/card_profiles.py
--rw-r--r--   0        0        0    17566 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/cards.py
--rw-r--r--   0        0        0    10985 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/check_deposits.py
--rw-r--r--   0        0        0    19654 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/check_transfers.py
--rw-r--r--   0        0        0     6995 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/declined_transactions.py
--rw-r--r--   0        0        0     6577 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/digital_wallet_tokens.py
--rw-r--r--   0        0        0     6425 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/documents.py
--rw-r--r--   0        0        0      282 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/entities/__init__.py
--rw-r--r--   0        0        0    13266 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/entities/entities.py
--rw-r--r--   0        0        0     3839 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/entities/supplemental_documents.py
--rw-r--r--   0        0        0    17879 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/event_subscriptions.py
--rw-r--r--   0        0        0     6438 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/events.py
--rw-r--r--   0        0        0     9804 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/exports.py
--rw-r--r--   0        0        0    14425 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/external_accounts.py
--rw-r--r--   0        0        0    12069 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/files.py
--rw-r--r--   0        0        0     2040 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/groups.py
--rw-r--r--   0        0        0    11207 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/inbound_ach_transfer_returns.py
--rw-r--r--   0        0        0     6239 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/inbound_wire_drawdown_requests.py
--rw-r--r--   0        0        0    13407 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/limits.py
--rw-r--r--   0        0        0     5833 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/oauth_connections.py
--rw-r--r--   0        0        0     7572 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/pending_transactions.py
--rw-r--r--   0        0        0     5552 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/programs.py
--rw-r--r--   0        0        0     7616 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/real_time_decisions.py
--rw-r--r--   0        0        0    14164 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/real_time_payments_transfers.py
--rw-r--r--   0        0        0     4951 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/routing_numbers.py
--rw-r--r--   0        0        0     1906 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/simulations/__init__.py
--rw-r--r--   0        0        0     4026 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/simulations/account_statements.py
--rw-r--r--   0        0        0     3102 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/simulations/account_transfers.py
--rw-r--r--   0        0        0    16455 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/simulations/ach_transfers.py
--rw-r--r--   0        0        0     4919 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/simulations/card_disputes.py
--rw-r--r--   0        0        0     3967 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/simulations/card_refunds.py
--rw-r--r--   0        0        0    11463 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/simulations/cards.py
--rw-r--r--   0        0        0     7407 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/simulations/check_deposits.py
--rw-r--r--   0        0        0     8993 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/simulations/check_transfers.py
--rw-r--r--   0        0        0     4085 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/simulations/digital_wallet_token_requests.py
--rw-r--r--   0        0        0     3639 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/simulations/documents.py
--rw-r--r--   0        0        0    13466 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/simulations/inbound_wire_drawdown_requests.py
--rw-r--r--   0        0        0     4411 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/simulations/interest_payments.py
--rw-r--r--   0        0        0    11027 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/simulations/real_time_payments_transfers.py
--rw-r--r--   0        0        0     4404 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/simulations/simulations.py
--rw-r--r--   0        0        0    12351 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/simulations/wire_transfers.py
--rw-r--r--   0        0        0     7036 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/transactions.py
--rw-r--r--   0        0        0    12534 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/wire_drawdown_requests.py
--rw-r--r--   0        0        0    23155 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/wire_transfers.py
--rw-r--r--   0        0        0     8739 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/types/__init__.py
--rw-r--r--   0        0        0     1452 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/types/account.py
--rw-r--r--   0        0        0      690 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/types/account_create_params.py
--rw-r--r--   0        0        0     1571 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/types/account_list_params.py
--rw-r--r--   0        0        0     1026 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/types/account_number.py
--rw-r--r--   0        0        0      408 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/types/account_number_create_params.py
--rw-r--r--   0        0        0     1598 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/types/account_number_list_params.py
--rw-r--r--   0        0        0      435 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/types/account_number_update_params.py
--rw-r--r--   0        0        0     1347 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/types/account_statement.py
--rw-r--r--   0        0        0     1534 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/types/account_statement_list_params.py
--rw-r--r--   0        0        0     2648 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/types/account_transfer.py
--rw-r--r--   0        0        0      814 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/types/account_transfer_create_params.py
--rw-r--r--   0        0        0     1494 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/types/account_transfer_list_params.py
--rw-r--r--   0        0        0      271 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/types/account_update_params.py
--rw-r--r--   0        0        0     2152 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/types/ach_prenotification.py
--rw-r--r--   0        0        0     1847 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/ach_prenotification_create_params.py
--rw-r--r--   0        0        0     1391 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/ach_prenotification_list_params.py
--rw-r--r--   0        0        0     6791 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/ach_transfer.py
--rw-r--r--   0        0        0     3388 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/ach_transfer_create_params.py
--rw-r--r--   0        0        0     1592 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/ach_transfer_list_params.py
--rw-r--r--   0        0        0      585 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/balance_lookup_lookup_params.py
--rw-r--r--   0        0        0      780 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/balance_lookup_lookup_response.py
--rw-r--r--   0        0        0      823 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/bookkeeping_account.py
--rw-r--r--   0        0        0      626 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/bookkeeping_account_create_params.py
--rw-r--r--   0        0        0      428 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/bookkeeping_account_list_params.py
--rw-r--r--   0        0        0      698 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/bookkeeping_entry.py
--rw-r--r--   0        0        0      424 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/bookkeeping_entry_list_params.py
--rw-r--r--   0        0        0      895 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/bookkeeping_entry_set.py
--rw-r--r--   0        0        0     1133 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/bookkeeping_entry_set_create_params.py
--rw-r--r--   0        0        0     2342 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/card.py
--rw-r--r--   0        0        0     1767 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/card_create_params.py
--rw-r--r--   0        0        0      907 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/card_details.py
--rw-r--r--   0        0        0     2011 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/card_dispute.py
--rw-r--r--   0        0        0      483 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/card_dispute_create_params.py
--rw-r--r--   0        0        0     1661 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/card_dispute_list_params.py
--rw-r--r--   0        0        0     1451 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/card_list_params.py
--rw-r--r--   0        0        0     2186 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/card_profile.py
--rw-r--r--   0        0        0     1820 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/card_profile_create_params.py
--rw-r--r--   0        0        0      715 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/card_profile_list_params.py
--rw-r--r--   0        0        0     1619 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/card_update_params.py
--rw-r--r--   0        0        0     4861 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/check_deposit.py
--rw-r--r--   0        0        0      748 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/check_deposit_create_params.py
--rw-r--r--   0        0        0     1477 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/check_deposit_list_params.py
--rw-r--r--   0        0        0     6608 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/check_transfer.py
--rw-r--r--   0        0        0     1939 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/check_transfer_create_params.py
--rw-r--r--   0        0        0     1488 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/check_transfer_list_params.py
--rw-r--r--   0        0        0    13910 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/declined_transaction.py
--rw-r--r--   0        0        0     1598 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/declined_transaction_list_params.py
--rw-r--r--   0        0        0      950 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/digital_wallet_token.py
--rw-r--r--   0        0        0     1489 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/digital_wallet_token_list_params.py
--rw-r--r--   0        0        0     2581 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/document.py
--rw-r--r--   0        0        0     3899 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/document_list_params.py
--rw-r--r--   0        0        0      217 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/entities/__init__.py
--rw-r--r--   0        0        0      343 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/entities/supplemental_document_create_params.py
--rw-r--r--   0        0        0    11352 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/entity.py
--rw-r--r--   0        0        0    25685 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/entity_create_params.py
--rw-r--r--   0        0        0     1367 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/entity_list_params.py
--rw-r--r--   0        0        0     2724 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/event.py
--rw-r--r--   0        0        0     4044 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/event_list_params.py
--rw-r--r--   0        0        0     3124 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/event_subscription.py
--rw-r--r--   0        0        0     2526 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/event_subscription_create_params.py
--rw-r--r--   0        0        0      426 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/event_subscription_list_params.py
--rw-r--r--   0        0        0      360 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/event_subscription_update_params.py
--rw-r--r--   0        0        0     1147 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/export.py
--rw-r--r--   0        0        0     2946 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/export_create_params.py
--rw-r--r--   0        0        0      404 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/export_list_params.py
--rw-r--r--   0        0        0     1205 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/external_account.py
--rw-r--r--   0        0        0      706 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/external_account_create_params.py
--rw-r--r--   0        0        0      700 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/external_account_list_params.py
--rw-r--r--   0        0        0      420 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/external_account_update_params.py
--rw-r--r--   0        0        0     1546 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/file.py
--rw-r--r--   0        0        0     1041 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/file_create_params.py
--rw-r--r--   0        0        0     2120 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/file_list_params.py
--rw-r--r--   0        0        0      738 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/group.py
--rw-r--r--   0        0        0     1693 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/inbound_ach_transfer_return.py
--rw-r--r--   0        0        0     1109 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/inbound_ach_transfer_return_create_params.py
--rw-r--r--   0        0        0      440 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/inbound_ach_transfer_return_list_params.py
--rw-r--r--   0        0        0     2916 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/inbound_wire_drawdown_request.py
--rw-r--r--   0        0        0      444 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/inbound_wire_drawdown_request_list_params.py
--rw-r--r--   0        0        0     1041 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/limit.py
--rw-r--r--   0        0        0      696 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/limit_create_params.py
--rw-r--r--   0        0        0      527 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/limit_list_params.py
--rw-r--r--   0        0        0      332 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/limit_update_params.py
--rw-r--r--   0        0        0      779 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/oauth_connection.py
--rw-r--r--   0        0        0      422 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/oauth_connection_list_params.py
--rw-r--r--   0        0        0    13613 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/pending_transaction.py
--rw-r--r--   0        0        0     1955 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/pending_transaction_list_params.py
--rw-r--r--   0        0        0      735 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/program.py
--rw-r--r--   0        0        0      406 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/program_list_params.py
--rw-r--r--   0        0        0     6113 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/real_time_decision.py
--rw-r--r--   0        0        0     2451 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/real_time_decision_action_params.py
--rw-r--r--   0        0        0     5096 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/real_time_payments_transfer.py
--rw-r--r--   0        0        0     1283 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/real_time_payments_transfer_create_params.py
--rw-r--r--   0        0        0     1664 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/real_time_payments_transfer_list_params.py
--rw-r--r--   0        0        0      895 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/routing_number.py
--rw-r--r--   0        0        0      522 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/routing_number_list_params.py
--rw-r--r--   0        0        0      155 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/shared/__init__.py
--rw-r--r--   0        0        0      489 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/shared/point_of_service_entry_mode.py
--rw-r--r--   0        0        0      155 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/shared_params/__init__.py
--rw-r--r--   0        0        0      525 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/shared_params/point_of_service_entry_mode.py
--rw-r--r--   0        0        0     2530 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/simulations/__init__.py
--rw-r--r--   0        0        0      338 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/simulations/account_statement_create_params.py
--rw-r--r--   0        0        0     1027 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/simulations/ach_transfer_create_inbound_params.py
--rw-r--r--   0        0        0     1317 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/simulations/ach_transfer_return_params.py
--rw-r--r--   0        0        0    54696 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/simulations/ach_transfer_simulation.py
--rw-r--r--   0        0        0    29427 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/simulations/card_authorization_simulation.py
--rw-r--r--   0        0        0      823 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/simulations/card_authorize_params.py
--rw-r--r--   0        0        0      443 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/simulations/card_dispute_action_params.py
--rw-r--r--   0        0        0      400 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/simulations/card_refund_create_params.py
--rw-r--r--   0        0        0      610 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/simulations/card_settlement_params.py
--rw-r--r--   0        0        0      425 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/simulations/check_transfer_return_params.py
--rw-r--r--   0        0        0      346 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/simulations/digital_wallet_token_request_create_params.py
--rw-r--r--   0        0        0      953 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/simulations/digital_wallet_token_request_create_response.py
--rw-r--r--   0        0        0      325 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/simulations/document_create_params.py
--rw-r--r--   0        0        0    54867 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/simulations/inbound_real_time_payments_transfer_simulation_result.py
--rw-r--r--   0        0        0     2648 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/simulations/inbound_wire_drawdown_request_create_params.py
--rw-r--r--   0        0        0      435 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/simulations/interest_payment_create_params.py
--rw-r--r--   0        0        0    40063 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/simulations/interest_payment_simulation_result.py
--rw-r--r--   0        0        0     1362 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/simulations/real_time_payments_transfer_complete_params.py
--rw-r--r--   0        0        0     1020 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/simulations/real_time_payments_transfer_create_inbound_params.py
--rw-r--r--   0        0        0     2591 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/simulations/wire_transfer_create_inbound_params.py
--rw-r--r--   0        0        0    40107 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/simulations/wire_transfer_simulation.py
--rw-r--r--   0        0        0    38323 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/transaction.py
--rw-r--r--   0        0        0     3652 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/transaction_list_params.py
--rw-r--r--   0        0        0     2239 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/wire_drawdown_request.py
--rw-r--r--   0        0        0     1148 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/wire_drawdown_request_create_params.py
--rw-r--r--   0        0        0      430 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/wire_drawdown_request_list_params.py
--rw-r--r--   0        0        0     5343 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/wire_transfer.py
--rw-r--r--   0        0        0     1367 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/wire_transfer_create_params.py
--rw-r--r--   0        0        0     1588 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/wire_transfer_list_params.py
--rw-r--r--   0        0        0     9346 1970-01-01 00:00:00.000000 increase-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    11338 2023-06-09 14:49:47.009392 increase-0.6.1/LICENSE
+-rw-r--r--   0        0        0     8443 2023-06-09 14:49:47.009392 increase-0.6.1/README.md
+-rw-r--r--   0        0        0     1883 2023-06-09 14:49:47.013392 increase-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     2587 2023-06-09 14:49:47.013392 increase-0.6.1/src/increase/__init__.py
+-rw-r--r--   0        0        0    45082 2023-06-09 14:49:47.013392 increase-0.6.1/src/increase/_base_client.py
+-rw-r--r--   0        0        0     3889 2023-06-09 14:49:47.013392 increase-0.6.1/src/increase/_base_exceptions.py
+-rw-r--r--   0        0        0    26762 2023-06-09 14:49:47.013392 increase-0.6.1/src/increase/_client.py
+-rw-r--r--   0        0        0    10875 2023-06-09 14:49:47.013392 increase-0.6.1/src/increase/_exceptions.py
+-rw-r--r--   0        0        0     7343 2023-06-09 14:49:47.013392 increase-0.6.1/src/increase/_models.py
+-rw-r--r--   0        0        0     4781 2023-06-09 14:49:47.013392 increase-0.6.1/src/increase/_qs.py
+-rw-r--r--   0        0        0      890 2023-06-09 14:49:47.013392 increase-0.6.1/src/increase/_resource.py
+-rw-r--r--   0        0        0     5884 2023-06-09 14:49:47.013392 increase-0.6.1/src/increase/_streaming.py
+-rw-r--r--   0        0        0     4229 2023-06-09 14:49:47.013392 increase-0.6.1/src/increase/_types.py
+-rw-r--r--   0        0        0     1277 2023-06-09 14:49:47.013392 increase-0.6.1/src/increase/_utils/__init__.py
+-rw-r--r--   0        0        0     6710 2023-06-09 14:49:47.013392 increase-0.6.1/src/increase/_utils/_transform.py
+-rw-r--r--   0        0        0     9411 2023-06-09 14:49:47.013392 increase-0.6.1/src/increase/_utils/_utils.py
+-rw-r--r--   0        0        0      127 2023-06-09 14:49:47.013392 increase-0.6.1/src/increase/_version.py
+-rw-r--r--   0        0        0     1109 2023-06-09 14:49:47.013392 increase-0.6.1/src/increase/pagination.py
+-rw-r--r--   0        0        0        0 2023-06-09 14:49:47.013392 increase-0.6.1/src/increase/py.typed
+-rw-r--r--   0        0        0     4478 2023-06-09 14:49:47.013392 increase-0.6.1/src/increase/resources/__init__.py
+-rw-r--r--   0        0        0    15065 2023-06-09 14:49:47.013392 increase-0.6.1/src/increase/resources/account_numbers.py
+-rw-r--r--   0        0        0     7400 2023-06-09 14:49:47.013392 increase-0.6.1/src/increase/resources/account_statements.py
+-rw-r--r--   0        0        0    18102 2023-06-09 14:49:47.013392 increase-0.6.1/src/increase/resources/account_transfers.py
+-rw-r--r--   0        0        0    18476 2023-06-09 14:49:47.013392 increase-0.6.1/src/increase/resources/accounts.py
+-rw-r--r--   0        0        0    15600 2023-06-09 14:49:47.013392 increase-0.6.1/src/increase/resources/ach_prenotifications.py
+-rw-r--r--   0        0        0    26071 2023-06-09 14:49:47.013392 increase-0.6.1/src/increase/resources/ach_transfers.py
+-rw-r--r--   0        0        0     4285 2023-06-09 14:49:47.013392 increase-0.6.1/src/increase/resources/balance_lookups.py
+-rw-r--r--   0        0        0     8651 2023-06-09 14:49:47.013392 increase-0.6.1/src/increase/resources/bookkeeping_accounts.py
+-rw-r--r--   0        0        0     4122 2023-06-09 14:49:47.013392 increase-0.6.1/src/increase/resources/bookkeeping_entries.py
+-rw-r--r--   0        0        0     4842 2023-06-09 14:49:47.013392 increase-0.6.1/src/increase/resources/bookkeeping_entry_sets.py
+-rw-r--r--   0        0        0    10707 2023-06-09 14:49:47.013392 increase-0.6.1/src/increase/resources/card_disputes.py
+-rw-r--r--   0        0        0    10597 2023-06-09 14:49:47.013392 increase-0.6.1/src/increase/resources/card_profiles.py
+-rw-r--r--   0        0        0    19120 2023-06-09 14:49:47.013392 increase-0.6.1/src/increase/resources/cards.py
+-rw-r--r--   0        0        0    11757 2023-06-09 14:49:47.013392 increase-0.6.1/src/increase/resources/check_deposits.py
+-rw-r--r--   0        0        0    23188 2023-06-09 14:49:47.013392 increase-0.6.1/src/increase/resources/check_transfers.py
+-rw-r--r--   0        0        0     7771 2023-06-09 14:49:47.013392 increase-0.6.1/src/increase/resources/declined_transactions.py
+-rw-r--r--   0        0        0     7353 2023-06-09 14:49:47.013392 increase-0.6.1/src/increase/resources/digital_wallet_tokens.py
+-rw-r--r--   0        0        0     7177 2023-06-09 14:49:47.013392 increase-0.6.1/src/increase/resources/documents.py
+-rw-r--r--   0        0        0      282 2023-06-09 14:49:47.013392 increase-0.6.1/src/increase/resources/entities/__init__.py
+-rw-r--r--   0        0        0    14010 2023-06-09 14:49:47.013392 increase-0.6.1/src/increase/resources/entities/entities.py
+-rw-r--r--   0        0        0     8071 2023-06-09 14:49:47.013392 increase-0.6.1/src/increase/resources/entities/supplemental_documents.py
+-rw-r--r--   0        0        0    18799 2023-06-09 14:49:47.013392 increase-0.6.1/src/increase/resources/event_subscriptions.py
+-rw-r--r--   0        0        0     7154 2023-06-09 14:49:47.013392 increase-0.6.1/src/increase/resources/events.py
+-rw-r--r--   0        0        0    10548 2023-06-09 14:49:47.013392 increase-0.6.1/src/increase/resources/exports.py
+-rw-r--r--   0        0        0    15315 2023-06-09 14:49:47.013392 increase-0.6.1/src/increase/resources/external_accounts.py
+-rw-r--r--   0        0        0    12781 2023-06-09 14:49:47.013392 increase-0.6.1/src/increase/resources/files.py
+-rw-r--r--   0        0        0     2040 2023-06-09 14:49:47.013392 increase-0.6.1/src/increase/resources/groups.py
+-rw-r--r--   0        0        0    12035 2023-06-09 14:49:47.013392 increase-0.6.1/src/increase/resources/inbound_ach_transfer_returns.py
+-rw-r--r--   0        0        0     7075 2023-06-09 14:49:47.013392 increase-0.6.1/src/increase/resources/inbound_wire_drawdown_requests.py
+-rw-r--r--   0        0        0    14231 2023-06-09 14:49:47.013392 increase-0.6.1/src/increase/resources/limits.py
+-rw-r--r--   0        0        0     6593 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/resources/oauth_connections.py
+-rw-r--r--   0        0        0     8344 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/resources/pending_transactions.py
+-rw-r--r--   0        0        0     6300 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/resources/programs.py
+-rw-r--r--   0        0        0     8536 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/resources/real_time_decisions.py
+-rw-r--r--   0        0        0    14968 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/resources/real_time_payments_transfers.py
+-rw-r--r--   0        0        0     4951 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/resources/routing_numbers.py
+-rw-r--r--   0        0        0     1989 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/resources/simulations/__init__.py
+-rw-r--r--   0        0        0     4026 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/resources/simulations/account_statements.py
+-rw-r--r--   0        0        0     4024 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/resources/simulations/account_transfers.py
+-rw-r--r--   0        0        0    21877 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/resources/simulations/ach_transfers.py
+-rw-r--r--   0        0        0     5051 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/resources/simulations/card_disputes.py
+-rw-r--r--   0        0        0     3967 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/resources/simulations/card_refunds.py
+-rw-r--r--   0        0        0    11463 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/resources/simulations/cards.py
+-rw-r--r--   0        0        0    10125 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/resources/simulations/check_deposits.py
+-rw-r--r--   0        0        0    11013 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/resources/simulations/check_transfers.py
+-rw-r--r--   0        0        0     4085 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/resources/simulations/digital_wallet_token_requests.py
+-rw-r--r--   0        0        0     3639 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/resources/simulations/documents.py
+-rw-r--r--   0        0        0    13466 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/resources/simulations/inbound_wire_drawdown_requests.py
+-rw-r--r--   0        0        0     4411 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/resources/simulations/interest_payments.py
+-rw-r--r--   0        0        0     3919 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/resources/simulations/programs.py
+-rw-r--r--   0        0        0    11257 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/resources/simulations/real_time_payments_transfers.py
+-rw-r--r--   0        0        0     4588 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/resources/simulations/simulations.py
+-rw-r--r--   0        0        0    12351 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/resources/simulations/wire_transfers.py
+-rw-r--r--   0        0        0     7800 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/resources/transactions.py
+-rw-r--r--   0        0        0    13338 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/resources/wire_drawdown_requests.py
+-rw-r--r--   0        0        0    27583 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/resources/wire_transfers.py
+-rw-r--r--   0        0        0     8739 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/types/__init__.py
+-rw-r--r--   0        0        0     1666 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/types/account.py
+-rw-r--r--   0        0        0      747 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/types/account_create_params.py
+-rw-r--r--   0        0        0     1693 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/types/account_list_params.py
+-rw-r--r--   0        0        0     1026 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/types/account_number.py
+-rw-r--r--   0        0        0      408 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/types/account_number_create_params.py
+-rw-r--r--   0        0        0     1598 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/types/account_number_list_params.py
+-rw-r--r--   0        0        0      435 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/types/account_number_update_params.py
+-rw-r--r--   0        0        0     1347 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/types/account_statement.py
+-rw-r--r--   0        0        0     1534 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/types/account_statement_list_params.py
+-rw-r--r--   0        0        0     2648 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/types/account_transfer.py
+-rw-r--r--   0        0        0      814 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/types/account_transfer_create_params.py
+-rw-r--r--   0        0        0     1494 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/types/account_transfer_list_params.py
+-rw-r--r--   0        0        0      271 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/types/account_update_params.py
+-rw-r--r--   0        0        0     2152 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/types/ach_prenotification.py
+-rw-r--r--   0        0        0     1847 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/types/ach_prenotification_create_params.py
+-rw-r--r--   0        0        0     1391 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/types/ach_prenotification_list_params.py
+-rw-r--r--   0        0        0     8881 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/types/ach_transfer.py
+-rw-r--r--   0        0        0     3388 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/types/ach_transfer_create_params.py
+-rw-r--r--   0        0        0     1592 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/types/ach_transfer_list_params.py
+-rw-r--r--   0        0        0      585 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/types/balance_lookup_lookup_params.py
+-rw-r--r--   0        0        0      780 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/types/balance_lookup_lookup_response.py
+-rw-r--r--   0        0        0      823 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/types/bookkeeping_account.py
+-rw-r--r--   0        0        0      626 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/types/bookkeeping_account_create_params.py
+-rw-r--r--   0        0        0      428 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/types/bookkeeping_account_list_params.py
+-rw-r--r--   0        0        0      698 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/types/bookkeeping_entry.py
+-rw-r--r--   0        0        0      424 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/types/bookkeeping_entry_list_params.py
+-rw-r--r--   0        0        0      895 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/types/bookkeeping_entry_set.py
+-rw-r--r--   0        0        0     1133 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/types/bookkeeping_entry_set_create_params.py
+-rw-r--r--   0        0        0     2342 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/types/card.py
+-rw-r--r--   0        0        0     1767 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/types/card_create_params.py
+-rw-r--r--   0        0        0      907 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/types/card_details.py
+-rw-r--r--   0        0        0     2011 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/types/card_dispute.py
+-rw-r--r--   0        0        0      483 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/types/card_dispute_create_params.py
+-rw-r--r--   0        0        0     1661 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/types/card_dispute_list_params.py
+-rw-r--r--   0        0        0     1451 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/types/card_list_params.py
+-rw-r--r--   0        0        0     2186 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/types/card_profile.py
+-rw-r--r--   0        0        0     1820 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/types/card_profile_create_params.py
+-rw-r--r--   0        0        0      716 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/types/card_profile_list_params.py
+-rw-r--r--   0        0        0     1619 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/types/card_update_params.py
+-rw-r--r--   0        0        0     4861 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/types/check_deposit.py
+-rw-r--r--   0        0        0      748 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/types/check_deposit_create_params.py
+-rw-r--r--   0        0        0     1477 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/types/check_deposit_list_params.py
+-rw-r--r--   0        0        0     6608 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/types/check_transfer.py
+-rw-r--r--   0        0        0     1939 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/types/check_transfer_create_params.py
+-rw-r--r--   0        0        0     1488 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/types/check_transfer_list_params.py
+-rw-r--r--   0        0        0    13934 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/types/declined_transaction.py
+-rw-r--r--   0        0        0     1598 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/types/declined_transaction_list_params.py
+-rw-r--r--   0        0        0      950 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/types/digital_wallet_token.py
+-rw-r--r--   0        0        0     1489 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/types/digital_wallet_token_list_params.py
+-rw-r--r--   0        0        0     2581 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/types/document.py
+-rw-r--r--   0        0        0     3900 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/types/document_list_params.py
+-rw-r--r--   0        0        0      418 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/types/entities/__init__.py
+-rw-r--r--   0        0        0      634 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/types/entities/supplemental_document.py
+-rw-r--r--   0        0        0      343 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/types/entities/supplemental_document_create_params.py
+-rw-r--r--   0        0        0      547 2023-06-09 14:49:47.017392 increase-0.6.1/src/increase/types/entities/supplemental_document_list_params.py
+-rw-r--r--   0        0        0    11893 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/entity.py
+-rw-r--r--   0        0        0    25685 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/entity_create_params.py
+-rw-r--r--   0        0        0     1367 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/entity_list_params.py
+-rw-r--r--   0        0        0     2724 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/event.py
+-rw-r--r--   0        0        0     4044 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/event_list_params.py
+-rw-r--r--   0        0        0     3124 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/event_subscription.py
+-rw-r--r--   0        0        0     2526 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/event_subscription_create_params.py
+-rw-r--r--   0        0        0      426 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/event_subscription_list_params.py
+-rw-r--r--   0        0        0      360 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/event_subscription_update_params.py
+-rw-r--r--   0        0        0     1147 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/export.py
+-rw-r--r--   0        0        0     2946 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/export_create_params.py
+-rw-r--r--   0        0        0      404 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/export_list_params.py
+-rw-r--r--   0        0        0     1205 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/external_account.py
+-rw-r--r--   0        0        0      706 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/external_account_create_params.py
+-rw-r--r--   0        0        0      701 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/external_account_list_params.py
+-rw-r--r--   0        0        0      420 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/external_account_update_params.py
+-rw-r--r--   0        0        0     1546 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/file.py
+-rw-r--r--   0        0        0     1041 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/file_create_params.py
+-rw-r--r--   0        0        0     2120 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/file_list_params.py
+-rw-r--r--   0        0        0      738 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/group.py
+-rw-r--r--   0        0        0     1693 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/inbound_ach_transfer_return.py
+-rw-r--r--   0        0        0     1109 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/inbound_ach_transfer_return_create_params.py
+-rw-r--r--   0        0        0      440 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/inbound_ach_transfer_return_list_params.py
+-rw-r--r--   0        0        0     2916 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/inbound_wire_drawdown_request.py
+-rw-r--r--   0        0        0      444 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/inbound_wire_drawdown_request_list_params.py
+-rw-r--r--   0        0        0     1041 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/limit.py
+-rw-r--r--   0        0        0      696 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/limit_create_params.py
+-rw-r--r--   0        0        0      527 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/limit_list_params.py
+-rw-r--r--   0        0        0      332 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/limit_update_params.py
+-rw-r--r--   0        0        0      779 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/oauth_connection.py
+-rw-r--r--   0        0        0      422 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/oauth_connection_list_params.py
+-rw-r--r--   0        0        0    13613 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/pending_transaction.py
+-rw-r--r--   0        0        0     1956 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/pending_transaction_list_params.py
+-rw-r--r--   0        0        0      735 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/program.py
+-rw-r--r--   0        0        0      406 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/program_list_params.py
+-rw-r--r--   0        0        0     6113 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/real_time_decision.py
+-rw-r--r--   0        0        0     2451 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/real_time_decision_action_params.py
+-rw-r--r--   0        0        0     5096 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/real_time_payments_transfer.py
+-rw-r--r--   0        0        0     1283 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/real_time_payments_transfer_create_params.py
+-rw-r--r--   0        0        0     1664 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/real_time_payments_transfer_list_params.py
+-rw-r--r--   0        0        0      895 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/routing_number.py
+-rw-r--r--   0        0        0      522 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/routing_number_list_params.py
+-rw-r--r--   0        0        0      155 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/shared/__init__.py
+-rw-r--r--   0        0        0      489 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/shared/point_of_service_entry_mode.py
+-rw-r--r--   0        0        0      155 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/shared_params/__init__.py
+-rw-r--r--   0        0        0      525 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/shared_params/point_of_service_entry_mode.py
+-rw-r--r--   0        0        0     2608 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/simulations/__init__.py
+-rw-r--r--   0        0        0      338 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/simulations/account_statement_create_params.py
+-rw-r--r--   0        0        0     1027 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/simulations/ach_transfer_create_inbound_params.py
+-rw-r--r--   0        0        0     3302 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/simulations/ach_transfer_return_params.py
+-rw-r--r--   0        0        0    56837 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/simulations/ach_transfer_simulation.py
+-rw-r--r--   0        0        0    29451 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/simulations/card_authorization_simulation.py
+-rw-r--r--   0        0        0      823 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/simulations/card_authorize_params.py
+-rw-r--r--   0        0        0      443 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/simulations/card_dispute_action_params.py
+-rw-r--r--   0        0        0      400 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/simulations/card_refund_create_params.py
+-rw-r--r--   0        0        0      610 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/simulations/card_settlement_params.py
+-rw-r--r--   0        0        0      425 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/simulations/check_transfer_return_params.py
+-rw-r--r--   0        0        0      346 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/simulations/digital_wallet_token_request_create_params.py
+-rw-r--r--   0        0        0      953 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/simulations/digital_wallet_token_request_create_response.py
+-rw-r--r--   0        0        0      325 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/simulations/document_create_params.py
+-rw-r--r--   0        0        0    57008 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/simulations/inbound_real_time_payments_transfer_simulation_result.py
+-rw-r--r--   0        0        0     2648 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/simulations/inbound_wire_drawdown_request_create_params.py
+-rw-r--r--   0        0        0      435 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/simulations/interest_payment_create_params.py
+-rw-r--r--   0        0        0    42180 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/simulations/interest_payment_simulation_result.py
+-rw-r--r--   0        0        0      299 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/simulations/program_create_params.py
+-rw-r--r--   0        0        0     1362 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/simulations/real_time_payments_transfer_complete_params.py
+-rw-r--r--   0        0        0     1020 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/simulations/real_time_payments_transfer_create_inbound_params.py
+-rw-r--r--   0        0        0     2591 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/simulations/wire_transfer_create_inbound_params.py
+-rw-r--r--   0        0        0    42224 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/simulations/wire_transfer_simulation.py
+-rw-r--r--   0        0        0    40440 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/transaction.py
+-rw-r--r--   0        0        0     3652 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/transaction_list_params.py
+-rw-r--r--   0        0        0     2239 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/wire_drawdown_request.py
+-rw-r--r--   0        0        0     1148 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/wire_drawdown_request_create_params.py
+-rw-r--r--   0        0        0      430 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/wire_drawdown_request_list_params.py
+-rw-r--r--   0        0        0     5343 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/wire_transfer.py
+-rw-r--r--   0        0        0     1367 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/wire_transfer_create_params.py
+-rw-r--r--   0        0        0     1588 2023-06-09 14:49:47.021392 increase-0.6.1/src/increase/types/wire_transfer_list_params.py
+-rw-r--r--   0        0        0     9346 1970-01-01 00:00:00.000000 increase-0.6.1/PKG-INFO
```

### Comparing `increase-0.6.0/LICENSE` & `increase-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/README.md` & `increase-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/pyproject.toml` & `increase-0.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "increase"
-version = "0.6.0"
+version = "0.6.1"
 description = "Client library for the increase API"
 readme = "README.md"
 authors = ["Increase <dev-feedback@increase.com>"]
 license = "Apache-2.0"
 repository = "https://github.com/increase/increase-python"
 packages = [
   { include = "increase", from = "src" }
```

### Comparing `increase-0.6.0/src/increase/__init__.py` & `increase-0.6.1/src/increase/__init__.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/_base_client.py` & `increase-0.6.1/src/increase/_base_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import uuid
 import inspect
 import platform
 from random import random
 from typing import (
     Any,
     Dict,
-    List,
     Type,
     Union,
     Generic,
     Mapping,
     TypeVar,
     Iterable,
     Iterator,
@@ -41,14 +40,15 @@
     Omit,
     Query,
     ModelT,
     Headers,
     Timeout,
     NoneType,
     NotGiven,
+    ResponseT,
     Transport,
     AnyMapping,
     ProxiesTypes,
     RequestFiles,
     RequestOptions,
     UnknownResponse,
     ModelBuilderProtocol,
@@ -57,148 +57,44 @@
 from ._models import (
     BaseModel,
     GenericModel,
     FinalRequestOptions,
     validate_type,
     construct_type,
 )
+from ._streaming import Stream, AsyncStream
 from ._base_exceptions import (
     APIStatusError,
     APITimeoutError,
     APIConnectionError,
     APIResponseValidationError,
 )
 
 # TODO: make base page type vars covariant
 SyncPageT = TypeVar("SyncPageT", bound="BaseSyncPage[Any]")
 AsyncPageT = TypeVar("AsyncPageT", bound="BaseAsyncPage[Any]")
 
 
-ResponseT = TypeVar(
-    "ResponseT",
-    bound=Union[
-        str,
-        None,
-        BaseModel,
-        List[Any],
-        Dict[str, Any],
-        httpx.Response,
-        UnknownResponse,
-        ModelBuilderProtocol,
-    ],
-)
-
 _T = TypeVar("_T")
 _T_co = TypeVar("_T_co", covariant=True)
 
+_StreamT = TypeVar("_StreamT", bound=Stream[Any])
+_AsyncStreamT = TypeVar("_AsyncStreamT", bound=AsyncStream[Any])
+
+
 DEFAULT_TIMEOUT = Timeout(timeout=60.0, connect=5.0)
 DEFAULT_MAX_RETRIES = 2
 DEFAULT_LIMITS = Limits(max_connections=100, max_keepalive_connections=20)
 
 
-class StopStreaming(Exception):
-    """Raised internally when processing of a streamed response should be stopped."""
-
-
-class Stream(Generic[ResponseT]):
-    response: httpx.Response
-
-    def __init__(
-        self,
-        *,
-        cast_to: type[ResponseT],
-        response: httpx.Response,
-        client: SyncAPIClient,
-    ) -> None:
-        self.response = response
-        self._cast_to = cast_to
-        self._client = client
-        self._iterator = self.__iter()
-
-    def __next__(self) -> ResponseT:
-        return self._iterator.__next__()
-
-    def __iter__(self) -> Iterator[ResponseT]:
-        for item in self._iterator:
-            yield item
-
-    def __iter(self) -> Iterator[ResponseT]:
-        cast_to = self._cast_to
-        response = self.response
-        process_line = self._client._process_stream_line
-        process_data = self._client._process_response_data
-
-        awaiting_ping_data = False
-        for raw_line in response.iter_lines():
-            if not raw_line or raw_line == "\n":
-                continue
-
-            if raw_line.startswith("event: ping"):
-                awaiting_ping_data = True
-                continue
-            if awaiting_ping_data:
-                awaiting_ping_data = False
-                continue
-
-            try:
-                line = process_line(raw_line)
-            except StopStreaming:
-                # we are done!
-                break
-
-            yield process_data(data=json.loads(line), cast_to=cast_to, response=response)
-
-
-class AsyncStream(Generic[ResponseT]):
-    response: httpx.Response
-
-    def __init__(
-        self,
-        *,
-        cast_to: type[ResponseT],
-        response: httpx.Response,
-        client: AsyncAPIClient,
-    ) -> None:
-        self.response = response
-        self._cast_to = cast_to
-        self._client = client
-        self._iterator = self.__iter()
-
-    async def __anext__(self) -> ResponseT:
-        return await self._iterator.__anext__()
-
-    async def __aiter__(self) -> AsyncIterator[ResponseT]:
-        async for item in self._iterator:
-            yield item
-
-    async def __iter(self) -> AsyncIterator[ResponseT]:
-        cast_to = self._cast_to
-        response = self.response
-        process_line = self._client._process_stream_line
-        process_data = self._client._process_response_data
-
-        awaiting_ping_data = False
-        async for raw_line in response.aiter_lines():
-            if not raw_line or raw_line == "\n":
-                continue
-
-            if raw_line.startswith("event: ping"):
-                awaiting_ping_data = True
-                continue
-            if awaiting_ping_data:
-                awaiting_ping_data = False
-                continue
-
-            try:
-                line = process_line(raw_line)
-            except StopStreaming:
-                # we are done!
-                break
-
-            yield process_data(data=json.loads(line), cast_to=cast_to, response=response)
+class MissingStreamClassError(TypeError):
+    def __init__(self) -> None:
+        super().__init__(
+            "The `stream` argument was set to `True` but the `stream_cls` argument was not given. See `increase._streaming` for reference",
+        )
 
 
 class PageInfo:
     """Stores the necesary information to build the request to retrieve the next page.
 
     Either `url` or `params` must be set.
     """
@@ -631,24 +527,14 @@
             return cast(ResponseT, cast_to.build(response=response, data=data))
 
         if self._strict_response_validation:
             return cast(ResponseT, validate_type(type_=cast_to, value=data))
 
         return cast(ResponseT, construct_type(type_=cast_to, value=data))
 
-    def _process_stream_line(self, contents: str) -> str:
-        """Pre-process an indiviudal line from a streaming response"""
-        if contents.startswith("data: [DONE]"):
-            raise StopStreaming()
-
-        if contents.startswith("data: "):
-            return contents[6:]
-
-        return contents
-
     @property
     def qs(self) -> Querystring:
         return Querystring()
 
     @property
     def custom_auth(self) -> httpx.Auth | None:
         return None
@@ -752,14 +638,15 @@
 
     def _idempotency_key(self) -> str:
         return f"stainless-python-retry-{uuid.uuid4()}"
 
 
 class SyncAPIClient(BaseClient):
     _client: httpx.Client
+    _default_stream_cls: type[Stream[Any]] | None = None
 
     def __init__(
         self,
         *,
         version: str,
         base_url: str,
         max_retries: int = DEFAULT_MAX_RETRIES,
@@ -794,15 +681,16 @@
     def request(
         self,
         cast_to: Type[ResponseT],
         options: FinalRequestOptions,
         remaining_retries: Optional[int] = None,
         *,
         stream: Literal[True],
-    ) -> Stream[ResponseT]:
+        stream_cls: Type[_StreamT],
+    ) -> _StreamT:
         ...
 
     @overload
     def request(
         self,
         cast_to: Type[ResponseT],
         options: FinalRequestOptions,
@@ -816,65 +704,79 @@
     def request(
         self,
         cast_to: Type[ResponseT],
         options: FinalRequestOptions,
         remaining_retries: Optional[int] = None,
         *,
         stream: bool = False,
-    ) -> ResponseT | Stream[ResponseT]:
+        stream_cls: Type[_StreamT] | None = None,
+    ) -> ResponseT | _StreamT:
         ...
 
     def request(
         self,
         cast_to: Type[ResponseT],
         options: FinalRequestOptions,
         remaining_retries: Optional[int] = None,
         *,
         stream: bool = False,
-    ) -> ResponseT | Stream[ResponseT]:
+        stream_cls: type[_StreamT] | None = None,
+    ) -> ResponseT | _StreamT:
         return self._request(
             cast_to=cast_to,
             options=options,
             stream=stream,
+            stream_cls=stream_cls,
             remaining_retries=remaining_retries,
         )
 
     def _request(
         self,
         *,
         cast_to: Type[ResponseT],
         options: FinalRequestOptions,
         remaining_retries: int | None,
         stream: bool,
-    ) -> ResponseT | Stream[ResponseT]:
+        stream_cls: type[_StreamT] | None,
+    ) -> ResponseT | _StreamT:
         retries = self._remaining_retries(remaining_retries, options)
         request = self._build_request(options)
 
         try:
             response = self._client.send(request, auth=self.custom_auth, stream=stream)
             response.raise_for_status()
         except httpx.HTTPStatusError as err:  # thrown on 4xx and 5xx status code
             if retries > 0 and self._should_retry(err.response):
-                return self._retry_request(options, cast_to, retries, err.response.headers, stream=stream)
+                return self._retry_request(
+                    options,
+                    cast_to,
+                    retries,
+                    err.response.headers,
+                    stream=stream,
+                    stream_cls=stream_cls,
+                )
 
             # If the response is streamed then we need to explicitly read the response
             # to completion before attempting to access the response text.
             err.response.read()
             raise self._make_status_error_from_response(request, err.response) from None
         except httpx.TimeoutException as err:
             if retries > 0:
-                return self._retry_request(options, cast_to, retries, stream=stream)
+                return self._retry_request(options, cast_to, retries, stream=stream, stream_cls=stream_cls)
             raise APITimeoutError(request=request) from err
         except Exception as err:
             if retries > 0:
-                return self._retry_request(options, cast_to, retries, stream=stream)
+                return self._retry_request(options, cast_to, retries, stream=stream, stream_cls=stream_cls)
             raise APIConnectionError(request=request) from err
 
         if stream:
-            return Stream(cast_to=cast_to, response=response, client=self)
+            stream_cls = stream_cls or cast("type[_StreamT] | None", self._default_stream_cls)
+            if stream_cls is None:
+                raise MissingStreamClassError()
+            return stream_cls(cast_to=cast_to, response=response, client=self)
 
         try:
             rsp = self._process_response(cast_to=cast_to, options=options, response=response)
         except pydantic.ValidationError as err:
             raise APIResponseValidationError(request=request, response=response) from err
 
         return rsp
@@ -883,27 +785,29 @@
         self,
         options: FinalRequestOptions,
         cast_to: Type[ResponseT],
         remaining_retries: int,
         response_headers: Optional[httpx.Headers] = None,
         *,
         stream: bool,
-    ) -> ResponseT | Stream[ResponseT]:
+        stream_cls: type[_StreamT] | None,
+    ) -> ResponseT | _StreamT:
         remaining = remaining_retries - 1
         timeout = self._calculate_retry_timeout(remaining, options, response_headers)
 
         # In a synchronous context we are blocking the entire thread. Up to the library user to run the client in a
         # different thread if necessary.
         time.sleep(timeout)
 
         return self._request(
             options=options,
             cast_to=cast_to,
             remaining_retries=remaining,
             stream=stream,
+            stream_cls=stream_cls,
         )
 
     def _request_api_list(
         self,
         model: Type[ModelT],
         page: Type[SyncPageT],
         options: FinalRequestOptions,
@@ -947,42 +851,45 @@
         path: str,
         *,
         cast_to: Type[ResponseT],
         body: Body | None = None,
         options: RequestOptions = {},
         files: RequestFiles | None = None,
         stream: Literal[True],
-    ) -> Stream[ResponseT]:
+        stream_cls: type[_StreamT],
+    ) -> _StreamT:
         ...
 
     @overload
     def post(
         self,
         path: str,
         *,
         cast_to: Type[ResponseT],
         body: Body | None = None,
         options: RequestOptions = {},
         files: RequestFiles | None = None,
         stream: bool,
-    ) -> ResponseT | Stream[ResponseT]:
+        stream_cls: type[_StreamT] | None = None,
+    ) -> ResponseT | _StreamT:
         ...
 
     def post(
         self,
         path: str,
         *,
         cast_to: Type[ResponseT],
         body: Body | None = None,
         options: RequestOptions = {},
         files: RequestFiles | None = None,
         stream: bool = False,
-    ) -> ResponseT | Stream[ResponseT]:
+        stream_cls: type[_StreamT] | None = None,
+    ) -> ResponseT | _StreamT:
         opts = FinalRequestOptions.construct(method="post", url=path, json_data=body, files=files, **options)
-        return cast(ResponseT, self.request(cast_to, opts, stream=stream))
+        return cast(ResponseT, self.request(cast_to, opts, stream=stream, stream_cls=stream_cls))
 
     def patch(
         self,
         path: str,
         *,
         cast_to: Type[ResponseT],
         body: Body | None = None,
@@ -1026,14 +933,15 @@
     ) -> SyncPageT:
         opts = FinalRequestOptions.construct(method=method, url=path, json_data=body, **options)
         return self._request_api_list(model, page, opts)
 
 
 class AsyncAPIClient(BaseClient):
     _client: httpx.AsyncClient
+    _default_stream_cls: type[AsyncStream[Any]] | None = None
 
     def __init__(
         self,
         *,
         version: str,
         base_url: str,
         _strict_response_validation: bool,
@@ -1078,87 +986,102 @@
     @overload
     async def request(
         self,
         cast_to: Type[ResponseT],
         options: FinalRequestOptions,
         *,
         stream: Literal[True],
+        stream_cls: type[_AsyncStreamT],
         remaining_retries: Optional[int] = None,
-    ) -> AsyncStream[ResponseT]:
+    ) -> _AsyncStreamT:
         ...
 
     @overload
     async def request(
         self,
         cast_to: Type[ResponseT],
         options: FinalRequestOptions,
         *,
         stream: bool,
+        stream_cls: type[_AsyncStreamT] | None = None,
         remaining_retries: Optional[int] = None,
-    ) -> ResponseT | AsyncStream[ResponseT]:
+    ) -> ResponseT | _AsyncStreamT:
         ...
 
     async def request(
         self,
         cast_to: Type[ResponseT],
         options: FinalRequestOptions,
         *,
         stream: bool = False,
+        stream_cls: type[_AsyncStreamT] | None = None,
         remaining_retries: Optional[int] = None,
-    ) -> ResponseT | AsyncStream[ResponseT]:
+    ) -> ResponseT | _AsyncStreamT:
         return await self._request(
             cast_to=cast_to,
             options=options,
             stream=stream,
+            stream_cls=stream_cls,
             remaining_retries=remaining_retries,
         )
 
     async def _request(
         self,
         cast_to: Type[ResponseT],
         options: FinalRequestOptions,
         *,
         stream: bool,
+        stream_cls: type[_AsyncStreamT] | None,
         remaining_retries: int | None,
-    ) -> ResponseT | AsyncStream[ResponseT]:
+    ) -> ResponseT | _AsyncStreamT:
         retries = self._remaining_retries(remaining_retries, options)
         request = self._build_request(options)
 
         try:
             response = await self._client.send(request, auth=self.custom_auth, stream=stream)
             response.raise_for_status()
         except httpx.HTTPStatusError as err:  # thrown on 4xx and 5xx status code
             if retries > 0 and self._should_retry(err.response):
-                return await self._retry_request(options, cast_to, retries, err.response.headers, stream=stream)
+                return await self._retry_request(
+                    options,
+                    cast_to,
+                    retries,
+                    err.response.headers,
+                    stream=stream,
+                    stream_cls=stream_cls,
+                )
 
             # If the response is streamed then we need to explicitly read the response
             # to completion before attempting to access the response text.
             await err.response.aread()
             raise self._make_status_error_from_response(request, err.response) from None
         except httpx.ConnectTimeout as err:
             if retries > 0:
-                return await self._retry_request(options, cast_to, retries, stream=stream)
+                return await self._retry_request(options, cast_to, retries, stream=stream, stream_cls=stream_cls)
             raise APITimeoutError(request=request) from err
         except httpx.ReadTimeout as err:
             # We explicitly do not retry on ReadTimeout errors as this means
             # that the server processing the request has taken 60 seconds
             # (our default timeout). This likely indicates that something
             # is not working as expected on the server side.
             raise
         except httpx.TimeoutException as err:
             if retries > 0:
-                return await self._retry_request(options, cast_to, retries, stream=stream)
+                return await self._retry_request(options, cast_to, retries, stream=stream, stream_cls=stream_cls)
             raise APITimeoutError(request=request) from err
         except Exception as err:
             if retries > 0:
-                return await self._retry_request(options, cast_to, retries, stream=stream)
+                return await self._retry_request(options, cast_to, retries, stream=stream, stream_cls=stream_cls)
             raise APIConnectionError(request=request) from err
 
         if stream:
-            return AsyncStream(cast_to=cast_to, response=response, client=self)
+            stream_cls = stream_cls or cast("type[_AsyncStreamT] | None", self._default_stream_cls)
+            if stream_cls is None:
+                raise MissingStreamClassError()
+            return stream_cls(cast_to=cast_to, response=response, client=self)
 
         try:
             rsp = self._process_response(cast_to=cast_to, options=options, response=response)
         except pydantic.ValidationError as err:
             raise APIResponseValidationError(request=request, response=response) from err
 
         return rsp
@@ -1167,25 +1090,27 @@
         self,
         options: FinalRequestOptions,
         cast_to: Type[ResponseT],
         remaining_retries: int,
         response_headers: Optional[httpx.Headers] = None,
         *,
         stream: bool,
-    ) -> ResponseT | AsyncStream[ResponseT]:
+        stream_cls: type[_AsyncStreamT] | None,
+    ) -> ResponseT | _AsyncStreamT:
         remaining = remaining_retries - 1
         timeout = self._calculate_retry_timeout(remaining, options, response_headers)
 
         await anyio.sleep(timeout)
 
         return await self._request(
             options=options,
             cast_to=cast_to,
             remaining_retries=remaining,
             stream=stream,
+            stream_cls=stream_cls,
         )
 
     def _request_api_list(
         self,
         model: Type[ModelT],
         page: Type[AsyncPageT],
         options: FinalRequestOptions,
@@ -1221,42 +1146,45 @@
         path: str,
         *,
         cast_to: Type[ResponseT],
         body: Body | None = None,
         files: RequestFiles | None = None,
         options: RequestOptions = {},
         stream: Literal[True],
-    ) -> AsyncStream[ResponseT]:
+        stream_cls: type[_AsyncStreamT],
+    ) -> _AsyncStreamT:
         ...
 
     @overload
     async def post(
         self,
         path: str,
         *,
         cast_to: Type[ResponseT],
         body: Body | None = None,
         files: RequestFiles | None = None,
         options: RequestOptions = {},
         stream: bool,
-    ) -> ResponseT | AsyncStream[ResponseT]:
+        stream_cls: type[_AsyncStreamT] | None = None,
+    ) -> ResponseT | _AsyncStreamT:
         ...
 
     async def post(
         self,
         path: str,
         *,
         cast_to: Type[ResponseT],
         body: Body | None = None,
         files: RequestFiles | None = None,
         options: RequestOptions = {},
         stream: bool = False,
-    ) -> ResponseT | AsyncStream[ResponseT]:
+        stream_cls: type[_AsyncStreamT] | None = None,
+    ) -> ResponseT | _AsyncStreamT:
         opts = FinalRequestOptions.construct(method="post", url=path, json_data=body, files=files, **options)
-        return await self.request(cast_to, opts, stream=stream)
+        return await self.request(cast_to, opts, stream=stream, stream_cls=stream_cls)
 
     async def patch(
         self,
         path: str,
         *,
         cast_to: Type[ResponseT],
         body: Body | None = None,
```

### Comparing `increase-0.6.0/src/increase/_base_exceptions.py` & `increase-0.6.1/src/increase/_base_exceptions.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/_client.py` & `increase-0.6.1/src/increase/_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,18 +17,23 @@
     NotGiven,
     Transport,
     ProxiesTypes,
     RequestOptions,
 )
 from ._utils import is_mapping
 from ._version import __version__
-from ._base_client import DEFAULT_LIMITS, DEFAULT_TIMEOUT, DEFAULT_MAX_RETRIES
-from ._base_client import Stream as Stream
-from ._base_client import AsyncStream as AsyncStream
-from ._base_client import SyncAPIClient, AsyncAPIClient
+from ._streaming import Stream as Stream
+from ._streaming import AsyncStream as AsyncStream
+from ._base_client import (
+    DEFAULT_LIMITS,
+    DEFAULT_TIMEOUT,
+    DEFAULT_MAX_RETRIES,
+    SyncAPIClient,
+    AsyncAPIClient,
+)
 
 __all__ = [
     "ENVIRONMENTS",
     "Timeout",
     "Transport",
     "ProxiesTypes",
     "RequestOptions",
```

### Comparing `increase-0.6.0/src/increase/_exceptions.py` & `increase-0.6.1/src/increase/_exceptions.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/_models.py` & `increase-0.6.1/src/increase/_models.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/_qs.py` & `increase-0.6.1/src/increase/_qs.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/_resource.py` & `increase-0.6.1/src/increase/_resource.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/_types.py` & `increase-0.6.1/src/increase/_types.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 from __future__ import annotations
 
 from typing import (
     IO,
     TYPE_CHECKING,
+    Any,
     Dict,
+    List,
     Type,
     Tuple,
     Union,
     Mapping,
     TypeVar,
     Optional,
     Sequence,
 )
 from typing_extensions import Literal, Protocol, TypedDict, runtime_checkable
 
+import httpx
 import pydantic
 from httpx import Proxy, Timeout, Response, BaseTransport
 
+if TYPE_CHECKING:
+    from ._models import BaseModel
+
 Transport = BaseTransport
 Query = Mapping[str, object]
 Body = object
 AnyMapping = Mapping[str, object]
 ModelT = TypeVar("ModelT", bound=pydantic.BaseModel)
 _T = TypeVar("_T")
 
@@ -139,7 +145,12 @@
 
 class HeadersLikeProtocol(Protocol):
     def get(self, __key: str) -> str | None:
         ...
 
 
 HeadersLike = Union[Headers, HeadersLikeProtocol]
+
+ResponseT = TypeVar(
+    "ResponseT",
+    bound="Union[str, None, BaseModel, List[Any], Dict[str, Any], httpx.Response, UnknownResponse, ModelBuilderProtocol]",
+)
```

### Comparing `increase-0.6.0/src/increase/_utils/__init__.py` & `increase-0.6.1/src/increase/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/_utils/_transform.py` & `increase-0.6.1/src/increase/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/_utils/_utils.py` & `increase-0.6.1/src/increase/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/pagination.py` & `increase-0.6.1/src/increase/pagination.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/resources/__init__.py` & `increase-0.6.1/src/increase/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/resources/account_numbers.py` & `increase-0.6.1/src/increase/resources/account_numbers.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> AccountNumber:
-        """Retrieve an Account Number"""
+        """
+        Retrieve an Account Number
+
+        Args:
+          account_number_id: The identifier of the Account Number to retrieve.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return self._get(
             f"/account_numbers/{account_number_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=AccountNumber,
         )
@@ -104,14 +117,16 @@
         timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> AccountNumber:
         """
         Update an Account Number
 
         Args:
+          account_number_id: The identifier of the Account Number.
+
           name: The name you choose for the Account Number.
 
           status: This indicates if transfers can be made to the Account Number.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
@@ -183,19 +198,19 @@
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
+                        "account_id": account_id,
+                        "created_at": created_at,
                         "cursor": cursor,
                         "limit": limit,
                         "status": status,
-                        "account_id": account_id,
-                        "created_at": created_at,
                     },
                     account_number_list_params.AccountNumberListParams,
                 ),
             ),
             model=AccountNumber,
         )
 
@@ -258,15 +273,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> AccountNumber:
-        """Retrieve an Account Number"""
+        """
+        Retrieve an Account Number
+
+        Args:
+          account_number_id: The identifier of the Account Number to retrieve.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return await self._get(
             f"/account_numbers/{account_number_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=AccountNumber,
         )
@@ -285,14 +313,16 @@
         timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> AccountNumber:
         """
         Update an Account Number
 
         Args:
+          account_number_id: The identifier of the Account Number.
+
           name: The name you choose for the Account Number.
 
           status: This indicates if transfers can be made to the Account Number.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
@@ -364,18 +394,18 @@
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
+                        "account_id": account_id,
+                        "created_at": created_at,
                         "cursor": cursor,
                         "limit": limit,
                         "status": status,
-                        "account_id": account_id,
-                        "created_at": created_at,
                     },
                     account_number_list_params.AccountNumberListParams,
                 ),
             ),
             model=AccountNumber,
         )
```

### Comparing `increase-0.6.0/src/increase/resources/account_statements.py` & `increase-0.6.1/src/increase/resources/account_statements.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,15 +20,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> AccountStatement:
-        """Retrieve an Account Statement"""
+        """
+        Retrieve an Account Statement
+
+        Args:
+          account_statement_id: The identifier of the Account Statement to retrieve.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return self._get(
             f"/account_statements/{account_statement_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=AccountStatement,
         )
@@ -72,17 +85,17 @@
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
+                        "account_id": account_id,
                         "cursor": cursor,
                         "limit": limit,
-                        "account_id": account_id,
                         "statement_period_start": statement_period_start,
                     },
                     account_statement_list_params.AccountStatementListParams,
                 ),
             ),
             model=AccountStatement,
         )
@@ -96,15 +109,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> AccountStatement:
-        """Retrieve an Account Statement"""
+        """
+        Retrieve an Account Statement
+
+        Args:
+          account_statement_id: The identifier of the Account Statement to retrieve.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return await self._get(
             f"/account_statements/{account_statement_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=AccountStatement,
         )
@@ -148,17 +174,17 @@
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
+                        "account_id": account_id,
                         "cursor": cursor,
                         "limit": limit,
-                        "account_id": account_id,
                         "statement_period_start": statement_period_start,
                     },
                     account_statement_list_params.AccountStatementListParams,
                 ),
             ),
             model=AccountStatement,
         )
```

### Comparing `increase-0.6.0/src/increase/resources/account_transfers.py` & `increase-0.6.1/src/increase/resources/account_transfers.py`

 * *Files 17% similar despite different names*

```diff
@@ -87,15 +87,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> AccountTransfer:
-        """Retrieve an Account Transfer"""
+        """
+        Retrieve an Account Transfer
+
+        Args:
+          account_transfer_id: The identifier of the Account Transfer.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return self._get(
             f"/account_transfers/{account_transfer_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=AccountTransfer,
         )
@@ -139,18 +152,18 @@
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
-                        "cursor": cursor,
-                        "limit": limit,
                         "account_id": account_id,
                         "created_at": created_at,
+                        "cursor": cursor,
+                        "limit": limit,
                     },
                     account_transfer_list_params.AccountTransferListParams,
                 ),
             ),
             model=AccountTransfer,
         )
 
@@ -162,15 +175,30 @@
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> AccountTransfer:
-        """Approve an Account Transfer"""
+        """
+        Approve an Account Transfer
+
+        Args:
+          account_transfer_id: The identifier of the Account Transfer to approve.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+
+          idempotency_key: Specify a custom idempotency key for this request
+        """
         return self._post(
             f"/account_transfers/{account_transfer_id}/approve",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
@@ -187,15 +215,30 @@
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> AccountTransfer:
-        """Cancel an Account Transfer"""
+        """
+        Cancel an Account Transfer
+
+        Args:
+          account_transfer_id: The identifier of the pending Account Transfer to cancel.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+
+          idempotency_key: Specify a custom idempotency key for this request
+        """
         return self._post(
             f"/account_transfers/{account_transfer_id}/cancel",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
@@ -276,15 +319,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> AccountTransfer:
-        """Retrieve an Account Transfer"""
+        """
+        Retrieve an Account Transfer
+
+        Args:
+          account_transfer_id: The identifier of the Account Transfer.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return await self._get(
             f"/account_transfers/{account_transfer_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=AccountTransfer,
         )
@@ -328,18 +384,18 @@
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
-                        "cursor": cursor,
-                        "limit": limit,
                         "account_id": account_id,
                         "created_at": created_at,
+                        "cursor": cursor,
+                        "limit": limit,
                     },
                     account_transfer_list_params.AccountTransferListParams,
                 ),
             ),
             model=AccountTransfer,
         )
 
@@ -351,15 +407,30 @@
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> AccountTransfer:
-        """Approve an Account Transfer"""
+        """
+        Approve an Account Transfer
+
+        Args:
+          account_transfer_id: The identifier of the Account Transfer to approve.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+
+          idempotency_key: Specify a custom idempotency key for this request
+        """
         return await self._post(
             f"/account_transfers/{account_transfer_id}/approve",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
@@ -376,15 +447,30 @@
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> AccountTransfer:
-        """Cancel an Account Transfer"""
+        """
+        Cancel an Account Transfer
+
+        Args:
+          account_transfer_id: The identifier of the pending Account Transfer to cancel.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+
+          idempotency_key: Specify a custom idempotency key for this request
+        """
         return await self._post(
             f"/account_transfers/{account_transfer_id}/cancel",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
```

### Comparing `increase-0.6.0/src/increase/resources/accounts.py` & `increase-0.6.1/src/increase/resources/accounts.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,16 @@
           name: The name you choose for the Account.
 
           entity_id: The identifier for the Entity that will own the Account.
 
           informational_entity_id: The identifier of an Entity that, while not owning the Account, is associated
               with its activity. Its relationship to your group must be `informational`.
 
-          program_id: The identifier for the Program that this Account falls under.
+          program_id: The identifier for the Program that this Account falls under. Required if you
+              operate more than one Program.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
@@ -58,18 +59,18 @@
 
           idempotency_key: Specify a custom idempotency key for this request
         """
         return self._post(
             "/accounts",
             body=maybe_transform(
                 {
+                    "name": name,
                     "entity_id": entity_id,
-                    "program_id": program_id,
                     "informational_entity_id": informational_entity_id,
-                    "name": name,
+                    "program_id": program_id,
                 },
                 account_create_params.AccountCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
@@ -86,15 +87,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> Account:
-        """Retrieve an Account"""
+        """
+        Retrieve an Account
+
+        Args:
+          account_id: The identifier of the Account to retrieve.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return self._get(
             f"/accounts/{account_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=Account,
         )
@@ -112,14 +126,16 @@
         timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> Account:
         """
         Update an Account
 
         Args:
+          account_id: The identifier of the Account to update.
+
           name: The new name of the Account.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
@@ -143,14 +159,15 @@
 
     def list(
         self,
         *,
         created_at: account_list_params.CreatedAt | NotGiven = NOT_GIVEN,
         cursor: str | NotGiven = NOT_GIVEN,
         entity_id: str | NotGiven = NOT_GIVEN,
+        informational_entity_id: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         status: Literal["open", "closed"] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
@@ -160,14 +177,16 @@
         List Accounts
 
         Args:
           cursor: Return the page of entries after this one.
 
           entity_id: Filter Accounts for those belonging to the specified Entity.
 
+          informational_entity_id: Filter Accounts for those belonging to the specified Entity as informational.
+
           limit: Limit the size of the list that is returned. The default (and maximum) is 100
               objects.
 
           status: Filter Accounts for those with the specified status.
 
           extra_headers: Send extra headers
 
@@ -183,19 +202,20 @@
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
+                        "created_at": created_at,
                         "cursor": cursor,
-                        "limit": limit,
                         "entity_id": entity_id,
+                        "informational_entity_id": informational_entity_id,
+                        "limit": limit,
                         "status": status,
-                        "created_at": created_at,
                     },
                     account_list_params.AccountListParams,
                 ),
             ),
             model=Account,
         )
 
@@ -207,15 +227,30 @@
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> Account:
-        """Close an Account"""
+        """
+        Close an Account
+
+        Args:
+          account_id: The identifier of the Account to close.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+
+          idempotency_key: Specify a custom idempotency key for this request
+        """
         return self._post(
             f"/accounts/{account_id}/close",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
@@ -248,15 +283,16 @@
           name: The name you choose for the Account.
 
           entity_id: The identifier for the Entity that will own the Account.
 
           informational_entity_id: The identifier of an Entity that, while not owning the Account, is associated
               with its activity. Its relationship to your group must be `informational`.
 
-          program_id: The identifier for the Program that this Account falls under.
+          program_id: The identifier for the Program that this Account falls under. Required if you
+              operate more than one Program.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
@@ -264,18 +300,18 @@
 
           idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._post(
             "/accounts",
             body=maybe_transform(
                 {
+                    "name": name,
                     "entity_id": entity_id,
-                    "program_id": program_id,
                     "informational_entity_id": informational_entity_id,
-                    "name": name,
+                    "program_id": program_id,
                 },
                 account_create_params.AccountCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
@@ -292,15 +328,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> Account:
-        """Retrieve an Account"""
+        """
+        Retrieve an Account
+
+        Args:
+          account_id: The identifier of the Account to retrieve.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return await self._get(
             f"/accounts/{account_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=Account,
         )
@@ -318,14 +367,16 @@
         timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> Account:
         """
         Update an Account
 
         Args:
+          account_id: The identifier of the Account to update.
+
           name: The new name of the Account.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
@@ -349,14 +400,15 @@
 
     def list(
         self,
         *,
         created_at: account_list_params.CreatedAt | NotGiven = NOT_GIVEN,
         cursor: str | NotGiven = NOT_GIVEN,
         entity_id: str | NotGiven = NOT_GIVEN,
+        informational_entity_id: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         status: Literal["open", "closed"] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
@@ -366,14 +418,16 @@
         List Accounts
 
         Args:
           cursor: Return the page of entries after this one.
 
           entity_id: Filter Accounts for those belonging to the specified Entity.
 
+          informational_entity_id: Filter Accounts for those belonging to the specified Entity as informational.
+
           limit: Limit the size of the list that is returned. The default (and maximum) is 100
               objects.
 
           status: Filter Accounts for those with the specified status.
 
           extra_headers: Send extra headers
 
@@ -389,19 +443,20 @@
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
+                        "created_at": created_at,
                         "cursor": cursor,
-                        "limit": limit,
                         "entity_id": entity_id,
+                        "informational_entity_id": informational_entity_id,
+                        "limit": limit,
                         "status": status,
-                        "created_at": created_at,
                     },
                     account_list_params.AccountListParams,
                 ),
             ),
             model=Account,
         )
 
@@ -413,15 +468,30 @@
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> Account:
-        """Close an Account"""
+        """
+        Close an Account
+
+        Args:
+          account_id: The identifier of the Account to close.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+
+          idempotency_key: Specify a custom idempotency key for this request
+        """
         return await self._post(
             f"/accounts/{account_id}/close",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
```

### Comparing `increase-0.6.0/src/increase/resources/ach_prenotifications.py` & `increase-0.6.1/src/increase/resources/ach_prenotifications.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,24 +89,24 @@
           idempotency_key: Specify a custom idempotency key for this request
         """
         return self._post(
             "/ach_prenotifications",
             body=maybe_transform(
                 {
                     "account_number": account_number,
+                    "routing_number": routing_number,
                     "addendum": addendum,
                     "company_descriptive_date": company_descriptive_date,
                     "company_discretionary_data": company_discretionary_data,
                     "company_entry_description": company_entry_description,
                     "company_name": company_name,
                     "credit_debit_indicator": credit_debit_indicator,
                     "effective_date": effective_date,
                     "individual_id": individual_id,
                     "individual_name": individual_name,
-                    "routing_number": routing_number,
                     "standard_entry_class_code": standard_entry_class_code,
                 },
                 ach_prenotification_create_params.ACHPrenotificationCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
@@ -124,15 +124,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> ACHPrenotification:
-        """Retrieve an ACH Prenotification"""
+        """
+        Retrieve an ACH Prenotification
+
+        Args:
+          ach_prenotification_id: The identifier of the ACH Prenotification to retrieve.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return self._get(
             f"/ach_prenotifications/{ach_prenotification_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=ACHPrenotification,
         )
@@ -173,17 +186,17 @@
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
+                        "created_at": created_at,
                         "cursor": cursor,
                         "limit": limit,
-                        "created_at": created_at,
                     },
                     ach_prenotification_list_params.ACHPrenotificationListParams,
                 ),
             ),
             model=ACHPrenotification,
         )
 
@@ -257,24 +270,24 @@
           idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._post(
             "/ach_prenotifications",
             body=maybe_transform(
                 {
                     "account_number": account_number,
+                    "routing_number": routing_number,
                     "addendum": addendum,
                     "company_descriptive_date": company_descriptive_date,
                     "company_discretionary_data": company_discretionary_data,
                     "company_entry_description": company_entry_description,
                     "company_name": company_name,
                     "credit_debit_indicator": credit_debit_indicator,
                     "effective_date": effective_date,
                     "individual_id": individual_id,
                     "individual_name": individual_name,
-                    "routing_number": routing_number,
                     "standard_entry_class_code": standard_entry_class_code,
                 },
                 ach_prenotification_create_params.ACHPrenotificationCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
@@ -292,15 +305,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> ACHPrenotification:
-        """Retrieve an ACH Prenotification"""
+        """
+        Retrieve an ACH Prenotification
+
+        Args:
+          ach_prenotification_id: The identifier of the ACH Prenotification to retrieve.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return await self._get(
             f"/ach_prenotifications/{ach_prenotification_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=ACHPrenotification,
         )
@@ -341,16 +367,16 @@
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
+                        "created_at": created_at,
                         "cursor": cursor,
                         "limit": limit,
-                        "created_at": created_at,
                     },
                     ach_prenotification_list_params.ACHPrenotificationListParams,
                 ),
             ),
             model=ACHPrenotification,
         )
```

### Comparing `increase-0.6.0/src/increase/resources/ach_transfers.py` & `increase-0.6.1/src/increase/resources/ach_transfers.py`

 * *Files 4% similar despite different names*

```diff
@@ -113,30 +113,30 @@
           idempotency_key: Specify a custom idempotency key for this request
         """
         return self._post(
             "/ach_transfers",
             body=maybe_transform(
                 {
                     "account_id": account_id,
+                    "amount": amount,
+                    "statement_descriptor": statement_descriptor,
                     "account_number": account_number,
                     "addendum": addendum,
-                    "amount": amount,
                     "company_descriptive_date": company_descriptive_date,
                     "company_discretionary_data": company_discretionary_data,
                     "company_entry_description": company_entry_description,
                     "company_name": company_name,
                     "effective_date": effective_date,
                     "external_account_id": external_account_id,
                     "funding": funding,
                     "individual_id": individual_id,
                     "individual_name": individual_name,
                     "require_approval": require_approval,
                     "routing_number": routing_number,
                     "standard_entry_class_code": standard_entry_class_code,
-                    "statement_descriptor": statement_descriptor,
                 },
                 ach_transfer_create_params.ACHTransferCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
@@ -153,15 +153,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> ACHTransfer:
-        """Retrieve an ACH Transfer"""
+        """
+        Retrieve an ACH Transfer
+
+        Args:
+          ach_transfer_id: The identifier of the ACH Transfer.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return self._get(
             f"/ach_transfers/{ach_transfer_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=ACHTransfer,
         )
@@ -208,19 +221,19 @@
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
-                        "cursor": cursor,
-                        "limit": limit,
                         "account_id": account_id,
-                        "external_account_id": external_account_id,
                         "created_at": created_at,
+                        "cursor": cursor,
+                        "external_account_id": external_account_id,
+                        "limit": limit,
                     },
                     ach_transfer_list_params.ACHTransferListParams,
                 ),
             ),
             model=ACHTransfer,
         )
 
@@ -232,15 +245,30 @@
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> ACHTransfer:
-        """Approves an ACH Transfer in a pending_approval state."""
+        """
+        Approves an ACH Transfer in a pending_approval state.
+
+        Args:
+          ach_transfer_id: The identifier of the ACH Transfer to approve.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+
+          idempotency_key: Specify a custom idempotency key for this request
+        """
         return self._post(
             f"/ach_transfers/{ach_transfer_id}/approve",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
@@ -257,15 +285,30 @@
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> ACHTransfer:
-        """Cancels an ACH Transfer in a pending_approval state."""
+        """
+        Cancels an ACH Transfer in a pending_approval state.
+
+        Args:
+          ach_transfer_id: The identifier of the pending ACH Transfer to cancel.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+
+          idempotency_key: Specify a custom idempotency key for this request
+        """
         return self._post(
             f"/ach_transfers/{ach_transfer_id}/cancel",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
@@ -372,30 +415,30 @@
           idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._post(
             "/ach_transfers",
             body=maybe_transform(
                 {
                     "account_id": account_id,
+                    "amount": amount,
+                    "statement_descriptor": statement_descriptor,
                     "account_number": account_number,
                     "addendum": addendum,
-                    "amount": amount,
                     "company_descriptive_date": company_descriptive_date,
                     "company_discretionary_data": company_discretionary_data,
                     "company_entry_description": company_entry_description,
                     "company_name": company_name,
                     "effective_date": effective_date,
                     "external_account_id": external_account_id,
                     "funding": funding,
                     "individual_id": individual_id,
                     "individual_name": individual_name,
                     "require_approval": require_approval,
                     "routing_number": routing_number,
                     "standard_entry_class_code": standard_entry_class_code,
-                    "statement_descriptor": statement_descriptor,
                 },
                 ach_transfer_create_params.ACHTransferCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
@@ -412,15 +455,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> ACHTransfer:
-        """Retrieve an ACH Transfer"""
+        """
+        Retrieve an ACH Transfer
+
+        Args:
+          ach_transfer_id: The identifier of the ACH Transfer.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return await self._get(
             f"/ach_transfers/{ach_transfer_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=ACHTransfer,
         )
@@ -467,19 +523,19 @@
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
-                        "cursor": cursor,
-                        "limit": limit,
                         "account_id": account_id,
-                        "external_account_id": external_account_id,
                         "created_at": created_at,
+                        "cursor": cursor,
+                        "external_account_id": external_account_id,
+                        "limit": limit,
                     },
                     ach_transfer_list_params.ACHTransferListParams,
                 ),
             ),
             model=ACHTransfer,
         )
 
@@ -491,15 +547,30 @@
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> ACHTransfer:
-        """Approves an ACH Transfer in a pending_approval state."""
+        """
+        Approves an ACH Transfer in a pending_approval state.
+
+        Args:
+          ach_transfer_id: The identifier of the ACH Transfer to approve.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+
+          idempotency_key: Specify a custom idempotency key for this request
+        """
         return await self._post(
             f"/ach_transfers/{ach_transfer_id}/approve",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
@@ -516,15 +587,30 @@
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> ACHTransfer:
-        """Cancels an ACH Transfer in a pending_approval state."""
+        """
+        Cancels an ACH Transfer in a pending_approval state.
+
+        Args:
+          ach_transfer_id: The identifier of the pending ACH Transfer to cancel.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+
+          idempotency_key: Specify a custom idempotency key for this request
+        """
         return await self._post(
             f"/ach_transfers/{ach_transfer_id}/cancel",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
```

### Comparing `increase-0.6.0/src/increase/resources/balance_lookups.py` & `increase-0.6.1/src/increase/resources/balance_lookups.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/resources/bookkeeping_accounts.py` & `increase-0.6.1/src/increase/resources/bookkeeping_accounts.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -56,18 +56,18 @@
 
           idempotency_key: Specify a custom idempotency key for this request
         """
         return self._post(
             "/bookkeeping_accounts",
             body=maybe_transform(
                 {
+                    "name": name,
+                    "account_id": account_id,
                     "compliance_category": compliance_category,
                     "entity_id": entity_id,
-                    "account_id": account_id,
-                    "name": name,
                 },
                 bookkeeping_account_create_params.BookkeepingAccountCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
@@ -164,18 +164,18 @@
 
           idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._post(
             "/bookkeeping_accounts",
             body=maybe_transform(
                 {
+                    "name": name,
+                    "account_id": account_id,
                     "compliance_category": compliance_category,
                     "entity_id": entity_id,
-                    "account_id": account_id,
-                    "name": name,
                 },
                 bookkeeping_account_create_params.BookkeepingAccountCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
```

### Comparing `increase-0.6.0/src/increase/resources/bookkeeping_entries.py` & `increase-0.6.1/src/increase/resources/bookkeeping_entries.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/resources/bookkeeping_entry_sets.py` & `increase-0.6.1/src/increase/resources/bookkeeping_entry_sets.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -50,17 +50,17 @@
 
           idempotency_key: Specify a custom idempotency key for this request
         """
         return self._post(
             "/bookkeeping_entry_sets",
             body=maybe_transform(
                 {
+                    "entries": entries,
                     "date": date,
                     "transaction_id": transaction_id,
-                    "entries": entries,
                 },
                 bookkeeping_entry_set_create_params.BookkeepingEntrySetCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
@@ -107,17 +107,17 @@
 
           idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._post(
             "/bookkeeping_entry_sets",
             body=maybe_transform(
                 {
+                    "entries": entries,
                     "date": date,
                     "transaction_id": transaction_id,
-                    "entries": entries,
                 },
                 bookkeeping_entry_set_create_params.BookkeepingEntrySetCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
```

### Comparing `increase-0.6.0/src/increase/resources/card_disputes.py` & `increase-0.6.1/src/increase/resources/card_disputes.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> CardDispute:
-        """Retrieve a Card Dispute"""
+        """
+        Retrieve a Card Dispute
+
+        Args:
+          card_dispute_id: The identifier of the Card Dispute.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return self._get(
             f"/card_disputes/{card_dispute_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=CardDispute,
         )
@@ -121,17 +134,17 @@
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
+                        "created_at": created_at,
                         "cursor": cursor,
                         "limit": limit,
-                        "created_at": created_at,
                         "status": status,
                     },
                     card_dispute_list_params.CardDisputeListParams,
                 ),
             ),
             model=CardDispute,
         )
@@ -196,15 +209,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> CardDispute:
-        """Retrieve a Card Dispute"""
+        """
+        Retrieve a Card Dispute
+
+        Args:
+          card_dispute_id: The identifier of the Card Dispute.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return await self._get(
             f"/card_disputes/{card_dispute_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=CardDispute,
         )
@@ -246,17 +272,17 @@
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
+                        "created_at": created_at,
                         "cursor": cursor,
                         "limit": limit,
-                        "created_at": created_at,
                         "status": status,
                     },
                     card_dispute_list_params.CardDisputeListParams,
                 ),
             ),
             model=CardDispute,
         )
```

### Comparing `increase-0.6.0/src/increase/resources/card_profiles.py` & `increase-0.6.1/src/increase/resources/card_profiles.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,15 +71,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> CardProfile:
-        """Retrieve a Card Profile"""
+        """
+        Retrieve a Card Profile
+
+        Args:
+          card_profile_id: The identifier of the Card Profile.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return self._get(
             f"/card_profiles/{card_profile_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=CardProfile,
         )
@@ -194,15 +207,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> CardProfile:
-        """Retrieve a Card Profile"""
+        """
+        Retrieve a Card Profile
+
+        Args:
+          card_profile_id: The identifier of the Card Profile.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return await self._get(
             f"/card_profiles/{card_profile_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=CardProfile,
         )
```

### Comparing `increase-0.6.0/src/increase/resources/cards.py` & `increase-0.6.1/src/increase/resources/cards.py`

 * *Files 8% similar despite different names*

```diff
@@ -63,16 +63,16 @@
           idempotency_key: Specify a custom idempotency key for this request
         """
         return self._post(
             "/cards",
             body=maybe_transform(
                 {
                     "account_id": account_id,
-                    "description": description,
                     "billing_address": billing_address,
+                    "description": description,
                     "digital_wallet": digital_wallet,
                 },
                 card_create_params.CardCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
@@ -90,15 +90,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> Card:
-        """Retrieve a Card"""
+        """
+        Retrieve a Card
+
+        Args:
+          card_id: The identifier of the Card.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return self._get(
             f"/cards/{card_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=Card,
         )
@@ -119,14 +132,16 @@
         timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> Card:
         """
         Update a Card
 
         Args:
+          card_id: The card identifier.
+
           billing_address: The card's updated billing address.
 
           description: The description you choose to give the card.
 
           digital_wallet: The contact information used in the two-factor steps for digital wallet card
               creation. At least one field must be present to complete the digital wallet
               steps.
@@ -143,18 +158,18 @@
 
           idempotency_key: Specify a custom idempotency key for this request
         """
         return self._patch(
             f"/cards/{card_id}",
             body=maybe_transform(
                 {
-                    "description": description,
-                    "status": status,
                     "billing_address": billing_address,
+                    "description": description,
                     "digital_wallet": digital_wallet,
+                    "status": status,
                 },
                 card_update_params.CardUpdateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
@@ -203,18 +218,18 @@
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
-                        "cursor": cursor,
-                        "limit": limit,
                         "account_id": account_id,
                         "created_at": created_at,
+                        "cursor": cursor,
+                        "limit": limit,
                     },
                     card_list_params.CardListParams,
                 ),
             ),
             model=Card,
         )
 
@@ -225,15 +240,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> CardDetails:
-        """Retrieve sensitive details for a Card"""
+        """
+        Retrieve sensitive details for a Card
+
+        Args:
+          card_id: The identifier of the Card to retrieve details for.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return self._get(
             f"/cards/{card_id}/details",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=CardDetails,
         )
@@ -282,16 +310,16 @@
           idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._post(
             "/cards",
             body=maybe_transform(
                 {
                     "account_id": account_id,
-                    "description": description,
                     "billing_address": billing_address,
+                    "description": description,
                     "digital_wallet": digital_wallet,
                 },
                 card_create_params.CardCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
@@ -309,15 +337,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> Card:
-        """Retrieve a Card"""
+        """
+        Retrieve a Card
+
+        Args:
+          card_id: The identifier of the Card.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return await self._get(
             f"/cards/{card_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=Card,
         )
@@ -338,14 +379,16 @@
         timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> Card:
         """
         Update a Card
 
         Args:
+          card_id: The card identifier.
+
           billing_address: The card's updated billing address.
 
           description: The description you choose to give the card.
 
           digital_wallet: The contact information used in the two-factor steps for digital wallet card
               creation. At least one field must be present to complete the digital wallet
               steps.
@@ -362,18 +405,18 @@
 
           idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._patch(
             f"/cards/{card_id}",
             body=maybe_transform(
                 {
-                    "description": description,
-                    "status": status,
                     "billing_address": billing_address,
+                    "description": description,
                     "digital_wallet": digital_wallet,
+                    "status": status,
                 },
                 card_update_params.CardUpdateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
@@ -422,18 +465,18 @@
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
-                        "cursor": cursor,
-                        "limit": limit,
                         "account_id": account_id,
                         "created_at": created_at,
+                        "cursor": cursor,
+                        "limit": limit,
                     },
                     card_list_params.CardListParams,
                 ),
             ),
             model=Card,
         )
 
@@ -444,15 +487,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> CardDetails:
-        """Retrieve sensitive details for a Card"""
+        """
+        Retrieve sensitive details for a Card
+
+        Args:
+          card_id: The identifier of the Card to retrieve details for.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return await self._get(
             f"/cards/{card_id}/details",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=CardDetails,
         )
```

### Comparing `increase-0.6.0/src/increase/resources/check_deposits.py` & `increase-0.6.1/src/increase/resources/check_deposits.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,17 +56,17 @@
         """
         return self._post(
             "/check_deposits",
             body=maybe_transform(
                 {
                     "account_id": account_id,
                     "amount": amount,
+                    "back_image_file_id": back_image_file_id,
                     "currency": currency,
                     "front_image_file_id": front_image_file_id,
-                    "back_image_file_id": back_image_file_id,
                 },
                 check_deposit_create_params.CheckDepositCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
@@ -83,15 +83,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> CheckDeposit:
-        """Retrieve a Check Deposit"""
+        """
+        Retrieve a Check Deposit
+
+        Args:
+          check_deposit_id: The identifier of the Check Deposit to retrieve.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return self._get(
             f"/check_deposits/{check_deposit_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=CheckDeposit,
         )
@@ -135,18 +148,18 @@
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
-                        "cursor": cursor,
-                        "limit": limit,
                         "account_id": account_id,
                         "created_at": created_at,
+                        "cursor": cursor,
+                        "limit": limit,
                     },
                     check_deposit_list_params.CheckDepositListParams,
                 ),
             ),
             model=CheckDeposit,
         )
 
@@ -195,17 +208,17 @@
         """
         return await self._post(
             "/check_deposits",
             body=maybe_transform(
                 {
                     "account_id": account_id,
                     "amount": amount,
+                    "back_image_file_id": back_image_file_id,
                     "currency": currency,
                     "front_image_file_id": front_image_file_id,
-                    "back_image_file_id": back_image_file_id,
                 },
                 check_deposit_create_params.CheckDepositCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
@@ -222,15 +235,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> CheckDeposit:
-        """Retrieve a Check Deposit"""
+        """
+        Retrieve a Check Deposit
+
+        Args:
+          check_deposit_id: The identifier of the Check Deposit to retrieve.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return await self._get(
             f"/check_deposits/{check_deposit_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=CheckDeposit,
         )
@@ -274,17 +300,17 @@
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
-                        "cursor": cursor,
-                        "limit": limit,
                         "account_id": account_id,
                         "created_at": created_at,
+                        "cursor": cursor,
+                        "limit": limit,
                     },
                     check_deposit_list_params.CheckDepositListParams,
                 ),
             ),
             model=CheckDeposit,
         )
```

### Comparing `increase-0.6.0/src/increase/resources/check_transfers.py` & `increase-0.6.1/src/increase/resources/check_transfers.py`

 * *Files 5% similar despite different names*

```diff
@@ -80,25 +80,25 @@
           idempotency_key: Specify a custom idempotency key for this request
         """
         return self._post(
             "/check_transfers",
             body=maybe_transform(
                 {
                     "account_id": account_id,
-                    "address_line1": address_line1,
-                    "address_line2": address_line2,
                     "address_city": address_city,
+                    "address_line1": address_line1,
                     "address_state": address_state,
                     "address_zip": address_zip,
-                    "return_address": return_address,
                     "amount": amount,
                     "message": message,
-                    "note": note,
                     "recipient_name": recipient_name,
+                    "address_line2": address_line2,
+                    "note": note,
                     "require_approval": require_approval,
+                    "return_address": return_address,
                 },
                 check_transfer_create_params.CheckTransferCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
@@ -115,15 +115,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> CheckTransfer:
-        """Retrieve a Check Transfer"""
+        """
+        Retrieve a Check Transfer
+
+        Args:
+          check_transfer_id: The identifier of the Check Transfer.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return self._get(
             f"/check_transfers/{check_transfer_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=CheckTransfer,
         )
@@ -167,18 +180,18 @@
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
-                        "cursor": cursor,
-                        "limit": limit,
                         "account_id": account_id,
                         "created_at": created_at,
+                        "cursor": cursor,
+                        "limit": limit,
                     },
                     check_transfer_list_params.CheckTransferListParams,
                 ),
             ),
             model=CheckTransfer,
         )
 
@@ -190,15 +203,30 @@
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> CheckTransfer:
-        """Approve a Check Transfer"""
+        """
+        Approve a Check Transfer
+
+        Args:
+          check_transfer_id: The identifier of the Check Transfer to approve.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+
+          idempotency_key: Specify a custom idempotency key for this request
+        """
         return self._post(
             f"/check_transfers/{check_transfer_id}/approve",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
@@ -215,15 +243,30 @@
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> CheckTransfer:
-        """Cancel a pending Check Transfer"""
+        """
+        Cancel a pending Check Transfer
+
+        Args:
+          check_transfer_id: The identifier of the pending Check Transfer to cancel.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+
+          idempotency_key: Specify a custom idempotency key for this request
+        """
         return self._post(
             f"/check_transfers/{check_transfer_id}/cancel",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
@@ -240,15 +283,30 @@
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> CheckTransfer:
-        """Request a stop payment on a Check Transfer"""
+        """
+        Request a stop payment on a Check Transfer
+
+        Args:
+          check_transfer_id: The identifier of the Check Transfer.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+
+          idempotency_key: Specify a custom idempotency key for this request
+        """
         return self._post(
             f"/check_transfers/{check_transfer_id}/stop_payment",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
@@ -322,25 +380,25 @@
           idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._post(
             "/check_transfers",
             body=maybe_transform(
                 {
                     "account_id": account_id,
-                    "address_line1": address_line1,
-                    "address_line2": address_line2,
                     "address_city": address_city,
+                    "address_line1": address_line1,
                     "address_state": address_state,
                     "address_zip": address_zip,
-                    "return_address": return_address,
                     "amount": amount,
                     "message": message,
-                    "note": note,
                     "recipient_name": recipient_name,
+                    "address_line2": address_line2,
+                    "note": note,
                     "require_approval": require_approval,
+                    "return_address": return_address,
                 },
                 check_transfer_create_params.CheckTransferCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
@@ -357,15 +415,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> CheckTransfer:
-        """Retrieve a Check Transfer"""
+        """
+        Retrieve a Check Transfer
+
+        Args:
+          check_transfer_id: The identifier of the Check Transfer.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return await self._get(
             f"/check_transfers/{check_transfer_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=CheckTransfer,
         )
@@ -409,18 +480,18 @@
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
-                        "cursor": cursor,
-                        "limit": limit,
                         "account_id": account_id,
                         "created_at": created_at,
+                        "cursor": cursor,
+                        "limit": limit,
                     },
                     check_transfer_list_params.CheckTransferListParams,
                 ),
             ),
             model=CheckTransfer,
         )
 
@@ -432,15 +503,30 @@
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> CheckTransfer:
-        """Approve a Check Transfer"""
+        """
+        Approve a Check Transfer
+
+        Args:
+          check_transfer_id: The identifier of the Check Transfer to approve.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+
+          idempotency_key: Specify a custom idempotency key for this request
+        """
         return await self._post(
             f"/check_transfers/{check_transfer_id}/approve",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
@@ -457,15 +543,30 @@
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> CheckTransfer:
-        """Cancel a pending Check Transfer"""
+        """
+        Cancel a pending Check Transfer
+
+        Args:
+          check_transfer_id: The identifier of the pending Check Transfer to cancel.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+
+          idempotency_key: Specify a custom idempotency key for this request
+        """
         return await self._post(
             f"/check_transfers/{check_transfer_id}/cancel",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
@@ -482,15 +583,30 @@
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> CheckTransfer:
-        """Request a stop payment on a Check Transfer"""
+        """
+        Request a stop payment on a Check Transfer
+
+        Args:
+          check_transfer_id: The identifier of the Check Transfer.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+
+          idempotency_key: Specify a custom idempotency key for this request
+        """
         return await self._post(
             f"/check_transfers/{check_transfer_id}/stop_payment",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
```

### Comparing `increase-0.6.0/src/increase/resources/declined_transactions.py` & `increase-0.6.1/src/increase/resources/declined_transactions.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> DeclinedTransaction:
-        """Retrieve a Declined Transaction"""
+        """
+        Retrieve a Declined Transaction
+
+        Args:
+          declined_transaction_id: The identifier of the Declined Transaction.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return self._get(
             f"/declined_transactions/{declined_transaction_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=DeclinedTransaction,
         )
@@ -75,19 +88,19 @@
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
+                        "account_id": account_id,
+                        "created_at": created_at,
                         "cursor": cursor,
                         "limit": limit,
-                        "account_id": account_id,
                         "route_id": route_id,
-                        "created_at": created_at,
                     },
                     declined_transaction_list_params.DeclinedTransactionListParams,
                 ),
             ),
             model=DeclinedTransaction,
         )
 
@@ -100,15 +113,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> DeclinedTransaction:
-        """Retrieve a Declined Transaction"""
+        """
+        Retrieve a Declined Transaction
+
+        Args:
+          declined_transaction_id: The identifier of the Declined Transaction.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return await self._get(
             f"/declined_transactions/{declined_transaction_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=DeclinedTransaction,
         )
@@ -155,18 +181,18 @@
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
+                        "account_id": account_id,
+                        "created_at": created_at,
                         "cursor": cursor,
                         "limit": limit,
-                        "account_id": account_id,
                         "route_id": route_id,
-                        "created_at": created_at,
                     },
                     declined_transaction_list_params.DeclinedTransactionListParams,
                 ),
             ),
             model=DeclinedTransaction,
         )
```

### Comparing `increase-0.6.0/src/increase/resources/digital_wallet_tokens.py` & `increase-0.6.1/src/increase/resources/digital_wallet_tokens.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> DigitalWalletToken:
-        """Retrieve a Digital Wallet Token"""
+        """
+        Retrieve a Digital Wallet Token
+
+        Args:
+          digital_wallet_token_id: The identifier of the Digital Wallet Token.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return self._get(
             f"/digital_wallet_tokens/{digital_wallet_token_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=DigitalWalletToken,
         )
@@ -72,18 +85,18 @@
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
-                        "cursor": cursor,
-                        "limit": limit,
                         "card_id": card_id,
                         "created_at": created_at,
+                        "cursor": cursor,
+                        "limit": limit,
                     },
                     digital_wallet_token_list_params.DigitalWalletTokenListParams,
                 ),
             ),
             model=DigitalWalletToken,
         )
 
@@ -96,15 +109,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> DigitalWalletToken:
-        """Retrieve a Digital Wallet Token"""
+        """
+        Retrieve a Digital Wallet Token
+
+        Args:
+          digital_wallet_token_id: The identifier of the Digital Wallet Token.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return await self._get(
             f"/digital_wallet_tokens/{digital_wallet_token_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=DigitalWalletToken,
         )
@@ -148,17 +174,17 @@
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
-                        "cursor": cursor,
-                        "limit": limit,
                         "card_id": card_id,
                         "created_at": created_at,
+                        "cursor": cursor,
+                        "limit": limit,
                     },
                     digital_wallet_token_list_params.DigitalWalletTokenListParams,
                 ),
             ),
             model=DigitalWalletToken,
         )
```

### Comparing `increase-0.6.0/src/increase/resources/documents.py` & `increase-0.6.1/src/increase/resources/documents.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> Document:
-        """Retrieve a Document"""
+        """
+        Retrieve a Document
+
+        Args:
+          document_id: The identifier of the Document to retrieve.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return self._get(
             f"/documents/{document_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=Document,
         )
@@ -73,19 +86,19 @@
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
-                        "cursor": cursor,
-                        "limit": limit,
-                        "entity_id": entity_id,
                         "category": category,
                         "created_at": created_at,
+                        "cursor": cursor,
+                        "entity_id": entity_id,
+                        "limit": limit,
                     },
                     document_list_params.DocumentListParams,
                 ),
             ),
             model=Document,
         )
 
@@ -98,15 +111,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> Document:
-        """Retrieve a Document"""
+        """
+        Retrieve a Document
+
+        Args:
+          document_id: The identifier of the Document to retrieve.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return await self._get(
             f"/documents/{document_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=Document,
         )
@@ -151,18 +177,18 @@
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
-                        "cursor": cursor,
-                        "limit": limit,
-                        "entity_id": entity_id,
                         "category": category,
                         "created_at": created_at,
+                        "cursor": cursor,
+                        "entity_id": entity_id,
+                        "limit": limit,
                     },
                     document_list_params.DocumentListParams,
                 ),
             ),
             model=Document,
         )
```

### Comparing `increase-0.6.0/src/increase/resources/entities/entities.py` & `increase-0.6.1/src/increase/resources/entities/entities.py`

 * *Files 8% similar despite different names*

```diff
@@ -81,22 +81,22 @@
 
           idempotency_key: Specify a custom idempotency key for this request
         """
         return self._post(
             "/entities",
             body=maybe_transform(
                 {
+                    "relationship": relationship,
                     "structure": structure,
                     "corporation": corporation,
-                    "natural_person": natural_person,
-                    "joint": joint,
-                    "trust": trust,
                     "description": description,
-                    "relationship": relationship,
+                    "joint": joint,
+                    "natural_person": natural_person,
                     "supplemental_documents": supplemental_documents,
+                    "trust": trust,
                 },
                 entity_create_params.EntityCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
@@ -113,15 +113,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> Entity:
-        """Retrieve an Entity"""
+        """
+        Retrieve an Entity
+
+        Args:
+          entity_id: The identifier of the Entity to retrieve.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return self._get(
             f"/entities/{entity_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=Entity,
         )
@@ -162,17 +175,17 @@
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
+                        "created_at": created_at,
                         "cursor": cursor,
                         "limit": limit,
-                        "created_at": created_at,
                     },
                     entity_list_params.EntityListParams,
                 ),
             ),
             model=Entity,
         )
 
@@ -239,22 +252,22 @@
 
           idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._post(
             "/entities",
             body=maybe_transform(
                 {
+                    "relationship": relationship,
                     "structure": structure,
                     "corporation": corporation,
-                    "natural_person": natural_person,
-                    "joint": joint,
-                    "trust": trust,
                     "description": description,
-                    "relationship": relationship,
+                    "joint": joint,
+                    "natural_person": natural_person,
                     "supplemental_documents": supplemental_documents,
+                    "trust": trust,
                 },
                 entity_create_params.EntityCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
@@ -271,15 +284,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> Entity:
-        """Retrieve an Entity"""
+        """
+        Retrieve an Entity
+
+        Args:
+          entity_id: The identifier of the Entity to retrieve.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return await self._get(
             f"/entities/{entity_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=Entity,
         )
@@ -320,16 +346,16 @@
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
+                        "created_at": created_at,
                         "cursor": cursor,
                         "limit": limit,
-                        "created_at": created_at,
                     },
                     entity_list_params.EntityListParams,
                 ),
             ),
             model=Entity,
         )
```

### Comparing `increase-0.6.0/src/increase/resources/entities/supplemental_documents.py` & `increase-0.6.1/src/increase/resources/simulations/card_refunds.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,104 +1,104 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
-from ...types import Entity
+from ...types import Transaction
 from ..._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from ..._utils import maybe_transform
 from ..._resource import SyncAPIResource, AsyncAPIResource
 from ..._base_client import make_request_options
-from ...types.entities import supplemental_document_create_params
+from ...types.simulations import card_refund_create_params
 
-__all__ = ["SupplementalDocuments", "AsyncSupplementalDocuments"]
+__all__ = ["CardRefunds", "AsyncCardRefunds"]
 
 
-class SupplementalDocuments(SyncAPIResource):
+class CardRefunds(SyncAPIResource):
     def create(
         self,
-        entity_id: str,
         *,
-        file_id: str,
+        transaction_id: str,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
-    ) -> Entity:
-        """
-        Create a supplemental document for an Entity
+    ) -> Transaction:
+        """Simulates refunding a card transaction.
+
+        The full value of the original sandbox
+        transaction is refunded.
 
         Args:
-          file_id: The identifier of the File containing the document.
+          transaction_id: The identifier for the Transaction to refund. The Transaction's source must have
+              a category of card_settlement.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
 
           idempotency_key: Specify a custom idempotency key for this request
         """
         return self._post(
-            f"/entities/{entity_id}/supplemental_documents",
-            body=maybe_transform(
-                {"file_id": file_id}, supplemental_document_create_params.SupplementalDocumentCreateParams
-            ),
+            "/simulations/card_refunds",
+            body=maybe_transform({"transaction_id": transaction_id}, card_refund_create_params.CardRefundCreateParams),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
-            cast_to=Entity,
+            cast_to=Transaction,
         )
 
 
-class AsyncSupplementalDocuments(AsyncAPIResource):
+class AsyncCardRefunds(AsyncAPIResource):
     async def create(
         self,
-        entity_id: str,
         *,
-        file_id: str,
+        transaction_id: str,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
-    ) -> Entity:
-        """
-        Create a supplemental document for an Entity
+    ) -> Transaction:
+        """Simulates refunding a card transaction.
+
+        The full value of the original sandbox
+        transaction is refunded.
 
         Args:
-          file_id: The identifier of the File containing the document.
+          transaction_id: The identifier for the Transaction to refund. The Transaction's source must have
+              a category of card_settlement.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
 
           idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._post(
-            f"/entities/{entity_id}/supplemental_documents",
-            body=maybe_transform(
-                {"file_id": file_id}, supplemental_document_create_params.SupplementalDocumentCreateParams
-            ),
+            "/simulations/card_refunds",
+            body=maybe_transform({"transaction_id": transaction_id}, card_refund_create_params.CardRefundCreateParams),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
-            cast_to=Entity,
+            cast_to=Transaction,
         )
```

### Comparing `increase-0.6.0/src/increase/resources/event_subscriptions.py` & `increase-0.6.1/src/increase/resources/event_subscriptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -109,16 +109,16 @@
           idempotency_key: Specify a custom idempotency key for this request
         """
         return self._post(
             "/event_subscriptions",
             body=maybe_transform(
                 {
                     "url": url,
-                    "shared_secret": shared_secret,
                     "selected_event_category": selected_event_category,
+                    "shared_secret": shared_secret,
                 },
                 event_subscription_create_params.EventSubscriptionCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
@@ -135,15 +135,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> EventSubscription:
-        """Retrieve an Event Subscription"""
+        """
+        Retrieve an Event Subscription
+
+        Args:
+          event_subscription_id: The identifier of the Event Subscription.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return self._get(
             f"/event_subscriptions/{event_subscription_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=EventSubscription,
         )
@@ -161,14 +174,16 @@
         timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> EventSubscription:
         """
         Update an Event Subscription
 
         Args:
+          event_subscription_id: The identifier of the Event Subscription.
+
           status: The status to update the Event Subscription with.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
@@ -329,16 +344,16 @@
           idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._post(
             "/event_subscriptions",
             body=maybe_transform(
                 {
                     "url": url,
-                    "shared_secret": shared_secret,
                     "selected_event_category": selected_event_category,
+                    "shared_secret": shared_secret,
                 },
                 event_subscription_create_params.EventSubscriptionCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
@@ -355,15 +370,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> EventSubscription:
-        """Retrieve an Event Subscription"""
+        """
+        Retrieve an Event Subscription
+
+        Args:
+          event_subscription_id: The identifier of the Event Subscription.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return await self._get(
             f"/event_subscriptions/{event_subscription_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=EventSubscription,
         )
@@ -381,14 +409,16 @@
         timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> EventSubscription:
         """
         Update an Event Subscription
 
         Args:
+          event_subscription_id: The identifier of the Event Subscription.
+
           status: The status to update the Event Subscription with.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
```

### Comparing `increase-0.6.0/src/increase/resources/events.py` & `increase-0.6.1/src/increase/resources/events.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> Event:
-        """Retrieve an Event"""
+        """
+        Retrieve an Event
+
+        Args:
+          event_id: The identifier of the Event.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return self._get(
             f"/events/{event_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=Event,
         )
@@ -73,19 +86,19 @@
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
-                        "cursor": cursor,
-                        "limit": limit,
                         "associated_object_id": associated_object_id,
-                        "created_at": created_at,
                         "category": category,
+                        "created_at": created_at,
+                        "cursor": cursor,
+                        "limit": limit,
                     },
                     event_list_params.EventListParams,
                 ),
             ),
             model=Event,
         )
 
@@ -98,15 +111,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> Event:
-        """Retrieve an Event"""
+        """
+        Retrieve an Event
+
+        Args:
+          event_id: The identifier of the Event.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return await self._get(
             f"/events/{event_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=Event,
         )
@@ -151,18 +177,18 @@
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
-                        "cursor": cursor,
-                        "limit": limit,
                         "associated_object_id": associated_object_id,
-                        "created_at": created_at,
                         "category": category,
+                        "created_at": created_at,
+                        "cursor": cursor,
+                        "limit": limit,
                     },
                     event_list_params.EventListParams,
                 ),
             ),
             model=Event,
         )
```

### Comparing `increase-0.6.0/src/increase/resources/exports.py` & `increase-0.6.1/src/increase/resources/exports.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,16 +52,16 @@
           idempotency_key: Specify a custom idempotency key for this request
         """
         return self._post(
             "/exports",
             body=maybe_transform(
                 {
                     "category": category,
-                    "transaction_csv": transaction_csv,
                     "balance_csv": balance_csv,
+                    "transaction_csv": transaction_csv,
                 },
                 export_create_params.ExportCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
@@ -78,15 +78,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> Export:
-        """Retrieve an Export"""
+        """
+        Retrieve an Export
+
+        Args:
+          export_id: The identifier of the Export to retrieve.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return self._get(
             f"/exports/{export_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=Export,
         )
@@ -178,16 +191,16 @@
           idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._post(
             "/exports",
             body=maybe_transform(
                 {
                     "category": category,
-                    "transaction_csv": transaction_csv,
                     "balance_csv": balance_csv,
+                    "transaction_csv": transaction_csv,
                 },
                 export_create_params.ExportCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
@@ -204,15 +217,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> Export:
-        """Retrieve an Export"""
+        """
+        Retrieve an Export
+
+        Args:
+          export_id: The identifier of the Export to retrieve.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return await self._get(
             f"/exports/{export_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=Export,
         )
```

### Comparing `increase-0.6.0/src/increase/resources/external_accounts.py` & `increase-0.6.1/src/increase/resources/external_accounts.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,18 +58,18 @@
 
           idempotency_key: Specify a custom idempotency key for this request
         """
         return self._post(
             "/external_accounts",
             body=maybe_transform(
                 {
-                    "routing_number": routing_number,
                     "account_number": account_number,
-                    "funding": funding,
                     "description": description,
+                    "routing_number": routing_number,
+                    "funding": funding,
                 },
                 external_account_create_params.ExternalAccountCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
@@ -86,15 +86,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> ExternalAccount:
-        """Retrieve an External Account"""
+        """
+        Retrieve an External Account
+
+        Args:
+          external_account_id: The identifier of the External Account.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return self._get(
             f"/external_accounts/{external_account_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=ExternalAccount,
         )
@@ -113,14 +126,16 @@
         timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> ExternalAccount:
         """
         Update an External Account
 
         Args:
+          external_account_id: The external account identifier.
+
           description: The description you choose to give the external account.
 
           status: The status of the External Account.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
@@ -240,18 +255,18 @@
 
           idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._post(
             "/external_accounts",
             body=maybe_transform(
                 {
-                    "routing_number": routing_number,
                     "account_number": account_number,
-                    "funding": funding,
                     "description": description,
+                    "routing_number": routing_number,
+                    "funding": funding,
                 },
                 external_account_create_params.ExternalAccountCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
@@ -268,15 +283,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> ExternalAccount:
-        """Retrieve an External Account"""
+        """
+        Retrieve an External Account
+
+        Args:
+          external_account_id: The identifier of the External Account.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return await self._get(
             f"/external_accounts/{external_account_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=ExternalAccount,
         )
@@ -295,14 +323,16 @@
         timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> ExternalAccount:
         """
         Update an External Account
 
         Args:
+          external_account_id: The external account identifier.
+
           description: The description you choose to give the external account.
 
           status: The status of the External Account.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
```

### Comparing `increase-0.6.0/src/increase/resources/files.py` & `increase-0.6.1/src/increase/resources/files.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,16 +64,16 @@
           timeout: Override the client-level default timeout for this request, in seconds
 
           idempotency_key: Specify a custom idempotency key for this request
         """
         body = deepcopy_minimal(
             {
                 "file": file,
-                "description": description,
                 "purpose": purpose,
+                "description": description,
             }
         )
         files = extract_files(cast(Mapping[str, object], body), paths=[["file"]])
         if files:
             # It should be noted that the actual Content-Type header that will be
             # sent to the server will contain a `boundary` parameter, e.g.
             # multipart/form-data; boundary=---abc--
@@ -100,15 +100,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> File:
-        """Retrieve a File"""
+        """
+        Retrieve a File
+
+        Args:
+          file_id: The identifier of the File.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return self._get(
             f"/files/{file_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=File,
         )
@@ -150,17 +163,17 @@
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
+                        "created_at": created_at,
                         "cursor": cursor,
                         "limit": limit,
-                        "created_at": created_at,
                         "purpose": purpose,
                     },
                     file_list_params.FileListParams,
                 ),
             ),
             model=File,
         )
@@ -215,16 +228,16 @@
           timeout: Override the client-level default timeout for this request, in seconds
 
           idempotency_key: Specify a custom idempotency key for this request
         """
         body = deepcopy_minimal(
             {
                 "file": file,
-                "description": description,
                 "purpose": purpose,
+                "description": description,
             }
         )
         files = extract_files(cast(Mapping[str, object], body), paths=[["file"]])
         if files:
             # It should be noted that the actual Content-Type header that will be
             # sent to the server will contain a `boundary` parameter, e.g.
             # multipart/form-data; boundary=---abc--
@@ -251,15 +264,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> File:
-        """Retrieve a File"""
+        """
+        Retrieve a File
+
+        Args:
+          file_id: The identifier of the File.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return await self._get(
             f"/files/{file_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=File,
         )
@@ -301,17 +327,17 @@
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
+                        "created_at": created_at,
                         "cursor": cursor,
                         "limit": limit,
-                        "created_at": created_at,
                         "purpose": purpose,
                     },
                     file_list_params.FileListParams,
                 ),
             ),
             model=File,
         )
```

### Comparing `increase-0.6.0/src/increase/resources/groups.py` & `increase-0.6.1/src/increase/resources/groups.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/resources/inbound_ach_transfer_returns.py` & `increase-0.6.1/src/increase/resources/inbound_ach_transfer_returns.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,16 +61,16 @@
 
           idempotency_key: Specify a custom idempotency key for this request
         """
         return self._post(
             "/inbound_ach_transfer_returns",
             body=maybe_transform(
                 {
-                    "transaction_id": transaction_id,
                     "reason": reason,
+                    "transaction_id": transaction_id,
                 },
                 inbound_ach_transfer_return_create_params.InboundACHTransferReturnCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
@@ -87,15 +87,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> InboundACHTransferReturn:
-        """Retrieve an Inbound ACH Transfer Return"""
+        """
+        Retrieve an Inbound ACH Transfer Return
+
+        Args:
+          inbound_ach_transfer_return_id: The identifier of the Inbound ACH Transfer Return to retrieve.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return self._get(
             f"/inbound_ach_transfer_returns/{inbound_ach_transfer_return_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=InboundACHTransferReturn,
         )
@@ -192,16 +205,16 @@
 
           idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._post(
             "/inbound_ach_transfer_returns",
             body=maybe_transform(
                 {
-                    "transaction_id": transaction_id,
                     "reason": reason,
+                    "transaction_id": transaction_id,
                 },
                 inbound_ach_transfer_return_create_params.InboundACHTransferReturnCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
@@ -218,15 +231,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> InboundACHTransferReturn:
-        """Retrieve an Inbound ACH Transfer Return"""
+        """
+        Retrieve an Inbound ACH Transfer Return
+
+        Args:
+          inbound_ach_transfer_return_id: The identifier of the Inbound ACH Transfer Return to retrieve.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return await self._get(
             f"/inbound_ach_transfer_returns/{inbound_ach_transfer_return_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=InboundACHTransferReturn,
         )
```

### Comparing `increase-0.6.0/src/increase/resources/inbound_wire_drawdown_requests.py` & `increase-0.6.1/src/increase/resources/inbound_wire_drawdown_requests.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,15 +23,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> InboundWireDrawdownRequest:
-        """Retrieve an Inbound Wire Drawdown Request"""
+        """
+        Retrieve an Inbound Wire Drawdown Request
+
+        Args:
+          inbound_wire_drawdown_request_id: The identifier of the Inbound Wire Drawdown Request to retrieve.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return self._get(
             f"/inbound_wire_drawdown_requests/{inbound_wire_drawdown_request_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=InboundWireDrawdownRequest,
         )
@@ -93,15 +106,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> InboundWireDrawdownRequest:
-        """Retrieve an Inbound Wire Drawdown Request"""
+        """
+        Retrieve an Inbound Wire Drawdown Request
+
+        Args:
+          inbound_wire_drawdown_request_id: The identifier of the Inbound Wire Drawdown Request to retrieve.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return await self._get(
             f"/inbound_wire_drawdown_requests/{inbound_wire_drawdown_request_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=InboundWireDrawdownRequest,
         )
```

### Comparing `increase-0.6.0/src/increase/resources/limits.py` & `increase-0.6.1/src/increase/resources/limits.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,17 +54,17 @@
           idempotency_key: Specify a custom idempotency key for this request
         """
         return self._post(
             "/limits",
             body=maybe_transform(
                 {
                     "metric": metric,
-                    "interval": interval,
                     "model_id": model_id,
                     "value": value,
+                    "interval": interval,
                 },
                 limit_create_params.LimitCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
@@ -81,15 +81,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> Limit:
-        """Retrieve a Limit"""
+        """
+        Retrieve a Limit
+
+        Args:
+          limit_id: The identifier of the Limit to retrieve.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return self._get(
             f"/limits/{limit_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=Limit,
         )
@@ -107,14 +120,16 @@
         timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> Limit:
         """
         Update a Limit
 
         Args:
+          limit_id: The limit to update.
+
           status: The status to update the limit with.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
@@ -233,17 +248,17 @@
           idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._post(
             "/limits",
             body=maybe_transform(
                 {
                     "metric": metric,
-                    "interval": interval,
                     "model_id": model_id,
                     "value": value,
+                    "interval": interval,
                 },
                 limit_create_params.LimitCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
@@ -260,15 +275,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> Limit:
-        """Retrieve a Limit"""
+        """
+        Retrieve a Limit
+
+        Args:
+          limit_id: The identifier of the Limit to retrieve.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return await self._get(
             f"/limits/{limit_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=Limit,
         )
@@ -286,14 +314,16 @@
         timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> Limit:
         """
         Update a Limit
 
         Args:
+          limit_id: The limit to update.
+
           status: The status to update the limit with.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
```

### Comparing `increase-0.6.0/src/increase/resources/oauth_connections.py` & `increase-0.6.1/src/increase/resources/oauth_connections.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,15 +20,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> OauthConnection:
-        """Retrieve an OAuth Connection"""
+        """
+        Retrieve an OAuth Connection
+
+        Args:
+          oauth_connection_id: The identifier of the OAuth Connection.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return self._get(
             f"/oauth_connections/{oauth_connection_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=OauthConnection,
         )
@@ -90,15 +103,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> OauthConnection:
-        """Retrieve an OAuth Connection"""
+        """
+        Retrieve an OAuth Connection
+
+        Args:
+          oauth_connection_id: The identifier of the OAuth Connection.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return await self._get(
             f"/oauth_connections/{oauth_connection_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=OauthConnection,
         )
```

### Comparing `increase-0.6.0/src/increase/resources/pending_transactions.py` & `increase-0.6.1/src/increase/resources/pending_transactions.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> PendingTransaction:
-        """Retrieve a Pending Transaction"""
+        """
+        Retrieve a Pending Transaction
+
+        Args:
+          pending_transaction_id: The identifier of the Pending Transaction.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return self._get(
             f"/pending_transactions/{pending_transaction_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=PendingTransaction,
         )
@@ -79,21 +92,21 @@
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
+                        "account_id": account_id,
+                        "created_at": created_at,
                         "cursor": cursor,
                         "limit": limit,
-                        "account_id": account_id,
                         "route_id": route_id,
                         "source_id": source_id,
                         "status": status,
-                        "created_at": created_at,
                     },
                     pending_transaction_list_params.PendingTransactionListParams,
                 ),
             ),
             model=PendingTransaction,
         )
 
@@ -106,15 +119,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> PendingTransaction:
-        """Retrieve a Pending Transaction"""
+        """
+        Retrieve a Pending Transaction
+
+        Args:
+          pending_transaction_id: The identifier of the Pending Transaction.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return await self._get(
             f"/pending_transactions/{pending_transaction_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=PendingTransaction,
         )
@@ -165,20 +191,20 @@
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
+                        "account_id": account_id,
+                        "created_at": created_at,
                         "cursor": cursor,
                         "limit": limit,
-                        "account_id": account_id,
                         "route_id": route_id,
                         "source_id": source_id,
                         "status": status,
-                        "created_at": created_at,
                     },
                     pending_transaction_list_params.PendingTransactionListParams,
                 ),
             ),
             model=PendingTransaction,
         )
```

### Comparing `increase-0.6.0/src/increase/resources/programs.py` & `increase-0.6.1/src/increase/resources/routing_numbers.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,152 +1,126 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
-from ..types import Program, program_list_params
+from ..types import RoutingNumber, routing_number_list_params
 from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from .._utils import maybe_transform
 from .._resource import SyncAPIResource, AsyncAPIResource
 from ..pagination import SyncPage, AsyncPage
 from .._base_client import AsyncPaginator, make_request_options
 
-__all__ = ["Programs", "AsyncPrograms"]
+__all__ = ["RoutingNumbers", "AsyncRoutingNumbers"]
 
 
-class Programs(SyncAPIResource):
-    def retrieve(
-        self,
-        program_id: str,
-        *,
-        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
-        # The extra values given here take precedence over values defined on the client or passed to this method.
-        extra_headers: Headers | None = None,
-        extra_query: Query | None = None,
-        extra_body: Body | None = None,
-        timeout: float | None | NotGiven = NOT_GIVEN,
-    ) -> Program:
-        """Retrieve a Program"""
-        return self._get(
-            f"/programs/{program_id}",
-            options=make_request_options(
-                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
-            ),
-            cast_to=Program,
-        )
-
+class RoutingNumbers(SyncAPIResource):
     def list(
         self,
         *,
+        routing_number: str,
         cursor: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
-    ) -> SyncPage[Program]:
+    ) -> SyncPage[RoutingNumber]:
         """
-        List Programs
+        You can use this API to confirm if a routing number is valid, such as when a
+        user is providing you with bank account details. Since routing numbers uniquely
+        identify a bank, this will always return 0 or 1 entry. In Sandbox, the only
+        valid routing number for this method is 110000000.
 
         Args:
+          routing_number: Filter financial institutions by routing number.
+
           cursor: Return the page of entries after this one.
 
           limit: Limit the size of the list that is returned. The default (and maximum) is 100
               objects.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get_api_list(
-            "/programs",
-            page=SyncPage[Program],
+            "/routing_numbers",
+            page=SyncPage[RoutingNumber],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
+                        "routing_number": routing_number,
                         "cursor": cursor,
                         "limit": limit,
                     },
-                    program_list_params.ProgramListParams,
+                    routing_number_list_params.RoutingNumberListParams,
                 ),
             ),
-            model=Program,
+            model=RoutingNumber,
         )
 
 
-class AsyncPrograms(AsyncAPIResource):
-    async def retrieve(
-        self,
-        program_id: str,
-        *,
-        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
-        # The extra values given here take precedence over values defined on the client or passed to this method.
-        extra_headers: Headers | None = None,
-        extra_query: Query | None = None,
-        extra_body: Body | None = None,
-        timeout: float | None | NotGiven = NOT_GIVEN,
-    ) -> Program:
-        """Retrieve a Program"""
-        return await self._get(
-            f"/programs/{program_id}",
-            options=make_request_options(
-                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
-            ),
-            cast_to=Program,
-        )
-
+class AsyncRoutingNumbers(AsyncAPIResource):
     def list(
         self,
         *,
+        routing_number: str,
         cursor: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
-    ) -> AsyncPaginator[Program, AsyncPage[Program]]:
+    ) -> AsyncPaginator[RoutingNumber, AsyncPage[RoutingNumber]]:
         """
-        List Programs
+        You can use this API to confirm if a routing number is valid, such as when a
+        user is providing you with bank account details. Since routing numbers uniquely
+        identify a bank, this will always return 0 or 1 entry. In Sandbox, the only
+        valid routing number for this method is 110000000.
 
         Args:
+          routing_number: Filter financial institutions by routing number.
+
           cursor: Return the page of entries after this one.
 
           limit: Limit the size of the list that is returned. The default (and maximum) is 100
               objects.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get_api_list(
-            "/programs",
-            page=AsyncPage[Program],
+            "/routing_numbers",
+            page=AsyncPage[RoutingNumber],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
+                        "routing_number": routing_number,
                         "cursor": cursor,
                         "limit": limit,
                     },
-                    program_list_params.ProgramListParams,
+                    routing_number_list_params.RoutingNumberListParams,
                 ),
             ),
-            model=Program,
+            model=RoutingNumber,
         )
```

### Comparing `increase-0.6.0/src/increase/resources/real_time_decisions.py` & `increase-0.6.1/src/increase/resources/real_time_decisions.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> RealTimeDecision:
-        """Retrieve a Real-Time Decision"""
+        """
+        Retrieve a Real-Time Decision
+
+        Args:
+          real_time_decision_id: The identifier of the Real-Time Decision.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return self._get(
             f"/real_time_decisions/{real_time_decision_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=RealTimeDecision,
         )
@@ -48,14 +61,16 @@
         timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> RealTimeDecision:
         """
         Action a Real-Time Decision
 
         Args:
+          real_time_decision_id: The identifier of the Real-Time Decision.
+
           card_authorization: If the Real-Time Decision relates to a card authorization attempt, this object
               contains your response to the authorization.
 
           digital_wallet_authentication: If the Real-Time Decision relates to a digital wallet authentication attempt,
               this object contains your response to the authentication.
 
           digital_wallet_token: If the Real-Time Decision relates to a digital wallet token provisioning
@@ -72,16 +87,16 @@
           idempotency_key: Specify a custom idempotency key for this request
         """
         return self._post(
             f"/real_time_decisions/{real_time_decision_id}/action",
             body=maybe_transform(
                 {
                     "card_authorization": card_authorization,
-                    "digital_wallet_token": digital_wallet_token,
                     "digital_wallet_authentication": digital_wallet_authentication,
+                    "digital_wallet_token": digital_wallet_token,
                 },
                 real_time_decision_action_params.RealTimeDecisionActionParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
@@ -100,15 +115,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> RealTimeDecision:
-        """Retrieve a Real-Time Decision"""
+        """
+        Retrieve a Real-Time Decision
+
+        Args:
+          real_time_decision_id: The identifier of the Real-Time Decision.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return await self._get(
             f"/real_time_decisions/{real_time_decision_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=RealTimeDecision,
         )
@@ -129,14 +157,16 @@
         timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> RealTimeDecision:
         """
         Action a Real-Time Decision
 
         Args:
+          real_time_decision_id: The identifier of the Real-Time Decision.
+
           card_authorization: If the Real-Time Decision relates to a card authorization attempt, this object
               contains your response to the authorization.
 
           digital_wallet_authentication: If the Real-Time Decision relates to a digital wallet authentication attempt,
               this object contains your response to the authentication.
 
           digital_wallet_token: If the Real-Time Decision relates to a digital wallet token provisioning
@@ -153,16 +183,16 @@
           idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._post(
             f"/real_time_decisions/{real_time_decision_id}/action",
             body=maybe_transform(
                 {
                     "card_authorization": card_authorization,
-                    "digital_wallet_token": digital_wallet_token,
                     "digital_wallet_authentication": digital_wallet_authentication,
+                    "digital_wallet_token": digital_wallet_token,
                 },
                 real_time_decision_action_params.RealTimeDecisionActionParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
```

### Comparing `increase-0.6.0/src/increase/resources/real_time_payments_transfers.py` & `increase-0.6.1/src/increase/resources/real_time_payments_transfers.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,21 +70,21 @@
 
           idempotency_key: Specify a custom idempotency key for this request
         """
         return self._post(
             "/real_time_payments_transfers",
             body=maybe_transform(
                 {
+                    "amount": amount,
+                    "creditor_name": creditor_name,
+                    "remittance_information": remittance_information,
                     "source_account_number_id": source_account_number_id,
                     "destination_account_number": destination_account_number,
                     "destination_routing_number": destination_routing_number,
                     "external_account_id": external_account_id,
-                    "amount": amount,
-                    "creditor_name": creditor_name,
-                    "remittance_information": remittance_information,
                     "require_approval": require_approval,
                 },
                 real_time_payments_transfer_create_params.RealTimePaymentsTransferCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
@@ -102,15 +102,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> RealTimePaymentsTransfer:
-        """Retrieve a Real Time Payments Transfer"""
+        """
+        Retrieve a Real Time Payments Transfer
+
+        Args:
+          real_time_payments_transfer_id: The identifier of the Real Time Payments Transfer.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return self._get(
             f"/real_time_payments_transfers/{real_time_payments_transfer_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=RealTimePaymentsTransfer,
         )
@@ -158,19 +171,19 @@
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
-                        "cursor": cursor,
-                        "limit": limit,
                         "account_id": account_id,
-                        "external_account_id": external_account_id,
                         "created_at": created_at,
+                        "cursor": cursor,
+                        "external_account_id": external_account_id,
+                        "limit": limit,
                     },
                     real_time_payments_transfer_list_params.RealTimePaymentsTransferListParams,
                 ),
             ),
             model=RealTimePaymentsTransfer,
         )
 
@@ -229,21 +242,21 @@
 
           idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._post(
             "/real_time_payments_transfers",
             body=maybe_transform(
                 {
+                    "amount": amount,
+                    "creditor_name": creditor_name,
+                    "remittance_information": remittance_information,
                     "source_account_number_id": source_account_number_id,
                     "destination_account_number": destination_account_number,
                     "destination_routing_number": destination_routing_number,
                     "external_account_id": external_account_id,
-                    "amount": amount,
-                    "creditor_name": creditor_name,
-                    "remittance_information": remittance_information,
                     "require_approval": require_approval,
                 },
                 real_time_payments_transfer_create_params.RealTimePaymentsTransferCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
@@ -261,15 +274,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> RealTimePaymentsTransfer:
-        """Retrieve a Real Time Payments Transfer"""
+        """
+        Retrieve a Real Time Payments Transfer
+
+        Args:
+          real_time_payments_transfer_id: The identifier of the Real Time Payments Transfer.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return await self._get(
             f"/real_time_payments_transfers/{real_time_payments_transfer_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=RealTimePaymentsTransfer,
         )
@@ -317,18 +343,18 @@
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
-                        "cursor": cursor,
-                        "limit": limit,
                         "account_id": account_id,
-                        "external_account_id": external_account_id,
                         "created_at": created_at,
+                        "cursor": cursor,
+                        "external_account_id": external_account_id,
+                        "limit": limit,
                     },
                     real_time_payments_transfer_list_params.RealTimePaymentsTransferListParams,
                 ),
             ),
             model=RealTimePaymentsTransfer,
         )
```

### Comparing `increase-0.6.0/src/increase/resources/routing_numbers.py` & `increase-0.6.1/src/increase/resources/simulations/interest_payments.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,126 +1,122 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
-from ..types import RoutingNumber, routing_number_list_params
-from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
-from .._utils import maybe_transform
-from .._resource import SyncAPIResource, AsyncAPIResource
-from ..pagination import SyncPage, AsyncPage
-from .._base_client import AsyncPaginator, make_request_options
+from ..._types import NOT_GIVEN, Body, Query, Headers, NotGiven
+from ..._utils import maybe_transform
+from ..._resource import SyncAPIResource, AsyncAPIResource
+from ..._base_client import make_request_options
+from ...types.simulations import (
+    InterestPaymentSimulationResult,
+    interest_payment_create_params,
+)
 
-__all__ = ["RoutingNumbers", "AsyncRoutingNumbers"]
+__all__ = ["InterestPayments", "AsyncInterestPayments"]
 
 
-class RoutingNumbers(SyncAPIResource):
-    def list(
+class InterestPayments(SyncAPIResource):
+    def create(
         self,
         *,
-        routing_number: str,
-        cursor: str | NotGiven = NOT_GIVEN,
-        limit: int | NotGiven = NOT_GIVEN,
+        account_id: str,
+        amount: int,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
-    ) -> SyncPage[RoutingNumber]:
-        """
-        You can use this API to confirm if a routing number is valid, such as when a
-        user is providing you with bank account details. Since routing numbers uniquely
-        identify a bank, this will always return 0 or 1 entry. In Sandbox, the only
-        valid routing number for this method is 110000000.
+        idempotency_key: str | None = None,
+    ) -> InterestPaymentSimulationResult:
+        """Simulates an interest payment to your account.
 
-        Args:
-          routing_number: Filter financial institutions by routing number.
+        In production, this happens
+        automatically on the first of each month.
 
-          cursor: Return the page of entries after this one.
+        Args:
+          account_id: The identifier of the Account Number the Interest Payment is for.
 
-          limit: Limit the size of the list that is returned. The default (and maximum) is 100
-              objects.
+          amount: The interest amount in cents. Must be positive.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
+
+          idempotency_key: Specify a custom idempotency key for this request
         """
-        return self._get_api_list(
-            "/routing_numbers",
-            page=SyncPage[RoutingNumber],
+        return self._post(
+            "/simulations/interest_payment",
+            body=maybe_transform(
+                {
+                    "account_id": account_id,
+                    "amount": amount,
+                },
+                interest_payment_create_params.InterestPaymentCreateParams,
+            ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
-                query=maybe_transform(
-                    {
-                        "cursor": cursor,
-                        "limit": limit,
-                        "routing_number": routing_number,
-                    },
-                    routing_number_list_params.RoutingNumberListParams,
-                ),
+                idempotency_key=idempotency_key,
             ),
-            model=RoutingNumber,
+            cast_to=InterestPaymentSimulationResult,
         )
 
 
-class AsyncRoutingNumbers(AsyncAPIResource):
-    def list(
+class AsyncInterestPayments(AsyncAPIResource):
+    async def create(
         self,
         *,
-        routing_number: str,
-        cursor: str | NotGiven = NOT_GIVEN,
-        limit: int | NotGiven = NOT_GIVEN,
+        account_id: str,
+        amount: int,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
-    ) -> AsyncPaginator[RoutingNumber, AsyncPage[RoutingNumber]]:
-        """
-        You can use this API to confirm if a routing number is valid, such as when a
-        user is providing you with bank account details. Since routing numbers uniquely
-        identify a bank, this will always return 0 or 1 entry. In Sandbox, the only
-        valid routing number for this method is 110000000.
+        idempotency_key: str | None = None,
+    ) -> InterestPaymentSimulationResult:
+        """Simulates an interest payment to your account.
 
-        Args:
-          routing_number: Filter financial institutions by routing number.
+        In production, this happens
+        automatically on the first of each month.
 
-          cursor: Return the page of entries after this one.
+        Args:
+          account_id: The identifier of the Account Number the Interest Payment is for.
 
-          limit: Limit the size of the list that is returned. The default (and maximum) is 100
-              objects.
+          amount: The interest amount in cents. Must be positive.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
+
+          idempotency_key: Specify a custom idempotency key for this request
         """
-        return self._get_api_list(
-            "/routing_numbers",
-            page=AsyncPage[RoutingNumber],
+        return await self._post(
+            "/simulations/interest_payment",
+            body=maybe_transform(
+                {
+                    "account_id": account_id,
+                    "amount": amount,
+                },
+                interest_payment_create_params.InterestPaymentCreateParams,
+            ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
-                query=maybe_transform(
-                    {
-                        "cursor": cursor,
-                        "limit": limit,
-                        "routing_number": routing_number,
-                    },
-                    routing_number_list_params.RoutingNumberListParams,
-                ),
+                idempotency_key=idempotency_key,
             ),
-            model=RoutingNumber,
+            cast_to=InterestPaymentSimulationResult,
         )
```

### Comparing `increase-0.6.0/src/increase/resources/simulations/__init__.py` & `increase-0.6.1/src/increase/resources/simulations/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from .cards import Cards, AsyncCards
+from .programs import Programs, AsyncPrograms
 from .documents import Documents, AsyncDocuments
 from .simulations import Simulations, AsyncSimulations
 from .card_refunds import CardRefunds, AsyncCardRefunds
 from .ach_transfers import ACHTransfers, AsyncACHTransfers
 from .card_disputes import CardDisputes, AsyncCardDisputes
 from .check_deposits import CheckDeposits, AsyncCheckDeposits
 from .wire_transfers import WireTransfers, AsyncWireTransfers
@@ -40,14 +41,16 @@
     "AsyncCheckTransfers",
     "Documents",
     "AsyncDocuments",
     "DigitalWalletTokenRequests",
     "AsyncDigitalWalletTokenRequests",
     "CheckDeposits",
     "AsyncCheckDeposits",
+    "Programs",
+    "AsyncPrograms",
     "InboundWireDrawdownRequests",
     "AsyncInboundWireDrawdownRequests",
     "InterestPayments",
     "AsyncInterestPayments",
     "WireTransfers",
     "AsyncWireTransfers",
     "Cards",
```

### Comparing `increase-0.6.0/src/increase/resources/simulations/account_statements.py` & `increase-0.6.1/src/increase/resources/simulations/account_statements.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/resources/simulations/account_transfers.py` & `increase-0.6.1/src/increase/resources/simulations/account_transfers.py`

 * *Files 18% similar despite different names*

```diff
@@ -24,14 +24,27 @@
         idempotency_key: str | None = None,
     ) -> AccountTransfer:
         """
         If your account is configured to require approval for each transfer, this
         endpoint simulates the approval of an [Account Transfer](#account-transfers).
         You can also approve sandbox Account Transfers in the dashboard. This transfer
         must first have a `status` of `pending_approval`.
+
+        Args:
+          account_transfer_id: The identifier of the Account Transfer you wish to complete.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+
+          idempotency_key: Specify a custom idempotency key for this request
         """
         return self._post(
             f"/simulations/account_transfers/{account_transfer_id}/complete",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
@@ -56,14 +69,27 @@
         idempotency_key: str | None = None,
     ) -> AccountTransfer:
         """
         If your account is configured to require approval for each transfer, this
         endpoint simulates the approval of an [Account Transfer](#account-transfers).
         You can also approve sandbox Account Transfers in the dashboard. This transfer
         must first have a `status` of `pending_approval`.
+
+        Args:
+          account_transfer_id: The identifier of the Account Transfer you wish to complete.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+
+          idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._post(
             f"/simulations/account_transfers/{account_transfer_id}/complete",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
```

### Comparing `increase-0.6.0/src/increase/resources/simulations/card_disputes.py` & `increase-0.6.1/src/increase/resources/simulations/card_disputes.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,14 +32,16 @@
         """
         After a [Card Dispute](#card-disputes) is created in production, the dispute
         will be reviewed. Since no review happens in sandbox, this endpoint simulates
         moving a Card Dispute into a rejected or accepted state. A Card Dispute can only
         be actioned one time and must have a status of `pending_reviewing`.
 
         Args:
+          card_dispute_id: The dispute you would like to action.
+
           status: The status to move the dispute to.
 
           explanation: Why the dispute was rejected. Not required for accepting disputes.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
@@ -88,14 +90,16 @@
         """
         After a [Card Dispute](#card-disputes) is created in production, the dispute
         will be reviewed. Since no review happens in sandbox, this endpoint simulates
         moving a Card Dispute into a rejected or accepted state. A Card Dispute can only
         be actioned one time and must have a status of `pending_reviewing`.
 
         Args:
+          card_dispute_id: The dispute you would like to action.
+
           status: The status to move the dispute to.
 
           explanation: Why the dispute was rejected. Not required for accepting disputes.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
```

### Comparing `increase-0.6.0/src/increase/resources/simulations/card_refunds.py` & `increase-0.6.1/src/increase/resources/simulations/programs.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,104 +1,104 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
-from ...types import Transaction
+from ...types import Program
 from ..._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from ..._utils import maybe_transform
 from ..._resource import SyncAPIResource, AsyncAPIResource
 from ..._base_client import make_request_options
-from ...types.simulations import card_refund_create_params
+from ...types.simulations import program_create_params
 
-__all__ = ["CardRefunds", "AsyncCardRefunds"]
+__all__ = ["Programs", "AsyncPrograms"]
 
 
-class CardRefunds(SyncAPIResource):
+class Programs(SyncAPIResource):
     def create(
         self,
         *,
-        transaction_id: str,
+        name: str,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
-    ) -> Transaction:
-        """Simulates refunding a card transaction.
+    ) -> Program:
+        """Simulates a program being created in your group.
 
-        The full value of the original sandbox
-        transaction is refunded.
+        By default, your group has one
+        program called Commercial Banking. Note that when your group operates more than
+        one program, `program_id` is a required field when creating accounts.
 
         Args:
-          transaction_id: The identifier for the Transaction to refund. The Transaction's source must have
-              a category of card_settlement.
+          name: The name of the program being added.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
 
           idempotency_key: Specify a custom idempotency key for this request
         """
         return self._post(
-            "/simulations/card_refunds",
-            body=maybe_transform({"transaction_id": transaction_id}, card_refund_create_params.CardRefundCreateParams),
+            "/simulations/programs",
+            body=maybe_transform({"name": name}, program_create_params.ProgramCreateParams),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
-            cast_to=Transaction,
+            cast_to=Program,
         )
 
 
-class AsyncCardRefunds(AsyncAPIResource):
+class AsyncPrograms(AsyncAPIResource):
     async def create(
         self,
         *,
-        transaction_id: str,
+        name: str,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
-    ) -> Transaction:
-        """Simulates refunding a card transaction.
+    ) -> Program:
+        """Simulates a program being created in your group.
 
-        The full value of the original sandbox
-        transaction is refunded.
+        By default, your group has one
+        program called Commercial Banking. Note that when your group operates more than
+        one program, `program_id` is a required field when creating accounts.
 
         Args:
-          transaction_id: The identifier for the Transaction to refund. The Transaction's source must have
-              a category of card_settlement.
+          name: The name of the program being added.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
 
           idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._post(
-            "/simulations/card_refunds",
-            body=maybe_transform({"transaction_id": transaction_id}, card_refund_create_params.CardRefundCreateParams),
+            "/simulations/programs",
+            body=maybe_transform({"name": name}, program_create_params.ProgramCreateParams),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
-            cast_to=Transaction,
+            cast_to=Program,
         )
```

### Comparing `increase-0.6.0/src/increase/resources/simulations/cards.py` & `increase-0.6.1/src/increase/resources/simulations/cards.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/resources/simulations/check_transfers.py` & `increase-0.6.1/src/increase/resources/simulations/check_transfers.py`

 * *Files 17% similar despite different names*

```diff
@@ -27,14 +27,27 @@
         timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> CheckTransfer:
         """Simulates a [Check Transfer](#check-transfers) being deposited at a bank.
 
         This
         transfer must first have a `status` of `mailed`.
+
+        Args:
+          check_transfer_id: The identifier of the Check Transfer you wish to mark deposited.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+
+          idempotency_key: Specify a custom idempotency key for this request
         """
         return self._post(
             f"/simulations/check_transfers/{check_transfer_id}/deposit",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
@@ -56,14 +69,27 @@
         timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> CheckTransfer:
         """
         Simulates the mailing of a [Check Transfer](#check-transfers), which happens
         once per weekday in production but can be sped up in sandbox. This transfer must
         first have a `status` of `pending_approval` or `pending_submission`.
+
+        Args:
+          check_transfer_id: The identifier of the Check Transfer you wish to mail.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+
+          idempotency_key: Specify a custom idempotency key for this request
         """
         return self._post(
             f"/simulations/check_transfers/{check_transfer_id}/mail",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
@@ -87,14 +113,16 @@
         idempotency_key: str | None = None,
     ) -> CheckTransfer:
         """
         Simulates a [Check Transfer](#check-transfers) being returned via USPS to
         Increase. This transfer must first have a `status` of `mailed`.
 
         Args:
+          check_transfer_id: The identifier of the Check Transfer you wish to mark returned.
+
           reason: The reason why the Check Transfer was returned to Increase.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
@@ -130,14 +158,27 @@
         timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> CheckTransfer:
         """Simulates a [Check Transfer](#check-transfers) being deposited at a bank.
 
         This
         transfer must first have a `status` of `mailed`.
+
+        Args:
+          check_transfer_id: The identifier of the Check Transfer you wish to mark deposited.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+
+          idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._post(
             f"/simulations/check_transfers/{check_transfer_id}/deposit",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
@@ -159,14 +200,27 @@
         timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> CheckTransfer:
         """
         Simulates the mailing of a [Check Transfer](#check-transfers), which happens
         once per weekday in production but can be sped up in sandbox. This transfer must
         first have a `status` of `pending_approval` or `pending_submission`.
+
+        Args:
+          check_transfer_id: The identifier of the Check Transfer you wish to mail.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+
+          idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._post(
             f"/simulations/check_transfers/{check_transfer_id}/mail",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
@@ -190,14 +244,16 @@
         idempotency_key: str | None = None,
     ) -> CheckTransfer:
         """
         Simulates a [Check Transfer](#check-transfers) being returned via USPS to
         Increase. This transfer must first have a `status` of `mailed`.
 
         Args:
+          check_transfer_id: The identifier of the Check Transfer you wish to mark returned.
+
           reason: The reason why the Check Transfer was returned to Increase.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
```

### Comparing `increase-0.6.0/src/increase/resources/simulations/digital_wallet_token_requests.py` & `increase-0.6.1/src/increase/resources/simulations/digital_wallet_token_requests.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/resources/simulations/documents.py` & `increase-0.6.1/src/increase/resources/simulations/documents.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/resources/simulations/inbound_wire_drawdown_requests.py` & `increase-0.6.1/src/increase/resources/simulations/inbound_wire_drawdown_requests.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -105,34 +105,34 @@
 
           idempotency_key: Specify a custom idempotency key for this request
         """
         return self._post(
             "/simulations/inbound_wire_drawdown_requests",
             body=maybe_transform(
                 {
-                    "recipient_account_number_id": recipient_account_number_id,
-                    "originator_account_number": originator_account_number,
-                    "originator_routing_number": originator_routing_number,
+                    "amount": amount,
                     "beneficiary_account_number": beneficiary_account_number,
                     "beneficiary_routing_number": beneficiary_routing_number,
-                    "amount": amount,
                     "currency": currency,
                     "message_to_recipient": message_to_recipient,
+                    "originator_account_number": originator_account_number,
+                    "originator_routing_number": originator_routing_number,
+                    "recipient_account_number_id": recipient_account_number_id,
+                    "beneficiary_address_line1": beneficiary_address_line1,
+                    "beneficiary_address_line2": beneficiary_address_line2,
+                    "beneficiary_address_line3": beneficiary_address_line3,
+                    "beneficiary_name": beneficiary_name,
+                    "originator_address_line1": originator_address_line1,
+                    "originator_address_line2": originator_address_line2,
+                    "originator_address_line3": originator_address_line3,
+                    "originator_name": originator_name,
                     "originator_to_beneficiary_information_line1": originator_to_beneficiary_information_line1,
                     "originator_to_beneficiary_information_line2": originator_to_beneficiary_information_line2,
                     "originator_to_beneficiary_information_line3": originator_to_beneficiary_information_line3,
                     "originator_to_beneficiary_information_line4": originator_to_beneficiary_information_line4,
-                    "originator_name": originator_name,
-                    "originator_address_line1": originator_address_line1,
-                    "originator_address_line2": originator_address_line2,
-                    "originator_address_line3": originator_address_line3,
-                    "beneficiary_name": beneficiary_name,
-                    "beneficiary_address_line1": beneficiary_address_line1,
-                    "beneficiary_address_line2": beneficiary_address_line2,
-                    "beneficiary_address_line3": beneficiary_address_line3,
                 },
                 inbound_wire_drawdown_request_create_params.InboundWireDrawdownRequestCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
@@ -236,34 +236,34 @@
 
           idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._post(
             "/simulations/inbound_wire_drawdown_requests",
             body=maybe_transform(
                 {
-                    "recipient_account_number_id": recipient_account_number_id,
-                    "originator_account_number": originator_account_number,
-                    "originator_routing_number": originator_routing_number,
+                    "amount": amount,
                     "beneficiary_account_number": beneficiary_account_number,
                     "beneficiary_routing_number": beneficiary_routing_number,
-                    "amount": amount,
                     "currency": currency,
                     "message_to_recipient": message_to_recipient,
+                    "originator_account_number": originator_account_number,
+                    "originator_routing_number": originator_routing_number,
+                    "recipient_account_number_id": recipient_account_number_id,
+                    "beneficiary_address_line1": beneficiary_address_line1,
+                    "beneficiary_address_line2": beneficiary_address_line2,
+                    "beneficiary_address_line3": beneficiary_address_line3,
+                    "beneficiary_name": beneficiary_name,
+                    "originator_address_line1": originator_address_line1,
+                    "originator_address_line2": originator_address_line2,
+                    "originator_address_line3": originator_address_line3,
+                    "originator_name": originator_name,
                     "originator_to_beneficiary_information_line1": originator_to_beneficiary_information_line1,
                     "originator_to_beneficiary_information_line2": originator_to_beneficiary_information_line2,
                     "originator_to_beneficiary_information_line3": originator_to_beneficiary_information_line3,
                     "originator_to_beneficiary_information_line4": originator_to_beneficiary_information_line4,
-                    "originator_name": originator_name,
-                    "originator_address_line1": originator_address_line1,
-                    "originator_address_line2": originator_address_line2,
-                    "originator_address_line3": originator_address_line3,
-                    "beneficiary_name": beneficiary_name,
-                    "beneficiary_address_line1": beneficiary_address_line1,
-                    "beneficiary_address_line2": beneficiary_address_line2,
-                    "beneficiary_address_line3": beneficiary_address_line3,
                 },
                 inbound_wire_drawdown_request_create_params.InboundWireDrawdownRequestCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
```

### Comparing `increase-0.6.0/src/increase/resources/simulations/real_time_payments_transfers.py` & `increase-0.6.1/src/increase/resources/simulations/real_time_payments_transfers.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,16 @@
     ) -> RealTimePaymentsTransfer:
         """
         Simulates submission of a Real Time Payments transfer and handling the response
         from the destination financial institution. This transfer must first have a
         `status` of `pending_submission`.
 
         Args:
+          real_time_payments_transfer_id: The identifier of the Real Time Payments Transfer you wish to complete.
+
           rejection: If set, the simulation will reject the transfer.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
@@ -115,19 +117,19 @@
         """
         return self._post(
             "/simulations/inbound_real_time_payments_transfers",
             body=maybe_transform(
                 {
                     "account_number_id": account_number_id,
                     "amount": amount,
-                    "request_for_payment_id": request_for_payment_id,
-                    "debtor_name": debtor_name,
                     "debtor_account_number": debtor_account_number,
+                    "debtor_name": debtor_name,
                     "debtor_routing_number": debtor_routing_number,
                     "remittance_information": remittance_information,
+                    "request_for_payment_id": request_for_payment_id,
                 },
                 real_time_payments_transfer_create_inbound_params.RealTimePaymentsTransferCreateInboundParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
@@ -154,14 +156,16 @@
     ) -> RealTimePaymentsTransfer:
         """
         Simulates submission of a Real Time Payments transfer and handling the response
         from the destination financial institution. This transfer must first have a
         `status` of `pending_submission`.
 
         Args:
+          real_time_payments_transfer_id: The identifier of the Real Time Payments Transfer you wish to complete.
+
           rejection: If set, the simulation will reject the transfer.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
@@ -237,19 +241,19 @@
         """
         return await self._post(
             "/simulations/inbound_real_time_payments_transfers",
             body=maybe_transform(
                 {
                     "account_number_id": account_number_id,
                     "amount": amount,
-                    "request_for_payment_id": request_for_payment_id,
-                    "debtor_name": debtor_name,
                     "debtor_account_number": debtor_account_number,
+                    "debtor_name": debtor_name,
                     "debtor_routing_number": debtor_routing_number,
                     "remittance_information": remittance_information,
+                    "request_for_payment_id": request_for_payment_id,
                 },
                 real_time_payments_transfer_create_inbound_params.RealTimePaymentsTransferCreateInboundParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
```

### Comparing `increase-0.6.0/src/increase/resources/simulations/simulations.py` & `increase-0.6.1/src/increase/resources/simulations/simulations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from .cards import Cards, AsyncCards
+from .programs import Programs, AsyncPrograms
 from .documents import Documents, AsyncDocuments
 from ..._resource import SyncAPIResource, AsyncAPIResource
 from .card_refunds import CardRefunds, AsyncCardRefunds
 from .ach_transfers import ACHTransfers, AsyncACHTransfers
 from .card_disputes import CardDisputes, AsyncCardDisputes
 from .check_deposits import CheckDeposits, AsyncCheckDeposits
 from .wire_transfers import WireTransfers, AsyncWireTransfers
@@ -41,14 +42,15 @@
     ach_transfers: ACHTransfers
     card_disputes: CardDisputes
     card_refunds: CardRefunds
     check_transfers: CheckTransfers
     documents: Documents
     digital_wallet_token_requests: DigitalWalletTokenRequests
     check_deposits: CheckDeposits
+    programs: Programs
     inbound_wire_drawdown_requests: InboundWireDrawdownRequests
     interest_payments: InterestPayments
     wire_transfers: WireTransfers
     cards: Cards
     real_time_payments_transfers: RealTimePaymentsTransfers
 
     def __init__(self, client: Increase) -> None:
@@ -58,14 +60,15 @@
         self.ach_transfers = ACHTransfers(client)
         self.card_disputes = CardDisputes(client)
         self.card_refunds = CardRefunds(client)
         self.check_transfers = CheckTransfers(client)
         self.documents = Documents(client)
         self.digital_wallet_token_requests = DigitalWalletTokenRequests(client)
         self.check_deposits = CheckDeposits(client)
+        self.programs = Programs(client)
         self.inbound_wire_drawdown_requests = InboundWireDrawdownRequests(client)
         self.interest_payments = InterestPayments(client)
         self.wire_transfers = WireTransfers(client)
         self.cards = Cards(client)
         self.real_time_payments_transfers = RealTimePaymentsTransfers(client)
 
 
@@ -75,14 +78,15 @@
     ach_transfers: AsyncACHTransfers
     card_disputes: AsyncCardDisputes
     card_refunds: AsyncCardRefunds
     check_transfers: AsyncCheckTransfers
     documents: AsyncDocuments
     digital_wallet_token_requests: AsyncDigitalWalletTokenRequests
     check_deposits: AsyncCheckDeposits
+    programs: AsyncPrograms
     inbound_wire_drawdown_requests: AsyncInboundWireDrawdownRequests
     interest_payments: AsyncInterestPayments
     wire_transfers: AsyncWireTransfers
     cards: AsyncCards
     real_time_payments_transfers: AsyncRealTimePaymentsTransfers
 
     def __init__(self, client: AsyncIncrease) -> None:
@@ -92,12 +96,13 @@
         self.ach_transfers = AsyncACHTransfers(client)
         self.card_disputes = AsyncCardDisputes(client)
         self.card_refunds = AsyncCardRefunds(client)
         self.check_transfers = AsyncCheckTransfers(client)
         self.documents = AsyncDocuments(client)
         self.digital_wallet_token_requests = AsyncDigitalWalletTokenRequests(client)
         self.check_deposits = AsyncCheckDeposits(client)
+        self.programs = AsyncPrograms(client)
         self.inbound_wire_drawdown_requests = AsyncInboundWireDrawdownRequests(client)
         self.interest_payments = AsyncInterestPayments(client)
         self.wire_transfers = AsyncWireTransfers(client)
         self.cards = AsyncCards(client)
         self.real_time_payments_transfers = AsyncRealTimePaymentsTransfers(client)
```

### Comparing `increase-0.6.0/src/increase/resources/simulations/wire_transfers.py` & `increase-0.6.1/src/increase/resources/simulations/wire_transfers.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/resources/transactions.py` & `increase-0.6.1/src/increase/resources/transactions.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,15 +20,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> Transaction:
-        """Retrieve a Transaction"""
+        """
+        Retrieve a Transaction
+
+        Args:
+          transaction_id: The identifier of the Transaction to retrieve.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return self._get(
             f"/transactions/{transaction_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=Transaction,
         )
@@ -77,20 +90,20 @@
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
+                        "account_id": account_id,
+                        "category": category,
+                        "created_at": created_at,
                         "cursor": cursor,
                         "limit": limit,
-                        "account_id": account_id,
                         "route_id": route_id,
-                        "created_at": created_at,
-                        "category": category,
                     },
                     transaction_list_params.TransactionListParams,
                 ),
             ),
             model=Transaction,
         )
 
@@ -103,15 +116,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> Transaction:
-        """Retrieve a Transaction"""
+        """
+        Retrieve a Transaction
+
+        Args:
+          transaction_id: The identifier of the Transaction to retrieve.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return await self._get(
             f"/transactions/{transaction_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=Transaction,
         )
@@ -160,19 +186,19 @@
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
+                        "account_id": account_id,
+                        "category": category,
+                        "created_at": created_at,
                         "cursor": cursor,
                         "limit": limit,
-                        "account_id": account_id,
                         "route_id": route_id,
-                        "created_at": created_at,
-                        "category": category,
                     },
                     transaction_list_params.TransactionListParams,
                 ),
             ),
             model=Transaction,
         )
```

### Comparing `increase-0.6.0/src/increase/resources/wire_drawdown_requests.py` & `increase-0.6.1/src/increase/resources/wire_drawdown_requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,16 +73,16 @@
             "/wire_drawdown_requests",
             body=maybe_transform(
                 {
                     "account_number_id": account_number_id,
                     "amount": amount,
                     "message_to_recipient": message_to_recipient,
                     "recipient_account_number": recipient_account_number,
-                    "recipient_routing_number": recipient_routing_number,
                     "recipient_name": recipient_name,
+                    "recipient_routing_number": recipient_routing_number,
                     "recipient_address_line1": recipient_address_line1,
                     "recipient_address_line2": recipient_address_line2,
                     "recipient_address_line3": recipient_address_line3,
                 },
                 wire_drawdown_request_create_params.WireDrawdownRequestCreateParams,
             ),
             options=make_request_options(
@@ -102,15 +102,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> WireDrawdownRequest:
-        """Retrieve a Wire Drawdown Request"""
+        """
+        Retrieve a Wire Drawdown Request
+
+        Args:
+          wire_drawdown_request_id: The identifier of the Wire Drawdown Request to retrieve.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return self._get(
             f"/wire_drawdown_requests/{wire_drawdown_request_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=WireDrawdownRequest,
         )
@@ -221,16 +234,16 @@
             "/wire_drawdown_requests",
             body=maybe_transform(
                 {
                     "account_number_id": account_number_id,
                     "amount": amount,
                     "message_to_recipient": message_to_recipient,
                     "recipient_account_number": recipient_account_number,
-                    "recipient_routing_number": recipient_routing_number,
                     "recipient_name": recipient_name,
+                    "recipient_routing_number": recipient_routing_number,
                     "recipient_address_line1": recipient_address_line1,
                     "recipient_address_line2": recipient_address_line2,
                     "recipient_address_line3": recipient_address_line3,
                 },
                 wire_drawdown_request_create_params.WireDrawdownRequestCreateParams,
             ),
             options=make_request_options(
@@ -250,15 +263,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> WireDrawdownRequest:
-        """Retrieve a Wire Drawdown Request"""
+        """
+        Retrieve a Wire Drawdown Request
+
+        Args:
+          wire_drawdown_request_id: The identifier of the Wire Drawdown Request to retrieve.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return await self._get(
             f"/wire_drawdown_requests/{wire_drawdown_request_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=WireDrawdownRequest,
         )
```

### Comparing `increase-0.6.0/src/increase/resources/wire_transfers.py` & `increase-0.6.1/src/increase/resources/wire_transfers.py`

 * *Files 22% similar despite different names*

```diff
@@ -74,24 +74,24 @@
           idempotency_key: Specify a custom idempotency key for this request
         """
         return self._post(
             "/wire_transfers",
             body=maybe_transform(
                 {
                     "account_id": account_id,
-                    "account_number": account_number,
-                    "routing_number": routing_number,
-                    "external_account_id": external_account_id,
                     "amount": amount,
-                    "message_to_recipient": message_to_recipient,
                     "beneficiary_name": beneficiary_name,
+                    "message_to_recipient": message_to_recipient,
+                    "account_number": account_number,
                     "beneficiary_address_line1": beneficiary_address_line1,
                     "beneficiary_address_line2": beneficiary_address_line2,
                     "beneficiary_address_line3": beneficiary_address_line3,
+                    "external_account_id": external_account_id,
                     "require_approval": require_approval,
+                    "routing_number": routing_number,
                 },
                 wire_transfer_create_params.WireTransferCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
@@ -108,15 +108,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> WireTransfer:
-        """Retrieve a Wire Transfer"""
+        """
+        Retrieve a Wire Transfer
+
+        Args:
+          wire_transfer_id: The identifier of the Wire Transfer.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return self._get(
             f"/wire_transfers/{wire_transfer_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=WireTransfer,
         )
@@ -163,19 +176,19 @@
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
-                        "cursor": cursor,
-                        "limit": limit,
                         "account_id": account_id,
-                        "external_account_id": external_account_id,
                         "created_at": created_at,
+                        "cursor": cursor,
+                        "external_account_id": external_account_id,
+                        "limit": limit,
                     },
                     wire_transfer_list_params.WireTransferListParams,
                 ),
             ),
             model=WireTransfer,
         )
 
@@ -187,15 +200,30 @@
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> WireTransfer:
-        """Approve a Wire Transfer"""
+        """
+        Approve a Wire Transfer
+
+        Args:
+          wire_transfer_id: The identifier of the Wire Transfer to approve.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+
+          idempotency_key: Specify a custom idempotency key for this request
+        """
         return self._post(
             f"/wire_transfers/{wire_transfer_id}/approve",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
@@ -212,15 +240,30 @@
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> WireTransfer:
-        """Cancel a pending Wire Transfer"""
+        """
+        Cancel a pending Wire Transfer
+
+        Args:
+          wire_transfer_id: The identifier of the pending Wire Transfer to cancel.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+
+          idempotency_key: Specify a custom idempotency key for this request
+        """
         return self._post(
             f"/wire_transfers/{wire_transfer_id}/cancel",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
@@ -242,14 +285,27 @@
         idempotency_key: str | None = None,
     ) -> WireTransfer:
         """
         Simulates the reversal of a [Wire Transfer](#wire-transfers) by the Federal
         Reserve due to error conditions. This will also create a
         [Transaction](#transaction) to account for the returned funds. This Wire
         Transfer must first have a `status` of `complete`.'
+
+        Args:
+          wire_transfer_id: The identifier of the Wire Transfer you wish to reverse.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+
+          idempotency_key: Specify a custom idempotency key for this request
         """
         return self._post(
             f"/simulations/wire_transfers/{wire_transfer_id}/reverse",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
@@ -271,14 +327,27 @@
         timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> WireTransfer:
         """
         Simulates the submission of a [Wire Transfer](#wire-transfers) to the Federal
         Reserve. This transfer must first have a `status` of `pending_approval` or
         `pending_creating`.
+
+        Args:
+          wire_transfer_id: The identifier of the Wire Transfer you wish to submit.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+
+          idempotency_key: Specify a custom idempotency key for this request
         """
         return self._post(
             f"/simulations/wire_transfers/{wire_transfer_id}/submit",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
@@ -351,24 +420,24 @@
           idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._post(
             "/wire_transfers",
             body=maybe_transform(
                 {
                     "account_id": account_id,
-                    "account_number": account_number,
-                    "routing_number": routing_number,
-                    "external_account_id": external_account_id,
                     "amount": amount,
-                    "message_to_recipient": message_to_recipient,
                     "beneficiary_name": beneficiary_name,
+                    "message_to_recipient": message_to_recipient,
+                    "account_number": account_number,
                     "beneficiary_address_line1": beneficiary_address_line1,
                     "beneficiary_address_line2": beneficiary_address_line2,
                     "beneficiary_address_line3": beneficiary_address_line3,
+                    "external_account_id": external_account_id,
                     "require_approval": require_approval,
+                    "routing_number": routing_number,
                 },
                 wire_transfer_create_params.WireTransferCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
@@ -385,15 +454,28 @@
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> WireTransfer:
-        """Retrieve a Wire Transfer"""
+        """
+        Retrieve a Wire Transfer
+
+        Args:
+          wire_transfer_id: The identifier of the Wire Transfer.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+        """
         return await self._get(
             f"/wire_transfers/{wire_transfer_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=WireTransfer,
         )
@@ -440,19 +522,19 @@
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
-                        "cursor": cursor,
-                        "limit": limit,
                         "account_id": account_id,
-                        "external_account_id": external_account_id,
                         "created_at": created_at,
+                        "cursor": cursor,
+                        "external_account_id": external_account_id,
+                        "limit": limit,
                     },
                     wire_transfer_list_params.WireTransferListParams,
                 ),
             ),
             model=WireTransfer,
         )
 
@@ -464,15 +546,30 @@
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> WireTransfer:
-        """Approve a Wire Transfer"""
+        """
+        Approve a Wire Transfer
+
+        Args:
+          wire_transfer_id: The identifier of the Wire Transfer to approve.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+
+          idempotency_key: Specify a custom idempotency key for this request
+        """
         return await self._post(
             f"/wire_transfers/{wire_transfer_id}/approve",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
@@ -489,15 +586,30 @@
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> WireTransfer:
-        """Cancel a pending Wire Transfer"""
+        """
+        Cancel a pending Wire Transfer
+
+        Args:
+          wire_transfer_id: The identifier of the pending Wire Transfer to cancel.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+
+          idempotency_key: Specify a custom idempotency key for this request
+        """
         return await self._post(
             f"/wire_transfers/{wire_transfer_id}/cancel",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
@@ -519,14 +631,27 @@
         idempotency_key: str | None = None,
     ) -> WireTransfer:
         """
         Simulates the reversal of a [Wire Transfer](#wire-transfers) by the Federal
         Reserve due to error conditions. This will also create a
         [Transaction](#transaction) to account for the returned funds. This Wire
         Transfer must first have a `status` of `complete`.'
+
+        Args:
+          wire_transfer_id: The identifier of the Wire Transfer you wish to reverse.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+
+          idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._post(
             f"/simulations/wire_transfers/{wire_transfer_id}/reverse",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
@@ -548,14 +673,27 @@
         timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> WireTransfer:
         """
         Simulates the submission of a [Wire Transfer](#wire-transfers) to the Federal
         Reserve. This transfer must first have a `status` of `pending_approval` or
         `pending_creating`.
+
+        Args:
+          wire_transfer_id: The identifier of the Wire Transfer you wish to submit.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+
+          idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._post(
             f"/simulations/wire_transfers/{wire_transfer_id}/submit",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
```

### Comparing `increase-0.6.0/src/increase/types/__init__.py` & `increase-0.6.1/src/increase/types/__init__.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/types/account.py` & `increase-0.6.1/src/increase/types/account.py`

 * *Files 19% similar despite different names*

```diff
@@ -42,14 +42,21 @@
 
     interest_accrued_at: Optional[date]
     """
     The latest [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date on which
     interest was accrued.
     """
 
+    interest_rate: str
+    """
+    The Interest Rate currently being earned on the account, as a string containing
+    a decimal number. For example, a 1% interest rate would be represented as
+    "0.01".
+    """
+
     name: str
     """The name you choose for the Account."""
 
     status: Literal["open", "closed"]
     """The status of the Account."""
 
     type: Literal["account"]
```

### Comparing `increase-0.6.0/src/increase/types/account_create_params.py` & `increase-0.6.1/src/increase/types/account_create_params.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,8 +17,11 @@
     informational_entity_id: str
     """
     The identifier of an Entity that, while not owning the Account, is associated
     with its activity. Its relationship to your group must be `informational`.
     """
 
     program_id: str
-    """The identifier for the Program that this Account falls under."""
+    """The identifier for the Program that this Account falls under.
+
+    Required if you operate more than one Program.
+    """
```

### Comparing `increase-0.6.0/src/increase/types/account_list_params.py` & `increase-0.6.1/src/increase/types/account_list_params.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,36 @@
 from typing_extensions import Literal, Annotated, TypedDict
 
 from .._utils import PropertyInfo
 
 __all__ = ["AccountListParams", "CreatedAt"]
 
 
+class AccountListParams(TypedDict, total=False):
+    created_at: CreatedAt
+
+    cursor: str
+    """Return the page of entries after this one."""
+
+    entity_id: str
+    """Filter Accounts for those belonging to the specified Entity."""
+
+    informational_entity_id: str
+    """Filter Accounts for those belonging to the specified Entity as informational."""
+
+    limit: int
+    """Limit the size of the list that is returned.
+
+    The default (and maximum) is 100 objects.
+    """
+
+    status: Literal["open", "closed"]
+    """Filter Accounts for those with the specified status."""
+
+
 class CreatedAt(TypedDict, total=False):
     after: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
     """
     Return results after this [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601)
     timestamp.
     """
 
@@ -31,26 +53,7 @@
     """
 
     on_or_before: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
     """
     Return results on or before this
     [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) timestamp.
     """
-
-
-class AccountListParams(TypedDict, total=False):
-    created_at: CreatedAt
-
-    cursor: str
-    """Return the page of entries after this one."""
-
-    entity_id: str
-    """Filter Accounts for those belonging to the specified Entity."""
-
-    limit: int
-    """Limit the size of the list that is returned.
-
-    The default (and maximum) is 100 objects.
-    """
-
-    status: Literal["open", "closed"]
-    """Filter Accounts for those with the specified status."""
```

### Comparing `increase-0.6.0/src/increase/types/account_number.py` & `increase-0.6.1/src/increase/types/account_number.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/types/account_number_list_params.py` & `increase-0.6.1/src/increase/types/account_number_list_params.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,33 @@
 from typing_extensions import Literal, Annotated, TypedDict
 
 from .._utils import PropertyInfo
 
 __all__ = ["AccountNumberListParams", "CreatedAt"]
 
 
+class AccountNumberListParams(TypedDict, total=False):
+    account_id: str
+    """Filter Account Numbers to those belonging to the specified Account."""
+
+    created_at: CreatedAt
+
+    cursor: str
+    """Return the page of entries after this one."""
+
+    limit: int
+    """Limit the size of the list that is returned.
+
+    The default (and maximum) is 100 objects.
+    """
+
+    status: Literal["active", "disabled", "canceled"]
+    """The status to retrieve Account Numbers for."""
+
+
 class CreatedAt(TypedDict, total=False):
     after: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
     """
     Return results after this [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601)
     timestamp.
     """
 
@@ -31,26 +50,7 @@
     """
 
     on_or_before: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
     """
     Return results on or before this
     [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) timestamp.
     """
-
-
-class AccountNumberListParams(TypedDict, total=False):
-    account_id: str
-    """Filter Account Numbers to those belonging to the specified Account."""
-
-    created_at: CreatedAt
-
-    cursor: str
-    """Return the page of entries after this one."""
-
-    limit: int
-    """Limit the size of the list that is returned.
-
-    The default (and maximum) is 100 objects.
-    """
-
-    status: Literal["active", "disabled", "canceled"]
-    """The status to retrieve Account Numbers for."""
```

### Comparing `increase-0.6.0/src/increase/types/account_statement.py` & `increase-0.6.1/src/increase/types/account_statement.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/types/account_statement_list_params.py` & `increase-0.6.1/src/increase/types/account_statement_list_params.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,30 @@
 from typing_extensions import Annotated, TypedDict
 
 from .._utils import PropertyInfo
 
 __all__ = ["AccountStatementListParams", "StatementPeriodStart"]
 
 
+class AccountStatementListParams(TypedDict, total=False):
+    account_id: str
+    """Filter Account Statements to those belonging to the specified Account."""
+
+    cursor: str
+    """Return the page of entries after this one."""
+
+    limit: int
+    """Limit the size of the list that is returned.
+
+    The default (and maximum) is 100 objects.
+    """
+
+    statement_period_start: StatementPeriodStart
+
+
 class StatementPeriodStart(TypedDict, total=False):
     after: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
     """
     Return results after this [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601)
     timestamp.
     """
 
@@ -31,23 +47,7 @@
     """
 
     on_or_before: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
     """
     Return results on or before this
     [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) timestamp.
     """
-
-
-class AccountStatementListParams(TypedDict, total=False):
-    account_id: str
-    """Filter Account Statements to those belonging to the specified Account."""
-
-    cursor: str
-    """Return the page of entries after this one."""
-
-    limit: int
-    """Limit the size of the list that is returned.
-
-    The default (and maximum) is 100 objects.
-    """
-
-    statement_period_start: StatementPeriodStart
```

### Comparing `increase-0.6.0/src/increase/types/account_transfer.py` & `increase-0.6.1/src/increase/types/account_transfer.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/types/account_transfer_create_params.py` & `increase-0.6.1/src/increase/types/account_transfer_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/types/account_transfer_list_params.py` & `increase-0.6.1/src/increase/types/account_transfer_list_params.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,30 @@
 from typing_extensions import Annotated, TypedDict
 
 from .._utils import PropertyInfo
 
 __all__ = ["AccountTransferListParams", "CreatedAt"]
 
 
+class AccountTransferListParams(TypedDict, total=False):
+    account_id: str
+    """Filter Account Transfers to those that originated from the specified Account."""
+
+    created_at: CreatedAt
+
+    cursor: str
+    """Return the page of entries after this one."""
+
+    limit: int
+    """Limit the size of the list that is returned.
+
+    The default (and maximum) is 100 objects.
+    """
+
+
 class CreatedAt(TypedDict, total=False):
     after: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
     """
     Return results after this [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601)
     timestamp.
     """
 
@@ -31,23 +47,7 @@
     """
 
     on_or_before: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
     """
     Return results on or before this
     [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) timestamp.
     """
-
-
-class AccountTransferListParams(TypedDict, total=False):
-    account_id: str
-    """Filter Account Transfers to those that originated from the specified Account."""
-
-    created_at: CreatedAt
-
-    cursor: str
-    """Return the page of entries after this one."""
-
-    limit: int
-    """Limit the size of the list that is returned.
-
-    The default (and maximum) is 100 objects.
-    """
```

### Comparing `increase-0.6.0/src/increase/types/ach_prenotification.py` & `increase-0.6.1/src/increase/types/ach_prenotification.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/types/ach_prenotification_create_params.py` & `increase-0.6.1/src/increase/types/ach_prenotification_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/types/ach_prenotification_list_params.py` & `increase-0.6.1/src/increase/types/ach_prenotification_list_params.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,27 @@
 from typing_extensions import Annotated, TypedDict
 
 from .._utils import PropertyInfo
 
 __all__ = ["ACHPrenotificationListParams", "CreatedAt"]
 
 
+class ACHPrenotificationListParams(TypedDict, total=False):
+    created_at: CreatedAt
+
+    cursor: str
+    """Return the page of entries after this one."""
+
+    limit: int
+    """Limit the size of the list that is returned.
+
+    The default (and maximum) is 100 objects.
+    """
+
+
 class CreatedAt(TypedDict, total=False):
     after: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
     """
     Return results after this [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601)
     timestamp.
     """
 
@@ -31,20 +44,7 @@
     """
 
     on_or_before: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
     """
     Return results on or before this
     [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) timestamp.
     """
-
-
-class ACHPrenotificationListParams(TypedDict, total=False):
-    created_at: CreatedAt
-
-    cursor: str
-    """Return the page of entries after this one."""
-
-    limit: int
-    """Limit the size of the list that is returned.
-
-    The default (and maximum) is 100 objects.
-    """
```

### Comparing `increase-0.6.0/src/increase/types/ach_transfer.py` & `increase-0.6.1/src/increase/types/ach_transfer.py`

 * *Files 21% similar despite different names*

```diff
@@ -56,14 +56,17 @@
 class Return(BaseModel):
     created_at: datetime
     """
     The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
     the transfer was created.
     """
 
+    raw_return_reason_code: str
+    """The three character ACH return code, in the range R01 to R85."""
+
     return_reason_code: Literal[
         "insufficient_fund",
         "no_account",
         "account_closed",
         "invalid_account_number_structure",
         "account_frozen_entry_returned_per_ofac_instruction",
         "credit_entry_refused_by_receiver",
@@ -76,18 +79,66 @@
         "customer_advised_unauthorized_improper_ineligible_or_incomplete",
         "amount_field_error",
         "authorization_revoked_by_customer",
         "invalid_ach_routing_number",
         "file_record_edit_criteria",
         "enr_invalid_individual_name",
         "returned_per_odfi_request",
-        "addenda_error",
         "limited_participation_dfi",
         "incorrectly_coded_outbound_international_payment",
         "other",
+        "account_sold_to_another_dfi",
+        "addenda_error",
+        "beneficiary_or_account_holder_deceased",
+        "check_truncation_entry_return",
+        "corrected_return",
+        "duplicate_entry",
+        "duplicate_return",
+        "enr_duplicate_enrollment",
+        "enr_invalid_dfi_account_number",
+        "enr_invalid_individual_id_number",
+        "enr_invalid_representative_payee_indicator",
+        "enr_invalid_transaction_code",
+        "enr_return_of_enr_entry",
+        "enr_routing_number_check_digit_error",
+        "entry_not_processed_by_gateway",
+        "field_error",
+        "foreign_receiving_dfi_unable_to_settle",
+        "iat_entry_coding_error",
+        "improper_effective_entry_date",
+        "improper_source_document_source_document_presented",
+        "invalid_company_id",
+        "invalid_foreign_receiving_dfi_identification",
+        "invalid_individual_id_number",
+        "item_and_rck_entry_presented_for_payment",
+        "item_related_to_rck_entry_is_ineligible",
+        "mandatory_field_error",
+        "misrouted_dishonored_return",
+        "misrouted_return",
+        "no_errors_found",
+        "non_acceptance_of_r62_dishonored_return",
+        "non_participant_in_iat_program",
+        "permissible_return_entry",
+        "permissible_return_entry_not_accepted",
+        "rdfi_non_settlement",
+        "rdfi_participant_in_check_truncation_program",
+        "representative_payee_deceased_or_unable_to_continue_in_that_capacity",
+        "return_not_a_duplicate",
+        "return_of_erroneous_or_reversing_debit",
+        "return_of_improper_credit_entry",
+        "return_of_improper_debit_entry",
+        "return_of_xck_entry",
+        "source_document_presented_for_payment",
+        "state_law_affecting_rck_acceptance",
+        "stop_payment_on_item_related_to_rck_entry",
+        "stop_payment_on_source_document",
+        "timely_original_return",
+        "trace_number_error",
+        "untimely_dishonored_return",
+        "untimely_return",
     ]
     """Why the ACH Transfer was returned."""
 
     transaction_id: str
     """The identifier of the Tranasaction associated with this return."""
 
     transfer_id: str
```

### Comparing `increase-0.6.0/src/increase/types/ach_transfer_create_params.py` & `increase-0.6.1/src/increase/types/ach_transfer_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/types/ach_transfer_list_params.py` & `increase-0.6.1/src/increase/types/ach_transfer_list_params.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,33 @@
 from typing_extensions import Annotated, TypedDict
 
 from .._utils import PropertyInfo
 
 __all__ = ["ACHTransferListParams", "CreatedAt"]
 
 
+class ACHTransferListParams(TypedDict, total=False):
+    account_id: str
+    """Filter ACH Transfers to those that originated from the specified Account."""
+
+    created_at: CreatedAt
+
+    cursor: str
+    """Return the page of entries after this one."""
+
+    external_account_id: str
+    """Filter ACH Transfers to those made to the specified External Account."""
+
+    limit: int
+    """Limit the size of the list that is returned.
+
+    The default (and maximum) is 100 objects.
+    """
+
+
 class CreatedAt(TypedDict, total=False):
     after: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
     """
     Return results after this [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601)
     timestamp.
     """
 
@@ -31,26 +50,7 @@
     """
 
     on_or_before: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
     """
     Return results on or before this
     [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) timestamp.
     """
-
-
-class ACHTransferListParams(TypedDict, total=False):
-    account_id: str
-    """Filter ACH Transfers to those that originated from the specified Account."""
-
-    created_at: CreatedAt
-
-    cursor: str
-    """Return the page of entries after this one."""
-
-    external_account_id: str
-    """Filter ACH Transfers to those made to the specified External Account."""
-
-    limit: int
-    """Limit the size of the list that is returned.
-
-    The default (and maximum) is 100 objects.
-    """
```

### Comparing `increase-0.6.0/src/increase/types/balance_lookup_lookup_params.py` & `increase-0.6.1/src/increase/types/balance_lookup_lookup_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/types/balance_lookup_lookup_response.py` & `increase-0.6.1/src/increase/types/balance_lookup_lookup_response.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/types/bookkeeping_account.py` & `increase-0.6.1/src/increase/types/bookkeeping_account.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/types/bookkeeping_account_create_params.py` & `increase-0.6.1/src/increase/types/bookkeeping_account_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/types/bookkeeping_entry.py` & `increase-0.6.1/src/increase/types/bookkeeping_entry.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/types/bookkeeping_entry_set.py` & `increase-0.6.1/src/increase/types/bookkeeping_entry_set.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/types/bookkeeping_entry_set_create_params.py` & `increase-0.6.1/src/increase/types/bookkeeping_entry_set_create_params.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,32 +7,32 @@
 from typing_extensions import Required, Annotated, TypedDict
 
 from .._utils import PropertyInfo
 
 __all__ = ["BookkeepingEntrySetCreateParams", "Entry"]
 
 
-class Entry(TypedDict, total=False):
-    account_id: Required[str]
-    """The identifier for the Bookkeeping Account impacted by this entry."""
-
-    amount: Required[int]
-    """The entry amount in the minor unit of the account currency.
-
-    For dollars, for example, this is cents. Debit entries have positive amounts;
-    credit entries have negative amounts.
-    """
-
-
 class BookkeepingEntrySetCreateParams(TypedDict, total=False):
     entries: Required[List[Entry]]
     """The bookkeeping entries."""
 
     date: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
     """The date of the transaction.
 
     If `transaction_id` is provided, this must match the `created_at` field on that
     resource.
     """
 
     transaction_id: str
     """The identifier of the Transaction related to this entry set, if any."""
+
+
+class Entry(TypedDict, total=False):
+    account_id: Required[str]
+    """The identifier for the Bookkeeping Account impacted by this entry."""
+
+    amount: Required[int]
+    """The entry amount in the minor unit of the account currency.
+
+    For dollars, for example, this is cents. Debit entries have positive amounts;
+    credit entries have negative amounts.
+    """
```

### Comparing `increase-0.6.0/src/increase/types/card.py` & `increase-0.6.1/src/increase/types/card.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/types/card_create_params.py` & `increase-0.6.1/src/increase/types/card_create_params.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,34 @@
 from __future__ import annotations
 
 from typing_extensions import Required, TypedDict
 
 __all__ = ["CardCreateParams", "BillingAddress", "DigitalWallet"]
 
 
+class CardCreateParams(TypedDict, total=False):
+    account_id: Required[str]
+    """The Account the card should belong to."""
+
+    billing_address: BillingAddress
+    """The card's billing address."""
+
+    description: str
+    """The description you choose to give the card."""
+
+    digital_wallet: DigitalWallet
+    """
+    The contact information used in the two-factor steps for digital wallet card
+    creation. To add the card to a digital wallet, you may supply an email or phone
+    number with this request. Otherwise, subscribe and then action a Real Time
+    Decision with the category `digital_wallet_token_requested` or
+    `digital_wallet_authentication_requested`.
+    """
+
+
 class BillingAddress(TypedDict, total=False):
     city: Required[str]
     """The city of the billing address."""
 
     line1: Required[str]
     """The first line of the billing address."""
 
@@ -38,27 +58,7 @@
     """
 
     phone: str
     """
     A phone number that can be used to verify the cardholder via one-time passcode
     over SMS.
     """
-
-
-class CardCreateParams(TypedDict, total=False):
-    account_id: Required[str]
-    """The Account the card should belong to."""
-
-    billing_address: BillingAddress
-    """The card's billing address."""
-
-    description: str
-    """The description you choose to give the card."""
-
-    digital_wallet: DigitalWallet
-    """
-    The contact information used in the two-factor steps for digital wallet card
-    creation. To add the card to a digital wallet, you may supply an email or phone
-    number with this request. Otherwise, subscribe and then action a Real Time
-    Decision with the category `digital_wallet_token_requested` or
-    `digital_wallet_authentication_requested`.
-    """
```

### Comparing `increase-0.6.0/src/increase/types/card_details.py` & `increase-0.6.1/src/increase/types/card_details.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/types/card_dispute.py` & `increase-0.6.1/src/increase/types/card_dispute.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/types/card_dispute_list_params.py` & `increase-0.6.1/src/increase/types/card_dispute_list_params.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,29 @@
 from typing_extensions import Literal, Annotated, TypedDict
 
 from .._utils import PropertyInfo
 
 __all__ = ["CardDisputeListParams", "CreatedAt", "Status"]
 
 
+class CardDisputeListParams(TypedDict, total=False):
+    created_at: CreatedAt
+
+    cursor: str
+    """Return the page of entries after this one."""
+
+    limit: int
+    """Limit the size of the list that is returned.
+
+    The default (and maximum) is 100 objects.
+    """
+
+    status: Status
+
+
 class CreatedAt(TypedDict, total=False):
     after: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
     """
     Return results after this [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601)
     timestamp.
     """
 
@@ -44,22 +59,7 @@
     },
     total=False,
 )
 
 
 class Status(_StatusReservedKeywords, total=False):
     pass
-
-
-class CardDisputeListParams(TypedDict, total=False):
-    created_at: CreatedAt
-
-    cursor: str
-    """Return the page of entries after this one."""
-
-    limit: int
-    """Limit the size of the list that is returned.
-
-    The default (and maximum) is 100 objects.
-    """
-
-    status: Status
```

### Comparing `increase-0.6.0/src/increase/types/card_list_params.py` & `increase-0.6.1/src/increase/types/card_list_params.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,30 @@
 from typing_extensions import Annotated, TypedDict
 
 from .._utils import PropertyInfo
 
 __all__ = ["CardListParams", "CreatedAt"]
 
 
+class CardListParams(TypedDict, total=False):
+    account_id: str
+    """Filter Cards to ones belonging to the specified Account."""
+
+    created_at: CreatedAt
+
+    cursor: str
+    """Return the page of entries after this one."""
+
+    limit: int
+    """Limit the size of the list that is returned.
+
+    The default (and maximum) is 100 objects.
+    """
+
+
 class CreatedAt(TypedDict, total=False):
     after: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
     """
     Return results after this [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601)
     timestamp.
     """
 
@@ -31,23 +47,7 @@
     """
 
     on_or_before: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
     """
     Return results on or before this
     [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) timestamp.
     """
-
-
-class CardListParams(TypedDict, total=False):
-    account_id: str
-    """Filter Cards to ones belonging to the specified Account."""
-
-    created_at: CreatedAt
-
-    cursor: str
-    """Return the page of entries after this one."""
-
-    limit: int
-    """Limit the size of the list that is returned.
-
-    The default (and maximum) is 100 objects.
-    """
```

### Comparing `increase-0.6.0/src/increase/types/card_profile.py` & `increase-0.6.1/src/increase/types/card_profile.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/types/card_profile_create_params.py` & `increase-0.6.1/src/increase/types/card_profile_create_params.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,26 @@
 from __future__ import annotations
 
 from typing_extensions import Required, TypedDict
 
 __all__ = ["CardProfileCreateParams", "DigitalWallets", "DigitalWalletsTextColor"]
 
 
+class CardProfileCreateParams(TypedDict, total=False):
+    description: Required[str]
+    """A description you can use to identify the Card Profile."""
+
+    digital_wallets: Required[DigitalWallets]
+    """How Cards should appear in digital wallets such as Apple Pay.
+
+    Different wallets will use these values to render card artwork appropriately for
+    their app.
+    """
+
+
 class DigitalWalletsTextColor(TypedDict, total=False):
     blue: Required[int]
     """The value of the blue channel in the RGB color."""
 
     green: Required[int]
     """The value of the green channel in the RGB color."""
 
@@ -38,19 +50,7 @@
     """A phone number the user can contact to receive support for their card."""
 
     contact_website: str
     """A website the user can visit to view and receive support for their card."""
 
     text_color: DigitalWalletsTextColor
     """The Card's text color, specified as an RGB triple. The default is white."""
-
-
-class CardProfileCreateParams(TypedDict, total=False):
-    description: Required[str]
-    """A description you can use to identify the Card Profile."""
-
-    digital_wallets: Required[DigitalWallets]
-    """How Cards should appear in digital wallets such as Apple Pay.
-
-    Different wallets will use these values to render card artwork appropriately for
-    their app.
-    """
```

### Comparing `increase-0.6.0/src/increase/types/card_profile_list_params.py` & `increase-0.6.1/src/increase/types/card_profile_list_params.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,31 +3,32 @@
 from __future__ import annotations
 
 from typing import List
 from typing_extensions import Literal, TypedDict
 
 __all__ = ["CardProfileListParams", "Status"]
 
-_StatusReservedKeywords = TypedDict(
-    "_StatusReservedKeywords",
-    {
-        "in": List[Literal["pending", "rejected", "active", "archived"]],
-    },
-    total=False,
-)
-
-
-class Status(_StatusReservedKeywords, total=False):
-    pass
-
 
 class CardProfileListParams(TypedDict, total=False):
     cursor: str
     """Return the page of entries after this one."""
 
     limit: int
     """Limit the size of the list that is returned.
 
     The default (and maximum) is 100 objects.
     """
 
     status: Status
+
+
+_StatusReservedKeywords = TypedDict(
+    "_StatusReservedKeywords",
+    {
+        "in": List[Literal["pending", "rejected", "active", "archived"]],
+    },
+    total=False,
+)
+
+
+class Status(_StatusReservedKeywords, total=False):
+    pass
```

### Comparing `increase-0.6.0/src/increase/types/card_update_params.py` & `increase-0.6.1/src/increase/types/card_update_params.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,32 @@
 from __future__ import annotations
 
 from typing_extensions import Literal, Required, TypedDict
 
 __all__ = ["CardUpdateParams", "BillingAddress", "DigitalWallet"]
 
 
+class CardUpdateParams(TypedDict, total=False):
+    billing_address: BillingAddress
+    """The card's updated billing address."""
+
+    description: str
+    """The description you choose to give the card."""
+
+    digital_wallet: DigitalWallet
+    """
+    The contact information used in the two-factor steps for digital wallet card
+    creation. At least one field must be present to complete the digital wallet
+    steps.
+    """
+
+    status: Literal["active", "disabled", "canceled"]
+    """The status to update the Card with."""
+
+
 class BillingAddress(TypedDict, total=False):
     city: Required[str]
     """The city of the billing address."""
 
     line1: Required[str]
     """The first line of the billing address."""
 
@@ -38,25 +56,7 @@
     """
 
     phone: str
     """
     A phone number that can be used to verify the cardholder via one-time passcode
     over SMS.
     """
-
-
-class CardUpdateParams(TypedDict, total=False):
-    billing_address: BillingAddress
-    """The card's updated billing address."""
-
-    description: str
-    """The description you choose to give the card."""
-
-    digital_wallet: DigitalWallet
-    """
-    The contact information used in the two-factor steps for digital wallet card
-    creation. At least one field must be present to complete the digital wallet
-    steps.
-    """
-
-    status: Literal["active", "disabled", "canceled"]
-    """The status to update the Card with."""
```

### Comparing `increase-0.6.0/src/increase/types/check_deposit.py` & `increase-0.6.1/src/increase/types/check_deposit.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/types/check_deposit_create_params.py` & `increase-0.6.1/src/increase/types/check_deposit_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/types/check_deposit_list_params.py` & `increase-0.6.1/src/increase/types/check_deposit_list_params.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,30 @@
 from typing_extensions import Annotated, TypedDict
 
 from .._utils import PropertyInfo
 
 __all__ = ["CheckDepositListParams", "CreatedAt"]
 
 
+class CheckDepositListParams(TypedDict, total=False):
+    account_id: str
+    """Filter Check Deposits to those belonging to the specified Account."""
+
+    created_at: CreatedAt
+
+    cursor: str
+    """Return the page of entries after this one."""
+
+    limit: int
+    """Limit the size of the list that is returned.
+
+    The default (and maximum) is 100 objects.
+    """
+
+
 class CreatedAt(TypedDict, total=False):
     after: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
     """
     Return results after this [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601)
     timestamp.
     """
 
@@ -31,23 +47,7 @@
     """
 
     on_or_before: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
     """
     Return results on or before this
     [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) timestamp.
     """
-
-
-class CheckDepositListParams(TypedDict, total=False):
-    account_id: str
-    """Filter Check Deposits to those belonging to the specified Account."""
-
-    created_at: CreatedAt
-
-    cursor: str
-    """Return the page of entries after this one."""
-
-    limit: int
-    """Limit the size of the list that is returned.
-
-    The default (and maximum) is 100 objects.
-    """
```

### Comparing `increase-0.6.0/src/increase/types/check_transfer.py` & `increase-0.6.1/src/increase/types/check_transfer.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/types/check_transfer_create_params.py` & `increase-0.6.1/src/increase/types/check_transfer_create_params.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,34 +3,14 @@
 from __future__ import annotations
 
 from typing_extensions import Required, TypedDict
 
 __all__ = ["CheckTransferCreateParams", "ReturnAddress"]
 
 
-class ReturnAddress(TypedDict, total=False):
-    city: Required[str]
-    """The city of the return address."""
-
-    line1: Required[str]
-    """The first line of the return address."""
-
-    name: Required[str]
-    """The name of the return address."""
-
-    state: Required[str]
-    """The US state of the return address."""
-
-    zip: Required[str]
-    """The postal code of the return address."""
-
-    line2: str
-    """The second line of the return address."""
-
-
 class CheckTransferCreateParams(TypedDict, total=False):
     account_id: Required[str]
     """The identifier for the account that will send the transfer."""
 
     address_city: Required[str]
     """The city of the check's destination."""
 
@@ -63,7 +43,27 @@
 
     return_address: ReturnAddress
     """The return address to be printed on the check.
 
     If omitted this will default to the address of the Entity of the Account used to
     make the Check Transfer.
     """
+
+
+class ReturnAddress(TypedDict, total=False):
+    city: Required[str]
+    """The city of the return address."""
+
+    line1: Required[str]
+    """The first line of the return address."""
+
+    name: Required[str]
+    """The name of the return address."""
+
+    state: Required[str]
+    """The US state of the return address."""
+
+    zip: Required[str]
+    """The postal code of the return address."""
+
+    line2: str
+    """The second line of the return address."""
```

### Comparing `increase-0.6.0/src/increase/types/check_transfer_list_params.py` & `increase-0.6.1/src/increase/types/check_transfer_list_params.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,30 @@
 from typing_extensions import Annotated, TypedDict
 
 from .._utils import PropertyInfo
 
 __all__ = ["CheckTransferListParams", "CreatedAt"]
 
 
+class CheckTransferListParams(TypedDict, total=False):
+    account_id: str
+    """Filter Check Transfers to those that originated from the specified Account."""
+
+    created_at: CreatedAt
+
+    cursor: str
+    """Return the page of entries after this one."""
+
+    limit: int
+    """Limit the size of the list that is returned.
+
+    The default (and maximum) is 100 objects.
+    """
+
+
 class CreatedAt(TypedDict, total=False):
     after: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
     """
     Return results after this [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601)
     timestamp.
     """
 
@@ -31,23 +47,7 @@
     """
 
     on_or_before: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
     """
     Return results on or before this
     [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) timestamp.
     """
-
-
-class CheckTransferListParams(TypedDict, total=False):
-    account_id: str
-    """Filter Check Transfers to those that originated from the specified Account."""
-
-    created_at: CreatedAt
-
-    cursor: str
-    """Return the page of entries after this one."""
-
-    limit: int
-    """Limit the size of the list that is returned.
-
-    The default (and maximum) is 100 objects.
-    """
```

### Comparing `increase-0.6.0/src/increase/types/declined_transaction.py` & `increase-0.6.1/src/increase/types/declined_transaction.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,14 +177,15 @@
         "ach_route_canceled",
         "ach_route_disabled",
         "breaches_limit",
         "entity_not_active",
         "group_locked",
         "insufficient_funds",
         "unable_to_locate_account",
+        "not_our_item",
         "unable_to_process",
         "refer_to_image",
         "stop_payment_requested",
         "returned",
         "duplicate_presentment",
         "not_authorized",
         "altered_or_fictitious",
```

### Comparing `increase-0.6.0/src/increase/types/declined_transaction_list_params.py` & `increase-0.6.1/src/increase/types/declined_transaction_list_params.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,33 @@
 from typing_extensions import Annotated, TypedDict
 
 from .._utils import PropertyInfo
 
 __all__ = ["DeclinedTransactionListParams", "CreatedAt"]
 
 
+class DeclinedTransactionListParams(TypedDict, total=False):
+    account_id: str
+    """Filter Declined Transactions to ones belonging to the specified Account."""
+
+    created_at: CreatedAt
+
+    cursor: str
+    """Return the page of entries after this one."""
+
+    limit: int
+    """Limit the size of the list that is returned.
+
+    The default (and maximum) is 100 objects.
+    """
+
+    route_id: str
+    """Filter Declined Transactions to those belonging to the specified route."""
+
+
 class CreatedAt(TypedDict, total=False):
     after: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
     """
     Return results after this [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601)
     timestamp.
     """
 
@@ -31,26 +50,7 @@
     """
 
     on_or_before: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
     """
     Return results on or before this
     [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) timestamp.
     """
-
-
-class DeclinedTransactionListParams(TypedDict, total=False):
-    account_id: str
-    """Filter Declined Transactions to ones belonging to the specified Account."""
-
-    created_at: CreatedAt
-
-    cursor: str
-    """Return the page of entries after this one."""
-
-    limit: int
-    """Limit the size of the list that is returned.
-
-    The default (and maximum) is 100 objects.
-    """
-
-    route_id: str
-    """Filter Declined Transactions to those belonging to the specified route."""
```

### Comparing `increase-0.6.0/src/increase/types/digital_wallet_token.py` & `increase-0.6.1/src/increase/types/digital_wallet_token.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/types/digital_wallet_token_list_params.py` & `increase-0.6.1/src/increase/types/digital_wallet_token_list_params.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,30 @@
 from typing_extensions import Annotated, TypedDict
 
 from .._utils import PropertyInfo
 
 __all__ = ["DigitalWalletTokenListParams", "CreatedAt"]
 
 
+class DigitalWalletTokenListParams(TypedDict, total=False):
+    card_id: str
+    """Filter Digital Wallet Tokens to ones belonging to the specified Card."""
+
+    created_at: CreatedAt
+
+    cursor: str
+    """Return the page of entries after this one."""
+
+    limit: int
+    """Limit the size of the list that is returned.
+
+    The default (and maximum) is 100 objects.
+    """
+
+
 class CreatedAt(TypedDict, total=False):
     after: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
     """
     Return results after this [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601)
     timestamp.
     """
 
@@ -31,23 +47,7 @@
     """
 
     on_or_before: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
     """
     Return results on or before this
     [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) timestamp.
     """
-
-
-class DigitalWalletTokenListParams(TypedDict, total=False):
-    card_id: str
-    """Filter Digital Wallet Tokens to ones belonging to the specified Card."""
-
-    created_at: CreatedAt
-
-    cursor: str
-    """Return the page of entries after this one."""
-
-    limit: int
-    """Limit the size of the list that is returned.
-
-    The default (and maximum) is 100 objects.
-    """
```

### Comparing `increase-0.6.0/src/increase/types/document.py` & `increase-0.6.1/src/increase/types/document.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/types/document_list_params.py` & `increase-0.6.1/src/increase/types/document_list_params.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,33 @@
 from datetime import datetime
 from typing_extensions import Literal, Annotated, TypedDict
 
 from .._utils import PropertyInfo
 
 __all__ = ["DocumentListParams", "Category", "CreatedAt"]
 
+
+class DocumentListParams(TypedDict, total=False):
+    category: Category
+
+    created_at: CreatedAt
+
+    cursor: str
+    """Return the page of entries after this one."""
+
+    entity_id: str
+    """Filter Documents to ones belonging to the specified Entity."""
+
+    limit: int
+    """Limit the size of the list that is returned.
+
+    The default (and maximum) is 100 objects.
+    """
+
+
 _CategoryReservedKeywords = TypedDict(
     "_CategoryReservedKeywords",
     {
         "in": List[
             Literal[
                 "account_opening_disclosures",
                 "anti_money_laundering_policy",
@@ -95,25 +114,7 @@
     """
 
     on_or_before: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
     """
     Return results on or before this
     [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) timestamp.
     """
-
-
-class DocumentListParams(TypedDict, total=False):
-    category: Category
-
-    created_at: CreatedAt
-
-    cursor: str
-    """Return the page of entries after this one."""
-
-    entity_id: str
-    """Filter Documents to ones belonging to the specified Entity."""
-
-    limit: int
-    """Limit the size of the list that is returned.
-
-    The default (and maximum) is 100 objects.
-    """
```

### Comparing `increase-0.6.0/src/increase/types/entity.py` & `increase-0.6.1/src/increase/types/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from typing import List, Optional
-from datetime import date
+from datetime import date, datetime
 from typing_extensions import Literal
 
 from .._models import BaseModel
 
 __all__ = [
     "Entity",
     "Corporation",
@@ -391,17 +391,29 @@
     """The Employer Identification Number (EIN) of the trust itself."""
 
     trustees: List[TrustTrustee]
     """The trustees of the trust."""
 
 
 class SupplementalDocument(BaseModel):
+    created_at: datetime
+    """
+    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) time at which the
+    Supplemental Document was created.
+    """
+
     file_id: str
     """The File containing the document."""
 
+    type: Literal["entity_supplemental_document"]
+    """A constant representing the object's type.
+
+    For this resource it will always be `entity_supplemental_document`.
+    """
+
 
 class Entity(BaseModel):
     corporation: Optional[Corporation]
     """Details of the corporation entity.
 
     Will be present if `structure` is equal to `corporation`.
     """
@@ -427,15 +439,20 @@
     relationship: Literal["affiliated", "informational", "unaffiliated"]
     """The relationship between your group and the entity."""
 
     structure: Literal["corporation", "natural_person", "joint", "trust"]
     """The entity's legal structure."""
 
     supplemental_documents: List[SupplementalDocument]
-    """Additional documentation associated with the entity."""
+    """Additional documentation associated with the entity.
+
+    This is limited to the first 10 documents for an entity. If an entity has more
+    than 10 documents, use the GET /entity_supplemental_documents list endpoint to
+    retrieve them.
+    """
 
     trust: Optional[Trust]
     """Details of the trust entity.
 
     Will be present if `structure` is equal to `trust`.
     """
```

### Comparing `increase-0.6.0/src/increase/types/entity_create_params.py` & `increase-0.6.1/src/increase/types/entity_create_params.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -15,27 +15,28 @@
     "CorporationBeneficialOwner",
     "CorporationBeneficialOwnerIndividual",
     "CorporationBeneficialOwnerIndividualAddress",
     "CorporationBeneficialOwnerIndividualIdentification",
     "CorporationBeneficialOwnerIndividualIdentificationPassport",
     "CorporationBeneficialOwnerIndividualIdentificationDriversLicense",
     "CorporationBeneficialOwnerIndividualIdentificationOther",
-    "NaturalPerson",
-    "NaturalPersonAddress",
-    "NaturalPersonIdentification",
-    "NaturalPersonIdentificationPassport",
-    "NaturalPersonIdentificationDriversLicense",
-    "NaturalPersonIdentificationOther",
     "Joint",
     "JointIndividual",
     "JointIndividualAddress",
     "JointIndividualIdentification",
     "JointIndividualIdentificationPassport",
     "JointIndividualIdentificationDriversLicense",
     "JointIndividualIdentificationOther",
+    "NaturalPerson",
+    "NaturalPersonAddress",
+    "NaturalPersonIdentification",
+    "NaturalPersonIdentificationPassport",
+    "NaturalPersonIdentificationDriversLicense",
+    "NaturalPersonIdentificationOther",
+    "SupplementalDocument",
     "Trust",
     "TrustAddress",
     "TrustTrustee",
     "TrustTrusteeIndividual",
     "TrustTrusteeIndividualAddress",
     "TrustTrusteeIndividualIdentification",
     "TrustTrusteeIndividualIdentificationPassport",
@@ -43,18 +44,57 @@
     "TrustTrusteeIndividualIdentificationOther",
     "TrustGrantor",
     "TrustGrantorAddress",
     "TrustGrantorIdentification",
     "TrustGrantorIdentificationPassport",
     "TrustGrantorIdentificationDriversLicense",
     "TrustGrantorIdentificationOther",
-    "SupplementalDocument",
 ]
 
 
+class EntityCreateParams(TypedDict, total=False):
+    relationship: Required[Literal["affiliated", "informational", "unaffiliated"]]
+    """The relationship between your group and the entity."""
+
+    structure: Required[Literal["corporation", "natural_person", "joint", "trust"]]
+    """The type of Entity to create."""
+
+    corporation: Corporation
+    """Details of the corporation entity to create.
+
+    Required if `structure` is equal to `corporation`.
+    """
+
+    description: str
+    """The description you choose to give the entity."""
+
+    joint: Joint
+    """Details of the joint entity to create.
+
+    Required if `structure` is equal to `joint`.
+    """
+
+    natural_person: NaturalPerson
+    """Details of the natural person entity to create.
+
+    Required if `structure` is equal to `natural_person`. Natural people entities
+    should be submitted with `social_security_number` or
+    `individual_taxpayer_identification_number` identification methods.
+    """
+
+    supplemental_documents: List[SupplementalDocument]
+    """Additional documentation associated with the entity."""
+
+    trust: Trust
+    """Details of the trust entity to create.
+
+    Required if `structure` is equal to `trust`.
+    """
+
+
 class CorporationAddress(TypedDict, total=False):
     city: Required[str]
     """The city of the address."""
 
     line1: Required[str]
     """The first line of the address. This is usually the street number and street."""
 
@@ -222,15 +262,15 @@
     corporation's state of incorporation.
     """
 
     website: str
     """The website of the corporation."""
 
 
-class NaturalPersonAddress(TypedDict, total=False):
+class JointIndividualAddress(TypedDict, total=False):
     city: Required[str]
     """The city of the address."""
 
     line1: Required[str]
     """The first line of the address. This is usually the street number and street."""
 
     state: Required[str]
@@ -242,37 +282,37 @@
     zip: Required[str]
     """The ZIP code of the address."""
 
     line2: str
     """The second line of the address. This might be the floor or room number."""
 
 
-class NaturalPersonIdentificationPassport(TypedDict, total=False):
+class JointIndividualIdentificationPassport(TypedDict, total=False):
     country: Required[str]
     """The country that issued the passport."""
 
     expiration_date: Required[Annotated[Union[str, date], PropertyInfo(format="iso8601")]]
     """The passport's expiration date in YYYY-MM-DD format."""
 
     file_id: Required[str]
     """The identifier of the File containing the passport."""
 
 
-class NaturalPersonIdentificationDriversLicense(TypedDict, total=False):
+class JointIndividualIdentificationDriversLicense(TypedDict, total=False):
     expiration_date: Required[Annotated[Union[str, date], PropertyInfo(format="iso8601")]]
     """The driver's license's expiration date in YYYY-MM-DD format."""
 
     file_id: Required[str]
     """The identifier of the File containing the driver's license."""
 
     state: Required[str]
     """The state that issued the provided driver's license."""
 
 
-class NaturalPersonIdentificationOther(TypedDict, total=False):
+class JointIndividualIdentificationOther(TypedDict, total=False):
     country: Required[str]
     """
     The two-character ISO 3166-1 code representing the country that issued the
     document.
     """
 
     description: Required[str]
@@ -281,15 +321,15 @@
     file_id: Required[str]
     """The identifier of the File containing the document."""
 
     expiration_date: Annotated[Union[str, date], PropertyInfo(format="iso8601")]
     """The document's expiration date in YYYY-MM-DD format."""
 
 
-class NaturalPersonIdentification(TypedDict, total=False):
+class JointIndividualIdentification(TypedDict, total=False):
     method: Required[
         Literal[
             "social_security_number",
             "individual_taxpayer_identification_number",
             "passport",
             "drivers_license",
             "other",
@@ -299,56 +339,64 @@
 
     number: Required[str]
     """
     An identification number that can be used to verify the individual's identity,
     such as a social security number.
     """
 
-    drivers_license: NaturalPersonIdentificationDriversLicense
+    drivers_license: JointIndividualIdentificationDriversLicense
     """Information about the United States driver's license used for identification.
 
     Required if `method` is equal to `drivers_license`.
     """
 
-    other: NaturalPersonIdentificationOther
+    other: JointIndividualIdentificationOther
     """Information about the identification document provided.
 
     Required if `method` is equal to `other`.
     """
 
-    passport: NaturalPersonIdentificationPassport
+    passport: JointIndividualIdentificationPassport
     """Information about the passport used for identification.
 
     Required if `method` is equal to `passport`.
     """
 
 
-class NaturalPerson(TypedDict, total=False):
-    address: Required[NaturalPersonAddress]
+class JointIndividual(TypedDict, total=False):
+    address: Required[JointIndividualAddress]
     """The individual's address."""
 
     date_of_birth: Required[Annotated[Union[str, date], PropertyInfo(format="iso8601")]]
     """The person's date of birth in YYYY-MM-DD format."""
 
-    identification: Required[NaturalPersonIdentification]
+    identification: Required[JointIndividualIdentification]
     """A means of verifying the person's identity."""
 
     name: Required[str]
     """The person's legal name."""
 
     confirmed_no_us_tax_id: bool
     """
     The identification method for an individual can only be a passport, driver's
     license, or other document if you've confirmed the individual does not have a US
     tax id (either a Social Security Number or Individual Taxpayer Identification
     Number).
     """
 
 
-class JointIndividualAddress(TypedDict, total=False):
+class Joint(TypedDict, total=False):
+    individuals: Required[List[JointIndividual]]
+    """The two individuals that share control of the entity."""
+
+    name: str
+    """The name of the joint entity."""
+
+
+class NaturalPersonAddress(TypedDict, total=False):
     city: Required[str]
     """The city of the address."""
 
     line1: Required[str]
     """The first line of the address. This is usually the street number and street."""
 
     state: Required[str]
@@ -360,37 +408,37 @@
     zip: Required[str]
     """The ZIP code of the address."""
 
     line2: str
     """The second line of the address. This might be the floor or room number."""
 
 
-class JointIndividualIdentificationPassport(TypedDict, total=False):
+class NaturalPersonIdentificationPassport(TypedDict, total=False):
     country: Required[str]
     """The country that issued the passport."""
 
     expiration_date: Required[Annotated[Union[str, date], PropertyInfo(format="iso8601")]]
     """The passport's expiration date in YYYY-MM-DD format."""
 
     file_id: Required[str]
     """The identifier of the File containing the passport."""
 
 
-class JointIndividualIdentificationDriversLicense(TypedDict, total=False):
+class NaturalPersonIdentificationDriversLicense(TypedDict, total=False):
     expiration_date: Required[Annotated[Union[str, date], PropertyInfo(format="iso8601")]]
     """The driver's license's expiration date in YYYY-MM-DD format."""
 
     file_id: Required[str]
     """The identifier of the File containing the driver's license."""
 
     state: Required[str]
     """The state that issued the provided driver's license."""
 
 
-class JointIndividualIdentificationOther(TypedDict, total=False):
+class NaturalPersonIdentificationOther(TypedDict, total=False):
     country: Required[str]
     """
     The two-character ISO 3166-1 code representing the country that issued the
     document.
     """
 
     description: Required[str]
@@ -399,15 +447,15 @@
     file_id: Required[str]
     """The identifier of the File containing the document."""
 
     expiration_date: Annotated[Union[str, date], PropertyInfo(format="iso8601")]
     """The document's expiration date in YYYY-MM-DD format."""
 
 
-class JointIndividualIdentification(TypedDict, total=False):
+class NaturalPersonIdentification(TypedDict, total=False):
     method: Required[
         Literal[
             "social_security_number",
             "individual_taxpayer_identification_number",
             "passport",
             "drivers_license",
             "other",
@@ -417,61 +465,58 @@
 
     number: Required[str]
     """
     An identification number that can be used to verify the individual's identity,
     such as a social security number.
     """
 
-    drivers_license: JointIndividualIdentificationDriversLicense
+    drivers_license: NaturalPersonIdentificationDriversLicense
     """Information about the United States driver's license used for identification.
 
     Required if `method` is equal to `drivers_license`.
     """
 
-    other: JointIndividualIdentificationOther
+    other: NaturalPersonIdentificationOther
     """Information about the identification document provided.
 
     Required if `method` is equal to `other`.
     """
 
-    passport: JointIndividualIdentificationPassport
+    passport: NaturalPersonIdentificationPassport
     """Information about the passport used for identification.
 
     Required if `method` is equal to `passport`.
     """
 
 
-class JointIndividual(TypedDict, total=False):
-    address: Required[JointIndividualAddress]
+class NaturalPerson(TypedDict, total=False):
+    address: Required[NaturalPersonAddress]
     """The individual's address."""
 
     date_of_birth: Required[Annotated[Union[str, date], PropertyInfo(format="iso8601")]]
     """The person's date of birth in YYYY-MM-DD format."""
 
-    identification: Required[JointIndividualIdentification]
+    identification: Required[NaturalPersonIdentification]
     """A means of verifying the person's identity."""
 
     name: Required[str]
     """The person's legal name."""
 
     confirmed_no_us_tax_id: bool
     """
     The identification method for an individual can only be a passport, driver's
     license, or other document if you've confirmed the individual does not have a US
     tax id (either a Social Security Number or Individual Taxpayer Identification
     Number).
     """
 
 
-class Joint(TypedDict, total=False):
-    individuals: Required[List[JointIndividual]]
-    """The two individuals that share control of the entity."""
-
-    name: str
-    """The name of the joint entity."""
+class SupplementalDocument(TypedDict, total=False):
+    file_id: Required[str]
+    """The identifier of the File containing the document."""
 
 
 class TrustAddress(TypedDict, total=False):
     city: Required[str]
     """The city of the address."""
 
     line1: Required[str]
@@ -767,52 +812,7 @@
     """The grantor of the trust. Required if `category` is equal to `revocable`."""
 
     tax_identifier: str
     """The Employer Identification Number (EIN) for the trust.
 
     Required if `category` is equal to `irrevocable`.
     """
-
-
-class SupplementalDocument(TypedDict, total=False):
-    file_id: Required[str]
-    """The identifier of the File containing the document."""
-
-
-class EntityCreateParams(TypedDict, total=False):
-    relationship: Required[Literal["affiliated", "informational", "unaffiliated"]]
-    """The relationship between your group and the entity."""
-
-    structure: Required[Literal["corporation", "natural_person", "joint", "trust"]]
-    """The type of Entity to create."""
-
-    corporation: Corporation
-    """Details of the corporation entity to create.
-
-    Required if `structure` is equal to `corporation`.
-    """
-
-    description: str
-    """The description you choose to give the entity."""
-
-    joint: Joint
-    """Details of the joint entity to create.
-
-    Required if `structure` is equal to `joint`.
-    """
-
-    natural_person: NaturalPerson
-    """Details of the natural person entity to create.
-
-    Required if `structure` is equal to `natural_person`. Natural people entities
-    should be submitted with `social_security_number` or
-    `individual_taxpayer_identification_number` identification methods.
-    """
-
-    supplemental_documents: List[SupplementalDocument]
-    """Additional documentation associated with the entity."""
-
-    trust: Trust
-    """Details of the trust entity to create.
-
-    Required if `structure` is equal to `trust`.
-    """
```

### Comparing `increase-0.6.0/src/increase/types/entity_list_params.py` & `increase-0.6.1/src/increase/types/entity_list_params.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,27 @@
 from typing_extensions import Annotated, TypedDict
 
 from .._utils import PropertyInfo
 
 __all__ = ["EntityListParams", "CreatedAt"]
 
 
+class EntityListParams(TypedDict, total=False):
+    created_at: CreatedAt
+
+    cursor: str
+    """Return the page of entries after this one."""
+
+    limit: int
+    """Limit the size of the list that is returned.
+
+    The default (and maximum) is 100 objects.
+    """
+
+
 class CreatedAt(TypedDict, total=False):
     after: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
     """
     Return results after this [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601)
     timestamp.
     """
 
@@ -31,20 +44,7 @@
     """
 
     on_or_before: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
     """
     Return results on or before this
     [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) timestamp.
     """
-
-
-class EntityListParams(TypedDict, total=False):
-    created_at: CreatedAt
-
-    cursor: str
-    """Return the page of entries after this one."""
-
-    limit: int
-    """Limit the size of the list that is returned.
-
-    The default (and maximum) is 100 objects.
-    """
```

### Comparing `increase-0.6.0/src/increase/types/event.py` & `increase-0.6.1/src/increase/types/event.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/types/event_list_params.py` & `increase-0.6.1/src/increase/types/event_list_params.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,40 +4,32 @@
 
 from typing import List, Union
 from datetime import datetime
 from typing_extensions import Literal, Annotated, TypedDict
 
 from .._utils import PropertyInfo
 
-__all__ = ["EventListParams", "CreatedAt", "Category"]
+__all__ = ["EventListParams", "Category", "CreatedAt"]
 
 
-class CreatedAt(TypedDict, total=False):
-    after: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
-    """
-    Return results after this [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601)
-    timestamp.
-    """
+class EventListParams(TypedDict, total=False):
+    associated_object_id: str
+    """Filter Events to those belonging to the object with the provided identifier."""
 
-    before: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
-    """
-    Return results before this [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601)
-    timestamp.
-    """
+    category: Category
 
-    on_or_after: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
-    """
-    Return results on or after this
-    [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) timestamp.
-    """
+    created_at: CreatedAt
 
-    on_or_before: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
-    """
-    Return results on or before this
-    [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) timestamp.
+    cursor: str
+    """Return the page of entries after this one."""
+
+    limit: int
+    """Limit the size of the list that is returned.
+
+    The default (and maximum) is 100 objects.
     """
 
 
 _CategoryReservedKeywords = TypedDict(
     "_CategoryReservedKeywords",
     {
         "in": List[
@@ -99,23 +91,31 @@
 )
 
 
 class Category(_CategoryReservedKeywords, total=False):
     pass
 
 
-class EventListParams(TypedDict, total=False):
-    associated_object_id: str
-    """Filter Events to those belonging to the object with the provided identifier."""
-
-    category: Category
-
-    created_at: CreatedAt
+class CreatedAt(TypedDict, total=False):
+    after: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
+    """
+    Return results after this [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601)
+    timestamp.
+    """
 
-    cursor: str
-    """Return the page of entries after this one."""
+    before: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
+    """
+    Return results before this [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601)
+    timestamp.
+    """
 
-    limit: int
-    """Limit the size of the list that is returned.
+    on_or_after: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
+    """
+    Return results on or after this
+    [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) timestamp.
+    """
 
-    The default (and maximum) is 100 objects.
+    on_or_before: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
+    """
+    Return results on or before this
+    [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) timestamp.
     """
```

### Comparing `increase-0.6.0/src/increase/types/event_subscription.py` & `increase-0.6.1/src/increase/types/event_subscription.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/types/event_subscription_create_params.py` & `increase-0.6.1/src/increase/types/event_subscription_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/types/export.py` & `increase-0.6.1/src/increase/types/export.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/types/export_create_params.py` & `increase-0.6.1/src/increase/types/export_create_params.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,18 +4,35 @@
 
 from typing import Union
 from datetime import datetime
 from typing_extensions import Literal, Required, Annotated, TypedDict
 
 from .._utils import PropertyInfo
 
-__all__ = ["ExportCreateParams", "TransactionCsv", "TransactionCsvCreatedAt", "BalanceCsv", "BalanceCsvCreatedAt"]
+__all__ = ["ExportCreateParams", "BalanceCsv", "BalanceCsvCreatedAt", "TransactionCsv", "TransactionCsvCreatedAt"]
 
 
-class TransactionCsvCreatedAt(TypedDict, total=False):
+class ExportCreateParams(TypedDict, total=False):
+    category: Required[Literal["transaction_csv", "balance_csv"]]
+    """The type of Export to create."""
+
+    balance_csv: BalanceCsv
+    """Options for the created export.
+
+    Required if `category` is equal to `balance_csv`.
+    """
+
+    transaction_csv: TransactionCsv
+    """Options for the created export.
+
+    Required if `category` is equal to `transaction_csv`.
+    """
+
+
+class BalanceCsvCreatedAt(TypedDict, total=False):
     after: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
     """
     Return results after this [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601)
     timestamp.
     """
 
     before: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
@@ -33,23 +50,23 @@
     on_or_before: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
     """
     Return results on or before this
     [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) timestamp.
     """
 
 
-class TransactionCsv(TypedDict, total=False):
+class BalanceCsv(TypedDict, total=False):
     account_id: str
     """Filter exported Transactions to the specified Account."""
 
-    created_at: TransactionCsvCreatedAt
+    created_at: BalanceCsvCreatedAt
     """Filter results by time range on the `created_at` attribute."""
 
 
-class BalanceCsvCreatedAt(TypedDict, total=False):
+class TransactionCsvCreatedAt(TypedDict, total=False):
     after: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
     """
     Return results after this [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601)
     timestamp.
     """
 
     before: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
@@ -67,30 +84,13 @@
     on_or_before: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
     """
     Return results on or before this
     [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) timestamp.
     """
 
 
-class BalanceCsv(TypedDict, total=False):
+class TransactionCsv(TypedDict, total=False):
     account_id: str
     """Filter exported Transactions to the specified Account."""
 
-    created_at: BalanceCsvCreatedAt
+    created_at: TransactionCsvCreatedAt
     """Filter results by time range on the `created_at` attribute."""
-
-
-class ExportCreateParams(TypedDict, total=False):
-    category: Required[Literal["transaction_csv", "balance_csv"]]
-    """The type of Export to create."""
-
-    balance_csv: BalanceCsv
-    """Options for the created export.
-
-    Required if `category` is equal to `balance_csv`.
-    """
-
-    transaction_csv: TransactionCsv
-    """Options for the created export.
-
-    Required if `category` is equal to `transaction_csv`.
-    """
```

### Comparing `increase-0.6.0/src/increase/types/external_account.py` & `increase-0.6.1/src/increase/types/external_account.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/types/external_account_create_params.py` & `increase-0.6.1/src/increase/types/external_account_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/types/external_account_list_params.py` & `increase-0.6.1/src/increase/types/external_account_list_params.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,31 +3,32 @@
 from __future__ import annotations
 
 from typing import List
 from typing_extensions import Literal, TypedDict
 
 __all__ = ["ExternalAccountListParams", "Status"]
 
-_StatusReservedKeywords = TypedDict(
-    "_StatusReservedKeywords",
-    {
-        "in": List[Literal["active", "archived"]],
-    },
-    total=False,
-)
-
-
-class Status(_StatusReservedKeywords, total=False):
-    pass
-
 
 class ExternalAccountListParams(TypedDict, total=False):
     cursor: str
     """Return the page of entries after this one."""
 
     limit: int
     """Limit the size of the list that is returned.
 
     The default (and maximum) is 100 objects.
     """
 
     status: Status
+
+
+_StatusReservedKeywords = TypedDict(
+    "_StatusReservedKeywords",
+    {
+        "in": List[Literal["active", "archived"]],
+    },
+    total=False,
+)
+
+
+class Status(_StatusReservedKeywords, total=False):
+    pass
```

### Comparing `increase-0.6.0/src/increase/types/file.py` & `increase-0.6.1/src/increase/types/file.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/types/file_create_params.py` & `increase-0.6.1/src/increase/types/file_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/types/file_list_params.py` & `increase-0.6.1/src/increase/types/file_list_params.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,29 @@
 from typing_extensions import Literal, Annotated, TypedDict
 
 from .._utils import PropertyInfo
 
 __all__ = ["FileListParams", "CreatedAt", "Purpose"]
 
 
+class FileListParams(TypedDict, total=False):
+    created_at: CreatedAt
+
+    cursor: str
+    """Return the page of entries after this one."""
+
+    limit: int
+    """Limit the size of the list that is returned.
+
+    The default (and maximum) is 100 objects.
+    """
+
+    purpose: Purpose
+
+
 class CreatedAt(TypedDict, total=False):
     after: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
     """
     Return results after this [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601)
     timestamp.
     """
 
@@ -60,22 +75,7 @@
     },
     total=False,
 )
 
 
 class Purpose(_PurposeReservedKeywords, total=False):
     pass
-
-
-class FileListParams(TypedDict, total=False):
-    created_at: CreatedAt
-
-    cursor: str
-    """Return the page of entries after this one."""
-
-    limit: int
-    """Limit the size of the list that is returned.
-
-    The default (and maximum) is 100 objects.
-    """
-
-    purpose: Purpose
```

### Comparing `increase-0.6.0/src/increase/types/group.py` & `increase-0.6.1/src/increase/types/group.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/types/inbound_ach_transfer_return.py` & `increase-0.6.1/src/increase/types/inbound_ach_transfer_return.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/types/inbound_ach_transfer_return_create_params.py` & `increase-0.6.1/src/increase/types/inbound_ach_transfer_return_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/types/inbound_wire_drawdown_request.py` & `increase-0.6.1/src/increase/types/inbound_wire_drawdown_request.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/types/limit.py` & `increase-0.6.1/src/increase/types/limit.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/types/limit_create_params.py` & `increase-0.6.1/src/increase/types/limit_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/types/limit_list_params.py` & `increase-0.6.1/src/increase/types/limit_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/types/oauth_connection.py` & `increase-0.6.1/src/increase/types/oauth_connection.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/types/pending_transaction.py` & `increase-0.6.1/src/increase/types/pending_transaction.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/types/pending_transaction_list_params.py` & `increase-0.6.1/src/increase/types/pending_transaction_list_params.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,27 +4,39 @@
 
 from typing import List, Union
 from datetime import datetime
 from typing_extensions import Literal, Annotated, TypedDict
 
 from .._utils import PropertyInfo
 
-__all__ = ["PendingTransactionListParams", "Status", "CreatedAt"]
+__all__ = ["PendingTransactionListParams", "CreatedAt", "Status"]
 
-_StatusReservedKeywords = TypedDict(
-    "_StatusReservedKeywords",
-    {
-        "in": List[Literal["pending", "complete"]],
-    },
-    total=False,
-)
 
+class PendingTransactionListParams(TypedDict, total=False):
+    account_id: str
+    """Filter pending transactions to those belonging to the specified Account."""
 
-class Status(_StatusReservedKeywords, total=False):
-    pass
+    created_at: CreatedAt
+
+    cursor: str
+    """Return the page of entries after this one."""
+
+    limit: int
+    """Limit the size of the list that is returned.
+
+    The default (and maximum) is 100 objects.
+    """
+
+    route_id: str
+    """Filter pending transactions to those belonging to the specified Route."""
+
+    source_id: str
+    """Filter pending transactions to those caused by the specified source."""
+
+    status: Status
 
 
 class CreatedAt(TypedDict, total=False):
     after: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
     """
     Return results after this [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601)
     timestamp.
@@ -45,29 +57,18 @@
     on_or_before: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
     """
     Return results on or before this
     [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) timestamp.
     """
 
 
-class PendingTransactionListParams(TypedDict, total=False):
-    account_id: str
-    """Filter pending transactions to those belonging to the specified Account."""
-
-    created_at: CreatedAt
-
-    cursor: str
-    """Return the page of entries after this one."""
-
-    limit: int
-    """Limit the size of the list that is returned.
-
-    The default (and maximum) is 100 objects.
-    """
-
-    route_id: str
-    """Filter pending transactions to those belonging to the specified Route."""
+_StatusReservedKeywords = TypedDict(
+    "_StatusReservedKeywords",
+    {
+        "in": List[Literal["pending", "complete"]],
+    },
+    total=False,
+)
 
-    source_id: str
-    """Filter pending transactions to those caused by the specified source."""
 
-    status: Status
+class Status(_StatusReservedKeywords, total=False):
+    pass
```

### Comparing `increase-0.6.0/src/increase/types/program.py` & `increase-0.6.1/src/increase/types/program.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/types/real_time_decision.py` & `increase-0.6.1/src/increase/types/real_time_decision.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/types/real_time_decision_action_params.py` & `increase-0.6.1/src/increase/types/real_time_decision_action_params.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,26 +3,51 @@
 from __future__ import annotations
 
 from typing_extensions import Literal, Required, TypedDict
 
 __all__ = [
     "RealTimeDecisionActionParams",
     "CardAuthorization",
+    "DigitalWalletAuthentication",
     "DigitalWalletToken",
     "DigitalWalletTokenApproval",
     "DigitalWalletTokenDecline",
-    "DigitalWalletAuthentication",
 ]
 
 
+class RealTimeDecisionActionParams(TypedDict, total=False):
+    card_authorization: CardAuthorization
+    """
+    If the Real-Time Decision relates to a card authorization attempt, this object
+    contains your response to the authorization.
+    """
+
+    digital_wallet_authentication: DigitalWalletAuthentication
+    """
+    If the Real-Time Decision relates to a digital wallet authentication attempt,
+    this object contains your response to the authentication.
+    """
+
+    digital_wallet_token: DigitalWalletToken
+    """
+    If the Real-Time Decision relates to a digital wallet token provisioning
+    attempt, this object contains your response to the attempt.
+    """
+
+
 class CardAuthorization(TypedDict, total=False):
     decision: Required[Literal["approve", "decline"]]
     """Whether the card authorization should be approved or declined."""
 
 
+class DigitalWalletAuthentication(TypedDict, total=False):
+    result: Required[Literal["success", "failure"]]
+    """Whether your application was able to deliver the one-time passcode."""
+
+
 class DigitalWalletTokenApproval(TypedDict, total=False):
     card_profile_id: Required[str]
     """The identifier of the Card Profile to assign to the Digital Wallet token."""
 
     email: str
     """
     An email address that can be used to verify the cardholder via one-time
@@ -52,32 +77,7 @@
     """
 
     decline: DigitalWalletTokenDecline
     """
     If your application declines the provisioning attempt, this contains details
     about the decline.
     """
-
-
-class DigitalWalletAuthentication(TypedDict, total=False):
-    result: Required[Literal["success", "failure"]]
-    """Whether your application was able to deliver the one-time passcode."""
-
-
-class RealTimeDecisionActionParams(TypedDict, total=False):
-    card_authorization: CardAuthorization
-    """
-    If the Real-Time Decision relates to a card authorization attempt, this object
-    contains your response to the authorization.
-    """
-
-    digital_wallet_authentication: DigitalWalletAuthentication
-    """
-    If the Real-Time Decision relates to a digital wallet authentication attempt,
-    this object contains your response to the authentication.
-    """
-
-    digital_wallet_token: DigitalWalletToken
-    """
-    If the Real-Time Decision relates to a digital wallet token provisioning
-    attempt, this object contains your response to the attempt.
-    """
```

### Comparing `increase-0.6.0/src/increase/types/real_time_payments_transfer.py` & `increase-0.6.1/src/increase/types/real_time_payments_transfer.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/types/real_time_payments_transfer_create_params.py` & `increase-0.6.1/src/increase/types/real_time_payments_transfer_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/types/real_time_payments_transfer_list_params.py` & `increase-0.6.1/src/increase/types/real_time_payments_transfer_list_params.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,38 @@
 from typing_extensions import Annotated, TypedDict
 
 from .._utils import PropertyInfo
 
 __all__ = ["RealTimePaymentsTransferListParams", "CreatedAt"]
 
 
+class RealTimePaymentsTransferListParams(TypedDict, total=False):
+    account_id: str
+    """
+    Filter Real Time Payments Transfers to those belonging to the specified Account.
+    """
+
+    created_at: CreatedAt
+
+    cursor: str
+    """Return the page of entries after this one."""
+
+    external_account_id: str
+    """
+    Filter Real Time Payments Transfers to those made to the specified External
+    Account.
+    """
+
+    limit: int
+    """Limit the size of the list that is returned.
+
+    The default (and maximum) is 100 objects.
+    """
+
+
 class CreatedAt(TypedDict, total=False):
     after: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
     """
     Return results after this [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601)
     timestamp.
     """
 
@@ -31,31 +55,7 @@
     """
 
     on_or_before: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
     """
     Return results on or before this
     [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) timestamp.
     """
-
-
-class RealTimePaymentsTransferListParams(TypedDict, total=False):
-    account_id: str
-    """
-    Filter Real Time Payments Transfers to those belonging to the specified Account.
-    """
-
-    created_at: CreatedAt
-
-    cursor: str
-    """Return the page of entries after this one."""
-
-    external_account_id: str
-    """
-    Filter Real Time Payments Transfers to those made to the specified External
-    Account.
-    """
-
-    limit: int
-    """Limit the size of the list that is returned.
-
-    The default (and maximum) is 100 objects.
-    """
```

### Comparing `increase-0.6.0/src/increase/types/routing_number.py` & `increase-0.6.1/src/increase/types/routing_number.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/types/routing_number_list_params.py` & `increase-0.6.1/src/increase/types/routing_number_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/types/shared_params/point_of_service_entry_mode.py` & `increase-0.6.1/src/increase/types/shared_params/point_of_service_entry_mode.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/types/simulations/__init__.py` & `increase-0.6.1/src/increase/types/simulations/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
 from .card_authorize_params import CardAuthorizeParams as CardAuthorizeParams
+from .program_create_params import ProgramCreateParams as ProgramCreateParams
 from .card_settlement_params import CardSettlementParams as CardSettlementParams
 from .document_create_params import DocumentCreateParams as DocumentCreateParams
 from .ach_transfer_simulation import ACHTransferSimulation as ACHTransferSimulation
 from .wire_transfer_simulation import WireTransferSimulation as WireTransferSimulation
 from .card_refund_create_params import CardRefundCreateParams as CardRefundCreateParams
 from .ach_transfer_return_params import (
     ACHTransferReturnParams as ACHTransferReturnParams,
```

### Comparing `increase-0.6.0/src/increase/types/simulations/ach_transfer_create_inbound_params.py` & `increase-0.6.1/src/increase/types/simulations/ach_transfer_create_inbound_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/types/simulations/ach_transfer_simulation.py` & `increase-0.6.1/src/increase/types/simulations/ach_transfer_simulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,14 +135,17 @@
 class TransactionSourceACHTransferReturn(BaseModel):
     created_at: datetime
     """
     The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
     the transfer was created.
     """
 
+    raw_return_reason_code: str
+    """The three character ACH return code, in the range R01 to R85."""
+
     return_reason_code: Literal[
         "insufficient_fund",
         "no_account",
         "account_closed",
         "invalid_account_number_structure",
         "account_frozen_entry_returned_per_ofac_instruction",
         "credit_entry_refused_by_receiver",
@@ -155,18 +158,66 @@
         "customer_advised_unauthorized_improper_ineligible_or_incomplete",
         "amount_field_error",
         "authorization_revoked_by_customer",
         "invalid_ach_routing_number",
         "file_record_edit_criteria",
         "enr_invalid_individual_name",
         "returned_per_odfi_request",
-        "addenda_error",
         "limited_participation_dfi",
         "incorrectly_coded_outbound_international_payment",
         "other",
+        "account_sold_to_another_dfi",
+        "addenda_error",
+        "beneficiary_or_account_holder_deceased",
+        "check_truncation_entry_return",
+        "corrected_return",
+        "duplicate_entry",
+        "duplicate_return",
+        "enr_duplicate_enrollment",
+        "enr_invalid_dfi_account_number",
+        "enr_invalid_individual_id_number",
+        "enr_invalid_representative_payee_indicator",
+        "enr_invalid_transaction_code",
+        "enr_return_of_enr_entry",
+        "enr_routing_number_check_digit_error",
+        "entry_not_processed_by_gateway",
+        "field_error",
+        "foreign_receiving_dfi_unable_to_settle",
+        "iat_entry_coding_error",
+        "improper_effective_entry_date",
+        "improper_source_document_source_document_presented",
+        "invalid_company_id",
+        "invalid_foreign_receiving_dfi_identification",
+        "invalid_individual_id_number",
+        "item_and_rck_entry_presented_for_payment",
+        "item_related_to_rck_entry_is_ineligible",
+        "mandatory_field_error",
+        "misrouted_dishonored_return",
+        "misrouted_return",
+        "no_errors_found",
+        "non_acceptance_of_r62_dishonored_return",
+        "non_participant_in_iat_program",
+        "permissible_return_entry",
+        "permissible_return_entry_not_accepted",
+        "rdfi_non_settlement",
+        "rdfi_participant_in_check_truncation_program",
+        "representative_payee_deceased_or_unable_to_continue_in_that_capacity",
+        "return_not_a_duplicate",
+        "return_of_erroneous_or_reversing_debit",
+        "return_of_improper_credit_entry",
+        "return_of_improper_debit_entry",
+        "return_of_xck_entry",
+        "source_document_presented_for_payment",
+        "state_law_affecting_rck_acceptance",
+        "stop_payment_on_item_related_to_rck_entry",
+        "stop_payment_on_source_document",
+        "timely_original_return",
+        "trace_number_error",
+        "untimely_dishonored_return",
+        "untimely_return",
     ]
     """Why the ACH Transfer was returned."""
 
     transaction_id: str
     """The identifier of the Tranasaction associated with this return."""
 
     transfer_id: str
@@ -862,14 +913,15 @@
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the transaction
     currency.
     """
 
     reason: Literal[
+        "account_closure",
         "bank_migration",
         "cashback",
         "collection_receivable",
         "empyreal_adjustment",
         "error",
         "error_correction",
         "fees",
@@ -1514,14 +1566,15 @@
         "ach_route_canceled",
         "ach_route_disabled",
         "breaches_limit",
         "entity_not_active",
         "group_locked",
         "insufficient_funds",
         "unable_to_locate_account",
+        "not_our_item",
         "unable_to_process",
         "refer_to_image",
         "stop_payment_requested",
         "returned",
         "duplicate_presentment",
         "not_authorized",
         "altered_or_fictitious",
```

### Comparing `increase-0.6.0/src/increase/types/simulations/card_authorization_simulation.py` & `increase-0.6.1/src/increase/types/simulations/card_authorization_simulation.py`

 * *Files 0% similar despite different names*

```diff
@@ -635,14 +635,15 @@
         "ach_route_canceled",
         "ach_route_disabled",
         "breaches_limit",
         "entity_not_active",
         "group_locked",
         "insufficient_funds",
         "unable_to_locate_account",
+        "not_our_item",
         "unable_to_process",
         "refer_to_image",
         "stop_payment_requested",
         "returned",
         "duplicate_presentment",
         "not_authorized",
         "altered_or_fictitious",
```

### Comparing `increase-0.6.0/src/increase/types/simulations/card_authorize_params.py` & `increase-0.6.1/src/increase/types/simulations/card_authorize_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/types/simulations/card_settlement_params.py` & `increase-0.6.1/src/increase/types/simulations/card_settlement_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/types/simulations/digital_wallet_token_request_create_response.py` & `increase-0.6.1/src/increase/types/simulations/digital_wallet_token_request_create_response.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/types/simulations/inbound_real_time_payments_transfer_simulation_result.py` & `increase-0.6.1/src/increase/types/simulations/inbound_real_time_payments_transfer_simulation_result.py`

 * *Files 3% similar despite different names*

```diff
@@ -135,14 +135,17 @@
 class TransactionSourceACHTransferReturn(BaseModel):
     created_at: datetime
     """
     The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
     the transfer was created.
     """
 
+    raw_return_reason_code: str
+    """The three character ACH return code, in the range R01 to R85."""
+
     return_reason_code: Literal[
         "insufficient_fund",
         "no_account",
         "account_closed",
         "invalid_account_number_structure",
         "account_frozen_entry_returned_per_ofac_instruction",
         "credit_entry_refused_by_receiver",
@@ -155,18 +158,66 @@
         "customer_advised_unauthorized_improper_ineligible_or_incomplete",
         "amount_field_error",
         "authorization_revoked_by_customer",
         "invalid_ach_routing_number",
         "file_record_edit_criteria",
         "enr_invalid_individual_name",
         "returned_per_odfi_request",
-        "addenda_error",
         "limited_participation_dfi",
         "incorrectly_coded_outbound_international_payment",
         "other",
+        "account_sold_to_another_dfi",
+        "addenda_error",
+        "beneficiary_or_account_holder_deceased",
+        "check_truncation_entry_return",
+        "corrected_return",
+        "duplicate_entry",
+        "duplicate_return",
+        "enr_duplicate_enrollment",
+        "enr_invalid_dfi_account_number",
+        "enr_invalid_individual_id_number",
+        "enr_invalid_representative_payee_indicator",
+        "enr_invalid_transaction_code",
+        "enr_return_of_enr_entry",
+        "enr_routing_number_check_digit_error",
+        "entry_not_processed_by_gateway",
+        "field_error",
+        "foreign_receiving_dfi_unable_to_settle",
+        "iat_entry_coding_error",
+        "improper_effective_entry_date",
+        "improper_source_document_source_document_presented",
+        "invalid_company_id",
+        "invalid_foreign_receiving_dfi_identification",
+        "invalid_individual_id_number",
+        "item_and_rck_entry_presented_for_payment",
+        "item_related_to_rck_entry_is_ineligible",
+        "mandatory_field_error",
+        "misrouted_dishonored_return",
+        "misrouted_return",
+        "no_errors_found",
+        "non_acceptance_of_r62_dishonored_return",
+        "non_participant_in_iat_program",
+        "permissible_return_entry",
+        "permissible_return_entry_not_accepted",
+        "rdfi_non_settlement",
+        "rdfi_participant_in_check_truncation_program",
+        "representative_payee_deceased_or_unable_to_continue_in_that_capacity",
+        "return_not_a_duplicate",
+        "return_of_erroneous_or_reversing_debit",
+        "return_of_improper_credit_entry",
+        "return_of_improper_debit_entry",
+        "return_of_xck_entry",
+        "source_document_presented_for_payment",
+        "state_law_affecting_rck_acceptance",
+        "stop_payment_on_item_related_to_rck_entry",
+        "stop_payment_on_source_document",
+        "timely_original_return",
+        "trace_number_error",
+        "untimely_dishonored_return",
+        "untimely_return",
     ]
     """Why the ACH Transfer was returned."""
 
     transaction_id: str
     """The identifier of the Tranasaction associated with this return."""
 
     transfer_id: str
@@ -862,14 +913,15 @@
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the transaction
     currency.
     """
 
     reason: Literal[
+        "account_closure",
         "bank_migration",
         "cashback",
         "collection_receivable",
         "empyreal_adjustment",
         "error",
         "error_correction",
         "fees",
@@ -1514,14 +1566,15 @@
         "ach_route_canceled",
         "ach_route_disabled",
         "breaches_limit",
         "entity_not_active",
         "group_locked",
         "insufficient_funds",
         "unable_to_locate_account",
+        "not_our_item",
         "unable_to_process",
         "refer_to_image",
         "stop_payment_requested",
         "returned",
         "duplicate_presentment",
         "not_authorized",
         "altered_or_fictitious",
```

### Comparing `increase-0.6.0/src/increase/types/simulations/inbound_wire_drawdown_request_create_params.py` & `increase-0.6.1/src/increase/types/simulations/inbound_wire_drawdown_request_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/types/simulations/interest_payment_simulation_result.py` & `increase-0.6.1/src/increase/types/simulations/wire_transfer_simulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Optional
 from datetime import date, datetime
 from typing_extensions import Literal
 
 from ..._models import BaseModel
 
 __all__ = [
-    "InterestPaymentSimulationResult",
+    "WireTransferSimulation",
     "Transaction",
     "TransactionSource",
     "TransactionSourceAccountTransferIntention",
     "TransactionSourceACHCheckConversionReturn",
     "TransactionSourceACHCheckConversion",
     "TransactionSourceACHTransferIntention",
     "TransactionSourceACHTransferRejection",
@@ -123,14 +123,17 @@
 class TransactionSourceACHTransferReturn(BaseModel):
     created_at: datetime
     """
     The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
     the transfer was created.
     """
 
+    raw_return_reason_code: str
+    """The three character ACH return code, in the range R01 to R85."""
+
     return_reason_code: Literal[
         "insufficient_fund",
         "no_account",
         "account_closed",
         "invalid_account_number_structure",
         "account_frozen_entry_returned_per_ofac_instruction",
         "credit_entry_refused_by_receiver",
@@ -143,18 +146,66 @@
         "customer_advised_unauthorized_improper_ineligible_or_incomplete",
         "amount_field_error",
         "authorization_revoked_by_customer",
         "invalid_ach_routing_number",
         "file_record_edit_criteria",
         "enr_invalid_individual_name",
         "returned_per_odfi_request",
-        "addenda_error",
         "limited_participation_dfi",
         "incorrectly_coded_outbound_international_payment",
         "other",
+        "account_sold_to_another_dfi",
+        "addenda_error",
+        "beneficiary_or_account_holder_deceased",
+        "check_truncation_entry_return",
+        "corrected_return",
+        "duplicate_entry",
+        "duplicate_return",
+        "enr_duplicate_enrollment",
+        "enr_invalid_dfi_account_number",
+        "enr_invalid_individual_id_number",
+        "enr_invalid_representative_payee_indicator",
+        "enr_invalid_transaction_code",
+        "enr_return_of_enr_entry",
+        "enr_routing_number_check_digit_error",
+        "entry_not_processed_by_gateway",
+        "field_error",
+        "foreign_receiving_dfi_unable_to_settle",
+        "iat_entry_coding_error",
+        "improper_effective_entry_date",
+        "improper_source_document_source_document_presented",
+        "invalid_company_id",
+        "invalid_foreign_receiving_dfi_identification",
+        "invalid_individual_id_number",
+        "item_and_rck_entry_presented_for_payment",
+        "item_related_to_rck_entry_is_ineligible",
+        "mandatory_field_error",
+        "misrouted_dishonored_return",
+        "misrouted_return",
+        "no_errors_found",
+        "non_acceptance_of_r62_dishonored_return",
+        "non_participant_in_iat_program",
+        "permissible_return_entry",
+        "permissible_return_entry_not_accepted",
+        "rdfi_non_settlement",
+        "rdfi_participant_in_check_truncation_program",
+        "representative_payee_deceased_or_unable_to_continue_in_that_capacity",
+        "return_not_a_duplicate",
+        "return_of_erroneous_or_reversing_debit",
+        "return_of_improper_credit_entry",
+        "return_of_improper_debit_entry",
+        "return_of_xck_entry",
+        "source_document_presented_for_payment",
+        "state_law_affecting_rck_acceptance",
+        "stop_payment_on_item_related_to_rck_entry",
+        "stop_payment_on_source_document",
+        "timely_original_return",
+        "trace_number_error",
+        "untimely_dishonored_return",
+        "untimely_return",
     ]
     """Why the ACH Transfer was returned."""
 
     transaction_id: str
     """The identifier of the Tranasaction associated with this return."""
 
     transfer_id: str
@@ -850,14 +901,15 @@
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the transaction
     currency.
     """
 
     reason: Literal[
+        "account_closure",
         "bank_migration",
         "cashback",
         "collection_receivable",
         "empyreal_adjustment",
         "error",
         "error_correction",
         "fees",
@@ -1343,19 +1395,20 @@
     type: Literal["transaction"]
     """A constant representing the object's type.
 
     For this resource it will always be `transaction`.
     """
 
 
-class InterestPaymentSimulationResult(BaseModel):
+class WireTransferSimulation(BaseModel):
     transaction: Transaction
-    """This will contain the resulting [Transaction](#transactions) object.
-
-    The Transaction's `source` will be of `category: interest_payment`.
+    """
+    If the Wire Transfer attempt succeeds, this will contain the resulting
+    [Transaction](#transactions) object. The Transaction's `source` will be of
+    `category: inbound_wire_transfer`.
     """
 
-    type: Literal["interest_payment_simulation_result"]
+    type: Literal["inbound_wire_transfer_simulation_result"]
     """A constant representing the object's type.
 
-    For this resource it will always be `interest_payment_simulation_result`.
+    For this resource it will always be `inbound_wire_transfer_simulation_result`.
     """
```

### Comparing `increase-0.6.0/src/increase/types/simulations/real_time_payments_transfer_complete_params.py` & `increase-0.6.1/src/increase/types/simulations/real_time_payments_transfer_complete_params.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 from __future__ import annotations
 
 from typing_extensions import Literal, Required, TypedDict
 
 __all__ = ["RealTimePaymentsTransferCompleteParams", "Rejection"]
 
 
+class RealTimePaymentsTransferCompleteParams(TypedDict, total=False):
+    rejection: Rejection
+    """If set, the simulation will reject the transfer."""
+
+
 class Rejection(TypedDict, total=False):
     reject_reason_code: Required[
         Literal[
             "account_closed",
             "account_blocked",
             "invalid_creditor_account_type",
             "invalid_creditor_account_number",
@@ -30,12 +35,7 @@
             "real_time_payments_suspended",
             "instructed_agent_signed_off",
             "processing_error",
             "other",
         ]
     ]
     """The reason code that the simulated rejection will have."""
-
-
-class RealTimePaymentsTransferCompleteParams(TypedDict, total=False):
-    rejection: Rejection
-    """If set, the simulation will reject the transfer."""
```

### Comparing `increase-0.6.0/src/increase/types/simulations/real_time_payments_transfer_create_inbound_params.py` & `increase-0.6.1/src/increase/types/simulations/real_time_payments_transfer_create_inbound_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/types/simulations/wire_transfer_create_inbound_params.py` & `increase-0.6.1/src/increase/types/simulations/wire_transfer_create_inbound_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/types/simulations/wire_transfer_simulation.py` & `increase-0.6.1/src/increase/types/simulations/interest_payment_simulation_result.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Optional
 from datetime import date, datetime
 from typing_extensions import Literal
 
 from ..._models import BaseModel
 
 __all__ = [
-    "WireTransferSimulation",
+    "InterestPaymentSimulationResult",
     "Transaction",
     "TransactionSource",
     "TransactionSourceAccountTransferIntention",
     "TransactionSourceACHCheckConversionReturn",
     "TransactionSourceACHCheckConversion",
     "TransactionSourceACHTransferIntention",
     "TransactionSourceACHTransferRejection",
@@ -123,14 +123,17 @@
 class TransactionSourceACHTransferReturn(BaseModel):
     created_at: datetime
     """
     The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
     the transfer was created.
     """
 
+    raw_return_reason_code: str
+    """The three character ACH return code, in the range R01 to R85."""
+
     return_reason_code: Literal[
         "insufficient_fund",
         "no_account",
         "account_closed",
         "invalid_account_number_structure",
         "account_frozen_entry_returned_per_ofac_instruction",
         "credit_entry_refused_by_receiver",
@@ -143,18 +146,66 @@
         "customer_advised_unauthorized_improper_ineligible_or_incomplete",
         "amount_field_error",
         "authorization_revoked_by_customer",
         "invalid_ach_routing_number",
         "file_record_edit_criteria",
         "enr_invalid_individual_name",
         "returned_per_odfi_request",
-        "addenda_error",
         "limited_participation_dfi",
         "incorrectly_coded_outbound_international_payment",
         "other",
+        "account_sold_to_another_dfi",
+        "addenda_error",
+        "beneficiary_or_account_holder_deceased",
+        "check_truncation_entry_return",
+        "corrected_return",
+        "duplicate_entry",
+        "duplicate_return",
+        "enr_duplicate_enrollment",
+        "enr_invalid_dfi_account_number",
+        "enr_invalid_individual_id_number",
+        "enr_invalid_representative_payee_indicator",
+        "enr_invalid_transaction_code",
+        "enr_return_of_enr_entry",
+        "enr_routing_number_check_digit_error",
+        "entry_not_processed_by_gateway",
+        "field_error",
+        "foreign_receiving_dfi_unable_to_settle",
+        "iat_entry_coding_error",
+        "improper_effective_entry_date",
+        "improper_source_document_source_document_presented",
+        "invalid_company_id",
+        "invalid_foreign_receiving_dfi_identification",
+        "invalid_individual_id_number",
+        "item_and_rck_entry_presented_for_payment",
+        "item_related_to_rck_entry_is_ineligible",
+        "mandatory_field_error",
+        "misrouted_dishonored_return",
+        "misrouted_return",
+        "no_errors_found",
+        "non_acceptance_of_r62_dishonored_return",
+        "non_participant_in_iat_program",
+        "permissible_return_entry",
+        "permissible_return_entry_not_accepted",
+        "rdfi_non_settlement",
+        "rdfi_participant_in_check_truncation_program",
+        "representative_payee_deceased_or_unable_to_continue_in_that_capacity",
+        "return_not_a_duplicate",
+        "return_of_erroneous_or_reversing_debit",
+        "return_of_improper_credit_entry",
+        "return_of_improper_debit_entry",
+        "return_of_xck_entry",
+        "source_document_presented_for_payment",
+        "state_law_affecting_rck_acceptance",
+        "stop_payment_on_item_related_to_rck_entry",
+        "stop_payment_on_source_document",
+        "timely_original_return",
+        "trace_number_error",
+        "untimely_dishonored_return",
+        "untimely_return",
     ]
     """Why the ACH Transfer was returned."""
 
     transaction_id: str
     """The identifier of the Tranasaction associated with this return."""
 
     transfer_id: str
@@ -850,14 +901,15 @@
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the transaction
     currency.
     """
 
     reason: Literal[
+        "account_closure",
         "bank_migration",
         "cashback",
         "collection_receivable",
         "empyreal_adjustment",
         "error",
         "error_correction",
         "fees",
@@ -1343,20 +1395,19 @@
     type: Literal["transaction"]
     """A constant representing the object's type.
 
     For this resource it will always be `transaction`.
     """
 
 
-class WireTransferSimulation(BaseModel):
+class InterestPaymentSimulationResult(BaseModel):
     transaction: Transaction
-    """
-    If the Wire Transfer attempt succeeds, this will contain the resulting
-    [Transaction](#transactions) object. The Transaction's `source` will be of
-    `category: inbound_wire_transfer`.
+    """This will contain the resulting [Transaction](#transactions) object.
+
+    The Transaction's `source` will be of `category: interest_payment`.
     """
 
-    type: Literal["inbound_wire_transfer_simulation_result"]
+    type: Literal["interest_payment_simulation_result"]
     """A constant representing the object's type.
 
-    For this resource it will always be `inbound_wire_transfer_simulation_result`.
+    For this resource it will always be `interest_payment_simulation_result`.
     """
```

### Comparing `increase-0.6.0/src/increase/types/transaction.py` & `increase-0.6.1/src/increase/types/transaction.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,14 +122,17 @@
 class SourceACHTransferReturn(BaseModel):
     created_at: datetime
     """
     The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
     the transfer was created.
     """
 
+    raw_return_reason_code: str
+    """The three character ACH return code, in the range R01 to R85."""
+
     return_reason_code: Literal[
         "insufficient_fund",
         "no_account",
         "account_closed",
         "invalid_account_number_structure",
         "account_frozen_entry_returned_per_ofac_instruction",
         "credit_entry_refused_by_receiver",
@@ -142,18 +145,66 @@
         "customer_advised_unauthorized_improper_ineligible_or_incomplete",
         "amount_field_error",
         "authorization_revoked_by_customer",
         "invalid_ach_routing_number",
         "file_record_edit_criteria",
         "enr_invalid_individual_name",
         "returned_per_odfi_request",
-        "addenda_error",
         "limited_participation_dfi",
         "incorrectly_coded_outbound_international_payment",
         "other",
+        "account_sold_to_another_dfi",
+        "addenda_error",
+        "beneficiary_or_account_holder_deceased",
+        "check_truncation_entry_return",
+        "corrected_return",
+        "duplicate_entry",
+        "duplicate_return",
+        "enr_duplicate_enrollment",
+        "enr_invalid_dfi_account_number",
+        "enr_invalid_individual_id_number",
+        "enr_invalid_representative_payee_indicator",
+        "enr_invalid_transaction_code",
+        "enr_return_of_enr_entry",
+        "enr_routing_number_check_digit_error",
+        "entry_not_processed_by_gateway",
+        "field_error",
+        "foreign_receiving_dfi_unable_to_settle",
+        "iat_entry_coding_error",
+        "improper_effective_entry_date",
+        "improper_source_document_source_document_presented",
+        "invalid_company_id",
+        "invalid_foreign_receiving_dfi_identification",
+        "invalid_individual_id_number",
+        "item_and_rck_entry_presented_for_payment",
+        "item_related_to_rck_entry_is_ineligible",
+        "mandatory_field_error",
+        "misrouted_dishonored_return",
+        "misrouted_return",
+        "no_errors_found",
+        "non_acceptance_of_r62_dishonored_return",
+        "non_participant_in_iat_program",
+        "permissible_return_entry",
+        "permissible_return_entry_not_accepted",
+        "rdfi_non_settlement",
+        "rdfi_participant_in_check_truncation_program",
+        "representative_payee_deceased_or_unable_to_continue_in_that_capacity",
+        "return_not_a_duplicate",
+        "return_of_erroneous_or_reversing_debit",
+        "return_of_improper_credit_entry",
+        "return_of_improper_debit_entry",
+        "return_of_xck_entry",
+        "source_document_presented_for_payment",
+        "state_law_affecting_rck_acceptance",
+        "stop_payment_on_item_related_to_rck_entry",
+        "stop_payment_on_source_document",
+        "timely_original_return",
+        "trace_number_error",
+        "untimely_dishonored_return",
+        "untimely_return",
     ]
     """Why the ACH Transfer was returned."""
 
     transaction_id: str
     """The identifier of the Tranasaction associated with this return."""
 
     transfer_id: str
@@ -849,14 +900,15 @@
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the transaction
     currency.
     """
 
     reason: Literal[
+        "account_closure",
         "bank_migration",
         "cashback",
         "collection_receivable",
         "empyreal_adjustment",
         "error",
         "error_correction",
         "fees",
```

### Comparing `increase-0.6.0/src/increase/types/transaction_list_params.py` & `increase-0.6.1/src/increase/types/transaction_list_params.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,40 +4,38 @@
 
 from typing import List, Union
 from datetime import datetime
 from typing_extensions import Literal, Annotated, TypedDict
 
 from .._utils import PropertyInfo
 
-__all__ = ["TransactionListParams", "CreatedAt", "Category"]
+__all__ = ["TransactionListParams", "Category", "CreatedAt"]
 
 
-class CreatedAt(TypedDict, total=False):
-    after: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
-    """
-    Return results after this [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601)
-    timestamp.
-    """
+class TransactionListParams(TypedDict, total=False):
+    account_id: str
+    """Filter Transactions for those belonging to the specified Account."""
 
-    before: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
-    """
-    Return results before this [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601)
-    timestamp.
-    """
+    category: Category
 
-    on_or_after: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
-    """
-    Return results on or after this
-    [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) timestamp.
-    """
+    created_at: CreatedAt
 
-    on_or_before: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
+    cursor: str
+    """Return the page of entries after this one."""
+
+    limit: int
+    """Limit the size of the list that is returned.
+
+    The default (and maximum) is 100 objects.
     """
-    Return results on or before this
-    [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) timestamp.
+
+    route_id: str
+    """Filter Transactions for those belonging to the specified route.
+
+    This could be a Card ID or an Account Number ID.
     """
 
 
 _CategoryReservedKeywords = TypedDict(
     "_CategoryReservedKeywords",
     {
         "in": List[
@@ -89,29 +87,31 @@
 )
 
 
 class Category(_CategoryReservedKeywords, total=False):
     pass
 
 
-class TransactionListParams(TypedDict, total=False):
-    account_id: str
-    """Filter Transactions for those belonging to the specified Account."""
-
-    category: Category
-
-    created_at: CreatedAt
-
-    cursor: str
-    """Return the page of entries after this one."""
-
-    limit: int
-    """Limit the size of the list that is returned.
+class CreatedAt(TypedDict, total=False):
+    after: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
+    """
+    Return results after this [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601)
+    timestamp.
+    """
 
-    The default (and maximum) is 100 objects.
+    before: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
+    """
+    Return results before this [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601)
+    timestamp.
     """
 
-    route_id: str
-    """Filter Transactions for those belonging to the specified route.
+    on_or_after: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
+    """
+    Return results on or after this
+    [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) timestamp.
+    """
 
-    This could be a Card ID or an Account Number ID.
+    on_or_before: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
+    """
+    Return results on or before this
+    [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) timestamp.
     """
```

### Comparing `increase-0.6.0/src/increase/types/wire_drawdown_request.py` & `increase-0.6.1/src/increase/types/wire_drawdown_request.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/types/wire_drawdown_request_create_params.py` & `increase-0.6.1/src/increase/types/wire_drawdown_request_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/types/wire_transfer.py` & `increase-0.6.1/src/increase/types/wire_transfer.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/types/wire_transfer_create_params.py` & `increase-0.6.1/src/increase/types/wire_transfer_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.6.0/src/increase/types/wire_transfer_list_params.py` & `increase-0.6.1/src/increase/types/wire_transfer_list_params.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,33 @@
 from typing_extensions import Annotated, TypedDict
 
 from .._utils import PropertyInfo
 
 __all__ = ["WireTransferListParams", "CreatedAt"]
 
 
+class WireTransferListParams(TypedDict, total=False):
+    account_id: str
+    """Filter Wire Transfers to those belonging to the specified Account."""
+
+    created_at: CreatedAt
+
+    cursor: str
+    """Return the page of entries after this one."""
+
+    external_account_id: str
+    """Filter Wire Transfers to those made to the specified External Account."""
+
+    limit: int
+    """Limit the size of the list that is returned.
+
+    The default (and maximum) is 100 objects.
+    """
+
+
 class CreatedAt(TypedDict, total=False):
     after: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
     """
     Return results after this [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601)
     timestamp.
     """
 
@@ -31,26 +50,7 @@
     """
 
     on_or_before: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
     """
     Return results on or before this
     [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) timestamp.
     """
-
-
-class WireTransferListParams(TypedDict, total=False):
-    account_id: str
-    """Filter Wire Transfers to those belonging to the specified Account."""
-
-    created_at: CreatedAt
-
-    cursor: str
-    """Return the page of entries after this one."""
-
-    external_account_id: str
-    """Filter Wire Transfers to those made to the specified External Account."""
-
-    limit: int
-    """Limit the size of the list that is returned.
-
-    The default (and maximum) is 100 objects.
-    """
```

### Comparing `increase-0.6.0/PKG-INFO` & `increase-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: increase
-Version: 0.6.0
+Version: 0.6.1
 Summary: Client library for the increase API
 Home-page: https://github.com/increase/increase-python
 License: Apache-2.0
 Author: Increase
 Author-email: dev-feedback@increase.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

