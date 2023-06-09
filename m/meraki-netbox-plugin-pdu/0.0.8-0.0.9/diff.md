# Comparing `tmp/meraki-netbox-plugin-pdu-0.0.8.tar.gz` & `tmp/meraki-netbox-plugin-pdu-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meraki-netbox-plugin-pdu-0.0.8.tar", max compression
+gzip compressed data, was "meraki-netbox-plugin-pdu-0.0.9.tar", max compression
```

## Comparing `meraki-netbox-plugin-pdu-0.0.8.tar` & `meraki-netbox-plugin-pdu-0.0.9.tar`

### file list

```diff
@@ -1,41 +1,37 @@
--rw-r--r--   0        0        0     6129 2022-02-17 11:57:19.483656 meraki-netbox-plugin-pdu-0.0.8/README.md
--rw-r--r--   0        0        0      787 2022-02-17 11:57:19.483656 meraki-netbox-plugin-pdu-0.0.8/axians_netbox_pdu/__init__.py
--rw-r--r--   0        0        0       52 2022-02-17 11:57:19.483656 meraki-netbox-plugin-pdu-0.0.8/axians_netbox_pdu/api/__init__.py
--rw-r--r--   0        0        0     2142 2022-02-17 11:57:19.483656 meraki-netbox-plugin-pdu-0.0.8/axians_netbox_pdu/api/serializers.py
--rw-r--r--   0        0        0      250 2022-02-17 11:57:19.483656 meraki-netbox-plugin-pdu-0.0.8/axians_netbox_pdu/api/urls.py
--rw-r--r--   0        0        0      962 2022-02-17 11:57:19.483656 meraki-netbox-plugin-pdu-0.0.8/axians_netbox_pdu/api/views.py
--rw-r--r--   0        0        0      321 2022-02-17 11:57:19.483656 meraki-netbox-plugin-pdu-0.0.8/axians_netbox_pdu/choices.py
--rw-r--r--   0        0        0     2150 2022-02-17 11:57:19.483656 meraki-netbox-plugin-pdu-0.0.8/axians_netbox_pdu/filters.py
--rw-r--r--   0        0        0     2549 2022-02-17 11:57:19.483656 meraki-netbox-plugin-pdu-0.0.8/axians_netbox_pdu/forms.py
--rw-r--r--   0        0        0        0 2022-02-17 11:57:19.483656 meraki-netbox-plugin-pdu-0.0.8/axians_netbox_pdu/management/__init__.py
--rw-r--r--   0        0        0        0 2022-02-17 11:57:19.483656 meraki-netbox-plugin-pdu-0.0.8/axians_netbox_pdu/management/commands/__init__.py
--rw-r--r--   0        0        0     1041 2022-02-17 11:57:19.483656 meraki-netbox-plugin-pdu-0.0.8/axians_netbox_pdu/management/commands/pduscheduler.py
--rw-r--r--   0        0        0      904 2022-02-17 11:57:19.483656 meraki-netbox-plugin-pdu-0.0.8/axians_netbox_pdu/migrations/0001_initial.py
--rw-r--r--   0        0        0      915 2022-02-17 11:57:19.483656 meraki-netbox-plugin-pdu-0.0.8/axians_netbox_pdu/migrations/0002_pdustatus.py
--rw-r--r--   0        0        0        0 2022-02-17 11:57:19.483656 meraki-netbox-plugin-pdu-0.0.8/axians_netbox_pdu/migrations/__init__.py
--rw-r--r--   0        0        0     1408 2022-02-17 11:57:19.483656 meraki-netbox-plugin-pdu-0.0.8/axians_netbox_pdu/models.py
--rw-r--r--   0        0        0     1213 2022-02-17 11:57:19.483656 meraki-netbox-plugin-pdu-0.0.8/axians_netbox_pdu/navigation.py
--rw-r--r--   0        0        0      738 2022-02-17 11:57:19.483656 meraki-netbox-plugin-pdu-0.0.8/axians_netbox_pdu/tables.py
--rw-r--r--   0        0        0     2837 2022-02-17 11:57:19.483656 meraki-netbox-plugin-pdu-0.0.8/axians_netbox_pdu/template_content.py
--rw-r--r--   0        0        0      732 2022-02-17 11:57:19.483656 meraki-netbox-plugin-pdu-0.0.8/axians_netbox_pdu/templates/axians_netbox_pdu/device_power_usage.html
--rw-r--r--   0        0        0      837 2022-02-17 11:57:19.483656 meraki-netbox-plugin-pdu-0.0.8/axians_netbox_pdu/templates/axians_netbox_pdu/device_power_usage_3_x.html
--rw-r--r--   0        0        0      934 2022-02-17 11:57:19.483656 meraki-netbox-plugin-pdu-0.0.8/axians_netbox_pdu/templates/axians_netbox_pdu/device_type_pduconfig.html
--rw-r--r--   0        0        0     1011 2022-02-17 11:57:19.483656 meraki-netbox-plugin-pdu-0.0.8/axians_netbox_pdu/templates/axians_netbox_pdu/device_type_pduconfig_3_x.html
--rw-r--r--   0        0        0       65 2022-02-17 11:57:19.483656 meraki-netbox-plugin-pdu-0.0.8/axians_netbox_pdu/templates/axians_netbox_pdu/pduconfig_edit.html
--rw-r--r--   0        0        0       65 2022-02-17 11:57:19.483656 meraki-netbox-plugin-pdu-0.0.8/axians_netbox_pdu/templates/axians_netbox_pdu/pduconfig_edit_3_x.html
--rw-r--r--   0        0        0     3515 2022-02-17 11:57:19.483656 meraki-netbox-plugin-pdu-0.0.8/axians_netbox_pdu/templates/axians_netbox_pdu/pduconfig_list.html
--rw-r--r--   0        0        0       81 2022-02-17 11:57:19.483656 meraki-netbox-plugin-pdu-0.0.8/axians_netbox_pdu/templates/axians_netbox_pdu/pduconfig_view.html
--rw-r--r--   0        0        0      127 2022-02-17 11:57:19.483656 meraki-netbox-plugin-pdu-0.0.8/axians_netbox_pdu/templates/axians_netbox_pdu/pduconfig_view_3_x.html
--rw-r--r--   0        0        0     2112 2022-02-17 11:57:19.483656 meraki-netbox-plugin-pdu-0.0.8/axians_netbox_pdu/templates/axians_netbox_pdu/rack_power_usage.html
--rw-r--r--   0        0        0     2369 2022-02-17 11:57:19.483656 meraki-netbox-plugin-pdu-0.0.8/axians_netbox_pdu/templates/axians_netbox_pdu/rack_power_usage_3_x.html
--rw-r--r--   0        0        0       43 2022-02-17 11:57:19.483656 meraki-netbox-plugin-pdu-0.0.8/axians_netbox_pdu/tests/__init__.py
--rw-r--r--   0        0        0     7680 2022-02-17 11:57:19.483656 meraki-netbox-plugin-pdu-0.0.8/axians_netbox_pdu/tests/test_pduconfig_api.py
--rw-r--r--   0        0        0    13374 2022-02-17 11:57:19.483656 meraki-netbox-plugin-pdu-0.0.8/axians_netbox_pdu/tests/test_pduconfig_views.py
--rw-r--r--   0        0        0     8066 2022-02-17 11:57:19.483656 meraki-netbox-plugin-pdu-0.0.8/axians_netbox_pdu/tests/test_pdustatus_api.py
--rw-r--r--   0        0        0      632 2022-02-17 11:57:19.483656 meraki-netbox-plugin-pdu-0.0.8/axians_netbox_pdu/urls.py
--rw-r--r--   0        0        0     1648 2022-02-17 11:57:19.483656 meraki-netbox-plugin-pdu-0.0.8/axians_netbox_pdu/utilities.py
--rw-r--r--   0        0        0     2284 2022-02-17 11:57:19.483656 meraki-netbox-plugin-pdu-0.0.8/axians_netbox_pdu/views.py
--rw-r--r--   0        0        0     1317 2022-02-17 11:57:19.483656 meraki-netbox-plugin-pdu-0.0.8/axians_netbox_pdu/worker.py
--rw-r--r--   0        0        0     1380 2022-02-17 11:57:19.487656 meraki-netbox-plugin-pdu-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     7247 2022-02-17 11:58:01.836833 meraki-netbox-plugin-pdu-0.0.8/setup.py
--rw-r--r--   0        0        0     7074 2022-02-17 11:58:01.837349 meraki-netbox-plugin-pdu-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     6129 2022-08-17 15:42:10.719943 meraki-netbox-plugin-pdu-0.0.9/README.md
+-rw-r--r--   0        0        0      787 2022-08-17 15:42:10.719943 meraki-netbox-plugin-pdu-0.0.9/axians_netbox_pdu/__init__.py
+-rw-r--r--   0        0        0       52 2022-08-17 15:42:10.719943 meraki-netbox-plugin-pdu-0.0.9/axians_netbox_pdu/api/__init__.py
+-rw-r--r--   0        0        0     2142 2022-08-17 15:42:10.719943 meraki-netbox-plugin-pdu-0.0.9/axians_netbox_pdu/api/serializers.py
+-rw-r--r--   0        0        0      250 2022-08-17 15:42:10.719943 meraki-netbox-plugin-pdu-0.0.9/axians_netbox_pdu/api/urls.py
+-rw-r--r--   0        0        0      962 2022-08-17 15:42:10.719943 meraki-netbox-plugin-pdu-0.0.9/axians_netbox_pdu/api/views.py
+-rw-r--r--   0        0        0      321 2022-08-17 15:42:10.719943 meraki-netbox-plugin-pdu-0.0.9/axians_netbox_pdu/choices.py
+-rw-r--r--   0        0        0     2150 2022-08-17 15:42:10.719943 meraki-netbox-plugin-pdu-0.0.9/axians_netbox_pdu/filters.py
+-rw-r--r--   0        0        0     1650 2022-08-17 15:42:10.719943 meraki-netbox-plugin-pdu-0.0.9/axians_netbox_pdu/forms.py
+-rw-r--r--   0        0        0        0 2022-08-17 15:42:10.719943 meraki-netbox-plugin-pdu-0.0.9/axians_netbox_pdu/management/__init__.py
+-rw-r--r--   0        0        0        0 2022-08-17 15:42:10.719943 meraki-netbox-plugin-pdu-0.0.9/axians_netbox_pdu/management/commands/__init__.py
+-rw-r--r--   0        0        0     1041 2022-08-17 15:42:10.719943 meraki-netbox-plugin-pdu-0.0.9/axians_netbox_pdu/management/commands/pduscheduler.py
+-rw-r--r--   0        0        0      904 2022-08-17 15:42:10.719943 meraki-netbox-plugin-pdu-0.0.9/axians_netbox_pdu/migrations/0001_initial.py
+-rw-r--r--   0        0        0      915 2022-08-17 15:42:10.719943 meraki-netbox-plugin-pdu-0.0.9/axians_netbox_pdu/migrations/0002_pdustatus.py
+-rw-r--r--   0        0        0     2299 2022-08-17 15:42:10.719943 meraki-netbox-plugin-pdu-0.0.9/axians_netbox_pdu/migrations/0003_pduconfig_created_pduconfig_custom_field_data_and_more.py
+-rw-r--r--   0        0        0        0 2022-08-17 15:42:10.719943 meraki-netbox-plugin-pdu-0.0.9/axians_netbox_pdu/migrations/__init__.py
+-rw-r--r--   0        0        0     1444 2022-08-17 15:42:10.719943 meraki-netbox-plugin-pdu-0.0.9/axians_netbox_pdu/models.py
+-rw-r--r--   0        0        0      631 2022-08-17 15:42:10.719943 meraki-netbox-plugin-pdu-0.0.9/axians_netbox_pdu/navigation.py
+-rw-r--r--   0        0        0      745 2022-08-17 15:42:10.719943 meraki-netbox-plugin-pdu-0.0.9/axians_netbox_pdu/tables.py
+-rw-r--r--   0        0        0     2151 2022-08-17 15:42:10.719943 meraki-netbox-plugin-pdu-0.0.9/axians_netbox_pdu/template_content.py
+-rw-r--r--   0        0        0      837 2022-08-17 15:42:10.719943 meraki-netbox-plugin-pdu-0.0.9/axians_netbox_pdu/templates/axians_netbox_pdu/device_power_usage.html
+-rw-r--r--   0        0        0     1011 2022-08-17 15:42:10.719943 meraki-netbox-plugin-pdu-0.0.9/axians_netbox_pdu/templates/axians_netbox_pdu/device_type_pduconfig.html
+-rw-r--r--   0        0        0      127 2022-08-17 15:42:10.719943 meraki-netbox-plugin-pdu-0.0.9/axians_netbox_pdu/templates/axians_netbox_pdu/pduconfig.html
+-rw-r--r--   0        0        0       65 2022-08-17 15:42:10.719943 meraki-netbox-plugin-pdu-0.0.9/axians_netbox_pdu/templates/axians_netbox_pdu/pduconfig_edit.html
+-rw-r--r--   0        0        0     3554 2022-08-17 15:42:10.719943 meraki-netbox-plugin-pdu-0.0.9/axians_netbox_pdu/templates/axians_netbox_pdu/pduconfig_list.html
+-rw-r--r--   0        0        0     2369 2022-08-17 15:42:10.719943 meraki-netbox-plugin-pdu-0.0.9/axians_netbox_pdu/templates/axians_netbox_pdu/rack_power_usage.html
+-rw-r--r--   0        0        0       43 2022-08-17 15:42:10.719943 meraki-netbox-plugin-pdu-0.0.9/axians_netbox_pdu/tests/__init__.py
+-rw-r--r--   0        0        0     7680 2022-08-17 15:42:10.719943 meraki-netbox-plugin-pdu-0.0.9/axians_netbox_pdu/tests/test_pduconfig_api.py
+-rw-r--r--   0        0        0    13374 2022-08-17 15:42:10.719943 meraki-netbox-plugin-pdu-0.0.9/axians_netbox_pdu/tests/test_pduconfig_views.py
+-rw-r--r--   0        0        0     8066 2022-08-17 15:42:10.719943 meraki-netbox-plugin-pdu-0.0.9/axians_netbox_pdu/tests/test_pdustatus_api.py
+-rw-r--r--   0        0        0      973 2022-08-17 15:42:10.719943 meraki-netbox-plugin-pdu-0.0.9/axians_netbox_pdu/urls.py
+-rw-r--r--   0        0        0     1648 2022-08-17 15:42:10.719943 meraki-netbox-plugin-pdu-0.0.9/axians_netbox_pdu/utilities.py
+-rw-r--r--   0        0        0     2167 2022-08-17 15:42:10.719943 meraki-netbox-plugin-pdu-0.0.9/axians_netbox_pdu/views.py
+-rw-r--r--   0        0        0     1317 2022-08-17 15:42:10.719943 meraki-netbox-plugin-pdu-0.0.9/axians_netbox_pdu/worker.py
+-rw-r--r--   0        0        0     1380 2022-08-17 15:42:10.723943 meraki-netbox-plugin-pdu-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     7247 2022-08-17 15:42:55.664669 meraki-netbox-plugin-pdu-0.0.9/setup.py
+-rw-r--r--   0        0        0     7074 2022-08-17 15:42:55.665217 meraki-netbox-plugin-pdu-0.0.9/PKG-INFO
```

### Comparing `meraki-netbox-plugin-pdu-0.0.8/README.md` & `meraki-netbox-plugin-pdu-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `meraki-netbox-plugin-pdu-0.0.8/axians_netbox_pdu/__init__.py` & `meraki-netbox-plugin-pdu-0.0.9/axians_netbox_pdu/__init__.py`

 * *Files identical despite different names*

### Comparing `meraki-netbox-plugin-pdu-0.0.8/axians_netbox_pdu/api/serializers.py` & `meraki-netbox-plugin-pdu-0.0.9/axians_netbox_pdu/api/serializers.py`

 * *Files identical despite different names*

### Comparing `meraki-netbox-plugin-pdu-0.0.8/axians_netbox_pdu/api/views.py` & `meraki-netbox-plugin-pdu-0.0.9/axians_netbox_pdu/api/views.py`

 * *Files identical despite different names*

### Comparing `meraki-netbox-plugin-pdu-0.0.8/axians_netbox_pdu/filters.py` & `meraki-netbox-plugin-pdu-0.0.9/axians_netbox_pdu/filters.py`

 * *Files identical despite different names*

### Comparing `meraki-netbox-plugin-pdu-0.0.8/axians_netbox_pdu/forms.py` & `meraki-netbox-plugin-pdu-0.0.9/axians_netbox_pdu/forms.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from django import forms
 
 from dcim.models import DeviceType, Manufacturer
-from extras.forms import CustomFieldModelCSVForm
 from utilities.forms import BootstrapMixin
 
+from netbox.forms import NetBoxModelForm
+
 from .choices import PDUUnitChoices
 from .models import PDUConfig
 
 BLANK_CHOICE = (("", "---------"),)
 
 
-class PDUConfigForm(BootstrapMixin, forms.ModelForm):
+class PDUConfigForm(NetBoxModelForm):
     """Form for creating a new PDUConfig"""
 
     device_type = forms.ModelChoiceField(
         queryset=DeviceType.objects.filter(poweroutlettemplates__isnull=False).distinct(),
         required=True,
         to_field_name="slug",
         label="Device Type",
@@ -30,15 +31,15 @@
 
     class Meta:
         model = PDUConfig
         fields = ["device_type", "power_usage_oid", "power_usage_unit"]
         obj_type = "test"
 
 
-class PDUConfigFilterForm(BootstrapMixin, forms.ModelForm):
+class PDUConfigFilterForm(NetBoxModelForm):
     """Form for siltering PDUConfig instances."""
 
     device_type = forms.ModelChoiceField(
         queryset=DeviceType.objects.filter(poweroutlettemplates__isnull=False).distinct(),
         required=False,
         to_field_name="slug",
     )
@@ -50,32 +51,7 @@
     )
 
     q = forms.CharField(required=False, label="Search")
 
     class Meta:
         model = PDUConfig
         fields = ["q", "device_type", "manufacturer"]
-
-
-class PDUConfigCSVForm(CustomFieldModelCSVForm):
-    """Form for entering CSV to bulk-import PDUConfig entries."""
-
-    device_type = forms.ModelChoiceField(
-        queryset=DeviceType.objects.filter(poweroutlettemplates__isnull=False).distinct(),
-        required=True,
-        to_field_name="slug",
-        help_text="slug of device type",
-        error_messages={"invalid_choice": "Device Type not found",},
-    )
-
-    power_usage_oid = forms.CharField(required=True, help_text="OID string to collect power usage")
-
-    power_usage_unit = forms.CharField(required=True, help_text="The unit of power that will be collected")
-
-    class Meta:
-        model = PDUConfig
-        fields = PDUConfig.csv_headers
-
-    def save(self, commit=True, **kwargs):
-        """Save the model"""
-        model = super().save(commit=commit, **kwargs)
-        return model
```

### Comparing `meraki-netbox-plugin-pdu-0.0.8/axians_netbox_pdu/management/commands/pduscheduler.py` & `meraki-netbox-plugin-pdu-0.0.9/axians_netbox_pdu/management/commands/pduscheduler.py`

 * *Files identical despite different names*

### Comparing `meraki-netbox-plugin-pdu-0.0.8/axians_netbox_pdu/migrations/0001_initial.py` & `meraki-netbox-plugin-pdu-0.0.9/axians_netbox_pdu/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `meraki-netbox-plugin-pdu-0.0.8/axians_netbox_pdu/migrations/0002_pdustatus.py` & `meraki-netbox-plugin-pdu-0.0.9/axians_netbox_pdu/migrations/0002_pdustatus.py`

 * *Files identical despite different names*

### Comparing `meraki-netbox-plugin-pdu-0.0.8/axians_netbox_pdu/models.py` & `meraki-netbox-plugin-pdu-0.0.9/axians_netbox_pdu/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from django.db import models
 from django.urls import reverse
 from .choices import PDUUnitChoices
+from netbox.models import NetBoxModel
 
 
-class PDUConfig(models.Model):
+class PDUConfig(NetBoxModel):
     """PDU Configuration is contained within this model."""
 
     device_type = models.OneToOneField(to="dcim.DeviceType", on_delete=models.CASCADE, blank=True, null=True)
 
     power_usage_oid = models.CharField(
         max_length=255, help_text="OID string to collect power usage", blank=True, null=True
     )
@@ -22,15 +23,15 @@
         """String representation of an PDUConfig."""
         return f"{self.device_type}"
 
     def get_absolute_url(self):
         return reverse('dcim:devicetype', args=[self.device_type.id])
 
 
-class PDUStatus(models.Model):
+class PDUStatus(NetBoxModel):
     """PDU Status is contained within this model."""
 
     device = models.OneToOneField(to="dcim.Device", on_delete=models.CASCADE, blank=True, null=True)
 
     power_usage = models.PositiveSmallIntegerField(blank=True, null=True, help_text="Current PDU Power Usage")
 
     updated_at = models.DateTimeField(auto_now=True)
```

### Comparing `meraki-netbox-plugin-pdu-0.0.8/axians_netbox_pdu/tables.py` & `meraki-netbox-plugin-pdu-0.0.9/axians_netbox_pdu/tables.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 import django_tables2 as tables
 
-from utilities.tables import BaseTable, ToggleColumn
+from netbox.tables import NetBoxTable, ToggleColumn
 
 from .models import PDUConfig
 
 
-class PDUConfigTable(BaseTable):
+class PDUConfigTable(NetBoxTable):
     """Table for displaying PDUConfig information"""
 
     pk = ToggleColumn()
     device_type = tables.LinkColumn()
 
-    class Meta(BaseTable.Meta):
+    class Meta(NetBoxTable.Meta):
         model = PDUConfig
         fields = (
             "pk",
             "device_type",
             "power_usage_oid",
             "power_usage_unit",
         )
 
 
-class PDUConfigBulkTable(BaseTable):
+class PDUConfigBulkTable(NetBoxTable):
 
     device_type = tables.LinkColumn()
 
-    class Meta(BaseTable.Meta):
+    class Meta(NetBoxTable.Meta):
         model = PDUConfig
         fields = (
             "pk",
             "device_type",
             "power_usage_oid",
             "power_usage_unit",
         )
```

### Comparing `meraki-netbox-plugin-pdu-0.0.8/axians_netbox_pdu/templates/axians_netbox_pdu/device_power_usage.html` & `meraki-netbox-plugin-pdu-0.0.9/axians_netbox_pdu/templates/axians_netbox_pdu/device_power_usage.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 {% load humanize %}
 
-<div class="panel panel-default">
-    <div class="panel-heading">
+<div class="card card-default">
+    <div class="card-header">
         <strong>Power Information</strong>
     </div>
-    <table class="table table-hover panel-body attr-table">
-        <tbody>
-            <tr>
-                <td>
-                    <span title="">Power Usage</span>
-                </td>
-                <td>
-                    <span>{{ pdustatus.get_power_usage }}</span>
-                </td>
-            </tr>
-            <tr>
-                <td>
-                    <span>Last Updated</span>
-                </td>
-                <td>
-                    <span>{{ pdustatus.updated_at|naturaltime }}</span>
-                </td>
-            </tr>
-        </tbody>
-    </table>
-</div>
+    <div class="card-body">
+        <table class="table table-hover attr-table">
+            <tbody>
+                <tr>
+                    <td>
+                        <span title="">Power Usage</span>
+                    </td>
+                    <td>
+                        <span>{{ pdustatus.get_power_usage }}</span>
+                    </td>
+                </tr>
+                <tr>
+                    <td>
+                        <span>Last Updated</span>
+                    </td>
+                    <td>
+                        <span>{{ pdustatus.updated_at|naturaltime }}</span>
+                    </td>
+                </tr>
+            </tbody>
+        </table>
+    </div>
+</div>
```

### Comparing `meraki-netbox-plugin-pdu-0.0.8/axians_netbox_pdu/templates/axians_netbox_pdu/device_type_pduconfig_3_x.html` & `meraki-netbox-plugin-pdu-0.0.9/axians_netbox_pdu/templates/axians_netbox_pdu/device_type_pduconfig.html`

 * *Files identical despite different names*

### Comparing `meraki-netbox-plugin-pdu-0.0.8/axians_netbox_pdu/templates/axians_netbox_pdu/pduconfig_list.html` & `meraki-netbox-plugin-pdu-0.0.9/axians_netbox_pdu/templates/axians_netbox_pdu/pduconfig_list.html`

 * *Files 7% similar despite different names*

```diff
@@ -11,210 +11,213 @@
 000000a0: 7620 636c 6173 733d 2263 6f6e 7472 6f6c  v class="control
 000000b0: 7322 3e0a 2020 2020 3c64 6976 2063 6c61  s">.    <div cla
 000000c0: 7373 3d22 636f 6e74 726f 6c2d 6772 6f75  ss="control-grou
 000000d0: 7022 3e0a 2020 2020 2020 7b25 2062 6c6f  p">.      {% blo
 000000e0: 636b 2065 7874 7261 5f63 6f6e 7472 6f6c  ck extra_control
 000000f0: 7320 257d 7b25 2065 6e64 626c 6f63 6b20  s %}{% endblock 
 00000100: 257d 0a20 2020 2020 207b 2520 6966 2070  %}.      {% if p
-00000110: 6572 6d69 7373 696f 6e73 2e61 6464 2025  ermissions.add %
-00000120: 7d0a 2020 2020 2020 2020 2020 7b25 2061  }.          {% a
-00000130: 6464 5f62 7574 746f 6e20 2770 6c75 6769  dd_button 'plugi
-00000140: 6e73 3a61 7869 616e 735f 6e65 7462 6f78  ns:axians_netbox
-00000150: 5f70 6475 3a70 6475 636f 6e66 6967 5f61  _pdu:pduconfig_a
-00000160: 6464 2720 257d 0a20 2020 2020 207b 2520  dd' %}.      {% 
-00000170: 656e 6469 6620 257d 0a20 2020 2020 207b  endif %}.      {
-00000180: 2520 6966 2070 6572 6d69 7373 696f 6e73  % if permissions
-00000190: 2e61 6464 2025 7d0a 2020 2020 2020 2020  .add %}.        
-000001a0: 2020 7b25 2069 6d70 6f72 745f 6275 7474    {% import_butt
-000001b0: 6f6e 2027 706c 7567 696e 733a 6178 6961  on 'plugins:axia
-000001c0: 6e73 5f6e 6574 626f 785f 7064 753a 7064  ns_netbox_pdu:pd
-000001d0: 7563 6f6e 6669 675f 696d 706f 7274 2720  uconfig_import' 
-000001e0: 257d 0a20 2020 2020 207b 2520 656e 6469  %}.      {% endi
-000001f0: 6620 257d 0a20 2020 203c 2f64 6976 3e0a  f %}.    </div>.
-00000200: 2020 3c2f 6469 763e 0a7b 2520 656e 6462    </div>.{% endb
-00000210: 6c6f 636b 2063 6f6e 7472 6f6c 7320 257d  lock controls %}
-00000220: 0a0a 7b25 2062 6c6f 636b 2074 6162 7320  ..{% block tabs 
-00000230: 257d 0a20 203c 756c 2063 6c61 7373 3d22  %}.  <ul class="
-00000240: 6e61 7620 6e61 762d 7461 6273 2070 782d  nav nav-tabs px-
-00000250: 3322 3e0a 2020 2020 7b25 2062 6c6f 636b  3">.    {% block
-00000260: 2074 6162 5f69 7465 6d73 2025 7d0a 2020   tab_items %}.  
-00000270: 2020 2020 3c6c 6920 636c 6173 733d 226e      <li class="n
-00000280: 6176 2d69 7465 6d22 2072 6f6c 653d 2270  av-item" role="p
-00000290: 7265 7365 6e74 6174 696f 6e22 3e0a 2020  resentation">.  
-000002a0: 2020 2020 2020 3c62 7574 746f 6e20 636c        <button cl
-000002b0: 6173 733d 226e 6176 2d6c 696e 6b20 6163  ass="nav-link ac
-000002c0: 7469 7665 2220 6964 3d22 6f62 6a65 6374  tive" id="object
-000002d0: 2d6c 6973 742d 7461 6222 2064 6174 612d  -list-tab" data-
-000002e0: 6273 2d74 6f67 676c 653d 2274 6162 2220  bs-toggle="tab" 
-000002f0: 6461 7461 2d62 732d 7461 7267 6574 3d22  data-bs-target="
-00000300: 236f 626a 6563 742d 6c69 7374 2220 7479  #object-list" ty
-00000310: 7065 3d22 6275 7474 6f6e 2220 726f 6c65  pe="button" role
-00000320: 3d22 7461 6222 2061 7269 612d 636f 6e74  ="tab" aria-cont
-00000330: 726f 6c73 3d22 6564 6974 2d66 6f72 6d22  rols="edit-form"
-00000340: 2061 7269 612d 7365 6c65 6374 6564 3d22   aria-selected="
-00000350: 7472 7565 223e 0a20 2020 2020 2020 2020  true">.         
-00000360: 207b 2520 626c 6f63 6b20 7469 746c 6520   {% block title 
-00000370: 257d 5044 5520 4465 7669 6365 2054 7970  %}PDU Device Typ
-00000380: 6520 436f 6e66 6967 7572 6174 696f 6e7b  e Configuration{
-00000390: 2520 656e 6462 6c6f 636b 2025 7d0a 2020  % endblock %}.  
-000003a0: 2020 2020 2020 2020 7b25 2062 6164 6765          {% badge
-000003b0: 2074 6162 6c65 2e70 6167 652e 7061 6769   table.page.pagi
-000003c0: 6e61 746f 722e 636f 756e 7420 257d 0a20  nator.count %}. 
-000003d0: 2020 2020 2020 203c 2f62 7574 746f 6e3e         </button>
-000003e0: 0a20 2020 2020 203c 2f6c 693e 0a20 2020  .      </li>.   
-000003f0: 2020 207b 2520 6966 2066 696c 7465 725f     {% if filter_
-00000400: 666f 726d 2025 7d0a 2020 2020 2020 2020  form %}.        
-00000410: 3c6c 6920 636c 6173 733d 226e 6176 2d69  <li class="nav-i
-00000420: 7465 6d22 2072 6f6c 653d 2270 7265 7365  tem" role="prese
-00000430: 6e74 6174 696f 6e22 3e0a 2020 2020 2020  ntation">.      
-00000440: 2020 2020 3c62 7574 746f 6e20 636c 6173      <button clas
-00000450: 733d 226e 6176 2d6c 696e 6b22 2069 643d  s="nav-link" id=
-00000460: 2266 696c 7465 7273 2d66 6f72 6d2d 7461  "filters-form-ta
-00000470: 6222 2064 6174 612d 6273 2d74 6f67 676c  b" data-bs-toggl
-00000480: 653d 2274 6162 2220 6461 7461 2d62 732d  e="tab" data-bs-
-00000490: 7461 7267 6574 3d22 2366 696c 7465 7273  target="#filters
-000004a0: 2d66 6f72 6d22 2074 7970 653d 2262 7574  -form" type="but
-000004b0: 746f 6e22 2072 6f6c 653d 2274 6162 2220  ton" role="tab" 
-000004c0: 6172 6961 2d63 6f6e 7472 6f6c 733d 226f  aria-controls="o
-000004d0: 626a 6563 742d 6c69 7374 2220 6172 6961  bject-list" aria
-000004e0: 2d73 656c 6563 7465 643d 2266 616c 7365  -selected="false
-000004f0: 223e 0a20 2020 2020 2020 2020 2020 2046  ">.            F
-00000500: 696c 7465 7273 0a20 2020 2020 2020 2020  ilters.         
-00000510: 2020 207b 2520 6966 2066 696c 7465 725f     {% if filter_
-00000520: 666f 726d 2025 7d7b 2520 6261 6467 6520  form %}{% badge 
-00000530: 6669 6c74 6572 5f66 6f72 6d2e 6368 616e  filter_form.chan
-00000540: 6765 645f 6461 7461 7c6c 656e 6774 6820  ged_data|length 
-00000550: 6267 5f63 6c61 7373 3d22 7072 696d 6172  bg_class="primar
-00000560: 7922 2025 7d7b 2520 656e 6469 6620 257d  y" %}{% endif %}
-00000570: 0a20 2020 2020 2020 2020 203c 2f62 7574  .          </but
-00000580: 746f 6e3e 0a20 2020 2020 2020 203c 2f6c  ton>.        </l
-00000590: 693e 0a20 2020 2020 207b 2520 656e 6469  i>.      {% endi
-000005a0: 6620 257d 0a20 2020 207b 2520 656e 6462  f %}.    {% endb
-000005b0: 6c6f 636b 2074 6162 5f69 7465 6d73 2025  lock tab_items %
-000005c0: 7d0a 2020 3c2f 756c 3e0a 7b25 2065 6e64  }.  </ul>.{% end
-000005d0: 626c 6f63 6b20 7461 6273 2025 7d0a 0a7b  block tabs %}..{
-000005e0: 2520 626c 6f63 6b20 636f 6e74 656e 742d  % block content-
-000005f0: 7772 6170 7065 7220 257d 0a20 203c 6469  wrapper %}.  <di
-00000600: 7620 636c 6173 733d 2274 6162 2d63 6f6e  v class="tab-con
-00000610: 7465 6e74 223e 0a0a 2020 2020 3c64 6976  tent">..    <div
-00000620: 2063 6c61 7373 3d22 7461 622d 7061 6e65   class="tab-pane
-00000630: 2073 686f 7720 6163 7469 7665 2220 6964   show active" id
-00000640: 3d22 6f62 6a65 6374 2d6c 6973 7422 2072  ="object-list" r
-00000650: 6f6c 653d 2274 6162 7061 6e65 6c22 2061  ole="tabpanel" a
-00000660: 7269 612d 6c61 6265 6c6c 6564 6279 3d22  ria-labelledby="
-00000670: 6f62 6a65 6374 2d6c 6973 742d 7461 6222  object-list-tab"
-00000680: 3e0a 0a20 2020 2020 207b 2520 6966 2066  >..      {% if f
-00000690: 696c 7465 725f 666f 726d 2025 7d0a 2020  ilter_form %}.  
-000006a0: 2020 2020 2020 7b25 2061 7070 6c69 6564        {% applied
-000006b0: 5f66 696c 7465 7273 2066 696c 7465 725f  _filters filter_
-000006c0: 666f 726d 2072 6571 7565 7374 2e47 4554  form request.GET
-000006d0: 2025 7d0a 2020 2020 2020 7b25 2065 6e64   %}.      {% end
-000006e0: 6966 2025 7d0a 0a20 2020 2020 207b 2520  if %}..      {% 
-000006f0: 696e 636c 7564 6520 2769 6e63 2f74 6162  include 'inc/tab
-00000700: 6c65 5f63 6f6e 7472 6f6c 735f 6874 6d78  le_controls_htmx
-00000710: 2e68 746d 6c27 2077 6974 6820 7461 626c  .html' with tabl
-00000720: 655f 6d6f 6461 6c3d 2252 6563 6f72 6454  e_modal="RecordT
-00000730: 6162 6c65 5f63 6f6e 6669 6722 2025 7d0a  able_config" %}.
-00000740: 0a20 2020 2020 203c 666f 726d 206d 6574  .      <form met
-00000750: 686f 643d 2270 6f73 7422 2063 6c61 7373  hod="post" class
-00000760: 3d22 666f 726d 2066 6f72 6d2d 686f 7269  ="form form-hori
-00000770: 7a6f 6e74 616c 223e 0a20 2020 2020 2020  zontal">.       
-00000780: 207b 2520 6373 7266 5f74 6f6b 656e 2025   {% csrf_token %
-00000790: 7d0a 2020 2020 2020 2020 3c69 6e70 7574  }.        <input
-000007a0: 2074 7970 653d 2268 6964 6465 6e22 206e   type="hidden" n
-000007b0: 616d 653d 2272 6574 7572 6e5f 7572 6c22  ame="return_url"
-000007c0: 2076 616c 7565 3d22 7b25 2069 6620 7265   value="{% if re
-000007d0: 7475 726e 5f75 726c 2025 7d7b 7b20 7265  turn_url %}{{ re
-000007e0: 7475 726e 5f75 726c 207d 7d7b 2520 656c  turn_url }}{% el
-000007f0: 7365 2025 7d7b 7b20 7265 7175 6573 742e  se %}{{ request.
-00000800: 7061 7468 207d 7d7b 2520 6966 2072 6571  path }}{% if req
-00000810: 7565 7374 2e47 4554 2025 7d3f 7b7b 2072  uest.GET %}?{{ r
-00000820: 6571 7565 7374 2e47 4554 2e75 726c 656e  equest.GET.urlen
-00000830: 636f 6465 207d 7d7b 2520 656e 6469 6620  code }}{% endif 
-00000840: 257d 7b25 2065 6e64 6966 2025 7d22 202f  %}{% endif %}" /
-00000850: 3e0a 0a20 2020 2020 2020 203c 6469 7620  >..        <div 
-00000860: 636c 6173 733d 2263 6172 6422 3e0a 2020  class="card">.  
-00000870: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-00000880: 7373 3d22 6361 7264 2d62 6f64 7922 3e0a  ss="card-body">.
-00000890: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-000008a0: 2063 6c61 7373 3d22 7461 626c 652d 7265   class="table-re
-000008b0: 7370 6f6e 7369 7665 223e 0a20 2020 2020  sponsive">.     
-000008c0: 2020 2020 2020 2020 207b 2520 7265 6e64           {% rend
-000008d0: 6572 5f74 6162 6c65 2074 6162 6c65 2027  er_table table '
-000008e0: 696e 632f 7461 626c 652e 6874 6d6c 2720  inc/table.html' 
-000008f0: 257d 0a20 2020 2020 2020 2020 2020 203c  %}.            <
-00000900: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
-00000910: 3c2f 6469 763e 0a20 2020 2020 2020 203c  </div>.        <
-00000920: 2f64 6976 3e0a 0a20 2020 2020 2020 207b  /div>..        {
-00000930: 2520 6966 2070 6572 6d69 7373 696f 6e73  % if permissions
-00000940: 2e64 656c 6574 6520 257d 0a20 2020 2020  .delete %}.     
-00000950: 2020 2020 207b 2520 7769 7468 2062 756c       {% with bul
-00000960: 6b5f 6465 6c65 7465 5f75 726c 3d27 706c  k_delete_url='pl
-00000970: 7567 696e 733a 6178 6961 6e73 5f6e 6574  ugins:axians_net
-00000980: 626f 785f 7064 753a 7064 7563 6f6e 6669  box_pdu:pduconfi
-00000990: 675f 6275 6c6b 5f64 656c 6574 6527 2025  g_bulk_delete' %
-000009a0: 7d0a 2020 2020 2020 2020 2020 2020 3c64  }.            <d
-000009b0: 6976 2063 6c61 7373 3d22 6e6f 7072 696e  iv class="noprin
-000009c0: 7420 6275 6c6b 2d62 7574 746f 6e73 223e  t bulk-buttons">
-000009d0: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
-000009e0: 6469 7620 636c 6173 733d 2262 756c 6b2d  div class="bulk-
-000009f0: 6275 7474 6f6e 2d67 726f 7570 223e 0a20  button-group">. 
-00000a00: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00000a10: 2520 626c 6f63 6b20 6275 6c6b 5f62 7574  % block bulk_but
-00000a20: 746f 6e73 2025 7d7b 2520 656e 6462 6c6f  tons %}{% endblo
-00000a30: 636b 2025 7d0a 2020 2020 2020 2020 2020  ck %}.          
-00000a40: 2020 2020 2020 7b25 2069 6620 6275 6c6b        {% if bulk
-00000a50: 5f64 656c 6574 655f 7572 6c20 616e 6420  _delete_url and 
-00000a60: 7065 726d 6973 7369 6f6e 732e 6465 6c65  permissions.dele
-00000a70: 7465 2025 7d0a 2020 2020 2020 2020 2020  te %}.          
-00000a80: 2020 2020 2020 2020 3c62 7574 746f 6e20          <button 
-00000a90: 7479 7065 3d22 7375 626d 6974 2220 6e61  type="submit" na
-00000aa0: 6d65 3d22 5f64 656c 6574 6522 2066 6f72  me="_delete" for
-00000ab0: 6d61 6374 696f 6e3d 227b 2520 7572 6c20  maction="{% url 
-00000ac0: 6275 6c6b 5f64 656c 6574 655f 7572 6c20  bulk_delete_url 
-00000ad0: 257d 7b25 2069 6620 7265 7175 6573 742e  %}{% if request.
-00000ae0: 4745 5420 257d 3f7b 7b20 7265 7175 6573  GET %}?{{ reques
-00000af0: 742e 4745 542e 7572 6c65 6e63 6f64 6520  t.GET.urlencode 
-00000b00: 7d7d 7b25 2065 6e64 6966 2025 7d22 2063  }}{% endif %}" c
-00000b10: 6c61 7373 3d22 6274 6e20 6274 6e2d 6461  lass="btn btn-da
-00000b20: 6e67 6572 2062 746e 2d73 6d22 3e0a 2020  nger btn-sm">.  
-00000b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b40: 2020 3c69 2063 6c61 7373 3d22 6d64 6920    <i class="mdi 
-00000b50: 6d64 692d 7472 6173 682d 6361 6e2d 6f75  mdi-trash-can-ou
-00000b60: 746c 696e 6522 2061 7269 612d 6869 6464  tline" aria-hidd
-00000b70: 656e 3d22 7472 7565 223e 3c2f 693e 2044  en="true"></i> D
-00000b80: 656c 6574 6520 5365 6c65 6374 6564 0a20  elete Selected. 
-00000b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ba0: 203c 2f62 7574 746f 6e3e 0a20 2020 2020   </button>.     
-00000bb0: 2020 2020 2020 2020 2020 207b 2520 656e             {% en
-00000bc0: 6469 6620 257d 0a20 2020 2020 2020 2020  dif %}.         
-00000bd0: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
-00000be0: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
-00000bf0: 2020 2020 2020 2020 207b 2520 656e 6477           {% endw
-00000c00: 6974 6820 257d 0a20 2020 2020 2020 207b  ith %}.        {
-00000c10: 2520 656e 6469 6620 257d 0a0a 2020 2020  % endif %}..    
-00000c20: 2020 3c2f 666f 726d 3e0a 0a20 2020 2020    </form>..     
-00000c30: 207b 2520 696e 636c 7564 6520 2769 6e63   {% include 'inc
-00000c40: 2f70 6167 696e 6174 6f72 2e68 746d 6c27  /paginator.html'
-00000c50: 2077 6974 6820 7061 6769 6e61 746f 723d   with paginator=
-00000c60: 7461 626c 652e 7061 6769 6e61 746f 7220  table.paginator 
-00000c70: 7061 6765 3d74 6162 6c65 2e70 6167 6520  page=table.page 
-00000c80: 257d 0a20 2020 203c 2f64 6976 3e0a 0a20  %}.    </div>.. 
-00000c90: 2020 207b 2520 6966 2066 696c 7465 725f     {% if filter_
-00000ca0: 666f 726d 2025 7d0a 2020 2020 2020 3c64  form %}.      <d
-00000cb0: 6976 2063 6c61 7373 3d22 7461 622d 7061  iv class="tab-pa
-00000cc0: 6e65 2073 686f 7722 2069 643d 2266 696c  ne show" id="fil
-00000cd0: 7465 7273 2d66 6f72 6d22 2072 6f6c 653d  ters-form" role=
-00000ce0: 2274 6162 7061 6e65 6c22 2061 7269 612d  "tabpanel" aria-
-00000cf0: 6c61 6265 6c6c 6564 6279 3d22 6669 6c74  labelledby="filt
-00000d00: 6572 732d 666f 726d 2d74 6162 223e 0a20  ers-form-tab">. 
-00000d10: 2020 2020 2020 207b 2520 696e 636c 7564         {% includ
-00000d20: 6520 2769 6e63 2f66 696c 7465 725f 6c69  e 'inc/filter_li
-00000d30: 7374 2e68 746d 6c27 2025 7d0a 2020 2020  st.html' %}.    
-00000d40: 2020 3c2f 6469 763e 0a20 2020 207b 2520    </div>.    {% 
-00000d50: 656e 6469 6620 257d 0a20 203c 2f64 6976  endif %}.  </div
-00000d60: 3e0a 0a20 207b 2520 7461 626c 655f 636f  >..  {% table_co
-00000d70: 6e66 6967 5f66 6f72 6d20 7461 626c 6520  nfig_form table 
-00000d80: 7461 626c 655f 6e61 6d65 3d22 5265 636f  table_name="Reco
-00000d90: 7264 5461 626c 6522 2025 7d0a 7b25 2065  rdTable" %}.{% e
-00000da0: 6e64 626c 6f63 6b20 636f 6e74 656e 742d  ndblock content-
-00000db0: 7772 6170 7065 7220 257d 0a              wrapper %}.
+00000110: 6572 6d73 2e61 7869 616e 735f 6e65 7462  erms.axians_netb
+00000120: 6f78 5f70 6475 2e61 6464 5f70 6475 636f  ox_pdu.add_pduco
+00000130: 6e66 6967 2025 7d0a 2020 2020 2020 2020  nfig %}.        
+00000140: 2020 3c61 2068 7265 663d 227b 2520 7572    <a href="{% ur
+00000150: 6c20 2770 6c75 6769 6e73 3a61 7869 616e  l 'plugins:axian
+00000160: 735f 6e65 7462 6f78 5f70 6475 3a70 6475  s_netbox_pdu:pdu
+00000170: 636f 6e66 6967 5f61 6464 2720 257d 3f7a  config_add' %}?z
+00000180: 6f6e 653d 7b7b 206f 626a 6563 742e 6964  one={{ object.id
+00000190: 207d 7d22 2063 6c61 7373 3d22 6274 6e20   }}" class="btn 
+000001a0: 6274 6e2d 736d 2062 746e 2d67 7265 656e  btn-sm btn-green
+000001b0: 2220 726f 6c65 3d22 6275 7474 6f6e 223e  " role="button">
+000001c0: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
+000001d0: 6920 636c 6173 733d 226d 6469 206d 6469  i class="mdi mdi
+000001e0: 2d70 6c75 732d 7468 6963 6b22 3e3c 2f69  -plus-thick"></i
+000001f0: 3e20 4164 640a 2020 2020 2020 2020 2020  > Add.          
+00000200: 3c2f 613e 0a20 2020 2020 207b 2520 656e  </a>.      {% en
+00000210: 6469 6620 257d 0a20 2020 203c 2f64 6976  dif %}.    </div
+00000220: 3e0a 2020 3c2f 6469 763e 0a7b 2520 656e  >.  </div>.{% en
+00000230: 6462 6c6f 636b 2063 6f6e 7472 6f6c 7320  dblock controls 
+00000240: 257d 0a0a 7b25 2062 6c6f 636b 2074 6162  %}..{% block tab
+00000250: 7320 257d 0a20 203c 756c 2063 6c61 7373  s %}.  <ul class
+00000260: 3d22 6e61 7620 6e61 762d 7461 6273 2070  ="nav nav-tabs p
+00000270: 782d 3322 3e0a 2020 2020 7b25 2062 6c6f  x-3">.    {% blo
+00000280: 636b 2074 6162 5f69 7465 6d73 2025 7d0a  ck tab_items %}.
+00000290: 2020 2020 2020 3c6c 6920 636c 6173 733d        <li class=
+000002a0: 226e 6176 2d69 7465 6d22 2072 6f6c 653d  "nav-item" role=
+000002b0: 2270 7265 7365 6e74 6174 696f 6e22 3e0a  "presentation">.
+000002c0: 2020 2020 2020 2020 3c62 7574 746f 6e20          <button 
+000002d0: 636c 6173 733d 226e 6176 2d6c 696e 6b20  class="nav-link 
+000002e0: 6163 7469 7665 2220 6964 3d22 6f62 6a65  active" id="obje
+000002f0: 6374 2d6c 6973 742d 7461 6222 2064 6174  ct-list-tab" dat
+00000300: 612d 6273 2d74 6f67 676c 653d 2274 6162  a-bs-toggle="tab
+00000310: 2220 6461 7461 2d62 732d 7461 7267 6574  " data-bs-target
+00000320: 3d22 236f 626a 6563 742d 6c69 7374 2220  ="#object-list" 
+00000330: 7479 7065 3d22 6275 7474 6f6e 2220 726f  type="button" ro
+00000340: 6c65 3d22 7461 6222 2061 7269 612d 636f  le="tab" aria-co
+00000350: 6e74 726f 6c73 3d22 6564 6974 2d66 6f72  ntrols="edit-for
+00000360: 6d22 2061 7269 612d 7365 6c65 6374 6564  m" aria-selected
+00000370: 3d22 7472 7565 223e 0a20 2020 2020 2020  ="true">.       
+00000380: 2020 207b 2520 626c 6f63 6b20 7469 746c     {% block titl
+00000390: 6520 257d 5044 5520 4465 7669 6365 2054  e %}PDU Device T
+000003a0: 7970 6520 436f 6e66 6967 7572 6174 696f  ype Configuratio
+000003b0: 6e7b 2520 656e 6462 6c6f 636b 2025 7d0a  n{% endblock %}.
+000003c0: 2020 2020 2020 2020 2020 7b25 2062 6164            {% bad
+000003d0: 6765 2074 6162 6c65 2e70 6167 652e 7061  ge table.page.pa
+000003e0: 6769 6e61 746f 722e 636f 756e 7420 257d  ginator.count %}
+000003f0: 0a20 2020 2020 2020 203c 2f62 7574 746f  .        </butto
+00000400: 6e3e 0a20 2020 2020 203c 2f6c 693e 0a20  n>.      </li>. 
+00000410: 2020 2020 207b 2520 6966 2066 696c 7465       {% if filte
+00000420: 725f 666f 726d 2025 7d0a 2020 2020 2020  r_form %}.      
+00000430: 2020 3c6c 6920 636c 6173 733d 226e 6176    <li class="nav
+00000440: 2d69 7465 6d22 2072 6f6c 653d 2270 7265  -item" role="pre
+00000450: 7365 6e74 6174 696f 6e22 3e0a 2020 2020  sentation">.    
+00000460: 2020 2020 2020 3c62 7574 746f 6e20 636c        <button cl
+00000470: 6173 733d 226e 6176 2d6c 696e 6b22 2069  ass="nav-link" i
+00000480: 643d 2266 696c 7465 7273 2d66 6f72 6d2d  d="filters-form-
+00000490: 7461 6222 2064 6174 612d 6273 2d74 6f67  tab" data-bs-tog
+000004a0: 676c 653d 2274 6162 2220 6461 7461 2d62  gle="tab" data-b
+000004b0: 732d 7461 7267 6574 3d22 2366 696c 7465  s-target="#filte
+000004c0: 7273 2d66 6f72 6d22 2074 7970 653d 2262  rs-form" type="b
+000004d0: 7574 746f 6e22 2072 6f6c 653d 2274 6162  utton" role="tab
+000004e0: 2220 6172 6961 2d63 6f6e 7472 6f6c 733d  " aria-controls=
+000004f0: 226f 626a 6563 742d 6c69 7374 2220 6172  "object-list" ar
+00000500: 6961 2d73 656c 6563 7465 643d 2266 616c  ia-selected="fal
+00000510: 7365 223e 0a20 2020 2020 2020 2020 2020  se">.           
+00000520: 2046 696c 7465 7273 0a20 2020 2020 2020   Filters.       
+00000530: 2020 2020 207b 2520 6966 2066 696c 7465       {% if filte
+00000540: 725f 666f 726d 2025 7d7b 2520 6261 6467  r_form %}{% badg
+00000550: 6520 6669 6c74 6572 5f66 6f72 6d2e 6368  e filter_form.ch
+00000560: 616e 6765 645f 6461 7461 7c6c 656e 6774  anged_data|lengt
+00000570: 6820 6267 5f63 6f6c 6f72 3d22 7072 696d  h bg_color="prim
+00000580: 6172 7922 2025 7d7b 2520 656e 6469 6620  ary" %}{% endif 
+00000590: 257d 0a20 2020 2020 2020 2020 203c 2f62  %}.          </b
+000005a0: 7574 746f 6e3e 0a20 2020 2020 2020 203c  utton>.        <
+000005b0: 2f6c 693e 0a20 2020 2020 207b 2520 656e  /li>.      {% en
+000005c0: 6469 6620 257d 0a20 2020 207b 2520 656e  dif %}.    {% en
+000005d0: 6462 6c6f 636b 2074 6162 5f69 7465 6d73  dblock tab_items
+000005e0: 2025 7d0a 2020 3c2f 756c 3e0a 7b25 2065   %}.  </ul>.{% e
+000005f0: 6e64 626c 6f63 6b20 7461 6273 2025 7d0a  ndblock tabs %}.
+00000600: 0a7b 2520 626c 6f63 6b20 636f 6e74 656e  .{% block conten
+00000610: 742d 7772 6170 7065 7220 257d 0a20 203c  t-wrapper %}.  <
+00000620: 6469 7620 636c 6173 733d 2274 6162 2d63  div class="tab-c
+00000630: 6f6e 7465 6e74 223e 0a0a 2020 2020 3c64  ontent">..    <d
+00000640: 6976 2063 6c61 7373 3d22 7461 622d 7061  iv class="tab-pa
+00000650: 6e65 2073 686f 7720 6163 7469 7665 2220  ne show active" 
+00000660: 6964 3d22 6f62 6a65 6374 2d6c 6973 7422  id="object-list"
+00000670: 2072 6f6c 653d 2274 6162 7061 6e65 6c22   role="tabpanel"
+00000680: 2061 7269 612d 6c61 6265 6c6c 6564 6279   aria-labelledby
+00000690: 3d22 6f62 6a65 6374 2d6c 6973 742d 7461  ="object-list-ta
+000006a0: 6222 3e0a 0a20 2020 2020 207b 2520 6966  b">..      {% if
+000006b0: 2066 696c 7465 725f 666f 726d 2025 7d0a   filter_form %}.
+000006c0: 2020 2020 2020 2020 7b25 2061 7070 6c69          {% appli
+000006d0: 6564 5f66 696c 7465 7273 2066 696c 7465  ed_filters filte
+000006e0: 725f 666f 726d 2072 6571 7565 7374 2e47  r_form request.G
+000006f0: 4554 2025 7d0a 2020 2020 2020 7b25 2065  ET %}.      {% e
+00000700: 6e64 6966 2025 7d0a 0a20 2020 2020 207b  ndif %}..      {
+00000710: 2520 696e 636c 7564 6520 2769 6e63 2f74  % include 'inc/t
+00000720: 6162 6c65 5f63 6f6e 7472 6f6c 735f 6874  able_controls_ht
+00000730: 6d78 2e68 746d 6c27 2077 6974 6820 7461  mx.html' with ta
+00000740: 626c 655f 6d6f 6461 6c3d 2252 6563 6f72  ble_modal="Recor
+00000750: 6454 6162 6c65 5f63 6f6e 6669 6722 2025  dTable_config" %
+00000760: 7d0a 0a20 2020 2020 203c 666f 726d 206d  }..      <form m
+00000770: 6574 686f 643d 2270 6f73 7422 2063 6c61  ethod="post" cla
+00000780: 7373 3d22 666f 726d 2066 6f72 6d2d 686f  ss="form form-ho
+00000790: 7269 7a6f 6e74 616c 223e 0a20 2020 2020  rizontal">.     
+000007a0: 2020 207b 2520 6373 7266 5f74 6f6b 656e     {% csrf_token
+000007b0: 2025 7d0a 2020 2020 2020 2020 3c69 6e70   %}.        <inp
+000007c0: 7574 2074 7970 653d 2268 6964 6465 6e22  ut type="hidden"
+000007d0: 206e 616d 653d 2272 6574 7572 6e5f 7572   name="return_ur
+000007e0: 6c22 2076 616c 7565 3d22 7b25 2069 6620  l" value="{% if 
+000007f0: 7265 7475 726e 5f75 726c 2025 7d7b 7b20  return_url %}{{ 
+00000800: 7265 7475 726e 5f75 726c 207d 7d7b 2520  return_url }}{% 
+00000810: 656c 7365 2025 7d7b 7b20 7265 7175 6573  else %}{{ reques
+00000820: 742e 7061 7468 207d 7d7b 2520 6966 2072  t.path }}{% if r
+00000830: 6571 7565 7374 2e47 4554 2025 7d3f 7b7b  equest.GET %}?{{
+00000840: 2072 6571 7565 7374 2e47 4554 2e75 726c   request.GET.url
+00000850: 656e 636f 6465 207d 7d7b 2520 656e 6469  encode }}{% endi
+00000860: 6620 257d 7b25 2065 6e64 6966 2025 7d22  f %}{% endif %}"
+00000870: 202f 3e0a 0a20 2020 2020 2020 203c 6469   />..        <di
+00000880: 7620 636c 6173 733d 2263 6172 6422 3e0a  v class="card">.
+00000890: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+000008a0: 6c61 7373 3d22 6361 7264 2d62 6f64 7922  lass="card-body"
+000008b0: 3e0a 2020 2020 2020 2020 2020 2020 3c64  >.            <d
+000008c0: 6976 2063 6c61 7373 3d22 7461 626c 652d  iv class="table-
+000008d0: 7265 7370 6f6e 7369 7665 223e 0a20 2020  responsive">.   
+000008e0: 2020 2020 2020 2020 2020 207b 2520 7265             {% re
+000008f0: 6e64 6572 5f74 6162 6c65 2074 6162 6c65  nder_table table
+00000900: 2027 696e 632f 7461 626c 655f 6874 6d78   'inc/table_htmx
+00000910: 2e68 746d 6c27 2025 7d0a 2020 2020 2020  .html' %}.      
+00000920: 2020 2020 2020 3c2f 6469 763e 0a20 2020        </div>.   
+00000930: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
+00000940: 2020 2020 2020 3c2f 6469 763e 0a0a 2020        </div>..  
+00000950: 2020 2020 2020 7b25 2069 6620 7065 726d        {% if perm
+00000960: 6973 7369 6f6e 732e 6465 6c65 7465 2025  issions.delete %
+00000970: 7d0a 2020 2020 2020 2020 2020 7b25 2077  }.          {% w
+00000980: 6974 6820 6275 6c6b 5f64 656c 6574 655f  ith bulk_delete_
+00000990: 7572 6c3d 2770 6c75 6769 6e73 3a61 7869  url='plugins:axi
+000009a0: 616e 735f 6e65 7462 6f78 5f70 6475 3a70  ans_netbox_pdu:p
+000009b0: 6475 636f 6e66 6967 5f62 756c 6b5f 6465  duconfig_bulk_de
+000009c0: 6c65 7465 2720 257d 0a20 2020 2020 2020  lete' %}.       
+000009d0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+000009e0: 226e 6f70 7269 6e74 2062 756c 6b2d 6275  "noprint bulk-bu
+000009f0: 7474 6f6e 7322 3e0a 2020 2020 2020 2020  ttons">.        
+00000a00: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+00000a10: 3d22 6275 6c6b 2d62 7574 746f 6e2d 6772  ="bulk-button-gr
+00000a20: 6f75 7022 3e0a 2020 2020 2020 2020 2020  oup">.          
+00000a30: 2020 2020 2020 7b25 2062 6c6f 636b 2062        {% block b
+00000a40: 756c 6b5f 6275 7474 6f6e 7320 257d 7b25  ulk_buttons %}{%
+00000a50: 2065 6e64 626c 6f63 6b20 257d 0a20 2020   endblock %}.   
+00000a60: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
+00000a70: 6966 2062 756c 6b5f 6465 6c65 7465 5f75  if bulk_delete_u
+00000a80: 726c 2061 6e64 2070 6572 6d69 7373 696f  rl and permissio
+00000a90: 6e73 2e64 656c 6574 6520 257d 0a20 2020  ns.delete %}.   
+00000aa0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00000ab0: 6275 7474 6f6e 2074 7970 653d 2273 7562  button type="sub
+00000ac0: 6d69 7422 206e 616d 653d 225f 6465 6c65  mit" name="_dele
+00000ad0: 7465 2220 666f 726d 6163 7469 6f6e 3d22  te" formaction="
+00000ae0: 7b25 2075 726c 2062 756c 6b5f 6465 6c65  {% url bulk_dele
+00000af0: 7465 5f75 726c 2025 7d7b 2520 6966 2072  te_url %}{% if r
+00000b00: 6571 7565 7374 2e47 4554 2025 7d3f 7b7b  equest.GET %}?{{
+00000b10: 2072 6571 7565 7374 2e47 4554 2e75 726c   request.GET.url
+00000b20: 656e 636f 6465 207d 7d7b 2520 656e 6469  encode }}{% endi
+00000b30: 6620 257d 2220 636c 6173 733d 2262 746e  f %}" class="btn
+00000b40: 2062 746e 2d64 616e 6765 7220 6274 6e2d   btn-danger btn-
+00000b50: 736d 223e 0a20 2020 2020 2020 2020 2020  sm">.           
+00000b60: 2020 2020 2020 2020 203c 6920 636c 6173           <i clas
+00000b70: 733d 226d 6469 206d 6469 2d74 7261 7368  s="mdi mdi-trash
+00000b80: 2d63 616e 2d6f 7574 6c69 6e65 2220 6172  -can-outline" ar
+00000b90: 6961 2d68 6964 6465 6e3d 2274 7275 6522  ia-hidden="true"
+00000ba0: 3e3c 2f69 3e20 4465 6c65 7465 2053 656c  ></i> Delete Sel
+00000bb0: 6563 7465 640a 2020 2020 2020 2020 2020  ected.          
+00000bc0: 2020 2020 2020 2020 3c2f 6275 7474 6f6e          </button
+00000bd0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00000be0: 2020 7b25 2065 6e64 6966 2025 7d0a 2020    {% endif %}.  
+00000bf0: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
+00000c00: 763e 0a20 2020 2020 2020 2020 2020 203c  v>.            <
+00000c10: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
+00000c20: 7b25 2065 6e64 7769 7468 2025 7d0a 2020  {% endwith %}.  
+00000c30: 2020 2020 2020 7b25 2065 6e64 6966 2025        {% endif %
+00000c40: 7d0a 0a20 2020 2020 203c 2f66 6f72 6d3e  }..      </form>
+00000c50: 0a0a 2020 2020 2020 7b25 2069 6e63 6c75  ..      {% inclu
+00000c60: 6465 2027 696e 632f 7061 6769 6e61 746f  de 'inc/paginato
+00000c70: 722e 6874 6d6c 2720 7769 7468 2070 6167  r.html' with pag
+00000c80: 696e 6174 6f72 3d74 6162 6c65 2e70 6167  inator=table.pag
+00000c90: 696e 6174 6f72 2070 6167 653d 7461 626c  inator page=tabl
+00000ca0: 652e 7061 6765 2025 7d0a 2020 2020 3c2f  e.page %}.    </
+00000cb0: 6469 763e 0a0a 2020 2020 7b25 2069 6620  div>..    {% if 
+00000cc0: 6669 6c74 6572 5f66 6f72 6d20 257d 0a20  filter_form %}. 
+00000cd0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+00000ce0: 2274 6162 2d70 616e 6520 7368 6f77 2220  "tab-pane show" 
+00000cf0: 6964 3d22 6669 6c74 6572 732d 666f 726d  id="filters-form
+00000d00: 2220 726f 6c65 3d22 7461 6270 616e 656c  " role="tabpanel
+00000d10: 2220 6172 6961 2d6c 6162 656c 6c65 6462  " aria-labelledb
+00000d20: 793d 2266 696c 7465 7273 2d66 6f72 6d2d  y="filters-form-
+00000d30: 7461 6222 3e0a 2020 2020 2020 2020 7b25  tab">.        {%
+00000d40: 2069 6e63 6c75 6465 2027 696e 632f 6669   include 'inc/fi
+00000d50: 6c74 6572 5f6c 6973 742e 6874 6d6c 2720  lter_list.html' 
+00000d60: 257d 0a20 2020 2020 203c 2f64 6976 3e0a  %}.      </div>.
+00000d70: 2020 2020 7b25 2065 6e64 6966 2025 7d0a      {% endif %}.
+00000d80: 2020 3c2f 6469 763e 0a0a 2020 7b25 2074    </div>..  {% t
+00000d90: 6162 6c65 5f63 6f6e 6669 675f 666f 726d  able_config_form
+00000da0: 2074 6162 6c65 2074 6162 6c65 5f6e 616d   table table_nam
+00000db0: 653d 2252 6563 6f72 6454 6162 6c65 2220  e="RecordTable" 
+00000dc0: 257d 0a7b 2520 656e 6462 6c6f 636b 2063  %}.{% endblock c
+00000dd0: 6f6e 7465 6e74 2d77 7261 7070 6572 2025  ontent-wrapper %
+00000de0: 7d0a                                     }.
```

### Comparing `meraki-netbox-plugin-pdu-0.0.8/axians_netbox_pdu/templates/axians_netbox_pdu/rack_power_usage.html` & `meraki-netbox-plugin-pdu-0.0.9/axians_netbox_pdu/templates/axians_netbox_pdu/rack_power_usage.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,72 +1,76 @@
 {% load humanize %}
 {% load helpers %}
 
 {% with config=settings.PLUGINS_CONFIG.axians_netbox_pdu %}
 {% if config.rack_view_pdu_devices %}
-<div class="panel panel-default">
-    <div class="panel-heading">
+<div class="card card-default">
+    <div class="card-header">
         <strong>Power Usage Devices</strong>
     </div>
-    <table class="table table-hover panel-body attr-table">
-        <thead>
-            <tr>
-                <th>
-                    Device
-                </th>
-                <th>
-                    Power Usage
-                </th>
-                <th>
-                    Last Updated
-                </th>
-            </tr>
-        </thead>
-        <tbody>
-            {% for pdu in pdus %}
-            <tr>
-                <td>
-                    <a href="{{pdu.get_absolute_url}}">{{pdu.name}}</a>
-                </td>
-                <td>
-                    <span title="">{{pdu.pdustatus.get_power_usage}}</span>
-                </td>
-                <td>
-                    <span>{{ pdu.pdustatus.updated_at|naturaltime }}</span>
-                </td>
-            </tr>
-            {%endfor %}
-        </tbody>
-    </table>
+    <div class="card-body">
+        <table class="table table-hover attr-table">
+            <thead>
+                <tr>
+                    <th>
+                        Device
+                    </th>
+                    <th>
+                        Power Usage
+                    </th>
+                    <th>
+                        Last Updated
+                    </th>
+                </tr>
+            </thead>
+            <tbody>
+                {% for pdu in pdus %}
+                <tr>
+                    <td>
+                        <a href="{{pdu.get_absolute_url}}">{{pdu.name}}</a>
+                    </td>
+                    <td>
+                        <span title="">{{pdu.pdustatus.get_power_usage}}</span>
+                    </td>
+                    <td>
+                        <span>{{ pdu.pdustatus.updated_at|naturaltime }}</span>
+                    </td>
+                </tr>
+                {%endfor %}
+            </tbody>
+        </table>
+    </div>
 </div>
 {% endif %}
 
 {% if config.rack_view_usage_summary %}
-<div class="panel panel-default">
-    <div class="panel-heading">
+<div class="card card-default">
+    <div class="card-header">
         <strong>Power Usage Summary</strong>
     </div>
-    <table class="table table-hover panel-body attr-table">
-        <tbody>
-            {% if total_power_usage_unit %}
-            <tr>
-                <td>Total Power Usage</td>
-                <td>{{ total_power_usage }} {{ total_power_usage_unit|title }}</td>
-            </tr>
-            {% endif %}
-            {% if total_available_power %}
-            <tr>
-                <td>Total Power Available</td>
-                <td>{{ total_available_power }} {{ total_power_usage_unit|title }}</td>
-            </tr>
-            {% endif %}
-            {% if total_power_usage_percentage %}
-            <tr>
-                <td>Utilization</td>
-                <td>{% utilization_graph total_power_usage_percentage %}</td>
-            </tr>
-            {% endif %}
-        </tbody>
-    </table>
+    <div class="card-body">
+        <table class="table table-hover attr-table">
+            <tbody>
+                {% if total_power_usage_unit %}
+                <tr>
+                    <td>Total Power Usage</td>
+                    <td>{{ total_power_usage }} {{ total_power_usage_unit|title }}</td>
+                </tr>
+                {% endif %}
+                {% if total_available_power %}
+                <tr>
+                    <td>Total Power Available</td>
+                    <td>{{ total_available_power }} {{ total_power_usage_unit|title }}</td>
+                </tr>
+                {% endif %}
+                {% if total_power_usage_percentage %}
+                <tr>
+                    <td>Utilization</td>
+                    <td>{% utilization_graph total_power_usage_percentage %}</td>
+                </tr>
+                {% endif %}
+            </tbody>
+        </table>
+    </div>
 </div>
 {% endif %}
-{% endwith %}
+{% endwith %}
```

### Comparing `meraki-netbox-plugin-pdu-0.0.8/axians_netbox_pdu/tests/test_pduconfig_api.py` & `meraki-netbox-plugin-pdu-0.0.9/axians_netbox_pdu/tests/test_pduconfig_api.py`

 * *Files identical despite different names*

### Comparing `meraki-netbox-plugin-pdu-0.0.8/axians_netbox_pdu/tests/test_pduconfig_views.py` & `meraki-netbox-plugin-pdu-0.0.9/axians_netbox_pdu/tests/test_pduconfig_views.py`

 * *Files identical despite different names*

### Comparing `meraki-netbox-plugin-pdu-0.0.8/axians_netbox_pdu/tests/test_pdustatus_api.py` & `meraki-netbox-plugin-pdu-0.0.9/axians_netbox_pdu/tests/test_pdustatus_api.py`

 * *Files identical despite different names*

### Comparing `meraki-netbox-plugin-pdu-0.0.8/axians_netbox_pdu/urls.py` & `meraki-netbox-plugin-pdu-0.0.9/axians_netbox_pdu/urls.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,26 @@
 from django.urls import path
 
+from netbox.views.generic import ObjectChangeLogView
+
+from .models import PDUConfig
+
 from .views import (
+    PDUConfigView,
+    PDUConfigDeleteView,
     PDUConfigBulkDeleteView,
     PDUConfigCreateView,
     PDUConfigEditView,
-    PDUConfigImportView,
     PDUConfigListView,
 )
 
 urlpatterns = [
     path("pdu-config/", PDUConfigListView.as_view(), name="pduconfig_list"),
     path("pdu-config/add/", PDUConfigCreateView.as_view(), name="pduconfig_add"),
-    path("pdu-config/import/", PDUConfigImportView.as_view(), name="pduconfig_import"),
     path("pdu-config/delete/", PDUConfigBulkDeleteView.as_view(), name="pduconfig_bulk_delete"),
+    path("pdu-config/<int:pk>/", PDUConfigView.as_view(), name="pduconfig_view"),
+    path("pdu-config/<int:pk>/delete/", PDUConfigDeleteView.as_view(), name="pduconfig_delete"),
     path("pdu-config/<int:pk>/edit/", PDUConfigEditView.as_view(), name="pduconfig_edit"),
+    path("pdu-config/<int:pk>/changelog/", ObjectChangeLogView.as_view(), name="pduconfig_changelog", kwargs={
+        'model': PDUConfig
+    }),
 ]
```

### Comparing `meraki-netbox-plugin-pdu-0.0.8/axians_netbox_pdu/utilities.py` & `meraki-netbox-plugin-pdu-0.0.9/axians_netbox_pdu/utilities.py`

 * *Files identical despite different names*

### Comparing `meraki-netbox-plugin-pdu-0.0.8/axians_netbox_pdu/views.py` & `meraki-netbox-plugin-pdu-0.0.9/axians_netbox_pdu/views.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from django.contrib.auth.mixins import PermissionRequiredMixin
 from django.shortcuts import get_object_or_404, render
 from django.views.generic import View
 
-from netbox.views.generic import BulkDeleteView, BulkImportView, ObjectEditView, ObjectListView
+from netbox.views.generic import BulkDeleteView, BulkImportView, ObjectEditView, ObjectListView, ObjectView, ObjectDeleteView
 
 from .filters import PDUConfigFilter
-from .forms import PDUConfigCSVForm, PDUConfigFilterForm, PDUConfigForm
+from .forms import PDUConfigFilterForm, PDUConfigForm
 from .models import PDUConfig
 from .tables import PDUConfigBulkTable, PDUConfigTable
 
-from django.conf import settings
-from packaging import version
+class PDUConfigView(PermissionRequiredMixin, ObjectView):
+
+    permission_required = "axians_netbox_pdu.view_pduconfig"
+    queryset = PDUConfig.objects.all()
+    template_name = 'axians_netbox_pdu/pduconfig.html'
 
-NETBOX_CURRENT_VERSION = version.parse(settings.VERSION)
 
 class PDUConfigListView(PermissionRequiredMixin, ObjectListView):
     """View for listing all PDUConfig items"""
 
     permission_required = "axians_netbox_pdu.view_pduconfig"
     queryset = PDUConfig.objects.all()
     filterset = PDUConfigFilter
@@ -27,29 +29,24 @@
 
 class PDUConfigCreateView(PermissionRequiredMixin, ObjectEditView):
     """View for creating a new PDUConfig"""
 
     permission_required = "axians_netbox_pdu.add_pduconfig"
     model = PDUConfig
     queryset = PDUConfig.objects.all()
-    model_form = PDUConfigForm
-    if NETBOX_CURRENT_VERSION >= version.parse("3.0"):
-        template_name = "axians_netbox_pdu/pduconfig_edit_3_x.html"
-    else:
-        template_name = "axians_netbox_pdu/pduconfig_edit.html"
+    form = PDUConfigForm
+    template_name = "axians_netbox_pdu/pduconfig_edit.html"
     default_return_url = "plugins:axians_netbox_pdu:pduconfig_list"
 
 
-class PDUConfigImportView(PermissionRequiredMixin, BulkImportView):
-    """View for bulk-importing a CSV file to create PDUConfigs"""
+class PDUConfigDeleteView(PermissionRequiredMixin, ObjectDeleteView):
+    """View for deleting one PDUConfig."""
 
-    permission_required = "axians_netbox_pdu.add_pduconfig"
-    queryset = PDUConfig.objects.all()
-    model_form = PDUConfigCSVForm
-    table = PDUConfigBulkTable
+    permission_required = "axians_netbox_pdu.delete_pduconfig"
+    queryset = PDUConfig.objects.filter()
     default_return_url = "plugins:axians_netbox_pdu:pduconfig_list"
 
 
 class PDUConfigBulkDeleteView(PermissionRequiredMixin, BulkDeleteView):
     """View for deleting one or more PDUConfigs."""
 
     permission_required = "axians_netbox_pdu.delete_pduconfig"
```

### Comparing `meraki-netbox-plugin-pdu-0.0.8/axians_netbox_pdu/worker.py` & `meraki-netbox-plugin-pdu-0.0.9/axians_netbox_pdu/worker.py`

 * *Files identical despite different names*

### Comparing `meraki-netbox-plugin-pdu-0.0.8/pyproject.toml` & `meraki-netbox-plugin-pdu-0.0.9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "meraki-netbox-plugin-pdu"
-version = "0.0.8"
+version = "0.0.9"
 description = "A plugin for NetBox to easily display PDU information."
 authors = ["Alex Houlton <bob@meraki.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/minitriga/axians-netbox-plugin-pdu"
 repository = "https://github.com/minitriga/axians-netbox-plugin-pdu"
 keywords = ["netbox", "network", "pdu", "django", "apc"]
```

### Comparing `meraki-netbox-plugin-pdu-0.0.8/setup.py` & `meraki-netbox-plugin-pdu-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 install_requires = \
 ['easysnmp>=0.2.5,<0.3.0',
  'invoke>=1.4.1,<2.0.0',
  'rq-scheduler>=0.10.0,<0.11.0']
 
 setup_kwargs = {
     'name': 'meraki-netbox-plugin-pdu',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'A plugin for NetBox to easily display PDU information.',
     'long_description': '# Netbox PDU Plugin\n\nA plugin for [Netbox](https://github.com/netbox-community/netbox) to get power distribution unit Information.\n\n`axians-netbox-plugin-pdu` is using [Easy SNMP](https://easysnmp.readthedocs.io/en/latest/), [Django-RQ](https://github.com/rq/django-rq) and [RQ-Scheduler](https://github.com/rq/rq-scheduler) to display PDU information within Netbox.\n\n## Installation\nThe plugin is available as a Python package in pypi and can be installed with pip\n\n```\npip install axians-netbox-plugin-pdu\n```\n\n> The plugin is compatible with NetBox 2.9.1 and higher\n\nOnce installed, the plugin needs to be enabled in your `configuration.py`\n\n```python\nPLUGINS = ["axians_netbox_pdu"]\n\n# PLUGINS_CONFIG = {\n#   "axians_netbox_pdu": {\n#     ADD YOUR SETTINGS HERE\n#   }\n# }\n```\n\nThere are a number of default settings that can be altered using the following list of settings:\n\n* `schedule`: Boolean (default True). If True, this will enable automatic polling of your PDU Devices.\n* `schedule_interval`: Integer (default 300 seconds). Length of time between each scheduled poll.\n* `snmp_read`: String (default public) SNMP read value for your SNMP enabled PDU\'s.\n* `snmp_write`: String (default private) SNMP write value for your SNMP enabled PDU\'s.\n* `rack_view_pdu_devices`: Boolean (default True), if True, the power usage per PDU will be displayed on the rack page.\n* `rack_view_usage_summary`: Boolean (default True), if True, the a summary information tile will appear within the rack page to show true power utilization within the rack.\n* `rack_view_summary_unit`: String (default watts), option to display watts/kilowatts on the rack summary view. If "kilowatts" is used the power usage summary will display in Kilowatts.\n\n## Usage\n### Preparation\nFor this plugin to work there must be a new worker added to your Netbox installation. The new worker is a custom scheduler that will schedule the PDU Tasks to run on an interval and utilize the django-rq library.\n\n> You can utilize this library without the automated tasks by feeding Netbox the power usage information via the `axians_netbox_pdu` API.\n\n### Default Environment\nFor the standard install please use the included [netbox-pdu.service](contrib/netbox-pdu.service) and install using the standard [Netbox Documentation](https://netbox.readthedocs.io/en/stable/installation/migrating-to-systemd/).\n\n### Docker Environment\nTo use within Docker make sure you have a container running that runs the following command: `python manage.py pduschedule`\n\n### Adding a new PDU Configuration\nOnce installed and the `pduscheduler` is running you can attach a `PDUConfig` to a DeviceType. To do this you must have a DeviceType configured with PowerOutlets. You can specify the DeviceType, PDU SNMP OID and the Unit. This enables the plugin to know what SNMP OID to collect per DeviceType.\n\nNow a PDUConfig has been created a device must be created with a management IP. Once this is done the plugin can poll the PDU via SNMP and save the power usage.\n\nThis can also be done via Bulk Import or via the API.\n\n> If a a PDUConfig is not created for a DeviceType and the Device does not have a Primary IP no data will be collected.\n\n### API\nThe plugin includes several endpoints to manage the PDUConfig and PDUStatus.\n\n```\nGET       /api/plugins/pdu/pdu-config/         List PDUConfig\nPOST      /api/plugins/pdu/pdu-config/         Create PDUConfig\nPATCH/PUT /api/plugins/pdu/pdu-config/{id}/    Edit a specific PDUConfig\nDELETE /api/plugins/pdu/pdu-config/{id}/       Delete a specific PDUConfig\n\nGET       /api/plugins/pdu/pdu-status/         List PDUStatus\nPOST      /api/plugins/pdu/pdu-status/         Create PDUStatus\nPATCH/PUT /api/plugins/pdu/pdu-status/{id}/    Edit a specific PDUStatus\nDELETE /api/plugins/pdu/pdu-status/{id}/       Delete a specific PDUStatus\n```\n\n## Screen Shots\nList of PDUConfig Instances\n![PDUConfig List View](docs/images/PDUConfig_list.png)\n\nImport PDUConfig Instances\n![PDUConfig Import View](docs/images/PDUConfig_import.png)\n\nEdit PDUConfig Instances\n![PDUConfig Edit View](docs/images/PDUConfig_edit.png)\n\nView PDUStatus Device View\n![PDUStatus Device View](docs/images/PDUStatus_device.png)\n\nView PDUStatus Rack View\n![PDUStatus Rack View](docs/images/PDUStatus_rack.png)\n\n## Contributing\n\nPull requests are welcomed.\n\nThe project is packaged with a light development environment based on `docker-compose` to help with the local development of the project.\n\n- Black, Pylint, Bandit and pydockstyle for Python linting and formatting.\n- Django unit test to ensure the plugin is working properly.\n\n### CLI Helper Commands\n\nThe project comes with a CLI helper based on [invoke](http://www.pyinvoke.org/) to help setup the development environment. The commands are listed below in 3 categories `dev environment`, `utility` and `testing`.\n\nEach command can be executed with `invoke <command>`. All commands support the arguments `--netbox-ver` and `--python-ver` if you want to manually define the version of Python and Netbox to use. Each command also has its own help `invoke <command> --help`.\n\n#### Local dev environment\n```\n  build            Build all docker images.\n  debug            Start NetBox and its dependencies in debug mode.\n  destroy          Destroy all containers and volumes.\n  start            Start NetBox and its dependencies in detached mode.\n  stop             Stop NetBox and its dependencies.\n```\n\n\n#### Utility\n```\n  cli              Launch a bash shell inside the running NetBox container.\n  create-user      Create a new user in django (default: admin), will prompt for password.\n  makemigrations   Run Make Migration in Django.\n  nbshell          Launch a nbshell session.\n```\n#### Testing\n\n```\n  tests            Run all tests for this plugin.\n  pylint           Run pylint code analysis.\n  pydocstyle       Run pydocstyle to validate docstring formatting adheres to NTC defined standards.\n  bandit           Run bandit to validate basic static code security analysis.\n  black            Run black to check that Python files adhere to its style standards.\n  unittest         Run Django unit tests for the plugin.\n```',
     'author': 'Alex Houlton',
     'author_email': 'bob@meraki.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/minitriga/axians-netbox-plugin-pdu',
```

### Comparing `meraki-netbox-plugin-pdu-0.0.8/PKG-INFO` & `meraki-netbox-plugin-pdu-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meraki-netbox-plugin-pdu
-Version: 0.0.8
+Version: 0.0.9
 Summary: A plugin for NetBox to easily display PDU information.
 Home-page: https://github.com/minitriga/axians-netbox-plugin-pdu
 License: Apache-2.0
 Keywords: netbox,network,pdu,django,apc
 Author: Alex Houlton
 Author-email: bob@meraki.com
 Requires-Python: >=3.6,<4.0
```

