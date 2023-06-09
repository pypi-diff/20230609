# Comparing `tmp/netbox-unacceptable-events-users-computers-0.1.3.7.tar.gz` & `tmp/netbox-unacceptable-events-users-computers-0.1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-unacceptable-events-users-computers-0.1.3.7.tar", last modified: Thu Feb 23 18:22:40 2023, max compression
+gzip compressed data, was "netbox-unacceptable-events-users-computers-0.1.3.8.tar", last modified: Sat Feb 25 00:42:42 2023, max compression
```

## Comparing `netbox-unacceptable-events-users-computers-0.1.3.7.tar` & `netbox-unacceptable-events-users-computers-0.1.3.8.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-02-23 18:22:40.821640 netbox-unacceptable-events-users-computers-0.1.3.7/
--rw-rw-rw-   0        0        0    11558 2023-01-26 23:45:00.000000 netbox-unacceptable-events-users-computers-0.1.3.7/LICENSE
--rw-rw-rw-   0        0        0       36 2023-01-26 23:45:00.000000 netbox-unacceptable-events-users-computers-0.1.3.7/MANIFEST.in
--rw-rw-rw-   0        0        0     1063 2023-02-23 18:22:40.820639 netbox-unacceptable-events-users-computers-0.1.3.7/PKG-INFO
--rw-rw-rw-   0        0        0      360 2023-02-23 15:42:42.000000 netbox-unacceptable-events-users-computers-0.1.3.7/README.md
-drwxrwxrwx   0        0        0        0 2023-02-23 18:22:40.776668 netbox-unacceptable-events-users-computers-0.1.3.7/netbox_unacceptable_events_users_computers.egg-info/
--rw-rw-rw-   0        0        0     1063 2023-02-23 18:22:40.000000 netbox-unacceptable-events-users-computers-0.1.3.7/netbox_unacceptable_events_users_computers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1119 2023-02-23 18:22:40.000000 netbox-unacceptable-events-users-computers-0.1.3.7/netbox_unacceptable_events_users_computers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-23 18:22:40.000000 netbox-unacceptable-events-users-computers-0.1.3.7/netbox_unacceptable_events_users_computers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-02-23 15:27:27.000000 netbox-unacceptable-events-users-computers-0.1.3.7/netbox_unacceptable_events_users_computers.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       10 2023-02-23 18:22:40.000000 netbox-unacceptable-events-users-computers-0.1.3.7/netbox_unacceptable_events_users_computers.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-23 18:22:40.795635 netbox-unacceptable-events-users-computers-0.1.3.7/ptuevents/
--rw-rw-rw-   0        0        0      441 2023-02-23 18:22:27.000000 netbox-unacceptable-events-users-computers-0.1.3.7/ptuevents/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-23 18:22:40.801635 netbox-unacceptable-events-users-computers-0.1.3.7/ptuevents/api/
--rw-rw-rw-   0        0        0        0 2023-01-26 23:45:00.000000 netbox-unacceptable-events-users-computers-0.1.3.7/ptuevents/api/__init__.py
--rw-rw-rw-   0        0        0     5141 2023-01-26 23:45:00.000000 netbox-unacceptable-events-users-computers-0.1.3.7/ptuevents/api/serializers.py
--rw-rw-rw-   0        0        0      515 2023-01-26 23:45:00.000000 netbox-unacceptable-events-users-computers-0.1.3.7/ptuevents/api/urls.py
--rw-rw-rw-   0        0        0     1477 2023-01-26 23:45:00.000000 netbox-unacceptable-events-users-computers-0.1.3.7/ptuevents/api/views.py
--rw-rw-rw-   0        0        0     1873 2023-01-26 23:45:00.000000 netbox-unacceptable-events-users-computers-0.1.3.7/ptuevents/filtersets.py
--rw-rw-rw-   0        0        0     1610 2023-01-26 23:45:00.000000 netbox-unacceptable-events-users-computers-0.1.3.7/ptuevents/forms.py
--rw-rw-rw-   0        0        0     1719 2023-01-26 23:45:00.000000 netbox-unacceptable-events-users-computers-0.1.3.7/ptuevents/graphql.py
-drwxrwxrwx   0        0        0        0 2023-02-23 18:22:40.805635 netbox-unacceptable-events-users-computers-0.1.3.7/ptuevents/migrations/
--rw-rw-rw-   0        0        0     5626 2023-02-23 18:22:27.000000 netbox-unacceptable-events-users-computers-0.1.3.7/ptuevents/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2023-01-26 23:45:00.000000 netbox-unacceptable-events-users-computers-0.1.3.7/ptuevents/migrations/__init__.py
--rw-rw-rw-   0        0        0     4900 2023-01-26 23:45:00.000000 netbox-unacceptable-events-users-computers-0.1.3.7/ptuevents/models.py
--rw-rw-rw-   0        0        0     1271 2023-01-26 23:45:00.000000 netbox-unacceptable-events-users-computers-0.1.3.7/ptuevents/navigation.py
--rw-rw-rw-   0        0        0     2250 2023-01-26 23:45:00.000000 netbox-unacceptable-events-users-computers-0.1.3.7/ptuevents/tables.py
--rw-rw-rw-   0        0        0     3992 2023-01-26 23:45:00.000000 netbox-unacceptable-events-users-computers-0.1.3.7/ptuevents/template_content.py
-drwxrwxrwx   0        0        0        0 2023-02-23 18:22:40.759078 netbox-unacceptable-events-users-computers-0.1.3.7/ptuevents/templates/
-drwxrwxrwx   0        0        0        0 2023-02-23 18:22:40.818638 netbox-unacceptable-events-users-computers-0.1.3.7/ptuevents/templates/ptuevents/
--rw-rw-rw-   0        0        0      624 2023-01-26 23:45:00.000000 netbox-unacceptable-events-users-computers-0.1.3.7/ptuevents/templates/ptuevents/appsystem_assignment_edit.html
--rw-rw-rw-   0        0        0     1436 2023-01-26 23:45:00.000000 netbox-unacceptable-events-users-computers-0.1.3.7/ptuevents/templates/ptuevents/appsystem_panel.html
--rw-rw-rw-   0        0        0     1468 2023-01-26 23:45:00.000000 netbox-unacceptable-events-users-computers-0.1.3.7/ptuevents/templates/ptuevents/ptappsystem.html
--rw-rw-rw-   0        0        0      773 2023-01-26 23:45:00.000000 netbox-unacceptable-events-users-computers-0.1.3.7/ptuevents/templates/ptuevents/ptuevent.html
--rw-rw-rw-   0        0        0      616 2023-01-26 23:45:00.000000 netbox-unacceptable-events-users-computers-0.1.3.7/ptuevents/templates/ptuevents/ptuevent_assignment_edit.html
--rw-rw-rw-   0        0        0     1545 2023-01-26 23:45:00.000000 netbox-unacceptable-events-users-computers-0.1.3.7/ptuevents/templates/ptuevents/ptuevent_panel.html
--rw-rw-rw-   0        0        0      731 2023-01-26 23:45:00.000000 netbox-unacceptable-events-users-computers-0.1.3.7/ptuevents/templates/ptuevents/ptueventrelation.html
--rw-rw-rw-   0        0        0     3140 2023-01-26 23:45:00.000000 netbox-unacceptable-events-users-computers-0.1.3.7/ptuevents/urls.py
--rw-rw-rw-   0        0        0     5907 2023-01-26 23:45:00.000000 netbox-unacceptable-events-users-computers-0.1.3.7/ptuevents/views.py
--rw-rw-rw-   0        0        0       42 2023-02-23 18:22:40.821640 netbox-unacceptable-events-users-computers-0.1.3.7/setup.cfg
--rw-rw-rw-   0        0        0     1064 2023-02-23 18:22:27.000000 netbox-unacceptable-events-users-computers-0.1.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-02-25 00:42:42.704225 netbox-unacceptable-events-users-computers-0.1.3.8/
+-rw-rw-rw-   0        0        0    11558 2023-01-26 23:45:00.000000 netbox-unacceptable-events-users-computers-0.1.3.8/LICENSE
+-rw-rw-rw-   0        0        0       36 2023-01-26 23:45:00.000000 netbox-unacceptable-events-users-computers-0.1.3.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     1063 2023-02-25 00:42:42.704225 netbox-unacceptable-events-users-computers-0.1.3.8/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2023-02-23 15:42:42.000000 netbox-unacceptable-events-users-computers-0.1.3.8/README.md
+drwxrwxrwx   0        0        0        0 2023-02-25 00:42:42.643214 netbox-unacceptable-events-users-computers-0.1.3.8/netbox_unacceptable_events_users_computers.egg-info/
+-rw-rw-rw-   0        0        0     1063 2023-02-25 00:42:42.000000 netbox-unacceptable-events-users-computers-0.1.3.8/netbox_unacceptable_events_users_computers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1166 2023-02-25 00:42:42.000000 netbox-unacceptable-events-users-computers-0.1.3.8/netbox_unacceptable_events_users_computers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-02-25 00:42:42.000000 netbox-unacceptable-events-users-computers-0.1.3.8/netbox_unacceptable_events_users_computers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-02-23 15:27:27.000000 netbox-unacceptable-events-users-computers-0.1.3.8/netbox_unacceptable_events_users_computers.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       10 2023-02-25 00:42:42.000000 netbox-unacceptable-events-users-computers-0.1.3.8/netbox_unacceptable_events_users_computers.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-02-25 00:42:42.668214 netbox-unacceptable-events-users-computers-0.1.3.8/ptuevents/
+-rw-rw-rw-   0        0        0      441 2023-02-25 00:42:20.000000 netbox-unacceptable-events-users-computers-0.1.3.8/ptuevents/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-25 00:42:42.676214 netbox-unacceptable-events-users-computers-0.1.3.8/ptuevents/api/
+-rw-rw-rw-   0        0        0        0 2023-01-26 23:45:00.000000 netbox-unacceptable-events-users-computers-0.1.3.8/ptuevents/api/__init__.py
+-rw-rw-rw-   0        0        0     5141 2023-01-26 23:45:00.000000 netbox-unacceptable-events-users-computers-0.1.3.8/ptuevents/api/serializers.py
+-rw-rw-rw-   0        0        0      515 2023-01-26 23:45:00.000000 netbox-unacceptable-events-users-computers-0.1.3.8/ptuevents/api/urls.py
+-rw-rw-rw-   0        0        0     1477 2023-01-26 23:45:00.000000 netbox-unacceptable-events-users-computers-0.1.3.8/ptuevents/api/views.py
+-rw-rw-rw-   0        0        0     1873 2023-01-26 23:45:00.000000 netbox-unacceptable-events-users-computers-0.1.3.8/ptuevents/filtersets.py
+-rw-rw-rw-   0        0        0     2237 2023-02-25 00:40:09.000000 netbox-unacceptable-events-users-computers-0.1.3.8/ptuevents/forms.py
+-rw-rw-rw-   0        0        0     1719 2023-01-26 23:45:00.000000 netbox-unacceptable-events-users-computers-0.1.3.8/ptuevents/graphql.py
+drwxrwxrwx   0        0        0        0 2023-02-25 00:42:42.681218 netbox-unacceptable-events-users-computers-0.1.3.8/ptuevents/migrations/
+-rw-rw-rw-   0        0        0     8624 2023-02-25 00:40:09.000000 netbox-unacceptable-events-users-computers-0.1.3.8/ptuevents/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2023-01-26 23:45:00.000000 netbox-unacceptable-events-users-computers-0.1.3.8/ptuevents/migrations/__init__.py
+-rw-rw-rw-   0        0        0     7430 2023-02-25 00:40:09.000000 netbox-unacceptable-events-users-computers-0.1.3.8/ptuevents/models.py
+-rw-rw-rw-   0        0        0     1271 2023-01-26 23:45:00.000000 netbox-unacceptable-events-users-computers-0.1.3.8/ptuevents/navigation.py
+-rw-rw-rw-   0        0        0     3205 2023-02-25 00:40:09.000000 netbox-unacceptable-events-users-computers-0.1.3.8/ptuevents/tables.py
+-rw-rw-rw-   0        0        0     3992 2023-01-26 23:45:00.000000 netbox-unacceptable-events-users-computers-0.1.3.8/ptuevents/template_content.py
+drwxrwxrwx   0        0        0        0 2023-02-25 00:42:42.624212 netbox-unacceptable-events-users-computers-0.1.3.8/ptuevents/templates/
+drwxrwxrwx   0        0        0        0 2023-02-25 00:42:42.701214 netbox-unacceptable-events-users-computers-0.1.3.8/ptuevents/templates/ptuevents/
+-rw-rw-rw-   0        0        0      624 2023-01-26 23:45:00.000000 netbox-unacceptable-events-users-computers-0.1.3.8/ptuevents/templates/ptuevents/appsystem_assignment_edit.html
+-rw-rw-rw-   0        0        0     1436 2023-01-26 23:45:00.000000 netbox-unacceptable-events-users-computers-0.1.3.8/ptuevents/templates/ptuevents/appsystem_panel.html
+-rw-rw-rw-   0        0        0     1468 2023-01-26 23:45:00.000000 netbox-unacceptable-events-users-computers-0.1.3.8/ptuevents/templates/ptuevents/ptappsystem.html
+-rw-rw-rw-   0        0        0      773 2023-01-26 23:45:00.000000 netbox-unacceptable-events-users-computers-0.1.3.8/ptuevents/templates/ptuevents/ptuevent.html
+-rw-rw-rw-   0        0        0      616 2023-01-26 23:45:00.000000 netbox-unacceptable-events-users-computers-0.1.3.8/ptuevents/templates/ptuevents/ptuevent_assignment_edit.html
+-rw-rw-rw-   0        0        0     1545 2023-01-26 23:45:00.000000 netbox-unacceptable-events-users-computers-0.1.3.8/ptuevents/templates/ptuevents/ptuevent_panel.html
+-rw-rw-rw-   0        0        0      731 2023-01-26 23:45:00.000000 netbox-unacceptable-events-users-computers-0.1.3.8/ptuevents/templates/ptuevents/ptueventrelation.html
+-rw-rw-rw-   0        0        0     2202 2023-01-14 21:06:20.000000 netbox-unacceptable-events-users-computers-0.1.3.8/ptuevents/templates/ptuevents/ptusers_add.html
+-rw-rw-rw-   0        0        0     4423 2023-02-25 00:40:09.000000 netbox-unacceptable-events-users-computers-0.1.3.8/ptuevents/urls.py
+-rw-rw-rw-   0        0        0     6952 2023-02-25 00:40:09.000000 netbox-unacceptable-events-users-computers-0.1.3.8/ptuevents/views.py
+-rw-rw-rw-   0        0        0       42 2023-02-25 00:42:42.705214 netbox-unacceptable-events-users-computers-0.1.3.8/setup.cfg
+-rw-rw-rw-   0        0        0     1064 2023-02-25 00:42:20.000000 netbox-unacceptable-events-users-computers-0.1.3.8/setup.py
```

### Comparing `netbox-unacceptable-events-users-computers-0.1.3.7/LICENSE` & `netbox-unacceptable-events-users-computers-0.1.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-unacceptable-events-users-computers-0.1.3.7/PKG-INFO` & `netbox-unacceptable-events-users-computers-0.1.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-unacceptable-events-users-computers
-Version: 0.1.3.7
+Version: 0.1.3.8
 Summary: Netbox plugin. Assign devices and virtual machines and application systems to information security unacceptable events
 Download-URL: https://pypi.org/project/netbox-unacceptable-events-users-computers/
 Author: Artur Shamsiev
 Author-email: me@z-lab.me
 Maintainer: Artur Shamsiev
 Maintainer-email: me@z-lab.me
 License: MIT
```

### Comparing `netbox-unacceptable-events-users-computers-0.1.3.7/netbox_unacceptable_events_users_computers.egg-info/PKG-INFO` & `netbox-unacceptable-events-users-computers-0.1.3.8/netbox_unacceptable_events_users_computers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-unacceptable-events-users-computers
-Version: 0.1.3.7
+Version: 0.1.3.8
 Summary: Netbox plugin. Assign devices and virtual machines and application systems to information security unacceptable events
 Download-URL: https://pypi.org/project/netbox-unacceptable-events-users-computers/
 Author: Artur Shamsiev
 Author-email: me@z-lab.me
 Maintainer: Artur Shamsiev
 Maintainer-email: me@z-lab.me
 License: MIT
```

### Comparing `netbox-unacceptable-events-users-computers-0.1.3.7/netbox_unacceptable_events_users_computers.egg-info/SOURCES.txt` & `netbox-unacceptable-events-users-computers-0.1.3.8/netbox_unacceptable_events_users_computers.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -25,8 +25,9 @@
 ptuevents/migrations/__init__.py
 ptuevents/templates/ptuevents/appsystem_assignment_edit.html
 ptuevents/templates/ptuevents/appsystem_panel.html
 ptuevents/templates/ptuevents/ptappsystem.html
 ptuevents/templates/ptuevents/ptuevent.html
 ptuevents/templates/ptuevents/ptuevent_assignment_edit.html
 ptuevents/templates/ptuevents/ptuevent_panel.html
-ptuevents/templates/ptuevents/ptueventrelation.html
+ptuevents/templates/ptuevents/ptueventrelation.html
+ptuevents/templates/ptuevents/ptusers_add.html
```

### Comparing `netbox-unacceptable-events-users-computers-0.1.3.7/ptuevents/api/serializers.py` & `netbox-unacceptable-events-users-computers-0.1.3.8/ptuevents/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox-unacceptable-events-users-computers-0.1.3.7/ptuevents/api/urls.py` & `netbox-unacceptable-events-users-computers-0.1.3.8/ptuevents/api/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-unacceptable-events-users-computers-0.1.3.7/ptuevents/api/views.py` & `netbox-unacceptable-events-users-computers-0.1.3.8/ptuevents/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox-unacceptable-events-users-computers-0.1.3.7/ptuevents/filtersets.py` & `netbox-unacceptable-events-users-computers-0.1.3.8/ptuevents/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox-unacceptable-events-users-computers-0.1.3.7/ptuevents/forms.py` & `netbox-unacceptable-events-users-computers-0.1.3.8/ptuevents/forms.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from netbox.forms import NetBoxModelForm
 from tenancy.models import Tenant
 from pyrsistent import v
-from .models import PTUEvent, PTUEventRelation, PTUEventAssignment, PTAppSystem, PTAppSystemAssignment
+from .models import PTUEvent, PTUEventRelation, PTUEventAssignment, PTAppSystem, PTAppSystemAssignment, PTUsers, PTWorkstations
 from utilities.forms.fields import CommentField
 from utilities.forms import (
     BootstrapMixin, DynamicModelChoiceField)
 from django import forms
 
 
 class PTUEventForm(NetBoxModelForm):
@@ -49,7 +49,27 @@
     app_system = DynamicModelChoiceField(queryset=PTAppSystem.objects.all(), query_params={
         'tenant': '$tenant',
     })
 
     class Meta:
         model = PTAppSystemAssignment
         fields = ('app_system',)
+
+
+class PTUsersForm(NetBoxModelForm):
+    class Meta:
+        model = PTUsers
+        fields = ('name',
+                  'sAMAccountName',
+                  'status',
+                  'firstname',
+                  'lastname', 'ad_guid', 'ad_description', 'position', 'department', 'comment',
+                  'vpnIPaddress',
+                  'description',
+                  'comments')
+
+
+class PTWorkstationsForm(NetBoxModelForm):
+    class Meta:
+        model = PTWorkstations
+        fields = ('name', 'CN', 'DistinguishedName', 'ad_guid', 'ad_description', 'description')
+
```

### Comparing `netbox-unacceptable-events-users-computers-0.1.3.7/ptuevents/graphql.py` & `netbox-unacceptable-events-users-computers-0.1.3.8/ptuevents/graphql.py`

 * *Files identical despite different names*

### Comparing `netbox-unacceptable-events-users-computers-0.1.3.7/ptuevents/navigation.py` & `netbox-unacceptable-events-users-computers-0.1.3.8/ptuevents/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox-unacceptable-events-users-computers-0.1.3.7/ptuevents/tables.py` & `netbox-unacceptable-events-users-computers-0.1.3.8/ptuevents/tables.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import django_tables2 as tables
 from netbox.tables import NetBoxTable, columns
-from .models import PTUEvent, PTUEventRelation, PTUEventAssignment, PTAppSystem, PTAppSystemAssignment
+from .models import PTUEvent, PTUEventRelation, PTUEventAssignment, PTAppSystem, PTAppSystemAssignment, PTWorkstations, PTUsers
 
 
 class PTUEventTable(NetBoxTable):
     name = tables.Column(
         linkify=True
     )
     # default_action = ChoiceFieldColumn()
@@ -65,7 +65,34 @@
     app_system = tables.Column(linkify=True)
     actions = columns.ActionsColumn(actions=('edit', 'delete'))
 
     class Meta(NetBoxTable.Meta):
         model = PTAppSystemAssignment
         fields = ('pk', 'content_type', 'object', 'app_system', 'actions')
         default_columns = ('pk', 'content_type', 'object', 'app_system')
+
+
+class PTUsersTable(NetBoxTable):
+    name = tables.Column(
+        linkify=True
+    )
+
+    class Meta(NetBoxTable.Meta):
+        model = PTUsers
+        fields = ('pk', 'name', 'sAMAccountName',
+                  'status',
+                  'firstname',
+                  'lastname', 'ad_guid', 'ad_description', 'position', 'department', 'comment',
+                  'vpnIPaddress', 'description')
+        default_columns = ('name', 'sAMAccountName',
+                  'status',
+                  'firstname',
+                  'lastname', 'ad_guid', 'description')
+
+
+class PTWorkstationsTable(NetBoxTable):
+    name = tables.Column(linkify=True)
+
+    class Meta(NetBoxTable.Meta):
+        model = PTWorkstations
+        fields = ('pk', 'name', 'CN', 'DistinguishedName', 'ad_description', 'description')
+        default_columns = ('name', 'CN', 'DistinguishedName', 'ad_description', 'description')
```

### Comparing `netbox-unacceptable-events-users-computers-0.1.3.7/ptuevents/template_content.py` & `netbox-unacceptable-events-users-computers-0.1.3.8/ptuevents/template_content.py`

 * *Files identical despite different names*

### Comparing `netbox-unacceptable-events-users-computers-0.1.3.7/ptuevents/templates/ptuevents/appsystem_assignment_edit.html` & `netbox-unacceptable-events-users-computers-0.1.3.8/ptuevents/templates/ptuevents/appsystem_assignment_edit.html`

 * *Files identical despite different names*

### Comparing `netbox-unacceptable-events-users-computers-0.1.3.7/ptuevents/templates/ptuevents/appsystem_panel.html` & `netbox-unacceptable-events-users-computers-0.1.3.8/ptuevents/templates/ptuevents/appsystem_panel.html`

 * *Files identical despite different names*

### Comparing `netbox-unacceptable-events-users-computers-0.1.3.7/ptuevents/templates/ptuevents/ptappsystem.html` & `netbox-unacceptable-events-users-computers-0.1.3.8/ptuevents/templates/ptuevents/ptappsystem.html`

 * *Files identical despite different names*

### Comparing `netbox-unacceptable-events-users-computers-0.1.3.7/ptuevents/templates/ptuevents/ptuevent.html` & `netbox-unacceptable-events-users-computers-0.1.3.8/ptuevents/templates/ptuevents/ptuevent.html`

 * *Files identical despite different names*

### Comparing `netbox-unacceptable-events-users-computers-0.1.3.7/ptuevents/templates/ptuevents/ptuevent_assignment_edit.html` & `netbox-unacceptable-events-users-computers-0.1.3.8/ptuevents/templates/ptuevents/ptuevent_assignment_edit.html`

 * *Files identical despite different names*

### Comparing `netbox-unacceptable-events-users-computers-0.1.3.7/ptuevents/templates/ptuevents/ptuevent_panel.html` & `netbox-unacceptable-events-users-computers-0.1.3.8/ptuevents/templates/ptuevents/ptuevent_panel.html`

 * *Files identical despite different names*

### Comparing `netbox-unacceptable-events-users-computers-0.1.3.7/ptuevents/templates/ptuevents/ptueventrelation.html` & `netbox-unacceptable-events-users-computers-0.1.3.8/ptuevents/templates/ptuevents/ptueventrelation.html`

 * *Files identical despite different names*

### Comparing `netbox-unacceptable-events-users-computers-0.1.3.7/ptuevents/views.py` & `netbox-unacceptable-events-users-computers-0.1.3.8/ptuevents/views.py`

 * *Files 16% similar despite different names*

```diff
@@ -160,7 +160,47 @@
                 return HttpResponseRedirect(redirect_url)
 
         return super().post(request, *args, **kwargs)
 
 
 class PTAppSystemAssignmentDeleteView(generic.ObjectDeleteView):
     queryset = models.PTAppSystemAssignment.objects.all()
+
+
+# PTUsers
+class PTUsersView(generic.ObjectView):
+    queryset = models.PTUsers.objects.all()
+    template_name = 'ptuevents/ptusers_add.html'
+
+
+class PTUsersListView(generic.ObjectListView):
+    queryset = models.PTUsers.objects.all()
+    table = tables.PTUsersTable
+
+
+class PTUsersEditView(generic.ObjectEditView):
+    queryset = models.PTUsers.objects.all()
+    form = forms.PTUsersForm
+
+
+class PTUsersDeleteView(generic.ObjectDeleteView):
+    queryset = models.PTUsers.objects.all()
+
+
+# PTWorkstations
+
+class PTWorkstationsView(generic.ObjectView):
+    queryset = models.PTWorkstations.objects.all()
+
+
+class PTWorkstationsListView(generic.ObjectListView):
+    queryset = models.PTWorkstations.objects.all()
+    table = tables.PTWorkstationsTable
+
+
+class PTWorkstationsEditView(generic.ObjectEditView):
+    queryset = models.PTWorkstations.objects.all()
+    form = forms.PTWorkstationsForm
+
+
+class PTWorkstationsDeleteView(generic.ObjectDeleteView):
+    queryset = models.PTWorkstations.objects.all()
```

### Comparing `netbox-unacceptable-events-users-computers-0.1.3.7/setup.py` & `netbox-unacceptable-events-users-computers-0.1.3.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='netbox-unacceptable-events-users-computers',
-    version='0.1.3.0007',
+    version='0.1.3.0008',
     description='Netbox plugin. Assign devices and virtual machines and application systems to information security unacceptable events',
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[],
     download_url='https://pypi.org/project/netbox-unacceptable-events-users-computers/',
     packages=find_packages(),
     include_package_data=True,
```

