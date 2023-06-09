# Comparing `tmp/conekta-2.6.2.tar.gz` & `tmp/conekta-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conekta-2.6.2.tar", last modified: Mon Apr 17 13:59:08 2023, max compression
+gzip compressed data, was "conekta-6.0.0.tar", last modified: Fri Jun  9 16:02:01 2023, max compression
```

## Comparing `conekta-2.6.2.tar` & `conekta-6.0.0.tar`

### file list

```diff
@@ -1,29 +1,268 @@
-drwxr-xr-x   0 franklin   (501) staff       (20)        0 2023-04-17 13:59:08.256983 conekta-2.6.2/
--rw-r--r--   0 franklin   (501) staff       (20)     2716 2023-04-17 13:51:55.000000 conekta-2.6.2/CHANGELOG.md
--rw-r--r--   0 franklin   (501) staff       (20)     1101 2023-01-06 15:45:22.000000 conekta-2.6.2/LICENSE
--rw-r--r--   0 franklin   (501) staff       (20)       94 2023-01-06 15:45:22.000000 conekta-2.6.2/MANIFEST.in
--rw-r--r--   0 franklin   (501) staff       (20)      754 2023-04-17 13:59:08.256794 conekta-2.6.2/PKG-INFO
--rw-r--r--   0 franklin   (501) staff       (20)     8812 2023-04-17 13:51:55.000000 conekta-2.6.2/README.md
--rw-r--r--   0 franklin   (501) staff       (20)       81 2023-01-06 15:45:22.000000 conekta-2.6.2/README.txt
-drwxr-xr-x   0 franklin   (501) staff       (20)        0 2023-04-17 13:59:08.249375 conekta-2.6.2/conekta/
--rw-r--r--   0 franklin   (501) staff       (20)    24237 2023-04-17 13:51:55.000000 conekta-2.6.2/conekta/__init__.py
-drwxr-xr-x   0 franklin   (501) staff       (20)        0 2023-04-17 13:59:08.252667 conekta-2.6.2/conekta/ssl_data/
--rw-r--r--   0 franklin   (501) staff       (20)   261053 2023-01-06 15:45:22.000000 conekta-2.6.2/conekta/ssl_data/ca_bundle.crt
-drwxr-xr-x   0 franklin   (501) staff       (20)        0 2023-04-17 13:59:08.252333 conekta-2.6.2/conekta.egg-info/
--rw-r--r--   0 franklin   (501) staff       (20)      754 2023-04-17 13:59:08.000000 conekta-2.6.2/conekta.egg-info/PKG-INFO
--rw-r--r--   0 franklin   (501) staff       (20)      467 2023-04-17 13:59:08.000000 conekta-2.6.2/conekta.egg-info/SOURCES.txt
--rw-r--r--   0 franklin   (501) staff       (20)        1 2023-04-17 13:59:08.000000 conekta-2.6.2/conekta.egg-info/dependency_links.txt
--rw-r--r--   0 franklin   (501) staff       (20)       25 2023-04-17 13:59:08.000000 conekta-2.6.2/conekta.egg-info/requires.txt
--rw-r--r--   0 franklin   (501) staff       (20)       14 2023-04-17 13:59:08.000000 conekta-2.6.2/conekta.egg-info/top_level.txt
--rw-r--r--   0 franklin   (501) staff       (20)        1 2023-01-06 17:12:23.000000 conekta-2.6.2/conekta.egg-info/zip-safe
--rw-r--r--   0 franklin   (501) staff       (20)       38 2023-04-17 13:59:08.257079 conekta-2.6.2/setup.cfg
--rw-r--r--   0 franklin   (501) staff       (20)     1081 2023-04-17 13:51:55.000000 conekta-2.6.2/setup.py
-drwxr-xr-x   0 franklin   (501) staff       (20)        0 2023-04-17 13:59:08.256315 conekta-2.6.2/tests/
--rw-r--r--   0 franklin   (501) staff       (20)    15559 2023-04-17 13:51:55.000000 conekta-2.6.2/tests/__init__.py
--rw-r--r--   0 franklin   (501) staff       (20)     3510 2023-04-17 13:51:55.000000 conekta-2.6.2/tests/test_checkouts.py
--rw-r--r--   0 franklin   (501) staff       (20)     3593 2023-04-17 13:51:55.000000 conekta-2.6.2/tests/test_customer.py
--rw-r--r--   0 franklin   (501) staff       (20)     3745 2023-04-17 13:51:55.000000 conekta-2.6.2/tests/test_events.py
--rw-r--r--   0 franklin   (501) staff       (20)      508 2023-04-17 13:51:55.000000 conekta-2.6.2/tests/test_logs.py
--rw-r--r--   0 franklin   (501) staff       (20)    12832 2023-04-17 13:51:55.000000 conekta-2.6.2/tests/test_orders.py
--rw-r--r--   0 franklin   (501) staff       (20)     3113 2023-04-17 13:51:55.000000 conekta-2.6.2/tests/test_pagination.py
--rw-r--r--   0 franklin   (501) staff       (20)      575 2023-04-17 13:51:55.000000 conekta-2.6.2/tests/test_webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:02:01.189855 conekta-6.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-09 16:01:51.000000 conekta-6.0.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-09 16:01:51.000000 conekta-6.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-09 16:01:51.000000 conekta-6.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    27601 2023-06-09 16:02:01.189855 conekta-6.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    26852 2023-06-09 16:01:51.000000 conekta-6.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:02:01.157855 conekta-6.0.0/conekta/
+-rw-r--r--   0 runner    (1001) docker     (123)    16964 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:02:01.161855 conekta-6.0.0/conekta/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43665 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/api/antifraud_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40760 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/api/api_keys_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19076 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/api/charges_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16249 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/api/companies_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63028 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/api/customers_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28260 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/api/discounts_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25270 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/api/events_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18002 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/api/logs_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67602 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/api/orders_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51140 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/api/payment_link_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38951 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/api/payment_methods_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41008 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/api/plans_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27109 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/api/products_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28786 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/api/shipping_contacts_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27230 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/api/shippings_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57213 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/api/subscriptions_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27176 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/api/taxes_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8103 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/api/tokens_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18251 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/api/transactions_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18152 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/api/transfers_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39790 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/api/webhook_keys_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47871 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/api/webhooks_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30526 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14582 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:02:01.189855 conekta-6.0.0/conekta/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    15366 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/api_key_create_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/api_key_create_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/api_key_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/api_key_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/api_key_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/blacklist_rule_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6747 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/charge_data_payment_method_bank_transfer_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/charge_data_payment_method_card_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/charge_data_payment_method_cash_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/charge_order_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/charge_order_response_payment_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/charge_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/charge_request_payment_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/charge_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/charge_response_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7696 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/charge_response_payment_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/charge_response_refunds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/charge_response_refunds_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/charge_response_refunds_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/charges_data_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4852 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/checkout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/checkout_order_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/checkout_order_template_customer_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/checkout_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/checkout_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/checkouts_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/checkouts_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/company_fiscal_info_address_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/company_fiscal_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/company_payout_destination_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/company_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/create_customer_fiscal_entities_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/create_customer_fiscal_entities_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6483 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/create_customer_payment_methods_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/create_customer_payment_methods_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/create_risk_rules_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7153 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customer_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customer_antifraud_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customer_antifraud_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customer_fiscal_entities_data_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customer_fiscal_entities_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customer_fiscal_entities_request_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customer_fiscal_entities_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customer_fiscal_entities_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customer_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customer_info_just_customer_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customer_info_just_customer_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customer_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customer_payment_method_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customer_payment_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8201 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customer_payment_methods_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6355 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customer_payment_methods_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customer_payment_methods_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customer_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customer_response_shipping_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customer_response_shipping_contacts_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customer_shipping_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customer_shipping_contacts_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customer_shipping_contacts_data_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customer_shipping_contacts_data_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customer_shipping_contacts_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customer_shipping_contacts_response_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customer_update_fiscal_entities_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customer_update_shipping_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customers_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/customers_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/delete_api_keys_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/delete_api_keys_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/deleted_blacklist_rule_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/deleted_whitelist_rule_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/details_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/discount_lines_data_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/discount_lines_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/discount_lines_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/email_checkout_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/error_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/event_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/events_resend_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/get_api_keys_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/get_api_keys_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/get_charges_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/get_charges_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/get_companies_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/get_companies_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/get_customer_payment_method_data_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/get_events_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/get_events_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/get_orders_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/get_payment_method_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/get_payment_method_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/get_plans_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/get_plans_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/get_transactions_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/get_transactions_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/get_transfers_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/get_transfers_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/get_webhook_keys_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/get_webhook_keys_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/get_webhooks_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/get_webhooks_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/log_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/logs_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/logs_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/order_capture_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/order_discount_lines_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/order_refund_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7852 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/order_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5308 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/order_request_customer_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/order_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/order_response_charges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/order_response_charges_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5164 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/order_response_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/order_response_customer_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/order_response_customer_info_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/order_response_discount_lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/order_response_discount_lines_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/order_response_fiscal_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/order_response_fiscal_entity_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/order_response_fiscal_entity_address_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/order_response_products.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/order_response_products_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/order_response_shipping_contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/order_response_shipping_contact_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/order_tax_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/order_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/orders_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/payment_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/payment_method_bank_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/payment_method_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/payment_method_card_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/payment_method_card_request_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/payment_method_card_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/payment_method_card_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/payment_method_cash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/payment_method_cash_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/payment_method_cash_request_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/payment_method_cash_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/payment_method_cash_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/payment_method_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/payment_method_spei_recurrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/payment_method_spei_recurrent_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/payment_method_spei_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/plan_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/plan_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/plan_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/product.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/product_data_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/product_data_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/product_order_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/product_order_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/risk_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/risk_rules_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/risk_rules_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/shipping_order_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/shipping_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/sms_checkout_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/subscription_events_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/subscription_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/subscription_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/subscription_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/token_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/token_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/token_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/token_response_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/transaction_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/transfer_destination_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/transfer_method_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/transfer_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/transfers_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/update_customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/update_customer_antifraud_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/update_customer_fiscal_entities_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/update_customer_fiscal_entities_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/update_customer_payment_methods_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/update_order_discount_lines_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/update_order_tax_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/update_order_tax_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/update_order_tax_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/update_payment_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/update_product.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/webhook_key_create_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/webhook_key_delete_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/webhook_key_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/webhook_key_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/webhook_key_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/webhook_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/webhook_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/webhook_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/webhook_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/models/whitelistlist_rule_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12745 2023-06-09 16:01:51.000000 conekta-6.0.0/conekta/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:02:01.161855 conekta-6.0.0/conekta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    27601 2023-06-09 16:02:01.000000 conekta-6.0.0/conekta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10330 2023-06-09 16:02:01.000000 conekta-6.0.0/conekta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 16:02:01.000000 conekta-6.0.0/conekta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-09 16:02:01.000000 conekta-6.0.0/conekta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-09 16:02:01.000000 conekta-6.0.0/conekta.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-09 16:01:51.000000 conekta-6.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-09 16:02:01.193856 conekta-6.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-09 16:01:51.000000 conekta-6.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:02:01.189855 conekta-6.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-09 16:01:51.000000 conekta-6.0.0/test/test_antifraud_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-06-09 16:01:51.000000 conekta-6.0.0/test/test_api_keys_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-06-09 16:01:51.000000 conekta-6.0.0/test/test_charges_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-09 16:01:51.000000 conekta-6.0.0/test/test_companies_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-06-09 16:01:51.000000 conekta-6.0.0/test/test_customers_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-09 16:01:51.000000 conekta-6.0.0/test/test_discounts_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-06-09 16:01:51.000000 conekta-6.0.0/test/test_events_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-09 16:01:51.000000 conekta-6.0.0/test/test_logs_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-06-09 16:01:51.000000 conekta-6.0.0/test/test_orders_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-06-09 16:01:51.000000 conekta-6.0.0/test/test_payment_link_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-06-09 16:01:51.000000 conekta-6.0.0/test/test_payment_methods_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-09 16:01:51.000000 conekta-6.0.0/test/test_plans_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-06-09 16:01:51.000000 conekta-6.0.0/test/test_products_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-06-09 16:01:51.000000 conekta-6.0.0/test/test_shipping_contacts_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-09 16:01:51.000000 conekta-6.0.0/test/test_shippings_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-06-09 16:01:51.000000 conekta-6.0.0/test/test_subscriptions_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-06-09 16:01:51.000000 conekta-6.0.0/test/test_taxes_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-09 16:01:51.000000 conekta-6.0.0/test/test_tokens_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-09 16:01:51.000000 conekta-6.0.0/test/test_transactions_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-09 16:01:51.000000 conekta-6.0.0/test/test_transfers_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-09 16:01:51.000000 conekta-6.0.0/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-06-09 16:01:51.000000 conekta-6.0.0/test/test_webhook_keys_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-06-09 16:01:51.000000 conekta-6.0.0/test/test_webhooks_api.py
```

### Comparing `conekta-2.6.2/LICENSE` & `conekta-6.0.0/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-MIT Lcense
+MIT License
 
-Copyright (c) 2013-2014 - Conekta, Inc. (https://www.conekta.io)
+Copyright (c) 2014 - Conekta, Inc. (https://www.conekta.io)
 
 Permission is hereby granted, free of charge, to any person obtaining
 a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including
 without limitation the rights to use, copy, modify, merge, publish,
 distribute, sublicense, and/or sell copies of the Software, and to
 permit persons to whom the Software is furnished to do so, subject to
@@ -15,8 +15,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
 EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
 LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
 OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
-WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

