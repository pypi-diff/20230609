# Comparing `tmp/apis_bibsonomy-0.7.0.tar.gz` & `tmp/apis_bibsonomy-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apis_bibsonomy-0.7.0.tar", max compression
+gzip compressed data, was "apis_bibsonomy-0.7.1.tar", max compression
```

## Comparing `apis_bibsonomy-0.7.0.tar` & `apis_bibsonomy-0.7.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1141 2023-05-22 08:45:20.031105 apis_bibsonomy-0.7.0/LICENSE.txt
--rw-r--r--   0        0        0       22 2023-05-22 08:45:52.439519 apis_bibsonomy-0.7.0/apis_bibsonomy/__init__.py
--rw-r--r--   0        0        0     5385 2023-05-22 08:45:20.031105 apis_bibsonomy-0.7.0/apis_bibsonomy/api_views.py
--rw-r--r--   0        0        0      150 2023-05-22 08:45:20.031105 apis_bibsonomy-0.7.0/apis_bibsonomy/apps.py
--rw-r--r--   0        0        0     3778 2023-05-22 08:45:20.031105 apis_bibsonomy-0.7.0/apis_bibsonomy/autocompletes.py
--rw-r--r--   0        0        0        0 2023-05-22 08:45:20.031105 apis_bibsonomy-0.7.0/apis_bibsonomy/fields.py
--rw-r--r--   0        0        0     1707 2023-05-22 08:45:20.031105 apis_bibsonomy-0.7.0/apis_bibsonomy/forms.py
--rw-r--r--   0        0        0     1157 2023-05-22 08:45:20.031105 apis_bibsonomy-0.7.0/apis_bibsonomy/migrations/0001_initial.py
--rw-r--r--   0        0        0      484 2023-05-22 08:45:20.031105 apis_bibsonomy-0.7.0/apis_bibsonomy/migrations/0002_reference_folio.py
--rw-r--r--   0        0        0      704 2023-05-22 08:45:20.031105 apis_bibsonomy-0.7.0/apis_bibsonomy/migrations/0003_auto_20230202_0953.py
--rw-r--r--   0        0        0        0 2023-05-22 08:45:20.031105 apis_bibsonomy-0.7.0/apis_bibsonomy/migrations/__init__.py
--rw-r--r--   0        0        0     2660 2023-05-22 08:45:20.031105 apis_bibsonomy-0.7.0/apis_bibsonomy/models.py
--rw-r--r--   0        0        0      107 2023-05-22 08:45:20.031105 apis_bibsonomy-0.7.0/apis_bibsonomy/static/apis_bibsonomy/css/apis_bibsonomy.css
--rw-r--r--   0        0        0     5034 2023-05-22 08:45:20.031105 apis_bibsonomy-0.7.0/apis_bibsonomy/static/apis_bibsonomy/js/apis_bibsonomy_init.js
--rw-r--r--   0        0        0   116169 2023-05-22 08:45:20.031105 apis_bibsonomy-0.7.0/apis_bibsonomy/static/apis_bibsonomy/js/bibtex_js.js
--rw-r--r--   0        0        0      761 2023-05-22 08:45:20.035105 apis_bibsonomy-0.7.0/apis_bibsonomy/templates/apis_bibsonomy/apis_bibsonomy_include.html
--rw-r--r--   0        0        0      214 2023-05-22 08:45:20.035105 apis_bibsonomy-0.7.0/apis_bibsonomy/templates/apis_bibsonomy/form_tag.html
--rw-r--r--   0        0        0     1028 2023-05-22 08:45:20.035105 apis_bibsonomy-0.7.0/apis_bibsonomy/templates/apis_bibsonomy/reference_confirm_delete.html
--rw-r--r--   0        0        0      776 2023-05-22 08:45:20.035105 apis_bibsonomy-0.7.0/apis_bibsonomy/templates/apis_bibsonomy/reference_detail.html
--rw-r--r--   0        0        0      365 2023-05-22 08:45:20.035105 apis_bibsonomy-0.7.0/apis_bibsonomy/templates/apis_bibsonomy/reference_list.html
--rw-r--r--   0        0        0      394 2023-05-22 08:45:20.035105 apis_bibsonomy-0.7.0/apis_bibsonomy/templates/base.html
--rw-r--r--   0        0        0        0 2023-05-22 08:45:20.035105 apis_bibsonomy-0.7.0/apis_bibsonomy/templatetags/__init__.py
--rw-r--r--   0        0        0      774 2023-05-22 08:45:20.035105 apis_bibsonomy-0.7.0/apis_bibsonomy/templatetags/bibsonomy_templatetags.py
--rw-r--r--   0        0        0      659 2023-05-22 08:45:20.035105 apis_bibsonomy-0.7.0/apis_bibsonomy/urls.py
--rw-r--r--   0        0        0     3069 2023-05-22 08:45:20.035105 apis_bibsonomy-0.7.0/apis_bibsonomy/utils.py
--rw-r--r--   0        0        0      762 2023-05-22 08:45:20.035105 apis_bibsonomy-0.7.0/apis_bibsonomy/views.py
--rw-r--r--   0        0        0      345 2023-05-22 08:45:52.363518 apis_bibsonomy-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      835 1970-01-01 00:00:00.000000 apis_bibsonomy-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1141 2023-06-09 10:18:21.377382 apis_bibsonomy-0.7.1/LICENSE.txt
+-rw-r--r--   0        0        0       22 2023-06-09 10:18:48.721568 apis_bibsonomy-0.7.1/apis_bibsonomy/__init__.py
+-rw-r--r--   0        0        0     5385 2023-06-09 10:18:21.377382 apis_bibsonomy-0.7.1/apis_bibsonomy/api_views.py
+-rw-r--r--   0        0        0      150 2023-06-09 10:18:21.377382 apis_bibsonomy-0.7.1/apis_bibsonomy/apps.py
+-rw-r--r--   0        0        0     3778 2023-06-09 10:18:21.377382 apis_bibsonomy-0.7.1/apis_bibsonomy/autocompletes.py
+-rw-r--r--   0        0        0        0 2023-06-09 10:18:21.377382 apis_bibsonomy-0.7.1/apis_bibsonomy/fields.py
+-rw-r--r--   0        0        0     1707 2023-06-09 10:18:21.377382 apis_bibsonomy-0.7.1/apis_bibsonomy/forms.py
+-rw-r--r--   0        0        0     1157 2023-06-09 10:18:21.377382 apis_bibsonomy-0.7.1/apis_bibsonomy/migrations/0001_initial.py
+-rw-r--r--   0        0        0      484 2023-06-09 10:18:21.377382 apis_bibsonomy-0.7.1/apis_bibsonomy/migrations/0002_reference_folio.py
+-rw-r--r--   0        0        0      704 2023-06-09 10:18:21.377382 apis_bibsonomy-0.7.1/apis_bibsonomy/migrations/0003_auto_20230202_0953.py
+-rw-r--r--   0        0        0        0 2023-06-09 10:18:21.377382 apis_bibsonomy-0.7.1/apis_bibsonomy/migrations/__init__.py
+-rw-r--r--   0        0        0     2660 2023-06-09 10:18:21.377382 apis_bibsonomy-0.7.1/apis_bibsonomy/models.py
+-rw-r--r--   0        0        0      107 2023-06-09 10:18:21.377382 apis_bibsonomy-0.7.1/apis_bibsonomy/static/apis_bibsonomy/css/apis_bibsonomy.css
+-rw-r--r--   0        0        0     5034 2023-06-09 10:18:21.377382 apis_bibsonomy-0.7.1/apis_bibsonomy/static/apis_bibsonomy/js/apis_bibsonomy_init.js
+-rw-r--r--   0        0        0   116169 2023-06-09 10:18:21.377382 apis_bibsonomy-0.7.1/apis_bibsonomy/static/apis_bibsonomy/js/bibtex_js.js
+-rw-r--r--   0        0        0      761 2023-06-09 10:18:21.377382 apis_bibsonomy-0.7.1/apis_bibsonomy/templates/apis_bibsonomy/apis_bibsonomy_include.html
+-rw-r--r--   0        0        0      214 2023-06-09 10:18:21.377382 apis_bibsonomy-0.7.1/apis_bibsonomy/templates/apis_bibsonomy/form_tag.html
+-rw-r--r--   0        0        0     1028 2023-06-09 10:18:21.377382 apis_bibsonomy-0.7.1/apis_bibsonomy/templates/apis_bibsonomy/reference_confirm_delete.html
+-rw-r--r--   0        0        0      761 2023-06-09 10:18:21.377382 apis_bibsonomy-0.7.1/apis_bibsonomy/templates/apis_bibsonomy/reference_detail.html
+-rw-r--r--   0        0        0      365 2023-06-09 10:18:21.377382 apis_bibsonomy-0.7.1/apis_bibsonomy/templates/apis_bibsonomy/reference_list.html
+-rw-r--r--   0        0        0      394 2023-06-09 10:18:21.377382 apis_bibsonomy-0.7.1/apis_bibsonomy/templates/base.html
+-rw-r--r--   0        0        0        0 2023-06-09 10:18:21.377382 apis_bibsonomy-0.7.1/apis_bibsonomy/templatetags/__init__.py
+-rw-r--r--   0        0        0      774 2023-06-09 10:18:21.377382 apis_bibsonomy-0.7.1/apis_bibsonomy/templatetags/bibsonomy_templatetags.py
+-rw-r--r--   0        0        0      659 2023-06-09 10:18:21.377382 apis_bibsonomy-0.7.1/apis_bibsonomy/urls.py
+-rw-r--r--   0        0        0     3069 2023-06-09 10:18:21.377382 apis_bibsonomy-0.7.1/apis_bibsonomy/utils.py
+-rw-r--r--   0        0        0      762 2023-06-09 10:18:21.377382 apis_bibsonomy-0.7.1/apis_bibsonomy/views.py
+-rw-r--r--   0        0        0      345 2023-06-09 10:18:48.665567 apis_bibsonomy-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0      835 1970-01-01 00:00:00.000000 apis_bibsonomy-0.7.1/PKG-INFO
```

### Comparing `apis_bibsonomy-0.7.0/LICENSE.txt` & `apis_bibsonomy-0.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apis_bibsonomy-0.7.0/apis_bibsonomy/api_views.py` & `apis_bibsonomy-0.7.1/apis_bibsonomy/api_views.py`

 * *Files identical despite different names*

### Comparing `apis_bibsonomy-0.7.0/apis_bibsonomy/autocompletes.py` & `apis_bibsonomy-0.7.1/apis_bibsonomy/autocompletes.py`

 * *Files identical despite different names*

### Comparing `apis_bibsonomy-0.7.0/apis_bibsonomy/forms.py` & `apis_bibsonomy-0.7.1/apis_bibsonomy/forms.py`

 * *Files identical despite different names*

### Comparing `apis_bibsonomy-0.7.0/apis_bibsonomy/migrations/0001_initial.py` & `apis_bibsonomy-0.7.1/apis_bibsonomy/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `apis_bibsonomy-0.7.0/apis_bibsonomy/migrations/0003_auto_20230202_0953.py` & `apis_bibsonomy-0.7.1/apis_bibsonomy/migrations/0003_auto_20230202_0953.py`

 * *Files identical despite different names*

### Comparing `apis_bibsonomy-0.7.0/apis_bibsonomy/models.py` & `apis_bibsonomy-0.7.1/apis_bibsonomy/models.py`

 * *Files identical despite different names*

### Comparing `apis_bibsonomy-0.7.0/apis_bibsonomy/static/apis_bibsonomy/js/apis_bibsonomy_init.js` & `apis_bibsonomy-0.7.1/apis_bibsonomy/static/apis_bibsonomy/js/apis_bibsonomy_init.js`

 * *Files identical despite different names*

### Comparing `apis_bibsonomy-0.7.0/apis_bibsonomy/static/apis_bibsonomy/js/bibtex_js.js` & `apis_bibsonomy-0.7.1/apis_bibsonomy/static/apis_bibsonomy/js/bibtex_js.js`

 * *Files identical despite different names*

### Comparing `apis_bibsonomy-0.7.0/apis_bibsonomy/templates/apis_bibsonomy/apis_bibsonomy_include.html` & `apis_bibsonomy-0.7.1/apis_bibsonomy/templates/apis_bibsonomy/apis_bibsonomy_include.html`

 * *Files identical despite different names*

### Comparing `apis_bibsonomy-0.7.0/apis_bibsonomy/templates/apis_bibsonomy/reference_confirm_delete.html` & `apis_bibsonomy-0.7.1/apis_bibsonomy/templates/apis_bibsonomy/reference_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `apis_bibsonomy-0.7.0/apis_bibsonomy/templates/apis_bibsonomy/reference_detail.html` & `apis_bibsonomy-0.7.1/apis_bibsonomy/templates/apis_bibsonomy/reference_detail.html`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 <hr/>
 
 Also referenced by:
 <ul>
 {% for ref in similar_references %}
 <li>
-{% with similar_references.referenced_object as obj %}
+{% with ref.referenced_object as obj %}
 {% if obj.get_absolute_url %}<a href="{{ obj.get_absolute_url }}">{{ obj }}</a>{% else %}{{ obj }}{% endif %}
 (<a href="{{ ref.get_absolute_url }}">{{ ref.id }}</a>)
 <a href="{% url "apis_bibsonomy:referencedelete" ref.id %}?redirect={% url "apis_bibsonomy:referencedetail" reference.id %}">Delete</a>
 {% endwith %}
 </li>
 {% endfor %}
 </ul>
```

#### html2text {}

```diff
@@ -3,14 +3,14 @@
 on {{ reference.referenced_object }}
  bibtex
 {{ reference.bibtexjson }}
 
 ===============================================================================
 Also referenced by:
     * {% for ref in similar_references %}
-    * {% with similar_references.referenced_object as obj %} {% if
-      obj.get_absolute_url %}{{_obj_}}{% else %}{{ obj }}{% endif %} ({{_ref.id
-      }})  ref.id %}?redirect={% url "apis_bibsonomy:referencedetail"
-      reference.id %}">Delete
+    * {% with ref.referenced_object as obj %} {% if obj.get_absolute_url %}{
+      {_obj_}}{% else %}{{ obj }}{% endif %} ({{_ref.id_}})  ref.id
+      %}?redirect={% url "apis_bibsonomy:referencedetail" reference.id
+      %}">Delete
  {% endwith %}
 {% endfor %}
 {% endblock content %}
```

### Comparing `apis_bibsonomy-0.7.0/apis_bibsonomy/templatetags/bibsonomy_templatetags.py` & `apis_bibsonomy-0.7.1/apis_bibsonomy/templatetags/bibsonomy_templatetags.py`

 * *Files identical despite different names*

### Comparing `apis_bibsonomy-0.7.0/apis_bibsonomy/urls.py` & `apis_bibsonomy-0.7.1/apis_bibsonomy/urls.py`

 * *Files identical despite different names*

### Comparing `apis_bibsonomy-0.7.0/apis_bibsonomy/utils.py` & `apis_bibsonomy-0.7.1/apis_bibsonomy/utils.py`

 * *Files identical despite different names*

### Comparing `apis_bibsonomy-0.7.0/apis_bibsonomy/views.py` & `apis_bibsonomy-0.7.1/apis_bibsonomy/views.py`

 * *Files identical despite different names*

### Comparing `apis_bibsonomy-0.7.0/PKG-INFO` & `apis_bibsonomy-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apis-bibsonomy
-Version: 0.7.0
+Version: 0.7.1
 Summary: Bibsonomy/Zotero plugin for managing refernces in APIS framework
 License: MIT
 Author: Matthias Schlögl
 Author-email: m.schloegl@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
```

