# Comparing `tmp/django-sync-github-teams-0.0.0.tar.gz` & `tmp/django-sync-github-teams-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-sync-github-teams-0.0.0.tar", last modified: Fri Jun  9 20:49:50 2023, max compression
+gzip compressed data, was "django-sync-github-teams-0.1.1.tar", last modified: Fri Jun  9 21:57:39 2023, max compression
```

## Comparing `django-sync-github-teams-0.0.0.tar` & `django-sync-github-teams-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0       45 2023-06-06 00:11:02.569547 django-sync-github-teams-0.0.0/.gitignore
--rw-r--r--   0        0        0      384 2023-06-06 00:11:02.557547 django-sync-github-teams-0.0.0/.gitlab-ci.yml
--rw-r--r--   0        0        0      838 2023-06-06 16:21:14.663995 django-sync-github-teams-0.0.0/Dockerfile.ci-debian
--rw-r--r--   0        0        0      508 2023-06-06 16:21:18.023961 django-sync-github-teams-0.0.0/Dockerfile.ci-fedora
--rw-r--r--   0        0        0     1083 2023-06-06 00:11:32.713255 django-sync-github-teams-0.0.0/LICENSE
--rw-r--r--   0        0        0      115 2023-06-06 01:43:51.251283 django-sync-github-teams-0.0.0/Makefile
--rw-r--r--   0        0        0     2653 2023-06-09 20:41:38.873104 django-sync-github-teams-0.0.0/README.md
--rw-r--r--   0        0        0      157 2023-06-06 00:11:02.569547 django-sync-github-teams-0.0.0/debian/changelog
--rw-r--r--   0        0        0      754 2023-06-06 11:37:24.560521 django-sync-github-teams-0.0.0/debian/control
--rw-r--r--   0        0        0      100 2023-06-06 00:11:02.565547 django-sync-github-teams-0.0.0/debian/gbp.conf
--rwxr-xr-x   0        0        0      609 2023-06-06 00:11:02.565547 django-sync-github-teams-0.0.0/debian/rules
--rw-r--r--   0        0        0       12 2023-06-06 00:11:02.565547 django-sync-github-teams-0.0.0/debian/source/format
--rw-r--r--   0        0        0     1464 2023-06-06 13:36:30.340024 django-sync-github-teams-0.0.0/django-sync-github-teams.spec
--rw-r--r--   0        0        0       63 2023-06-06 00:38:49.792956 django-sync-github-teams-0.0.0/django_sync_github_teams/__init__.py
--rw-r--r--   0        0        0      371 2023-06-06 00:42:03.487012 django-sync-github-teams-0.0.0/django_sync_github_teams/apps.py
--rw-r--r--   0        0        0      402 2023-06-06 15:21:03.958397 django-sync-github-teams-0.0.0/django_sync_github_teams/management/commands/sync-github-teams.py
--rw-r--r--   0        0        0     1927 2023-06-06 01:31:47.809740 django-sync-github-teams-0.0.0/django_sync_github_teams/sync.py
--rw-r--r--   0        0        0       94 2023-06-06 00:36:02.694640 django-sync-github-teams-0.0.0/mypy.ini
--rw-r--r--   0        0        0      539 2023-06-06 16:19:31.553044 django-sync-github-teams-0.0.0/pyproject.toml
--rw-r--r--   0        0        0       63 2023-06-06 01:25:32.089438 django-sync-github-teams-0.0.0/pytest.ini
--rw-r--r--   0        0        0        0 2023-06-06 00:11:02.553547 django-sync-github-teams-0.0.0/test/__init__.py
--rw-r--r--   0        0        0      435 2023-06-06 01:16:52.630529 django-sync-github-teams-0.0.0/test/settings.py
--rw-r--r--   0        0        0     2648 2023-06-06 01:43:42.591359 django-sync-github-teams-0.0.0/test/test_django_sync_github_teams.py
--rw-r--r--   0        0        0     3049 1970-01-01 00:00:00.000000 django-sync-github-teams-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0       45 2023-06-09 21:57:37.780390 django-sync-github-teams-0.1.1/.gitignore
+-rw-r--r--   0        0        0      384 2023-06-09 21:57:37.780390 django-sync-github-teams-0.1.1/.gitlab-ci.yml
+-rw-r--r--   0        0        0      838 2023-06-09 21:57:37.780390 django-sync-github-teams-0.1.1/Dockerfile.ci-debian
+-rw-r--r--   0        0        0      508 2023-06-09 21:57:37.780390 django-sync-github-teams-0.1.1/Dockerfile.ci-fedora
+-rw-r--r--   0        0        0     1083 2023-06-09 21:57:37.780390 django-sync-github-teams-0.1.1/LICENSE
+-rw-r--r--   0        0        0      115 2023-06-09 21:57:37.780390 django-sync-github-teams-0.1.1/Makefile
+-rw-r--r--   0        0        0     2653 2023-06-09 21:57:37.780390 django-sync-github-teams-0.1.1/README.md
+-rw-r--r--   0        0        0      157 2023-06-09 21:57:37.780390 django-sync-github-teams-0.1.1/debian/changelog
+-rw-r--r--   0        0        0      754 2023-06-09 21:57:37.780390 django-sync-github-teams-0.1.1/debian/control
+-rw-r--r--   0        0        0      100 2023-06-09 21:57:37.780390 django-sync-github-teams-0.1.1/debian/gbp.conf
+-rwxr-xr-x   0        0        0      609 2023-06-09 21:57:37.780390 django-sync-github-teams-0.1.1/debian/rules
+-rw-r--r--   0        0        0       12 2023-06-09 21:57:37.780390 django-sync-github-teams-0.1.1/debian/source/format
+-rw-r--r--   0        0        0     1299 2023-06-09 21:57:37.781390 django-sync-github-teams-0.1.1/django-sync-github-teams.spec
+-rw-r--r--   0        0        0       63 2023-06-09 21:57:37.781390 django-sync-github-teams-0.1.1/django_sync_github_teams/__init__.py
+-rw-r--r--   0        0        0      371 2023-06-09 21:57:37.781390 django-sync-github-teams-0.1.1/django_sync_github_teams/apps.py
+-rw-r--r--   0        0        0      402 2023-06-09 21:57:37.781390 django-sync-github-teams-0.1.1/django_sync_github_teams/management/commands/sync-github-teams.py
+-rw-r--r--   0        0        0     1927 2023-06-09 21:57:37.781390 django-sync-github-teams-0.1.1/django_sync_github_teams/sync.py
+-rw-r--r--   0        0        0       94 2023-06-09 21:57:37.781390 django-sync-github-teams-0.1.1/mypy.ini
+-rw-r--r--   0        0        0      539 2023-06-09 21:57:37.781390 django-sync-github-teams-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       63 2023-06-09 21:57:37.781390 django-sync-github-teams-0.1.1/pytest.ini
+-rw-r--r--   0        0        0        0 2023-06-09 21:57:37.804390 django-sync-github-teams-0.1.1/test/__init__.py
+-rw-r--r--   0        0        0      435 2023-06-09 21:57:37.781390 django-sync-github-teams-0.1.1/test/settings.py
+-rw-r--r--   0        0        0     2648 2023-06-09 21:57:37.781390 django-sync-github-teams-0.1.1/test/test_django_sync_github_teams.py
+-rw-r--r--   0        0        0     3049 1970-01-01 00:00:00.000000 django-sync-github-teams-0.1.1/PKG-INFO
```

### Comparing `django-sync-github-teams-0.0.0/Dockerfile.ci-debian` & `django-sync-github-teams-0.1.1/Dockerfile.ci-debian`

 * *Files identical despite different names*

### Comparing `django-sync-github-teams-0.0.0/LICENSE` & `django-sync-github-teams-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-sync-github-teams-0.0.0/README.md` & `django-sync-github-teams-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `django-sync-github-teams-0.0.0/debian/control` & `django-sync-github-teams-0.1.1/debian/control`

 * *Files identical despite different names*

### Comparing `django-sync-github-teams-0.0.0/debian/rules` & `django-sync-github-teams-0.1.1/debian/rules`

 * *Files identical despite different names*

### Comparing `django-sync-github-teams-0.0.0/django-sync-github-teams.spec` & `django-sync-github-teams-0.1.1/django-sync-github-teams.spec`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Name:      django-sync-github-teams
-Version:   0.0.0
+Version:   0.1.1
 Release:   0%{?dist}
 Summary:   FIXME
 License:   FIXME
 URL:       FIXME
 Source0:   %{pypi_source}
 
 
@@ -31,34 +31,29 @@
 FIXME
 
 %prep
 %setup -q
 
 %build
 export FLIT_NO_NETWORK=1
-make run
 #make man
 #make bash_completion
 
 %check
 python3 -m pytest test/
 
 %install
 mkdir -p %{buildroot}/usr/share/%{name}/
-cp -r run %{dist} %{buildroot}/usr/share/%{name}/
-mkdir -p %{buildroot}/usr/bin
-ln -sf ../share/%{name}/run %{buildroot}/usr/bin/%{name}
 #mkdir -p %{buildroot}%{_mandir}/man1
 #install -m 644 %{name}.1 %{buildroot}%{_mandir}/man1/
 #mkdir -p %{buildroot}/usr/share/bash-completion/completions/
 #install -m 644 bash_completion/%{name} %{buildroot}/usr/share/bash-completion/completions/
 
 %files
 /usr/share/%{name}
-%{_bindir}/%{name}
 #%{_mandir}/man1/%{name}.1*
 #/usr/share/bash-completion/completions/%{name}
 
 %doc README.md
 %license LICENSE
 
 %changelog
```

### Comparing `django-sync-github-teams-0.0.0/django_sync_github_teams/sync.py` & `django-sync-github-teams-0.1.1/django_sync_github_teams/sync.py`

 * *Files identical despite different names*

### Comparing `django-sync-github-teams-0.0.0/pyproject.toml` & `django-sync-github-teams-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-sync-github-teams-0.0.0/test/test_django_sync_github_teams.py` & `django-sync-github-teams-0.1.1/test/test_django_sync_github_teams.py`

 * *Files identical despite different names*

### Comparing `django-sync-github-teams-0.0.0/PKG-INFO` & `django-sync-github-teams-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sync-github-teams
-Version: 0.0.0
+Version: 0.1.1
 Summary: django-sync-github-teams is ...
 Author-email: Antonio Terceiro <antonio.terceiro@linaro.org>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: django-allauth>=0.44
 Requires-Dist: Django>=3.2
 Project-URL: Home, https://gitlab.com/Linaro/django-sync-github-teams
```

