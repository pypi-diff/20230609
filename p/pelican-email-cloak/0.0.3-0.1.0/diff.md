# Comparing `tmp/pelican_email_cloak-0.0.3.tar.gz` & `tmp/pelican_email_cloak-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pelican_email_cloak-0.0.3.tar", max compression
+gzip compressed data, was "pelican_email_cloak-0.1.0.tar", max compression
```

## Comparing `pelican_email_cloak-0.0.3.tar` & `pelican_email_cloak-0.1.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1075 2023-06-08 13:02:48.379033 pelican_email_cloak-0.0.3/LICENSE
--rw-r--r--   0        0        0      826 2023-06-08 13:14:16.143047 pelican_email_cloak-0.0.3/README.md
--rw-r--r--   0        0        0       35 2023-06-08 11:14:20.652110 pelican_email_cloak-0.0.3/pelican/plugins/email_cloak/__init__.py
--rw-r--r--   0        0        0     1754 2023-06-08 12:30:17.060680 pelican_email_cloak-0.0.3/pelican/plugins/email_cloak/email_cloak.py
--rw-r--r--   0        0        0     2460 2023-06-08 13:13:45.474052 pelican_email_cloak-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2188 1970-01-01 00:00:00.000000 pelican_email_cloak-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-06-08 13:02:48.379033 pelican_email_cloak-0.1.0/LICENSE
+-rw-r--r--   0        0        0      826 2023-06-08 13:14:16.143047 pelican_email_cloak-0.1.0/README.md
+-rw-r--r--   0        0        0       35 2023-06-08 11:14:20.652110 pelican_email_cloak-0.1.0/pelican/plugins/email_cloak/__init__.py
+-rw-r--r--   0        0        0     2075 2023-06-09 12:53:31.768695 pelican_email_cloak-0.1.0/pelican/plugins/email_cloak/email_cloak.py
+-rw-r--r--   0        0        0     2472 2023-06-09 12:55:34.703029 pelican_email_cloak-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2200 1970-01-01 00:00:00.000000 pelican_email_cloak-0.1.0/PKG-INFO
```

### Comparing `pelican_email_cloak-0.0.3/LICENSE` & `pelican_email_cloak-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pelican_email_cloak-0.0.3/README.md` & `pelican_email_cloak-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pelican_email_cloak-0.0.3/pelican/plugins/email_cloak/email_cloak.py` & `pelican_email_cloak-0.1.0/pelican/plugins/email_cloak/email_cloak.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,14 +18,15 @@
       # Adds deobf.js to output root
       path = os.path.join(self.output_path, "deobf.js")
       with open(path, "w") as f:
         f.write(deobfuscator().replace('<script type="text/javascript">', "").replace("</script>", "").strip())
 
 def email_cloak(content: Page):
   all_emails = re.findall(EMAIL_REGEX, content._content)
+  all_emails = [email if not email.endswith(".") else email[:-1] for email in all_emails]
   all_javascriptified_emails = [javascriptify(email, do_scramble=True) for email in all_emails]
 
   # Replace all plaintext e-mails with obfuscated e-mails
   for email, javascriptified_email in zip(all_emails, all_javascriptified_emails):
       content._content = content._content.replace(email, javascriptified_email)
   
   # Add a script tag at the end of the page to deobfuscate the emails
@@ -34,14 +35,19 @@
       content._content += "<script type=\"text/javascript\" src=\"/deobf.js\"></script>"
   
   return content._content
 
 def _generator_write(generator, content: Page):
    email_cloak(content)
 
+def _generator_enrich_context(generator):
+    generator.context["javascriptify"] = javascriptify
+
 def get_generators(generators):
   return DeobfGenerator
 
 def register():
   signals.get_generators.connect(get_generators)
+  signals.page_generator_init.connect(_generator_enrich_context)
   signals.page_generator_write_page.connect(_generator_write)
+  signals.article_generator_init.connect(_generator_enrich_context)
   signals.article_generator_write_article.connect(_generator_write)
```

### Comparing `pelican_email_cloak-0.0.3/pyproject.toml` & `pelican_email_cloak-0.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "pelican-email-cloak"
-version = "0.0.3"
+version = "0.1.0"
 description = "E-mail cloaking plugin for Pelican"
 authors = ["Demetrio Battaglia <deme3.iot@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["pelican", "plugin"]
 repository = "https://github.com/deme3/pelican-email-cloak"
 documentation = "https://docs.getpelican.com"
 packages = [
     { include = "pelican" },
 ]
 
 classifiers = [
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Framework :: Pelican",
     "Framework :: Pelican :: Plugins",
     "Intended Audience :: End Users/Desktop",
     "Operating System :: OS Independent",
     "Topic :: Internet :: WWW/HTTP",
     "Topic :: Software Development :: Libraries :: Python Modules",
```

### Comparing `pelican_email_cloak-0.0.3/PKG-INFO` & `pelican_email_cloak-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: pelican-email-cloak
-Version: 0.0.3
+Version: 0.1.0
 Summary: E-mail cloaking plugin for Pelican
 Home-page: https://github.com/deme3/pelican-email-cloak
 License: MIT
 Keywords: pelican,plugin
 Author: Demetrio Battaglia
 Author-email: deme3.iot@gmail.com
 Requires-Python: >=3.8.1,<4.0
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Framework :: Pelican
 Classifier: Framework :: Pelican :: Plugins
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

