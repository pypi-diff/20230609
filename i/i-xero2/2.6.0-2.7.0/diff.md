# Comparing `tmp/i_xero2-2.6.0.tar.gz` & `tmp/i_xero2-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "i_xero2-2.6.0.tar", max compression
+gzip compressed data, was "i_xero2-2.7.0.tar", max compression
```

## Comparing `i_xero2-2.6.0.tar` & `i_xero2-2.7.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1079 2021-10-14 01:56:57.796205 i_xero2-2.6.0/LICENSE
--rw-r--r--   0        0        0     1403 2022-11-30 18:07:38.057869 i_xero2-2.6.0/README.md
--rw-r--r--   0        0        0      282 2022-11-03 18:19:48.298576 i_xero2-2.6.0/i_xero2/__init__.py
--rw-r--r--   0        0        0     2143 2022-11-03 18:19:48.298576 i_xero2-2.6.0/i_xero2/i_flask.py
--rw-r--r--   0        0        0    47070 2022-11-30 18:07:38.057869 i_xero2-2.6.0/i_xero2/i_xero.py
--rw-r--r--   0        0        0     7090 2022-11-03 18:19:48.298576 i_xero2-2.6.0/i_xero2/i_xero_ui.py
--rw-r--r--   0        0        0      829 2022-11-30 18:07:52.349974 i_xero2-2.6.0/pyproject.toml
--rw-r--r--   0        0        0     2260 1970-01-01 00:00:00.000000 i_xero2-2.6.0/setup.py
--rw-r--r--   0        0        0     2235 1970-01-01 00:00:00.000000 i_xero2-2.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1079 2021-10-14 01:56:57.796205 i_xero2-2.7.0/LICENSE
+-rw-r--r--   0        0        0     1403 2022-11-30 18:07:38.057869 i_xero2-2.7.0/README.md
+-rw-r--r--   0        0        0      229 2023-06-09 20:33:49.252776 i_xero2-2.7.0/i_xero2/__init__.py
+-rw-r--r--   0        0        0     2143 2022-11-03 18:19:48.298576 i_xero2-2.7.0/i_xero2/i_flask.py
+-rw-r--r--   0        0        0    49162 2023-06-09 20:33:20.776544 i_xero2-2.7.0/i_xero2/i_xero.py
+-rw-r--r--   0        0        0     7090 2022-11-03 18:19:48.298576 i_xero2-2.7.0/i_xero2/i_xero_ui.py
+-rw-r--r--   0        0        0      829 2023-06-09 20:33:33.640649 i_xero2-2.7.0/pyproject.toml
+-rw-r--r--   0        0        0     2260 1970-01-01 00:00:00.000000 i_xero2-2.7.0/setup.py
+-rw-r--r--   0        0        0     2235 1970-01-01 00:00:00.000000 i_xero2-2.7.0/PKG-INFO
```

### Comparing `i_xero2-2.6.0/LICENSE` & `i_xero2-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `i_xero2-2.6.0/README.md` & `i_xero2-2.7.0/README.md`

 * *Files identical despite different names*

### Comparing `i_xero2-2.6.0/i_xero2/i_flask.py` & `i_xero2-2.7.0/i_xero2/i_flask.py`

 * *Files identical despite different names*

### Comparing `i_xero2-2.6.0/i_xero2/i_xero.py` & `i_xero2-2.7.0/i_xero2/i_xero.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 """Class module to interface with Xero.
 """
 # import modules
 # pylint: disable=logging-fstring-interpolation,too-many-lines
 
+from collections import deque
+from datetime import datetime
 import os
+import time
 
 from aracnid_logger import Logger
 from i_mongodb import MongoDBInterface
 from pytz import timezone, utc
 from xero_python.accounting import AccountingApi
 from xero_python.accounting import CreditNotes
 from xero_python.accounting import Invoices
@@ -76,18 +79,38 @@
         # set the xero client
         self.set_client()
 
         # if self.client:
         #     # set the APIs
         #     self.accounting_api = AccountingApi(self.client)
 
+        # handle rate limit: 60 calls per minute
+        self.rate_limit_calls = 60
+        self.rate_limit_seconds = 60
+        self.call_window = deque([], maxlen=self.rate_limit_calls)
+
         # track class instances
         XeroInterface.instances.append(self)
         logger.debug(f'XeroInterface.instances: {len(XeroInterface.instances)}')
 
+    def throttle(self):
+        """Records the call time and implements a delay to comply with rate limit.
+
+        Rate limit is defined by self.rate_limit_calls and self.rate_limit_seconds.
+        """
+        # check for window length
+        if len(self.call_window) < self.rate_limit_calls:
+            self.call_window.append(datetime.now())
+            return
+
+        # check for window duration
+        if duration := datetime.now() - self.call_window[0] < self.rate_limit_seconds:
+            time.sleep(self.rate_limit_seconds - duration.total_seconds())
+            self.call_window.append(datetime.now())
+
     def set_client(self):
         """Connect to Xero and set the client.
         """
         token = self.get_token()
 
         if token:
             logger.debug(f'[setup] expires: {token["expires_at"]}')
@@ -323,23 +346,25 @@
         Returns:
             Dictionary or list or retrieved accounts.
         """
         account_id = kwargs.pop('id', None)
 
         try:
             if account_id:
+                self.throttle()
                 accounts = self.accounting_api.get_account(
                     self.tenant_id,
                     account_id=account_id
                 )
                 if len(accounts.accounts) == 1:
                     return accounts.accounts[0]
                 else:
                     return None
             else:
+                self.throttle()
                 accounts = self.accounting_api.get_accounts(
                     self.tenant_id,
                     **kwargs
                 )
                 return accounts.accounts
         except AccountingBadRequestException as err:
             logger.error(f'Exception: {err}\n')
@@ -356,14 +381,15 @@
         Args:
             credit_note_list: List of credit_notes to create.
 
         Returns:
             List of created Invoice objects.
         """
         try:
+            self.throttle()
             credit_notes = self.accounting_api.create_credit_notes(
                 self.tenant_id,
                 credit_notes=CreditNotes(credit_notes=credit_note_list),
                 unitdp=self.unitdp
             )
             return credit_notes.credit_notes
         except AccountingBadRequestException as err:
@@ -388,24 +414,26 @@
         Returns:
             Dictionary or list of retrieved credit_notes.
         """
         credit_note_id = kwargs.pop('id', None)
 
         try:
             if credit_note_id:
+                self.throttle()
                 credit_notes = self.accounting_api.get_credit_note(
                     self.tenant_id,
                     credit_note_id=credit_note_id,
                     unitdp=self.unitdp
                 )
                 if len(credit_notes.credit_notes) == 1:
                     return credit_notes.credit_notes[0]
                 else:
                     return None
             else:
+                self.throttle()
                 credit_notes = self.accounting_api.get_credit_notes(
                     self.tenant_id,
                     unitdp=self.unitdp,
                     **kwargs,
                 )
                 return credit_notes.credit_notes
         except AccountingBadRequestException as err:
@@ -424,14 +452,15 @@
         Args:
             credit_note_list: List of credit_notes to update
 
         Returns:
             Dictionary or list of retrieved credit_notes.
         """
         try:
+            self.throttle()
             credit_notes = self.accounting_api.update_or_create_credit_notes(
                 self.tenant_id,
                 credit_notes=CreditNotes(
                     credit_notes=credit_note_list
                 )
             )
             return credit_notes.credit_notes
@@ -513,14 +542,15 @@
         Args:
             invoice_list: List of invoices to create.
 
         Returns:
             List of created Invoice objects.
         """
         try:
+            self.throttle()
             invoices = self.accounting_api.create_invoices(
                 self.tenant_id,
                 invoices=Invoices(invoices=invoice_list),
                 unitdp=self.unitdp
             )
             return invoices.invoices
         except AccountingBadRequestException as err:
@@ -545,24 +575,26 @@
         Returns:
             Dictionary or list of retrieved invoices.
         """
         invoice_id = kwargs.pop('id', None)
 
         try:
             if invoice_id:
+                self.throttle()
                 invoices = self.accounting_api.get_invoice(
                     self.tenant_id,
                     invoice_id=invoice_id,
                     unitdp=self.unitdp
                 )
                 if len(invoices.invoices) == 1:
                     return invoices.invoices[0]
                 else:
                     return None
             else:
+                self.throttle()
                 invoices = self.accounting_api.get_invoices(
                     self.tenant_id,
                     unitdp=self.unitdp,
                     **kwargs,
                 )
                 return invoices.invoices
         except AccountingBadRequestException as err:
@@ -581,14 +613,15 @@
         Args:
             invoice_list: List of invoices to update
 
         Returns:
             Dictionary or list of retrieved invoices.
         """
         try:
+            self.throttle()
             invoices = self.accounting_api.update_or_create_invoices(
                 self.tenant_id,
                 invoices=Invoices(
                     invoices=invoice_list
                 )
             )
             return invoices.invoices
@@ -670,14 +703,15 @@
         Args:
             item_list: List of items to create.
 
         Returns:
             List of created Item objects.
         """
         try:
+            self.throttle()
             items = self.accounting_api.create_items(
                 self.tenant_id,
                 items=Items(
                     items=item_list
                 ),
                 unitdp=self.unitdp
             )
@@ -704,24 +738,26 @@
         Returns:
             Dictionary or list or retrieved items.
         """
         item_id = kwargs.pop('id', None)
 
         try:
             if item_id:
+                self.throttle()
                 items = self.accounting_api.get_item(
                     self.tenant_id,
                     item_id=item_id,
                     unitdp=self.unitdp
                 )
                 if len(items.items) == 1:
                     return items.items[0]
                 else:
                     return None
             else:
+                self.throttle()
                 items = self.accounting_api.get_items(
                     self.tenant_id,
                     unitdp=self.unitdp,
                     **kwargs
                 )
                 return items.items
         except AccountingBadRequestException as err:
@@ -742,14 +778,15 @@
         Args:
             item_list: List of items to update
 
         Returns:
             Dictionary or list of retrieved items.
         """
         try:
+            self.throttle()
             items = self.accounting_api.update_or_create_items(
                 self.tenant_id,
                 items=Items(
                     items=item_list
                 )
             )
             return items.items
@@ -776,30 +813,33 @@
             List of deleted items.
         """
         item_id = kwargs.pop('id', None)
         item_list = kwargs.pop('item_list', None)
 
         try:
             if item_id:
+                self.throttle()
                 self.accounting_api.delete_item(
                     self.tenant_id,
                     item_id=item_id
                 )
             elif item_list:
                 for item in item_list:
+                    self.throttle()
                     self.accounting_api.delete_item(
                         self.tenant_id,
                         item_id=item.item_id
                     )
             else:
                 item_list_read = self.read_items(**kwargs)
                 if not item_list_read:
                     return []
 
                 for item in item_list_read:
+                    self.throttle()
                     self.accounting_api.delete_item(
                         self.tenant_id,
                         item_id=item.item_id
                     )
 
         except AccountingBadRequestException as err:
             logger.error(f'Exception: {err}\n')
@@ -816,14 +856,15 @@
         Args:
             manual_journal_list: List of manual journals to create.
 
         Returns:
             List of created ManualJournal objects.
         """
         try:
+            self.throttle()
             manual_journals = self.accounting_api.create_manual_journals(
                 self.tenant_id,
                 manual_journals=ManualJournals(
                     manual_journals=manual_journal_list
                 )
             )
             return manual_journals.manual_journals
@@ -849,23 +890,25 @@
         Returns:
             Dictionary or list of retrieved manual journals.
         """
         manual_journal_id = kwargs.pop('id', None)
 
         try:
             if manual_journal_id:
+                self.throttle()
                 manual_journals = self.accounting_api.get_manual_journal(
                     self.tenant_id,
                     manual_journal_id=manual_journal_id
                 )
                 if len(manual_journals.manual_journals) == 1:
                     return manual_journals.manual_journals[0]
                 else:
                     return None
             else:
+                self.throttle()
                 manual_journals = self.accounting_api.get_manual_journals(
                     self.tenant_id,
                     **kwargs,
                 )
                 return manual_journals.manual_journals
         except AccountingBadRequestException as err:
             logger.error(f'Exception: {err}\n')
@@ -883,14 +926,15 @@
         Args:
             manual_journal_list: List of manual journals to update
 
         Returns:
             Dictionary or list of retrieved manual journals.
         """
         try:
+            self.throttle()
             manual_journals = self.accounting_api.update_or_create_manual_journals(
                 self.tenant_id,
                 manual_journals=ManualJournals(
                     manual_journals=manual_journal_list
                 )
             )
             return manual_journals.manual_journals
@@ -970,14 +1014,15 @@
             accounting.transactions
             accounting.transactions.read
 
         Returns:
             List of retrieved organizations.
         """
         try:
+            self.throttle()
             organizations = self.accounting_api.get_organisations(
                 self.tenant_id
             )
             return organizations.organisations
         except AccountingBadRequestException as err:
             logger.error(f'Exception: {err}\n')
 
@@ -993,14 +1038,15 @@
         Args:
             payment_list: List of payments to create.
 
         Returns:
             List of created Payment objects.
         """
         try:
+            self.throttle()
             payments = self.accounting_api.create_payments(
                 self.tenant_id,
                 payments=Payments(payments=payment_list)
             )
             return payments.payments
         except AccountingBadRequestException as err:
             logger.error(f'Exception: {err}\n')
@@ -1024,23 +1070,25 @@
         Returns:
             Dictionary or list of retrieved payments.
         """
         payment_id = kwargs.pop('id', None)
 
         try:
             if payment_id:
+                self.throttle()
                 payments = self.accounting_api.get_payment(
                     self.tenant_id,
                     payment_id=payment_id
                 )
                 if len(payments.payments) == 1:
                     return payments.payments[0]
                 else:
                     return None
             else:
+                self.throttle()
                 payments = self.accounting_api.get_payments(
                     self.tenant_id,
                     **kwargs,
                 )
                 return payments.payments
         except AccountingBadRequestException as err:
             logger.error(f'Exception: {err}\n')
@@ -1066,25 +1114,27 @@
         """
         payment_id = kwargs.pop('id', None)
         payment_list = kwargs.pop('payment_list', None)
 
         try:
             if payment_id:
                 payment_delete = PaymentDelete(status = "DELETED")
+                self.throttle()
                 payments = self.accounting_api.delete_payment(
                     self.tenant_id,
                     payment_id=payment_id,
                     payment_delete=payment_delete
                 )
                 return payments.payments
 
             elif payment_list:
                 payment_delete = PaymentDelete(status = "DELETED")
                 payment_list_deleted = []
                 for payment in payment_list:
+                    self.throttle()
                     payments = self.accounting_api.delete_payment(
                         self.tenant_id,
                         payment_id=payment.payment_id,
                         payment_delete=payment_delete
                     )
                     payment_list_deleted.append(payments.payments[0])
                 return payment_list_deleted
@@ -1093,14 +1143,15 @@
                 payment_delete = PaymentDelete(status="DELETED")
                 payment_list_read = self.read_payments(**kwargs)
                 if not payment_list_read:
                     return []
 
                 payment_list_deleted = []
                 for payment in payment_list_read:
+                    self.throttle()
                     payments = self.accounting_api.delete_payment(
                         self.tenant_id,
                         payment_id=payment.payment_id,
                         payment_delete=payment_delete
                     )
                     payment_list_deleted.append(payments.payments[0])
                 return payment_list_deleted
@@ -1120,14 +1171,15 @@
         Args:
             purchase_order_list: List of purchase_orders to create.
 
         Returns:
             List of created Invoice objects.
         """
         try:
+            self.throttle()
             purchase_orders = self.accounting_api.create_purchase_orders(
                 self.tenant_id,
                 purchase_orders=PurchaseOrders(purchase_orders=purchase_order_list)
             )
             return purchase_orders.purchase_orders
         except AccountingBadRequestException as err:
             logger.error(f'Exception: {err}\n')
@@ -1152,32 +1204,35 @@
             Dictionary or list of retrieved purchase_orders.
         """
         purchase_order_id = kwargs.pop('id', None)
         number = kwargs.pop('number', None)
 
         try:
             if purchase_order_id:
+                self.throttle()
                 purchase_orders = self.accounting_api.get_purchase_order(
                     self.tenant_id,
                     purchase_order_id=purchase_order_id
                 )
                 if len(purchase_orders.purchase_orders) == 1:
                     return purchase_orders.purchase_orders[0]
                 else:
                     return None
             elif number:
+                self.throttle()
                 purchase_orders = self.accounting_api.get_purchase_order_by_number(
                     self.tenant_id,
                     purchase_order_number=number
                 )
                 if len(purchase_orders.purchase_orders) == 1:
                     return purchase_orders.purchase_orders[0]
                 else:
                     return None
             else:
+                self.throttle()
                 purchase_orders = self.accounting_api.get_purchase_orders(
                     self.tenant_id,
                     **kwargs,
                 )
                 return purchase_orders.purchase_orders
         except AccountingBadRequestException as err:
             logger.error(f'Exception: {err}\n')
@@ -1206,26 +1261,28 @@
             Dictionary or list of retrieved purchase_orders.
         """
         number = kwargs.pop('number', None)
 
         try:
             if number:
                 page = 1
+                self.throttle()
                 purchase_orders = self.accounting_api.get_purchase_orders(
                     self.tenant_id,
                     page=page,
                     **kwargs,
                 )
                 while len(purchase_orders.purchase_orders) > 0:
                     for purchase_order in purchase_orders.purchase_orders:
                         if purchase_order.purchase_order_number == number:
                             return purchase_order
 
                     # read next page
                     page += 1
+                    self.throttle()
                     purchase_orders = self.accounting_api.get_purchase_orders(
                         self.tenant_id,
                         page=page,
                         **kwargs,
                     )
 
         except AccountingBadRequestException as err:
@@ -1244,14 +1301,15 @@
         Args:
             purchase_order_list: List of purchase_orders to update
 
         Returns:
             Dictionary or list of retrieved purchase_orders.
         """
         try:
+            self.throttle()
             purchase_orders = self.accounting_api.update_or_create_purchase_orders(
                 self.tenant_id,
                 purchase_orders=PurchaseOrders(
                     purchase_orders=purchase_order_list
                 )
             )
             return purchase_orders.purchase_orders
@@ -1332,14 +1390,15 @@
         Args:
             repeating_invoice_list: List of repeating invoices to create.
 
         Returns:
             List of created RepeatingInvoice objects.
         """
         try:
+            self.throttle()
             repeating_invoices = self.accounting_api.create_repeating_invoices(
                 self.tenant_id,
                 repeating_invoices=RepeatingInvoices(repeating_invoices=repeating_invoice_list)
             )
             return repeating_invoices.repeating_invoices
         except AccountingBadRequestException as err:
             logger.error(f'Exception: {err}\n')
@@ -1363,23 +1422,25 @@
         Returns:
             Dictionary or list of retrieved repeating invoices.
         """
         repeating_invoice_id = kwargs.pop('id', None)
 
         try:
             if repeating_invoice_id:
+                self.throttle()
                 repeating_invoices = self.accounting_api.get_repeating_invoice(
                     self.tenant_id,
                     repeating_invoice_id=repeating_invoice_id
                 )
                 if len(repeating_invoices.repeating_invoices) == 1:
                     return repeating_invoices.repeating_invoices[0]
                 else:
                     return None
             else:
+                self.throttle()
                 repeating_invoices = self.accounting_api.get_repeating_invoices(
                     self.tenant_id,
                     **kwargs
                 )
                 return repeating_invoices.repeating_invoices
         except AccountingBadRequestException as err:
             logger.error(f'Exception: {err}\n')
@@ -1399,14 +1460,15 @@
         Args:
             repeating_invoice_list: List of repeating invoices to update
 
         Returns:
             Dictionary or list of updated repeating invoices.
         """
         try:
+            self.throttle()
             repeating_invoices = self.accounting_api.update_or_create_repeating_invoices(
                 self.tenant_id,
                 repeating_invoices=RepeatingInvoices(
                     repeating_invoices=repeating_invoice_list
                 )
             )
             return repeating_invoices.repeating_invoices
```

### Comparing `i_xero2-2.6.0/i_xero2/i_xero_ui.py` & `i_xero2-2.7.0/i_xero2/i_xero_ui.py`

 * *Files identical despite different names*

### Comparing `i_xero2-2.6.0/pyproject.toml` & `i_xero2-2.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "i-xero2"
-version = "2.6.0"
+version = "2.7.0"
 description = "Custom connector to Xero"
 authors = ["Jason Romano <aracnid@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/aracnid/i-xero2"
 keywords = ["python", "xero"]
 packages = [{include = "i_xero2"}]
```

### Comparing `i_xero2-2.6.0/setup.py` & `i_xero2-2.7.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'flask>=2.1,<3.0',
  'i-mongodb>=2.0,<3.0',
  'pytz>=2022.1,<2023.0',
  'xero-python>=1.16,<2.0']
 
 setup_kwargs = {
     'name': 'i-xero2',
-    'version': '2.6.0',
+    'version': '2.7.0',
     'description': 'Custom connector to Xero',
     'long_description': '# i-Xero2\n\nThis is a standardized and customized connector to Xero.\n\n## Getting Started\n\nThese instructions will get you a copy of the project up and running on your local machine for development and testing purposes.\n\n### Prerequisites\n\nThis package supports the following version of Python. It probably supports older versions, but they have not been tested.\n\n- Python 3.10 or later\n\n### Installing\n\nInstall the latest package using pip.\n\n```bash\n$ pip install i-xero2\n```\n\nEnd with an example of getting some data out of the system or using it for a little demo\n\n## Running the tests\n\nBefore running the tests, you need to authorize the app with Xero and save the tenant ID in the environment.\n\n1. In Xero, switch to the "Demo Company".\n1. Run the app locally.\n\n    ```bash\n    $ python app.py\n    ```\n\n1. In the browser, navigate to `http://localhost:5000/`\n1. Follow the prompts to allow app to access Xero.\n1. Read tenants.\n1. Copy the `tenantId`.\n1. Save the tenant id as an environment variable named `XERO_TENANT_ID`.\n1. Run the tests.\n\n    ```bash\n    $ python -m pytest\n    ```\n\n## Usage\n\nTODO\n\n## Authors\n\n- **Jason Romano** - [Aracnid](https://github.com/aracnid)\n\nSee also the list of [contributors](https://github.com/aracnid/i-xero2/contributors) who participated in this project.\n\n## License\n\nThis project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details\n',
     'author': 'Jason Romano',
     'author_email': 'aracnid@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/aracnid/i-xero2',
```

### Comparing `i_xero2-2.6.0/PKG-INFO` & `i_xero2-2.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i-xero2
-Version: 2.6.0
+Version: 2.7.0
 Summary: Custom connector to Xero
 Home-page: https://github.com/aracnid/i-xero2
 License: MIT
 Keywords: python,xero
 Author: Jason Romano
 Author-email: aracnid@gmail.com
 Requires-Python: >=3.10,<4.0
```

