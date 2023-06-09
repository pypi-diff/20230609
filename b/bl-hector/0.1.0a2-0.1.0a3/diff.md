# Comparing `tmp/bl_hector-0.1.0a2.tar.gz` & `tmp/bl_hector-0.1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bl_hector-0.1.0a2.tar", max compression
+gzip compressed data, was "bl_hector-0.1.0a3.tar", max compression
```

## Comparing `bl_hector-0.1.0a2.tar` & `bl_hector-0.1.0a3.tar`

### file list

```diff
@@ -1,86 +1,88 @@
--rw-r--r--   0        0        0    34523 2023-05-31 09:45:12.827540 bl_hector-0.1.0a2/LICENSE
--rw-r--r--   0        0        0     1079 2023-06-07 16:14:27.658555 bl_hector-0.1.0a2/README.md
--rw-r--r--   0        0        0      807 2023-06-07 16:14:27.658555 bl_hector-0.1.0a2/bl_hector/__init__.py
--rw-r--r--   0        0        0      721 2023-06-07 16:14:27.658555 bl_hector-0.1.0a2/bl_hector/application/__init__.py
--rw-r--r--   0        0        0      721 2023-06-07 16:14:27.658555 bl_hector-0.1.0a2/bl_hector/application/use_cases/__init__.py
--rw-r--r--   0        0        0     2321 2023-06-07 16:14:27.658555 bl_hector-0.1.0a2/bl_hector/application/use_cases/add_book.py
--rw-r--r--   0        0        0     1985 2023-06-07 16:14:27.658555 bl_hector-0.1.0a2/bl_hector/application/use_cases/display_book.py
--rw-r--r--   0        0        0     3471 2023-06-07 16:14:27.658555 bl_hector-0.1.0a2/bl_hector/application/use_cases/import_books.py
--rw-r--r--   0        0        0     1829 2023-06-07 16:14:27.658555 bl_hector-0.1.0a2/bl_hector/application/use_cases/look_up_book.py
--rw-r--r--   0        0        0     2635 2023-06-07 16:14:27.658555 bl_hector-0.1.0a2/bl_hector/application/use_cases/search_books.py
--rw-r--r--   0        0        0     2396 2023-06-07 16:14:27.658555 bl_hector-0.1.0a2/bl_hector/application/use_cases/update_book.py
--rw-r--r--   0        0        0      944 2023-06-07 16:14:27.658555 bl_hector-0.1.0a2/bl_hector/configuration/__init__.py
--rw-r--r--   0        0        0      981 2023-06-07 16:14:27.658555 bl_hector-0.1.0a2/bl_hector/configuration/cli.py
--rw-r--r--   0        0        0      986 2023-06-07 16:14:27.658555 bl_hector-0.1.0a2/bl_hector/configuration/wsgi.py
--rw-r--r--   0        0        0      721 2023-06-07 16:14:27.658555 bl_hector-0.1.0a2/bl_hector/domain/__init__.py
--rw-r--r--   0        0        0      721 2023-06-07 16:14:27.658555 bl_hector-0.1.0a2/bl_hector/domain/administration/__init__.py
--rw-r--r--   0        0        0     1272 2023-06-07 16:14:27.658555 bl_hector-0.1.0a2/bl_hector/domain/administration/entities.py
--rw-r--r--   0        0        0     1452 2023-06-07 16:14:27.658555 bl_hector-0.1.0a2/bl_hector/domain/administration/repositories.py
--rw-r--r--   0        0        0     1196 2023-06-07 16:14:27.658555 bl_hector-0.1.0a2/bl_hector/domain/administration/services.py
--rw-r--r--   0        0        0      931 2023-06-07 16:14:27.658555 bl_hector-0.1.0a2/bl_hector/domain/administration/value_objects.py
--rw-r--r--   0        0        0      721 2023-06-07 16:14:27.658555 bl_hector-0.1.0a2/bl_hector/domain/collection_management/__init__.py
--rw-r--r--   0        0        0     1452 2023-06-07 16:14:27.658555 bl_hector-0.1.0a2/bl_hector/domain/collection_management/entities.py
--rw-r--r--   0        0        0      996 2023-06-07 16:14:27.658555 bl_hector-0.1.0a2/bl_hector/domain/collection_management/exceptions.py
--rw-r--r--   0        0        0     1509 2023-06-07 16:14:27.658555 bl_hector-0.1.0a2/bl_hector/domain/collection_management/repositories.py
--rw-r--r--   0        0        0      958 2023-06-07 16:14:27.658555 bl_hector-0.1.0a2/bl_hector/domain/collection_management/services.py
--rw-r--r--   0        0        0     3309 2023-06-07 16:14:27.658555 bl_hector-0.1.0a2/bl_hector/domain/collection_management/value_objects.py
--rw-r--r--   0        0        0      721 2023-06-07 16:14:27.658555 bl_hector-0.1.0a2/bl_hector/infrastructure/__init__.py
--rw-r--r--   0        0        0     2212 2023-06-07 16:14:27.658555 bl_hector-0.1.0a2/bl_hector/infrastructure/flask/__init__.py
--rw-r--r--   0        0        0     1064 2023-06-07 16:14:27.658555 bl_hector-0.1.0a2/bl_hector/infrastructure/flask/aliases/__init__.py
--rw-r--r--   0        0        0     3942 2023-06-07 16:14:27.658555 bl_hector-0.1.0a2/bl_hector/infrastructure/flask/books/__init__.py
--rw-r--r--   0        0        0     2899 2023-06-07 16:14:27.662555 bl_hector-0.1.0a2/bl_hector/infrastructure/flask/services.py
--rw-r--r--   0        0        0   207302 2023-06-07 16:14:27.662555 bl_hector-0.1.0a2/bl_hector/infrastructure/flask/static/css/bulma@0.9.4.min.css
--rw-r--r--   0        0        0    73117 2023-06-07 16:14:27.662555 bl_hector-0.1.0a2/bl_hector/infrastructure/flask/static/css/font-awesome@5.14.0.css
--rw-r--r--   0        0        0      482 2023-06-07 16:14:27.662555 bl_hector-0.1.0a2/bl_hector/infrastructure/flask/static/css/hector.css
--rw-r--r--   0        0        0      655 2023-06-07 16:14:27.662555 bl_hector-0.1.0a2/bl_hector/infrastructure/flask/static/favicon.svg
--rw-r--r--   0        0        0    35880 2023-06-07 16:14:27.662555 bl_hector-0.1.0a2/bl_hector/infrastructure/flask/static/img/placeholders/1280x960.png
--rw-r--r--   0        0        0      928 2023-06-07 16:14:27.662555 bl_hector-0.1.0a2/bl_hector/infrastructure/flask/static/img/placeholders/320x480.png
--rw-r--r--   0        0        0     3602 2023-06-07 16:14:27.662555 bl_hector-0.1.0a2/bl_hector/infrastructure/flask/static/img/placeholders/96x96.png
--rw-r--r--   0        0        0    42819 2023-06-07 16:14:27.670555 bl_hector-0.1.0a2/bl_hector/infrastructure/flask/static/js/htmx@1.9.2.min.js
--rw-r--r--   0        0        0    97249 2023-06-07 16:14:27.670555 bl_hector-0.1.0a2/bl_hector/infrastructure/flask/static/js/hyperscript@0.9.8.min.js
--rw-r--r--   0        0        0     6828 2023-06-07 16:14:27.670555 bl_hector-0.1.0a2/bl_hector/infrastructure/flask/static/js/simplewebauthn-browser@7.2.0.umd.min.js
--rw-r--r--   0        0        0   186112 2023-06-07 16:14:27.670555 bl_hector-0.1.0a2/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.ttf
--rw-r--r--   0        0        0   107460 2023-06-07 16:14:27.674555 bl_hector-0.1.0a2/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.woff2
--rw-r--r--   0        0        0    62048 2023-06-07 16:14:27.674555 bl_hector-0.1.0a2/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.ttf
--rw-r--r--   0        0        0    25096 2023-06-07 16:14:27.674555 bl_hector-0.1.0a2/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.woff2
--rw-r--r--   0        0        0   397728 2023-06-07 16:14:27.674555 bl_hector-0.1.0a2/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.ttf
--rw-r--r--   0        0        0   150472 2023-06-07 16:14:27.674555 bl_hector-0.1.0a2/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.woff2
--rw-r--r--   0        0        0     1802 2023-06-07 16:14:27.674555 bl_hector-0.1.0a2/bl_hector/infrastructure/flask/utils.py
--rw-r--r--   0        0        0     4421 2023-06-07 16:14:27.674555 bl_hector-0.1.0a2/bl_hector/infrastructure/flask/webauthn/__init__.py
--rw-r--r--   0        0        0     3119 2023-06-07 16:14:27.674555 bl_hector-0.1.0a2/bl_hector/infrastructure/flask/webauthn/security.py
--rw-r--r--   0        0        0     1641 2023-06-07 16:14:27.674555 bl_hector-0.1.0a2/bl_hector/infrastructure/isbnlib/__init__.py
--rw-r--r--   0        0        0     1639 2023-06-07 16:14:27.674555 bl_hector-0.1.0a2/bl_hector/infrastructure/settings.py
--rw-r--r--   0        0        0      721 2023-06-07 16:14:27.674555 bl_hector-0.1.0a2/bl_hector/infrastructure/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     7982 2023-06-07 16:14:27.674555 bl_hector-0.1.0a2/bl_hector/infrastructure/sqlalchemy/repositories.py
--rw-r--r--   0        0        0     2058 2023-06-07 16:14:27.674555 bl_hector-0.1.0a2/bl_hector/infrastructure/typer/__init__.py
--rw-r--r--   0        0        0     2718 2023-06-07 16:14:27.682555 bl_hector-0.1.0a2/bl_hector/infrastructure/typer/books.py
--rw-r--r--   0        0        0     1866 2023-06-07 16:14:27.682555 bl_hector-0.1.0a2/bl_hector/infrastructure/typer/services.py
--rw-r--r--   0        0        0      810 2023-06-07 16:14:27.682555 bl_hector-0.1.0a2/bl_hector/interfaces/__init__.py
--rw-r--r--   0        0        0     3454 2023-06-07 16:14:27.682555 bl_hector-0.1.0a2/bl_hector/interfaces/from_dict.py
--rw-r--r--   0        0        0     1517 2023-06-07 16:14:27.682555 bl_hector-0.1.0a2/bl_hector/interfaces/from_json.py
--rw-r--r--   0        0        0     1497 2023-06-07 16:14:27.682555 bl_hector-0.1.0a2/bl_hector/interfaces/l10n/__init__.py
--rw-r--r--   0        0        0     3791 2023-06-07 16:14:27.682555 bl_hector-0.1.0a2/bl_hector/interfaces/l10n/en-GB/main.ftl
--rw-r--r--   0        0        0     4284 2023-06-07 16:14:27.682555 bl_hector-0.1.0a2/bl_hector/interfaces/l10n/fr-FR/main.ftl
--rw-r--r--   0        0        0     1407 2023-06-07 16:14:27.682555 bl_hector-0.1.0a2/bl_hector/interfaces/to_http/__init__.py
--rw-r--r--   0        0        0    13595 2023-06-07 16:14:27.682555 bl_hector-0.1.0a2/bl_hector/interfaces/to_http/as_html/__init__.py
--rw-r--r--   0        0        0     3951 2023-06-07 16:14:27.682555 bl_hector-0.1.0a2/bl_hector/interfaces/to_http/as_html/templates/books/add.pug
--rw-r--r--   0        0        0     2006 2023-06-07 16:14:27.682555 bl_hector-0.1.0a2/bl_hector/interfaces/to_http/as_html/templates/books/display.pug
--rw-r--r--   0        0        0     1612 2023-06-07 16:14:27.682555 bl_hector-0.1.0a2/bl_hector/interfaces/to_http/as_html/templates/books/mixins/render_isbn.pug
--rw-r--r--   0        0        0     4925 2023-06-07 16:14:27.682555 bl_hector-0.1.0a2/bl_hector/interfaces/to_http/as_html/templates/books/search.pug
--rw-r--r--   0        0        0     3265 2023-06-07 16:14:27.682555 bl_hector-0.1.0a2/bl_hector/interfaces/to_http/as_html/templates/books/update.pug
--rw-r--r--   0        0        0      978 2023-06-07 16:14:27.682555 bl_hector-0.1.0a2/bl_hector/interfaces/to_http/as_html/templates/error.pug
--rw-r--r--   0        0        0     2062 2023-06-07 16:14:27.682555 bl_hector-0.1.0a2/bl_hector/interfaces/to_http/as_html/templates/layout.pug
--rw-r--r--   0        0        0     1122 2023-06-07 16:14:27.682555 bl_hector-0.1.0a2/bl_hector/interfaces/to_http/as_html/templates/mixins/flash.pug
--rw-r--r--   0        0        0     3812 2023-06-07 16:14:27.682555 bl_hector-0.1.0a2/bl_hector/interfaces/to_http/as_html/templates/mixins/form.pug
--rw-r--r--   0        0        0     2018 2023-06-07 16:14:27.682555 bl_hector-0.1.0a2/bl_hector/interfaces/to_http/as_html/templates/mixins/navbar.pug
--rw-r--r--   0        0        0     2010 2023-06-07 16:14:27.682555 bl_hector-0.1.0a2/bl_hector/interfaces/to_http/as_html/templates/webauthn/login.pug
--rw-r--r--   0        0        0     2045 2023-06-07 16:14:27.682555 bl_hector-0.1.0a2/bl_hector/interfaces/to_http/as_html/templates/webauthn/register.pug
--rw-r--r--   0        0        0     1310 2023-06-07 16:14:27.682555 bl_hector-0.1.0a2/bl_hector/interfaces/to_http/as_json/__init__.py
--rw-r--r--   0        0        0     1211 2023-06-07 16:14:27.682555 bl_hector-0.1.0a2/bl_hector/interfaces/to_terminal/__init__.py
--rw-r--r--   0        0        0     1816 2023-06-07 16:14:27.682555 bl_hector-0.1.0a2/bl_hector/interfaces/to_terminal/as_json.py
--rw-r--r--   0        0        0     4256 2023-06-07 16:14:27.682555 bl_hector-0.1.0a2/bl_hector/interfaces/to_terminal/as_text.py
--rw-r--r--   0        0        0     1519 2023-06-07 16:14:27.682555 bl_hector-0.1.0a2/bl_hector/interfaces/utils.py
--rw-r--r--   0        0        0     5154 2023-06-07 16:14:27.682555 bl_hector-0.1.0a2/bl_hector/interfaces/validators.py
--rw-r--r--   0        0        0     1332 2023-06-07 16:15:43.365625 bl_hector-0.1.0a2/pyproject.toml
--rw-r--r--   0        0        0     3460 2023-06-07 16:17:54.268783 bl_hector-0.1.0a2/setup.py
--rw-r--r--   0        0        0     1985 2023-06-07 16:17:54.269611 bl_hector-0.1.0a2/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-05-31 09:45:12.827540 bl_hector-0.1.0a3/LICENSE
+-rw-r--r--   0        0        0     1264 2023-06-09 06:16:19.346310 bl_hector-0.1.0a3/README.md
+-rw-r--r--   0        0        0      807 2023-06-07 16:14:27.658555 bl_hector-0.1.0a3/bl_hector/__init__.py
+-rw-r--r--   0        0        0      721 2023-06-07 16:14:27.658555 bl_hector-0.1.0a3/bl_hector/application/__init__.py
+-rw-r--r--   0        0        0      721 2023-06-07 16:14:27.658555 bl_hector-0.1.0a3/bl_hector/application/use_cases/__init__.py
+-rw-r--r--   0        0        0     2378 2023-06-09 06:16:19.346310 bl_hector-0.1.0a3/bl_hector/application/use_cases/add_book.py
+-rw-r--r--   0        0        0     1981 2023-06-09 06:16:19.350310 bl_hector-0.1.0a3/bl_hector/application/use_cases/display_book.py
+-rw-r--r--   0        0        0     3472 2023-06-09 06:16:19.350310 bl_hector-0.1.0a3/bl_hector/application/use_cases/import_books.py
+-rw-r--r--   0        0        0     1846 2023-06-09 06:16:19.350310 bl_hector-0.1.0a3/bl_hector/application/use_cases/look_up_book.py
+-rw-r--r--   0        0        0     2690 2023-06-09 06:16:19.350310 bl_hector-0.1.0a3/bl_hector/application/use_cases/search_books.py
+-rw-r--r--   0        0        0     2442 2023-06-09 06:16:19.350310 bl_hector-0.1.0a3/bl_hector/application/use_cases/update_book.py
+-rw-r--r--   0        0        0      944 2023-06-07 16:14:27.658555 bl_hector-0.1.0a3/bl_hector/configuration/__init__.py
+-rw-r--r--   0        0        0      981 2023-06-07 16:14:27.658555 bl_hector-0.1.0a3/bl_hector/configuration/cli.py
+-rw-r--r--   0        0        0      986 2023-06-07 16:14:27.658555 bl_hector-0.1.0a3/bl_hector/configuration/wsgi.py
+-rw-r--r--   0        0        0      721 2023-06-07 16:14:27.658555 bl_hector-0.1.0a3/bl_hector/domain/__init__.py
+-rw-r--r--   0        0        0      721 2023-06-07 16:14:27.658555 bl_hector-0.1.0a3/bl_hector/domain/administration/__init__.py
+-rw-r--r--   0        0        0     1272 2023-06-07 16:14:27.658555 bl_hector-0.1.0a3/bl_hector/domain/administration/entities.py
+-rw-r--r--   0        0        0     1452 2023-06-07 16:14:27.658555 bl_hector-0.1.0a3/bl_hector/domain/administration/repositories.py
+-rw-r--r--   0        0        0     1196 2023-06-07 16:14:27.658555 bl_hector-0.1.0a3/bl_hector/domain/administration/services.py
+-rw-r--r--   0        0        0      931 2023-06-07 16:14:27.658555 bl_hector-0.1.0a3/bl_hector/domain/administration/value_objects.py
+-rw-r--r--   0        0        0      721 2023-06-07 16:14:27.658555 bl_hector-0.1.0a3/bl_hector/domain/collection_management/__init__.py
+-rw-r--r--   0        0        0     1449 2023-06-09 06:16:19.350310 bl_hector-0.1.0a3/bl_hector/domain/collection_management/entities.py
+-rw-r--r--   0        0        0      996 2023-06-07 16:14:27.658555 bl_hector-0.1.0a3/bl_hector/domain/collection_management/exceptions.py
+-rw-r--r--   0        0        0     1509 2023-06-07 16:14:27.658555 bl_hector-0.1.0a3/bl_hector/domain/collection_management/repositories.py
+-rw-r--r--   0        0        0      958 2023-06-07 16:14:27.658555 bl_hector-0.1.0a3/bl_hector/domain/collection_management/services.py
+-rw-r--r--   0        0        0     3309 2023-06-07 16:14:27.658555 bl_hector-0.1.0a3/bl_hector/domain/collection_management/value_objects.py
+-rw-r--r--   0        0        0      721 2023-06-07 16:14:27.658555 bl_hector-0.1.0a3/bl_hector/infrastructure/__init__.py
+-rw-r--r--   0        0        0     2553 2023-06-09 06:16:19.354310 bl_hector-0.1.0a3/bl_hector/infrastructure/flask/__init__.py
+-rw-r--r--   0        0        0     1064 2023-06-07 16:14:27.658555 bl_hector-0.1.0a3/bl_hector/infrastructure/flask/aliases/__init__.py
+-rw-r--r--   0        0        0     1733 2023-06-09 06:16:19.354310 bl_hector-0.1.0a3/bl_hector/infrastructure/flask/auth/__init__.py
+-rw-r--r--   0        0        0     3942 2023-06-07 16:14:27.658555 bl_hector-0.1.0a3/bl_hector/infrastructure/flask/books/__init__.py
+-rw-r--r--   0        0        0     2899 2023-06-07 16:14:27.662555 bl_hector-0.1.0a3/bl_hector/infrastructure/flask/services.py
+-rw-r--r--   0        0        0   207302 2023-06-07 16:14:27.662555 bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/css/bulma@0.9.4.min.css
+-rw-r--r--   0        0        0    73117 2023-06-07 16:14:27.662555 bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/css/font-awesome@5.14.0.css
+-rw-r--r--   0        0        0      482 2023-06-07 16:14:27.662555 bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/css/hector.css
+-rw-r--r--   0        0        0      655 2023-06-07 16:14:27.662555 bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/favicon.svg
+-rw-r--r--   0        0        0    35880 2023-06-07 16:14:27.662555 bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/img/placeholders/1280x960.png
+-rw-r--r--   0        0        0      928 2023-06-07 16:14:27.662555 bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/img/placeholders/320x480.png
+-rw-r--r--   0        0        0     3602 2023-06-07 16:14:27.662555 bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/img/placeholders/96x96.png
+-rw-r--r--   0        0        0    42819 2023-06-07 16:14:27.670555 bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/js/htmx@1.9.2.min.js
+-rw-r--r--   0        0        0    97249 2023-06-07 16:14:27.670555 bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/js/hyperscript@0.9.8.min.js
+-rw-r--r--   0        0        0     6828 2023-06-07 16:14:27.670555 bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/js/simplewebauthn-browser@7.2.0.umd.min.js
+-rw-r--r--   0        0        0   186112 2023-06-07 16:14:27.670555 bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.ttf
+-rw-r--r--   0        0        0   107460 2023-06-07 16:14:27.674555 bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.woff2
+-rw-r--r--   0        0        0    62048 2023-06-07 16:14:27.674555 bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.ttf
+-rw-r--r--   0        0        0    25096 2023-06-07 16:14:27.674555 bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.woff2
+-rw-r--r--   0        0        0   397728 2023-06-07 16:14:27.674555 bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.ttf
+-rw-r--r--   0        0        0   150472 2023-06-07 16:14:27.674555 bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.woff2
+-rw-r--r--   0        0        0     1802 2023-06-07 16:14:27.674555 bl_hector-0.1.0a3/bl_hector/infrastructure/flask/utils.py
+-rw-r--r--   0        0        0     4400 2023-06-09 06:16:19.354310 bl_hector-0.1.0a3/bl_hector/infrastructure/flask/webauthn/__init__.py
+-rw-r--r--   0        0        0     3119 2023-06-07 16:14:27.674555 bl_hector-0.1.0a3/bl_hector/infrastructure/flask/webauthn/security.py
+-rw-r--r--   0        0        0     1641 2023-06-07 16:14:27.674555 bl_hector-0.1.0a3/bl_hector/infrastructure/isbnlib/__init__.py
+-rw-r--r--   0        0        0     1775 2023-06-09 06:16:19.354310 bl_hector-0.1.0a3/bl_hector/infrastructure/settings.py
+-rw-r--r--   0        0        0      721 2023-06-07 16:14:27.674555 bl_hector-0.1.0a3/bl_hector/infrastructure/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     7982 2023-06-07 16:14:27.674555 bl_hector-0.1.0a3/bl_hector/infrastructure/sqlalchemy/repositories.py
+-rw-r--r--   0        0        0     2058 2023-06-07 16:14:27.674555 bl_hector-0.1.0a3/bl_hector/infrastructure/typer/__init__.py
+-rw-r--r--   0        0        0     2718 2023-06-07 16:14:27.682555 bl_hector-0.1.0a3/bl_hector/infrastructure/typer/books.py
+-rw-r--r--   0        0        0     1866 2023-06-07 16:14:27.682555 bl_hector-0.1.0a3/bl_hector/infrastructure/typer/services.py
+-rw-r--r--   0        0        0      810 2023-06-07 16:14:27.682555 bl_hector-0.1.0a3/bl_hector/interfaces/__init__.py
+-rw-r--r--   0        0        0     3454 2023-06-07 16:14:27.682555 bl_hector-0.1.0a3/bl_hector/interfaces/from_dict.py
+-rw-r--r--   0        0        0     1517 2023-06-07 16:14:27.682555 bl_hector-0.1.0a3/bl_hector/interfaces/from_json.py
+-rw-r--r--   0        0        0     1435 2023-06-07 17:00:49.589157 bl_hector-0.1.0a3/bl_hector/interfaces/l10n/__init__.py
+-rw-r--r--   0        0        0     3901 2023-06-09 06:16:19.354310 bl_hector-0.1.0a3/bl_hector/interfaces/l10n/en-GB/main.ftl
+-rw-r--r--   0        0        0     4397 2023-06-09 06:16:19.354310 bl_hector-0.1.0a3/bl_hector/interfaces/l10n/fr-FR/main.ftl
+-rw-r--r--   0        0        0     1407 2023-06-07 16:14:27.682555 bl_hector-0.1.0a3/bl_hector/interfaces/to_http/__init__.py
+-rw-r--r--   0        0        0    13523 2023-06-09 06:16:19.358310 bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_html/__init__.py
+-rw-r--r--   0        0        0     1254 2023-06-09 06:16:19.358310 bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_html/templates/auth/login.pug
+-rw-r--r--   0        0        0     3951 2023-06-07 16:14:27.682555 bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_html/templates/books/add.pug
+-rw-r--r--   0        0        0     2001 2023-06-07 16:57:40.623777 bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_html/templates/books/display.pug
+-rw-r--r--   0        0        0     1612 2023-06-07 16:14:27.682555 bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_html/templates/books/mixins/render_isbn.pug
+-rw-r--r--   0        0        0     4925 2023-06-07 16:14:27.682555 bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_html/templates/books/search.pug
+-rw-r--r--   0        0        0     3255 2023-06-07 16:58:07.111390 bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_html/templates/books/update.pug
+-rw-r--r--   0        0        0      978 2023-06-07 16:14:27.682555 bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_html/templates/error.pug
+-rw-r--r--   0        0        0     2043 2023-06-07 16:57:22.668045 bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_html/templates/layout.pug
+-rw-r--r--   0        0        0     1122 2023-06-07 16:14:27.682555 bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_html/templates/mixins/flash.pug
+-rw-r--r--   0        0        0     3812 2023-06-07 16:14:27.682555 bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_html/templates/mixins/form.pug
+-rw-r--r--   0        0        0     2010 2023-06-09 06:16:19.358310 bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_html/templates/mixins/navbar.pug
+-rw-r--r--   0        0        0     2010 2023-06-07 16:14:27.682555 bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_html/templates/webauthn/login.pug
+-rw-r--r--   0        0        0     2045 2023-06-07 16:14:27.682555 bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_html/templates/webauthn/register.pug
+-rw-r--r--   0        0        0     1310 2023-06-07 16:14:27.682555 bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_json/__init__.py
+-rw-r--r--   0        0        0     1211 2023-06-07 16:14:27.682555 bl_hector-0.1.0a3/bl_hector/interfaces/to_terminal/__init__.py
+-rw-r--r--   0        0        0     1818 2023-06-09 06:16:19.358310 bl_hector-0.1.0a3/bl_hector/interfaces/to_terminal/as_json.py
+-rw-r--r--   0        0        0     4250 2023-06-09 06:16:19.358310 bl_hector-0.1.0a3/bl_hector/interfaces/to_terminal/as_text.py
+-rw-r--r--   0        0        0     1519 2023-06-07 16:14:27.682555 bl_hector-0.1.0a3/bl_hector/interfaces/utils.py
+-rw-r--r--   0        0        0     5187 2023-06-09 06:16:19.362310 bl_hector-0.1.0a3/bl_hector/interfaces/validators.py
+-rw-r--r--   0        0        0     1407 2023-06-09 06:18:32.252717 bl_hector-0.1.0a3/pyproject.toml
+-rw-r--r--   0        0        0     3829 2023-06-09 06:19:45.006316 bl_hector-0.1.0a3/setup.py
+-rw-r--r--   0        0        0     2216 2023-06-09 06:19:45.007271 bl_hector-0.1.0a3/PKG-INFO
```

### Comparing `bl_hector-0.1.0a2/LICENSE` & `bl_hector-0.1.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/README.md` & `bl_hector-0.1.0a3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -21,14 +21,24 @@
 
 Additional Python database drivers might be required depending on the DSN.
 
 See [the `settings` module](bl_hector/infrastructure/settings.py) for
 a comprehensive list of configuration variables.
 
 
+## Authentication
+
+To enable WebAuthn authentication, you must install extra dependencies (`bl-hector[webauthn]`)
+and enable it explicitly:
+
+```console
+$ export HECTOR_WEBAUTHN=1
+```
+
+
 ## Initialise
 
 Once configured, you must initialise Hector's database with the dedicated command:
 
 ```console
 $ hector init-db
 ```
```

### Comparing `bl_hector-0.1.0a2/bl_hector/__init__.py` & `bl_hector-0.1.0a3/bl_hector/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/bl_hector/application/__init__.py` & `bl_hector-0.1.0a3/bl_hector/application/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/bl_hector/application/use_cases/__init__.py` & `bl_hector-0.1.0a3/bl_hector/application/use_cases/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/bl_hector/application/use_cases/add_book.py` & `bl_hector-0.1.0a3/bl_hector/application/use_cases/add_book.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,21 +13,28 @@
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 
-from bl_hector.domain.collection_management import entities as e
-from bl_hector.domain.collection_management import exceptions as ex
-from bl_hector.domain.collection_management import repositories as r
-from bl_hector.domain.collection_management import value_objects as vo
+from bl_hector.domain.collection_management.entities import Book
+from bl_hector.domain.collection_management.exceptions import IncorrectValue
+from bl_hector.domain.collection_management.repositories import Books
+from bl_hector.domain.collection_management.value_objects import (
+    Author,
+    Cover,
+    Genre,
+    Isbn,
+    Title,
+    Year,
+)
 
 
-@dataclass
+@dataclass(frozen=True)
 class Request:
     isbn: str
     title: str
     year: int
     authors: list[str]
     genres: list[str]
     cover: str = ""
@@ -35,38 +42,38 @@
 
 class Presenter(ABC):
     @abstractmethod
     def bad_request(self) -> None:
         ...
 
     @abstractmethod
-    def book_already_exists(self, book: e.Book) -> None:
+    def book_already_exists(self, book: Book) -> None:
         ...
 
     @abstractmethod
-    def book_added(self, book: e.Book) -> None:
+    def book_added(self, book: Book) -> None:
         ...
 
 
 @dataclass(frozen=True)
 class Interactor:
     presenter: Presenter
-    books: r.Books
+    books: Books
 
     def execute(self, request: Request) -> None:
         try:
-            book = e.Book.instanciate(
-                vo.Isbn.instanciate(request.isbn),
-                vo.Title.instanciate(request.title),
-                vo.Year.instanciate(request.year),
-                [vo.Author.instanciate(a) for a in request.authors if a],
-                [vo.Genre.instanciate(g) for g in request.genres if g],
-                vo.Cover.instanciate(request.cover) if request.cover else None,
+            book = Book.instanciate(
+                Isbn.instanciate(request.isbn),
+                Title.instanciate(request.title),
+                Year.instanciate(request.year),
+                [Author.instanciate(a) for a in request.authors if a],
+                [Genre.instanciate(g) for g in request.genres if g],
+                Cover.instanciate(request.cover) if request.cover else None,
             )
-        except ex.IncorrectValue:
+        except IncorrectValue:
             return self.presenter.bad_request()
 
         if books := self.books.search(isbn=book.isbn):
             return self.presenter.book_already_exists(books[0])
 
         self.books.add(book)
         self.presenter.book_added(book)
```

### Comparing `bl_hector-0.1.0a2/bl_hector/application/use_cases/display_book.py` & `bl_hector-0.1.0a3/bl_hector/application/use_cases/display_book.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,54 +13,54 @@
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 
-from bl_hector.domain.collection_management import entities as e
-from bl_hector.domain.collection_management import exceptions as ex
-from bl_hector.domain.collection_management import repositories as r
-from bl_hector.domain.collection_management import value_objects as vo
+from bl_hector.domain.collection_management.entities import Book
+from bl_hector.domain.collection_management.exceptions import IncorrectValue
+from bl_hector.domain.collection_management.repositories import Books
+from bl_hector.domain.collection_management.value_objects import Isbn
 
 
-@dataclass
+@dataclass(frozen=True)
 class Request:
     isbn: str
 
 
 class Presenter(ABC):
     @abstractmethod
     def not_an_isbn(self, isbn: str) -> None:
         ...
 
     @abstractmethod
-    def book_does_not_exist(self, isbn: vo.Isbn) -> None:
+    def book_not_found(self, isbn: Isbn) -> None:
         ...
 
     @abstractmethod
-    def see_other(self, isbn: vo.Isbn) -> None:
+    def see_other(self, isbn: Isbn) -> None:
         ...
 
     @abstractmethod
-    def book(self, book: e.Book) -> None:
+    def book(self, book: Book) -> None:
         ...
 
 
 @dataclass(frozen=True)
 class Interactor:
     presenter: Presenter
-    books: r.Books
+    books: Books
 
     def execute(self, request: Request) -> None:
         try:
-            isbn = vo.Isbn.instanciate(request.isbn)
-        except ex.IncorrectValue:
+            isbn = Isbn.instanciate(request.isbn)
+        except IncorrectValue:
             return self.presenter.not_an_isbn(request.isbn)
 
         if str(isbn) != request.isbn:
             return self.presenter.see_other(isbn)
 
         if book := self.books.by_isbn(isbn):
             return self.presenter.book(book)
 
-        self.presenter.book_does_not_exist(isbn)
+        self.presenter.book_not_found(isbn)
```

### Comparing `bl_hector-0.1.0a2/bl_hector/application/use_cases/import_books.py` & `bl_hector-0.1.0a3/bl_hector/application/use_cases/import_books.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,44 +15,44 @@
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Optional
 
-from bl_hector.domain.collection_management import entities as e
-from bl_hector.domain.collection_management import repositories as r
-from bl_hector.domain.collection_management import services as s
-from bl_hector.domain.collection_management import value_objects as vo
+from bl_hector.domain.collection_management.entities import Book
+from bl_hector.domain.collection_management.repositories import Books
+from bl_hector.domain.collection_management.services import InfoProvider
+from bl_hector.domain.collection_management.value_objects import Isbn
 
 
-@dataclass
+@dataclass(frozen=True)
 class Request:
     path: str
 
 
 class Presenter(ABC):
     @abstractmethod
     def file_does_not_exist(self, path: str) -> None:
         ...
 
     @abstractmethod
     def line_skipped(self, line_number: int, text: str, reason: str) -> None:
         ...
 
     @abstractmethod
-    def book_already_exists(self, book: e.Book) -> None:
+    def book_already_exists(self, book: Book) -> None:
         ...
 
     @abstractmethod
-    def book_info_not_found(self, isbn: vo.Isbn) -> None:
+    def book_info_not_found(self, isbn: Isbn) -> None:
         ...
 
     @abstractmethod
-    def book_added(self, book: e.Book) -> None:
+    def book_added(self, book: Book) -> None:
         ...
 
 
 @dataclass(frozen=True)
 class Interactor:
     """
     **WARNING:** This use case is not specified, for it is not trivial!
@@ -60,16 +60,16 @@
     It might be better to implement it by wireing the other commands together.
     This would solve the problem of the commit of the data. For the time being
     the commit only happens once at the end of the command, even if thousands of books
     have to be imported!?
     """
 
     presenter: Presenter
-    info_provider: s.InfoProvider
-    books: r.Books
+    info_provider: InfoProvider
+    books: Books
 
     def execute(self, request: Request) -> None:
         path = Path(request.path)
         if not path.is_file():
             return self.presenter.file_does_not_exist(request.path)
 
         for isbn in self.__extract_isbn_from_file(path):
@@ -78,25 +78,25 @@
                 continue
             if not (book := self.info_provider.look_up(isbn)):
                 self.presenter.book_info_not_found(isbn)
                 continue
             self.books.add(book)
             self.presenter.book_added(book)
 
-    def __extract_isbn_from_file(self, path: Path) -> list[vo.Isbn]:
+    def __extract_isbn_from_file(self, path: Path) -> list[Isbn]:
         return [
             isbn
             for number, text in enumerate(path.read_text().splitlines())
             if (isbn := self.__extract_isbn_from_line(number, text))
         ]
 
-    def __extract_isbn_from_line(self, number: int, text: str) -> Optional[vo.Isbn]:
+    def __extract_isbn_from_line(self, number: int, text: str) -> Optional[Isbn]:
         _text = text.strip()
         if "#" in _text:
             if _text.startswith("#"):
                 return None
             _text = text.split("#", 1)[0]
 
         try:
-            return vo.Isbn.instanciate(_text)
+            return Isbn.instanciate(_text)
         except Exception as exc:
             return self.presenter.line_skipped(number, text, str(exc))
```

### Comparing `bl_hector-0.1.0a2/bl_hector/application/use_cases/look_up_book.py` & `bl_hector-0.1.0a3/bl_hector/application/use_cases/look_up_book.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,26 +19,26 @@
 
 from bl_hector.domain.collection_management.entities import Book
 from bl_hector.domain.collection_management.exceptions import IncorrectValue
 from bl_hector.domain.collection_management.services import InfoProvider
 from bl_hector.domain.collection_management.value_objects import Isbn
 
 
-@dataclass
+@dataclass(frozen=True)
 class Request:
     isbn: str
 
 
 class Presenter(ABC):
     @abstractmethod
     def not_an_isbn(self, isbn: str) -> None:
         ...
 
     @abstractmethod
-    def unknown_isbn(self, isbn: Isbn) -> None:
+    def book_not_found(self, isbn: Isbn) -> None:
         ...
 
     @abstractmethod
     def book(self, book: Book) -> None:
         ...
 
 
@@ -51,8 +51,8 @@
         try:
             isbn = Isbn.instanciate(request.isbn)
         except IncorrectValue:
             return self.presenter.not_an_isbn(request.isbn)
 
         if book := self.info_provider.look_up(isbn):
             return self.presenter.book(book)
-        return self.presenter.unknown_isbn(isbn)
+        return self.presenter.book_not_found(isbn)
```

### Comparing `bl_hector-0.1.0a2/bl_hector/application/use_cases/search_books.py` & `bl_hector-0.1.0a3/bl_hector/application/use_cases/search_books.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,21 +14,27 @@
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from typing import Optional
 
-from bl_hector.domain.collection_management import entities as e
-from bl_hector.domain.collection_management import exceptions as x
-from bl_hector.domain.collection_management import repositories as r
-from bl_hector.domain.collection_management import value_objects as vo
+from bl_hector.domain.collection_management.entities import Book
+from bl_hector.domain.collection_management.exceptions import IncorrectValue
+from bl_hector.domain.collection_management.repositories import Books
+from bl_hector.domain.collection_management.value_objects import (
+    Author,
+    Genre,
+    Isbn,
+    Title,
+    Year,
+)
 
 
-@dataclass
+@dataclass(frozen=True)
 class Request:
     isbn: Optional[str] = None
     title: Optional[str] = None
     year: Optional[int] = None
     author: Optional[str] = None
     genre: Optional[str] = None
     page_number: Optional[int] = None
@@ -37,42 +43,42 @@
 
 class Presenter(ABC):
     @abstractmethod
     def bad_request(self) -> None:
         ...
 
     @abstractmethod
-    def book(self, book: e.Book) -> None:
+    def book(self, book: Book) -> None:
         ...
 
 
 @dataclass(frozen=True)
 class Interactor:
     presenter: Presenter
-    books: r.Books
+    books: Books
 
     def execute(self, request: Request) -> None:
         isbn = None
         title = None
         year = None
         author = None
         genre = None
 
         try:
             if request.isbn:
-                isbn = vo.Isbn.instanciate(request.isbn)
+                isbn = Isbn.instanciate(request.isbn)
             if request.title:
-                title = vo.Title.instanciate(request.title)
+                title = Title.instanciate(request.title)
             if request.year is not None:
-                year = vo.Year.instanciate(request.year)
+                year = Year.instanciate(request.year)
             if request.author:
-                author = vo.Author.instanciate(request.author)
+                author = Author.instanciate(request.author)
             if request.genre:
-                genre = vo.Genre.instanciate(request.genre)
-        except x.IncorrectValue:
+                genre = Genre.instanciate(request.genre)
+        except IncorrectValue:
             return self.presenter.bad_request()
 
         books = self.books.search(
             isbn=isbn,
             title=title,
             year=year,
             author=author,
```

### Comparing `bl_hector-0.1.0a2/bl_hector/application/use_cases/update_book.py` & `bl_hector-0.1.0a3/bl_hector/application/use_cases/update_book.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,21 +13,28 @@
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 
-from bl_hector.domain.collection_management import entities as e
-from bl_hector.domain.collection_management import exceptions as ex
-from bl_hector.domain.collection_management import repositories as r
-from bl_hector.domain.collection_management import value_objects as vo
+from bl_hector.domain.collection_management.entities import Book
+from bl_hector.domain.collection_management.exceptions import IncorrectValue
+from bl_hector.domain.collection_management.repositories import Books
+from bl_hector.domain.collection_management.value_objects import (
+    Author,
+    Cover,
+    Genre,
+    Isbn,
+    Title,
+    Year,
+)
 
 
-@dataclass
+@dataclass(frozen=True)
 class Request:
     isbn: str
     title: str
     year: int
     authors: list[str]
     genres: list[str]
     cover: str = ""
@@ -35,39 +42,39 @@
 
 class Presenter(ABC):
     @abstractmethod
     def bad_request(self) -> None:
         ...
 
     @abstractmethod
-    def book_does_not_exist(self, isbn: vo.Isbn) -> None:
+    def book_not_found(self, isbn: Isbn) -> None:
         ...
 
     @abstractmethod
-    def book_updated(self, book: e.Book) -> None:
+    def book_updated(self, book: Book) -> None:
         ...
 
 
 @dataclass(frozen=True)
 class Interactor:
     presenter: Presenter
-    books: r.Books
+    books: Books
 
     def execute(self, request: Request) -> None:
         try:
             # There's no business logic to apply when updating a book.
-            book = e.Book.instanciate(
-                vo.Isbn.instanciate(request.isbn),
-                vo.Title.instanciate(request.title),
-                vo.Year.instanciate(request.year),
-                [vo.Author.instanciate(a) for a in request.authors if a],
-                [vo.Genre.instanciate(g) for g in request.genres if g],
-                vo.Cover.instanciate(request.cover) if request.cover else None,
+            book = Book.instanciate(
+                Isbn.instanciate(request.isbn),
+                Title.instanciate(request.title),
+                Year.instanciate(request.year),
+                [Author.instanciate(a) for a in request.authors if a],
+                [Genre.instanciate(g) for g in request.genres if g],
+                Cover.instanciate(request.cover) if request.cover else None,
             )
-        except ex.IncorrectValue:
+        except IncorrectValue:
             return self.presenter.bad_request()
 
         if not self.books.search(isbn=book.isbn):
-            return self.presenter.book_does_not_exist(book.isbn)
+            return self.presenter.book_not_found(book.isbn)
 
         self.books.update(book)
         self.presenter.book_updated(book)
```

### Comparing `bl_hector-0.1.0a2/bl_hector/configuration/__init__.py` & `bl_hector-0.1.0a3/bl_hector/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/bl_hector/configuration/cli.py` & `bl_hector-0.1.0a3/bl_hector/configuration/cli.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/bl_hector/configuration/wsgi.py` & `bl_hector-0.1.0a3/bl_hector/configuration/wsgi.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/bl_hector/domain/__init__.py` & `bl_hector-0.1.0a3/bl_hector/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/bl_hector/domain/administration/__init__.py` & `bl_hector-0.1.0a3/bl_hector/domain/administration/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/bl_hector/domain/administration/entities.py` & `bl_hector-0.1.0a3/bl_hector/domain/administration/entities.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/bl_hector/domain/administration/repositories.py` & `bl_hector-0.1.0a3/bl_hector/domain/administration/repositories.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/bl_hector/domain/administration/services.py` & `bl_hector-0.1.0a3/bl_hector/domain/administration/services.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/bl_hector/domain/administration/value_objects.py` & `bl_hector-0.1.0a3/bl_hector/domain/administration/value_objects.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/bl_hector/domain/collection_management/__init__.py` & `bl_hector-0.1.0a3/bl_hector/domain/collection_management/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/bl_hector/domain/collection_management/entities.py` & `bl_hector-0.1.0a3/bl_hector/domain/collection_management/entities.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,33 +13,33 @@
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 from dataclasses import dataclass
 from typing import Optional
 
-from . import value_objects as vo
 from .exceptions import IncorrectValue
+from .value_objects import Author, Cover, Genre, Isbn, Title, Year
 
 
 @dataclass
 class Book:
-    isbn: vo.Isbn
-    title: vo.Title
-    year: vo.Year
-    authors: list[vo.Author]
-    genres: list[vo.Genre]
-    cover: Optional[vo.Cover] = None
+    isbn: Isbn
+    title: Title
+    year: Year
+    authors: list[Author]
+    genres: list[Genre]
+    cover: Optional[Cover] = None
 
     @classmethod
     def instanciate(
         cls,
-        isbn: vo.Isbn,
-        title: vo.Title,
-        year: vo.Year,
-        authors: list[vo.Author],
-        genres: list[vo.Genre],
-        cover: Optional[vo.Cover] = None,
+        isbn: Isbn,
+        title: Title,
+        year: Year,
+        authors: list[Author],
+        genres: list[Genre],
+        cover: Optional[Cover] = None,
     ) -> "Book":
         if not authors:
             raise IncorrectValue("authors", "A book must have at least one author!")
         return Book(isbn, title, year, authors, genres, cover)
```

### Comparing `bl_hector-0.1.0a2/bl_hector/domain/collection_management/exceptions.py` & `bl_hector-0.1.0a3/bl_hector/domain/collection_management/exceptions.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/bl_hector/domain/collection_management/repositories.py` & `bl_hector-0.1.0a3/bl_hector/domain/collection_management/repositories.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/bl_hector/domain/collection_management/services.py` & `bl_hector-0.1.0a3/bl_hector/domain/collection_management/services.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/bl_hector/domain/collection_management/value_objects.py` & `bl_hector-0.1.0a3/bl_hector/domain/collection_management/value_objects.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/bl_hector/infrastructure/__init__.py` & `bl_hector-0.1.0a3/bl_hector/infrastructure/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/bl_hector/infrastructure/flask/__init__.py` & `bl_hector-0.1.0a3/bl_hector/infrastructure/flask/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,43 +16,55 @@
 
 from flask import Flask, g, get_flashed_messages, request, url_for
 from werkzeug.middleware.proxy_fix import ProxyFix
 
 from bl_hector import __version__
 from bl_hector.infrastructure.flask import services
 from bl_hector.infrastructure.flask.aliases import blueprint as aliases
+from bl_hector.infrastructure.flask.auth import blueprint as auth
 from bl_hector.infrastructure.flask.books import blueprint as books
-from bl_hector.infrastructure.flask.webauthn import blueprint as webauthn
 from bl_hector.infrastructure.settings import WsgiSettings
 from bl_hector.interfaces import l10n
-from bl_hector.interfaces.to_http import as_html as presenters
 
 
 def build_app(settings: WsgiSettings) -> Flask:
     services.define_settings(settings)
 
     app = Flask(__name__)
 
     # FIXME make it configurable?!
     app.wsgi_app = ProxyFix(app.wsgi_app, x_host=1)  # type: ignore
 
     app.config.update(
         SECRET_KEY=settings.SECRET_KEY,
     )
 
-    app.register_blueprint(aliases, url_prefix="/")
-    app.register_blueprint(webauthn, url_prefix="/auth/webauthn")
-    app.register_blueprint(books, url_prefix="/books")
-
-    presenters.register_jinja_global("version", __version__)
-    presenters.register_jinja_global("url_for", url_for)
-    presenters.register_jinja_global("get_flashed_messages", get_flashed_messages)
+    register_blueprints(app, settings)
+    register_jinja_globals()
 
     app.teardown_appcontext(services.close_connection)
 
     @app.before_request
     def guess_locale() -> None:
         g.locale = (
             request.accept_languages.best_match(l10n.LOCALES) or l10n.DEFAULT_LOCALE
         )
 
     return app
+
+
+def register_blueprints(app: Flask, settings: WsgiSettings) -> None:
+    app.register_blueprint(aliases, url_prefix="/")
+    app.register_blueprint(auth, url_prefix="/auth")
+    app.register_blueprint(books, url_prefix="/books")
+    if settings.WEBAUTHN:
+        from bl_hector.infrastructure.flask.webauthn import blueprint as webauthn
+
+        app.register_blueprint(webauthn, url_prefix="/auth/webauthn")
+
+
+def register_jinja_globals() -> None:
+    from bl_hector.interfaces.to_http import as_html as presenters
+
+    presenters.register_jinja_global("version", __version__)
+    presenters.register_jinja_global("url_for", url_for)
+    presenters.register_jinja_global("get_flashed_messages", get_flashed_messages)
```

### Comparing `bl_hector-0.1.0a2/bl_hector/infrastructure/flask/aliases/__init__.py` & `bl_hector-0.1.0a3/bl_hector/infrastructure/flask/aliases/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/bl_hector/infrastructure/flask/books/__init__.py` & `bl_hector-0.1.0a3/bl_hector/infrastructure/flask/books/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/bl_hector/infrastructure/flask/services.py` & `bl_hector-0.1.0a3/bl_hector/infrastructure/flask/services.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/bl_hector/infrastructure/flask/static/css/bulma@0.9.4.min.css` & `bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/css/bulma@0.9.4.min.css`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/bl_hector/infrastructure/flask/static/css/font-awesome@5.14.0.css` & `bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/css/font-awesome@5.14.0.css`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/bl_hector/infrastructure/flask/static/favicon.svg` & `bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/favicon.svg`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/bl_hector/infrastructure/flask/static/img/placeholders/1280x960.png` & `bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/img/placeholders/1280x960.png`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/bl_hector/infrastructure/flask/static/img/placeholders/320x480.png` & `bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/img/placeholders/320x480.png`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/bl_hector/infrastructure/flask/static/img/placeholders/96x96.png` & `bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/img/placeholders/96x96.png`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/bl_hector/infrastructure/flask/static/js/htmx@1.9.2.min.js` & `bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/js/htmx@1.9.2.min.js`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/bl_hector/infrastructure/flask/static/js/hyperscript@0.9.8.min.js` & `bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/js/hyperscript@0.9.8.min.js`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/bl_hector/infrastructure/flask/static/js/simplewebauthn-browser@7.2.0.umd.min.js` & `bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/js/simplewebauthn-browser@7.2.0.umd.min.js`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.ttf` & `bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.woff2` & `bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.ttf` & `bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.woff2` & `bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.ttf` & `bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.woff2` & `bl_hector-0.1.0a3/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/bl_hector/infrastructure/flask/utils.py` & `bl_hector-0.1.0a3/bl_hector/infrastructure/flask/utils.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/bl_hector/infrastructure/flask/webauthn/__init__.py` & `bl_hector-0.1.0a3/bl_hector/infrastructure/flask/webauthn/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,9 +121,8 @@
     session["user_id"] = user.id
     return as_json.Dict({"verified": True}, status_code=HTTP.OK)
 
 
 @blueprint.get("/logout")
 @presenter_to_response
 def logout() -> Any:
-    session.clear()
-    return Redirection(url_for("aliases.root"))
+    return Redirection(url_for("auth.logout"))
```

### Comparing `bl_hector-0.1.0a2/bl_hector/infrastructure/flask/webauthn/security.py` & `bl_hector-0.1.0a3/bl_hector/infrastructure/flask/webauthn/security.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/bl_hector/infrastructure/isbnlib/__init__.py` & `bl_hector-0.1.0a3/bl_hector/infrastructure/isbnlib/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/bl_hector/infrastructure/settings.py` & `bl_hector-0.1.0a3/bl_hector/infrastructure/settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,14 +29,19 @@
     """The data source name to access the database.
     See: <https://docs.sqlalchemy.org/en/20/core/engines.html#database-urls>."""
 
     DEBUG_SQL: bool = False
     """To enable SqlAlchemy logging.
     See: <https://docs.sqlalchemy.org/en/20/core/engines.html#configuring-logging>."""
 
+    WEBAUTHN: bool = False
+    """To WebAuthn authentication.
+    Extra dependencies must be installed: `bl-hector[webauthn]`.
+    """
+
 
 @dataclass(frozen=True)
 class CliSettings(bl_seth.Settings):
     DSN: str
     """The data source name to access the database.
     See: <https://docs.sqlalchemy.org/en/20/core/engines.html#database-urls>."""
```

### Comparing `bl_hector-0.1.0a2/bl_hector/infrastructure/sqlalchemy/__init__.py` & `bl_hector-0.1.0a3/bl_hector/infrastructure/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/bl_hector/infrastructure/sqlalchemy/repositories.py` & `bl_hector-0.1.0a3/bl_hector/infrastructure/sqlalchemy/repositories.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/bl_hector/infrastructure/typer/__init__.py` & `bl_hector-0.1.0a3/bl_hector/infrastructure/typer/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/bl_hector/infrastructure/typer/books.py` & `bl_hector-0.1.0a3/bl_hector/infrastructure/typer/books.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/bl_hector/infrastructure/typer/services.py` & `bl_hector-0.1.0a3/bl_hector/infrastructure/typer/services.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/bl_hector/interfaces/__init__.py` & `bl_hector-0.1.0a3/bl_hector/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/bl_hector/interfaces/from_dict.py` & `bl_hector-0.1.0a3/bl_hector/interfaces/from_dict.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/bl_hector/interfaces/from_json.py` & `bl_hector-0.1.0a3/bl_hector/interfaces/from_json.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/bl_hector/interfaces/l10n/__init__.py` & `bl_hector-0.1.0a3/bl_hector/interfaces/to_terminal/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,31 +10,31 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
-from pathlib import Path
-from typing import Any, Optional, Protocol
+from abc import ABC, abstractmethod
+from enum import Enum
 
-from fluent.runtime import FluentLocalization, FluentResourceLoader
+from bl_hector.application.use_cases import look_up_book
 
-DEFAULT_LOCALE = "en-GB"
-LOCALES = [DEFAULT_LOCALE, "fr-FR"]
-LOADER = FluentResourceLoader(str(Path(__file__).parent / "{locale}"))
 
-
-class Translator(Protocol):
-    def __call__(self, message_id: str, values: Optional[dict[str, Any]] = None) -> str:
-        ...
+class ExitCodes(Enum):
+    OK = 0
+    USAGE = 1
+    NOT_FOUND = 2
+    BAD_REQUEST = 3
 
 
-class DummyTranslator(Translator):
-    def __call__(self, message_id: str, values: Optional[dict[str, Any]] = None) -> str:
-        return message_id
+class WithExitCode(ABC):
+    @abstractmethod
+    def exit_code(self) -> int:
+        ...
 
 
-def localization(locale: str) -> FluentLocalization:
-    if locale not in LOCALES:
-        raise RuntimeError(f"Locale `{locale}` is not defined!")
-    return FluentLocalization([locale] + LOCALES, ["main.ftl"], LOADER)
+class LookUpBookInterface(look_up_book.Presenter, WithExitCode):
+    """
+    Interface required when using more than one presenter
+    inside a route/command, so MyPy can do it's job!
+    """
```

### Comparing `bl_hector-0.1.0a2/bl_hector/interfaces/l10n/en-GB/main.ftl` & `bl_hector-0.1.0a3/bl_hector/interfaces/l10n/en-GB/main.ftl`

 * *Files 4% similar despite different names*

```diff
@@ -54,14 +54,18 @@
 book-genres = genres
 book-genres-description = The list of genres the book belongs to, comma separated.
 
 mandatory-value = This value is mandatory!
 incorrect-value = Incorrect value!
 not-an-isbn = This is not an ISBN!
 
+auth-login-title = Log in
+# method (string) The sign in method
+auth-login-method = Sign in using { $method }
+
 webauthn-register-title = Device registration
 webauthn-register-description = Your browser should be asking you to tap your security device…
 webauthn-register-success = Your security device has been succesfully registered!
 webauthn-register-failure = Your security device could not be registered!?
 
 webauthn-login-title = Log in
 webauthn-login-description = Your browser should be asking you to tap your security device…
```

#### html2text {}

```diff
@@ -22,28 +22,30 @@
 year book-year-description = The year the book was published in. book-author =
 author book-author-description = One of the authors of the book. book-authors =
 authors book-authors-description = The list of authors of the book, comma
 separated. book-genre = genre book-genre-description = One of the genres the
 book belongs to. book-genres = genres book-genres-description = The list of
 genres the book belongs to, comma separated. mandatory-value = This value is
 mandatory! incorrect-value = Incorrect value! not-an-isbn = This is not an
-ISBN! webauthn-register-title = Device registration webauthn-register-
+ISBN! auth-login-title = Log in # method (string) The sign in method auth-
+login-method = Sign in using { $method } webauthn-register-title = Device
+registration webauthn-register-description = Your browser should be asking you
+to tap your security deviceâ¦ webauthn-register-success = Your security device
+has been succesfully registered! webauthn-register-failure = Your security
+device could not be registered!? webauthn-login-title = Log in webauthn-login-
 description = Your browser should be asking you to tap your security deviceâ¦
-webauthn-register-success = Your security device has been succesfully
-registered! webauthn-register-failure = Your security device could not be
-registered!? webauthn-login-title = Log in webauthn-login-description = Your
-browser should be asking you to tap your security deviceâ¦ webauthn-login-
-failure = You couldn't be logged in!? add-book-requires-authentification = You
-must be authenticated before adding a book! add-book-title = Add a new book to
-the collection add-book-action = Add a book add-book-cancel = Cancel add-book-
-add = Add search-books-title = Search for a book search-books-action = Look up
-book search-books-clear = Clear search-books-search = Search search-books-no-
-result = No matching book! search-books-previous-page = Previous search-books-
-next-page = Next # title (string) The title of the book display-book-title =
-Details for "{ $title }" update-book-requires-authentification = You must be
-authenticated before editing a book! # isbn (string) The ISBN of the book
-update-book-title = Edit information for `{ $isbn }` update-book-action = Edit
-update-book-failure = Book cannot be updated! update-book-success = Book has
-been updated! update-book-cancel = Cancel update-book-update = Save book-
-already-exists = Book already in the collection! book-added = Book successfully
-added! book-not-found = Book not found! book-cannot-be-added = The book cannot
-be added! books-cannot-be-found = The search cannot be performed!
+webauthn-login-failure = You couldn't be logged in!? add-book-requires-
+authentification = You must be authenticated before adding a book! add-book-
+title = Add a new book to the collection add-book-action = Add a book add-book-
+cancel = Cancel add-book-add = Add search-books-title = Search for a book
+search-books-action = Look up book search-books-clear = Clear search-books-
+search = Search search-books-no-result = No matching book! search-books-
+previous-page = Previous search-books-next-page = Next # title (string) The
+title of the book display-book-title = Details for "{ $title }" update-book-
+requires-authentification = You must be authenticated before editing a book! #
+isbn (string) The ISBN of the book update-book-title = Edit information for `
+{ $isbn }` update-book-action = Edit update-book-failure = Book cannot be
+updated! update-book-success = Book has been updated! update-book-cancel =
+Cancel update-book-update = Save book-already-exists = Book already in the
+collection! book-added = Book successfully added! book-not-found = Book not
+found! book-cannot-be-added = The book cannot be added! books-cannot-be-found =
+The search cannot be performed!
```

### Comparing `bl_hector-0.1.0a2/bl_hector/interfaces/l10n/fr-FR/main.ftl` & `bl_hector-0.1.0a3/bl_hector/interfaces/l10n/fr-FR/main.ftl`

 * *Files 8% similar despite different names*

```diff
@@ -54,14 +54,18 @@
 book-genres = genres
 book-genres-description = La liste des genres auxquels le livre se rattache, séparés par des virgules.
 
 mandatory-value = Cette valeur est obligatoire !
 incorrect-value = Cette valeur est incorrecte !
 not-an-isbn = Ceci n'est pas un ISBN !
 
+auth-login-title = Connexion
+# method (string) The sign in method
+auth-login-method = Sign in using { $method }
+
 webauthn-register-title = Association du dispositif de sécurité
 webauthn-register-description = Votre navigateur devrait être en train de vous demander de toucher votre dispositif de sécurité…
 webauthn-register-success = Votre dispositif de sécurité a été correctement associé !
 webauthn-register-failure = Votre dispositif de sécurité n'a pas pu être associé !?
 
 webauthn-login-title = Connexion
 webauthn-login-description = Votre navigateur devrait être en train de vous demander de toucher votre dispositif de sécurité…
```

#### html2text {}

```diff
@@ -24,33 +24,34 @@
 description = UnÂ·e des autÂ·riceÂ·eurÂ·s du livre. book-authors =
 autÂ·riceÂ·eurÂ·s book-authors-description = La liste des autÂ·riceÂ·eurÂ·s du
 livre, sÃ©parÃ©Â·eÂ·s par des virgules. book-genre = genre book-genre-
 description = Un des genres auxquels le livre se rattache. book-genres = genres
 book-genres-description = La liste des genres auxquels le livre se rattache,
 sÃ©parÃ©s par des virgules. mandatory-value = Cette valeur est obligatoireÂ !
 incorrect-value = Cette valeur est incorrecteÂ ! not-an-isbn = Ceci n'est pas
-un ISBNÂ ! webauthn-register-title = Association du dispositif de sÃ©curitÃ©
-webauthn-register-description = Votre navigateur devrait Ãªtre en train de vous
-demander de toucher votre dispositif de sÃ©curitÃ©â¦ webauthn-register-success
-= Votre dispositif de sÃ©curitÃ© a Ã©tÃ© correctement associÃ©Â ! webauthn-
-register-failure = Votre dispositif de sÃ©curitÃ© n'a pas pu Ãªtre associÃ©Â !?
-webauthn-login-title = Connexion webauthn-login-description = Votre navigateur
-devrait Ãªtre en train de vous demander de toucher votre dispositif de
-sÃ©curitÃ©â¦ webauthn-login-failure = Vous n'avez pas pu Ãªtre
-connectÃ©Â·eÂ !? add-book-requires-authentification = Vous devez Ãªtre
-authentifiÃ©Â·e pour pouvoir ajouter un livreÂ ! add-book-title = Ajouter un
-nouveau livre Ã  la collection add-book-action = Ajouter un livre add-book-
-cancel = Annuler add-book-add = Ajouter search-books-title = Chercher un livre
-dans la collection search-books-action = Chercher un livre search-books-clear =
-RÃ©initialiser search-books-search = Chercher search-books-no-result = Aucun
-livre ne correspondÂ ! search-books-previous-page = PrÃ©cÃ©dent search-books-
-next-page = Suivant # title (string) The title of the book display-book-title =
-DÃ©tails pour Â«Â { $title }Â Â» update-book-requires-authentification = Vous
-devez Ãªtre authentifiÃ©Â·e pour pouvoir Ã©diter un livreÂ ! # isbn (string)
-The ISBN of the book update-book-title = Ãditer les informations de `{ $isbn
-}` update-book-action = Ãditer update-book-failure = Le livre n'a pas pu Ãªtre
-mis Ã  jourÂ ! update-book-success = Le livre a bien Ã©tÃ© mis Ã  jourÂ !
-update-book-cancel = Annuler update-book-update = Enregistrer book-already-
-exists = Ce livre est dÃ©jÃ  dans la collectionÂ ! book-added = Le livre a bien
-Ã©tÃ© ajoutÃ©. book-not-found = Le livre n'a pas Ã©tÃ© trouvÃ©Â ! book-cannot-
-be-added = Le livre n'a pas pu Ãªtre ajoutÃ©Â ! books-cannot-be-found = La
-recherche n'a pas pu Ãªtre effectuÃ©eÂ !
+un ISBNÂ ! auth-login-title = Connexion # method (string) The sign in method
+auth-login-method = Sign in using { $method } webauthn-register-title =
+Association du dispositif de sÃ©curitÃ© webauthn-register-description = Votre
+navigateur devrait Ãªtre en train de vous demander de toucher votre dispositif
+de sÃ©curitÃ©â¦ webauthn-register-success = Votre dispositif de sÃ©curitÃ© a
+Ã©tÃ© correctement associÃ©Â ! webauthn-register-failure = Votre dispositif de
+sÃ©curitÃ© n'a pas pu Ãªtre associÃ©Â !? webauthn-login-title = Connexion
+webauthn-login-description = Votre navigateur devrait Ãªtre en train de vous
+demander de toucher votre dispositif de sÃ©curitÃ©â¦ webauthn-login-failure =
+Vous n'avez pas pu Ãªtre connectÃ©Â·eÂ !? add-book-requires-authentification =
+Vous devez Ãªtre authentifiÃ©Â·e pour pouvoir ajouter un livreÂ ! add-book-
+title = Ajouter un nouveau livre Ã  la collection add-book-action = Ajouter un
+livre add-book-cancel = Annuler add-book-add = Ajouter search-books-title =
+Chercher un livre dans la collection search-books-action = Chercher un livre
+search-books-clear = RÃ©initialiser search-books-search = Chercher search-
+books-no-result = Aucun livre ne correspondÂ ! search-books-previous-page =
+PrÃ©cÃ©dent search-books-next-page = Suivant # title (string) The title of the
+book display-book-title = DÃ©tails pour Â«Â { $title }Â Â» update-book-
+requires-authentification = Vous devez Ãªtre authentifiÃ©Â·e pour pouvoir
+Ã©diter un livreÂ ! # isbn (string) The ISBN of the book update-book-title =
+Ãditer les informations de `{ $isbn }` update-book-action = Ãditer update-
+book-failure = Le livre n'a pas pu Ãªtre mis Ã  jourÂ ! update-book-success =
+Le livre a bien Ã©tÃ© mis Ã  jourÂ ! update-book-cancel = Annuler update-book-
+update = Enregistrer book-already-exists = Ce livre est dÃ©jÃ  dans la
+collectionÂ ! book-added = Le livre a bien Ã©tÃ© ajoutÃ©. book-not-found = Le
+livre n'a pas Ã©tÃ© trouvÃ©Â ! book-cannot-be-added = Le livre n'a pas pu Ãªtre
+ajoutÃ©Â ! books-cannot-be-found = La recherche n'a pas pu Ãªtre effectuÃ©eÂ !
```

### Comparing `bl_hector-0.1.0a2/bl_hector/interfaces/to_http/__init__.py` & `bl_hector-0.1.0a3/bl_hector/interfaces/to_http/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/bl_hector/interfaces/to_http/as_html/__init__.py` & `bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_html/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 from bl_hector.application.use_cases import (
     add_book,
     display_book,
     look_up_book,
     search_books,
     update_book,
 )
-from bl_hector.domain.collection_management import entities as e
-from bl_hector.domain.collection_management import value_objects as vo
+from bl_hector.domain.collection_management.entities import Book
+from bl_hector.domain.collection_management.value_objects import Isbn
 from bl_hector.interfaces import User, l10n, validators
 from bl_hector.interfaces.to_http import HttpPresenter
 
 ENVIRONMENT = Environment(
     loader=FileSystemLoader([Path(__file__).parent / "templates"]),
     autoescape=select_autoescape(),
     extensions=["bl_hector.interfaces.utils.PatchedPyPugJSExtension"],
@@ -71,16 +71,16 @@
 
         self.__adapt_to(user)
 
     def __adapt_to(self, user: Optional[User] = None) -> None:
         locale = user.locale if (user and user.locale) else l10n.DEFAULT_LOCALE
         self.__localization = l10n.localization(locale)
 
-    def _(self, message_id: str, values: Optional[dict[str, Any]] = None) -> str:
-        return str(self.__localization.format_value(message_id, values))
+    def _(self, message_id: str, **kwargs: Any) -> str:
+        return str(self.__localization.format_value(message_id, kwargs))
 
     def status_code(self) -> int:
         return int(self.__status_code)
 
     def headers(self) -> dict[str, str]:
         return self.__headers
 
@@ -179,15 +179,15 @@
     def render(self, **context: Any) -> str:
         return super().render(**self.__context, **context, data=self.__data)
 
     def bad_request(self) -> None:
         # FIXME setting status code to 404 is not supported by htmx!?
         self.__context["error"] = self._("books-cannot-be-found")
 
-    def book(self, book: e.Book) -> None:
+    def book(self, book: Book) -> None:
         if "books" not in self.__context:
             self.__context["books"] = []
         self.__context["books"].append(
             {
                 "isbn": str(book.isbn),
                 "title": str(book.title),
                 "year": int(book.year),
@@ -233,19 +233,19 @@
     def render(self, **context: Any) -> str:
         return super().render(**self.__context, **context, data=self.__data)
 
     def bad_request(self) -> None:
         # FIXME setting status code to 404 is not supported by htmx!?
         self.__context["error"] = self._("book-cannot-be-added")
 
-    def book_already_exists(self, book: e.Book) -> None:
+    def book_already_exists(self, book: Book) -> None:
         self.__notify(self._("book-already-exists"), "info")
         self.redirect(url_for("books.search", isbn=str(book.isbn)))
 
-    def book_added(self, book: e.Book) -> None:
+    def book_added(self, book: Book) -> None:
         self.__notify(self._("book-added"), "success")
         self.redirect(url_for("books.search", isbn=str(book.isbn)))
 
 
 class LookUpBook(JinjaPresenter, look_up_book.Presenter):
     def __init__(self, /, *, user: Optional[User] = None) -> None:
         super().__init__("books/add", fragment="form", user=user)
@@ -259,19 +259,19 @@
         self.__data["isbn"] = isbn
         self.__context["errors"] = {"isbn": self._("not-an-isbn")}
 
     def unknown_error(self, message: str) -> None:
         logging.error(f"LookUpBook: {message}")
         self.__context["errors"] = {"isbn": self._("unknown-error")}
 
-    def unknown_isbn(self, isbn: vo.Isbn) -> None:
+    def book_not_found(self, isbn: Isbn) -> None:
         self.__data["isbn"] = str(isbn)
         self.__context["errors"] = {"isbn": self._("unknown-isbn")}
 
-    def book(self, book: e.Book) -> None:
+    def book(self, book: Book) -> None:
         self.__data = {
             "isbn": str(book.isbn),
             "title": str(book.title),
             "year": int(book.year),
             "authors": ", ".join([str(a) for a in book.authors]),
             "genres": ", ".join([str(g) for g in book.genres]),
         }
@@ -292,22 +292,22 @@
     def render(self, **context: Any) -> str:
         return super().render(**self.__context, **context)
 
     def not_an_isbn(self, isbn: str) -> None:
         self.__notify(self._("not-an-isbn"), "warning")
         self.redirect(url_for("books.search"))
 
-    def book_does_not_exist(self, isbn: vo.Isbn) -> None:
+    def book_not_found(self, isbn: Isbn) -> None:
         self.__notify(self._("book-does-not-exist"), "warning")
         self.redirect(url_for("books.search"))
 
-    def see_other(self, isbn: vo.Isbn) -> None:
+    def see_other(self, isbn: Isbn) -> None:
         self.redirect(url_for("books.display", isbn=str(isbn)), HTTP.MOVED_PERMANENTLY)
 
-    def book(self, book: e.Book) -> None:
+    def book(self, book: Book) -> None:
         self.__context["book"] = {
             "isbn": str(book.isbn),
             "title": str(book.title),
             "year": int(book.year),
             "authors": ", ".join([str(a) for a in book.authors]),
             "genres": ", ".join([str(g) for g in book.genres]),
             "cover": str(book.cover) if book.cover else "",
@@ -330,22 +330,22 @@
     def render(self, **context: Any) -> str:
         return super().render(**self.__context, **context)
 
     def not_an_isbn(self, isbn: str) -> None:
         self.__notify(self._("not-an-isbn"), "warning")
         self.redirect(url_for("books.search"))
 
-    def book_does_not_exist(self, isbn: vo.Isbn) -> None:
+    def book_not_found(self, isbn: Isbn) -> None:
         self.__notify(self._("book-does-not-exist"), "warning")
         self.redirect(url_for("books.search"))
 
-    def see_other(self, isbn: vo.Isbn) -> None:
+    def see_other(self, isbn: Isbn) -> None:
         self.redirect(url_for("books.display", isbn=str(isbn)), HTTP.MOVED_PERMANENTLY)
 
-    def book(self, book: e.Book) -> None:
+    def book(self, book: Book) -> None:
         self.__context["data"] = {
             "isbn": str(book.isbn),
             "title": str(book.title),
             "year": int(book.year),
             "authors": ", ".join([str(a) for a in book.authors]),
             "genres": ", ".join([str(g) for g in book.genres]),
             "cover": str(book.cover) if book.cover else "",
@@ -371,14 +371,14 @@
     def render(self, **context: Any) -> str:
         return super().render(**self.__context, **context, data=self.__data)
 
     def bad_request(self) -> None:
         # FIXME setting status code to 404 is not supported by htmx!?
         self.__context["error"] = self._("update-book-failure")
 
-    def book_does_not_exist(self, isbn: vo.Isbn) -> None:
+    def book_not_found(self, isbn: Isbn) -> None:
         self.__notify(self._("book-not-found"), "warning")
         self.redirect(url_for("books.search"))
 
-    def book_updated(self, book: e.Book) -> None:
+    def book_updated(self, book: Book) -> None:
         self.__notify(self._("update-book-success"), "success")
         self.redirect(url_for("books.display", isbn=str(book.isbn)))
```

### Comparing `bl_hector-0.1.0a2/bl_hector/interfaces/to_http/as_html/templates/books/add.pug` & `bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_html/templates/books/add.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/bl_hector/interfaces/to_http/as_html/templates/books/display.pug` & `bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_html/templates/books/display.pug`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 //-
 //- You should have received a copy of the GNU Affero General Public License
 //- along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 extends layout
 
 block title
-  title= _("hector") + " – " + _("display-book-title", {"title": book.title})
+  title= _("hector") + " – " + _("display-book-title", title=book.title)
 
 block content
   section.section
     .container
       .buttons.is-pulled-right
         if user.id
           a.button.is-link(href="#{url_for('books.update', isbn=book.isbn)}")
```

### Comparing `bl_hector-0.1.0a2/bl_hector/interfaces/to_http/as_html/templates/books/mixins/render_isbn.pug` & `bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_html/templates/books/mixins/render_isbn.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/bl_hector/interfaces/to_http/as_html/templates/books/search.pug` & `bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_html/templates/books/search.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/bl_hector/interfaces/to_http/as_html/templates/books/update.pug` & `bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_html/templates/books/update.pug`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 //-
 //- You should have received a copy of the GNU Affero General Public License
 //- along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 extends layout
 
 block title
-  title= _("hector") + " – " + _("update-book-title", {"isbn": isbn})
+  title= _("hector") + " – " + _("update-book-title", isbn=isbn)
 
 block scripts
   script.
     function loadIntoImage(from, toImage, toInput) {
       if (from.files && from.files[0]) {
         const reader = new FileReader()
         reader.onload = e => {
@@ -31,15 +31,15 @@
         reader.readAsDataURL(from.files[0])
       }
     }
 
 block content
   section.section
     .container
-      h1.title.is-3= _("update-book-title", {"isbn": isbn})
+      h1.title.is-3= _("update-book-title", isbn=isbn)
 
       #form
         block form
           include mixins/form
           form(method="POST")
             .columns
               .column.is-one-quarter
```

### Comparing `bl_hector-0.1.0a2/bl_hector/interfaces/to_http/as_html/templates/error.pug` & `bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_html/templates/error.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/bl_hector/interfaces/to_http/as_html/templates/layout.pug` & `bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_html/templates/layout.pug`

 * *Files 5% similar despite different names*

```diff
@@ -41,14 +41,14 @@
       +flash(messages)
 
       block content
 
     footer.footer
       .content.has-text-centered
         p
-          span= _("copyright", {"version": version, "years": "2023", "holders": "Bioneland"}) | safe
+          span= _("copyright", version=version, years="2023", holders="Bioneland") | safe
           br
-          span= _("license", {"name": "AGPL", "url": "https://www.gnu.org/licenses/agpl-3.0.fr.html"}) | safe
+          span= _("license", name="AGPL", url="https://www.gnu.org/licenses/agpl-3.0.fr.html") | safe
 
     script(src="#{url_for('static', filename='js/hyperscript@0.9.8.min.js')}")
     script(src="#{url_for('static', filename='js/htmx@1.9.2.min.js')}")
     block scripts
```

### Comparing `bl_hector-0.1.0a2/bl_hector/interfaces/to_http/as_html/templates/mixins/flash.pug` & `bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_html/templates/mixins/flash.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/bl_hector/interfaces/to_http/as_html/templates/mixins/form.pug` & `bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_html/templates/mixins/form.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/bl_hector/interfaces/to_http/as_html/templates/mixins/navbar.pug` & `bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_html/templates/mixins/navbar.pug`

 * *Files 11% similar despite different names*

```diff
@@ -35,14 +35,14 @@
           a.navbar-item(href="#{url_for('books.search')}")= _("menu-books")
         .navbar-end
           .navbar-item
             .field.is-grouped
               //- Auth pages contains JS and should be properly loaded.
               p.control(hx-boost="false")
                 if user.id
-                  a.button.is-success.is-light(href="#{url_for('webauthn.logout')}")
+                  a.button.is-success.is-light(href="#{url_for('auth.logout')}")
                     span.icon: i.fa.fa-lock
                     span= _("menu-logout")
                 else
-                  a.button.is-warning.is-light(href="#{url_for('webauthn.login')}")
+                  a.button.is-warning.is-light(href="#{url_for('auth.login')}")
                     span.icon: i.fa.fa-lock-open
                     span= _("menu-login")
```

### Comparing `bl_hector-0.1.0a2/bl_hector/interfaces/to_http/as_html/templates/webauthn/login.pug` & `bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_html/templates/webauthn/login.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/bl_hector/interfaces/to_http/as_html/templates/webauthn/register.pug` & `bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_html/templates/webauthn/register.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/bl_hector/interfaces/to_http/as_json/__init__.py` & `bl_hector-0.1.0a3/bl_hector/interfaces/to_http/as_json/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/bl_hector/interfaces/to_terminal/__init__.py` & `bl_hector-0.1.0a3/bl_hector/interfaces/to_terminal/as_json.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,31 +10,41 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
-from abc import ABC, abstractmethod
-from enum import Enum
+import json
+from typing import Callable
 
-from bl_hector.application.use_cases import look_up_book
+from bl_hector.domain.collection_management.entities import Book
+from bl_hector.domain.collection_management.value_objects import Isbn
+from bl_hector.interfaces.to_terminal import ExitCodes, LookUpBookInterface
+
+
+class LookUpBook(LookUpBookInterface):
+    def __init__(self, printer: Callable[[str], None]) -> None:
+        self.__printer = printer
+        self.__exit_code = ExitCodes.USAGE
+
+    def not_an_isbn(self, isbn: str) -> None:
+        self.__exit_code = ExitCodes.BAD_REQUEST
+
+    def book_not_found(self, isbn: Isbn) -> None:
+        self.__exit_code = ExitCodes.NOT_FOUND
+
+    def book(self, book: Book) -> None:
+        self.__exit_code = ExitCodes.OK
+        data = {
+            "isbn": str(book.isbn),
+            "title": str(book.title),
+            "year": int(book.year),
+            "authors": [str(b) for b in book.authors],
+        }
+        if book.genres:
+            data["genres"] = [str(g) for g in book.genres]
 
+        self.__printer(json.dumps(data))
 
-class ExitCodes(Enum):
-    OK = 0
-    USAGE = 1
-    NOT_FOUND = 2
-    BAD_REQUEST = 3
-
-
-class WithExitCode(ABC):
-    @abstractmethod
     def exit_code(self) -> int:
-        ...
-
-
-class LookUpBookInterface(look_up_book.Presenter, WithExitCode):
-    """
-    Interface required when using more than one presenter
-    inside a route/command, so MyPy can do it's job!
-    """
+        return self.__exit_code.value
```

### Comparing `bl_hector-0.1.0a2/bl_hector/interfaces/to_terminal/as_text.py` & `bl_hector-0.1.0a3/bl_hector/interfaces/to_terminal/as_text.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,29 +35,29 @@
         self.__exit_code = ExitCodes.USAGE
         self._ = translator
 
     def not_an_isbn(self, isbn: str) -> None:
         self.__exit_code = ExitCodes.BAD_REQUEST
         self.__printer(self._("not-an-isbn"))
 
-    def unknown_isbn(self, isbn: Isbn) -> None:
+    def book_not_found(self, isbn: Isbn) -> None:
         self.__exit_code = ExitCodes.NOT_FOUND
         self.__printer(self._("book-not-found"))
 
     def book(self, book: Book) -> None:
         self.__exit_code = ExitCodes.OK
         self.__info(self._("book-isbn"), str(book.isbn))
         self.__info(self._("book-title"), str(book.title))
         self.__info(self._("book-year"), str(book.year))
         self.__info(self._("book-authors"), ", ".join([str(b) for b in book.authors]))
         if book.genres:
             self.__info(self._("book-genres"), ", ".join([str(g) for g in book.genres]))
 
     def __info(self, name: str, value: str) -> None:
-        self.__printer(self._("info-line", {"name": name, "value": value}))
+        self.__printer(self._("info-line", name=name, value=value))
 
     def exit_code(self) -> int:
         return self.__exit_code.value
 
 
 class AddBook(add_book.Presenter):
     def __init__(
```

### Comparing `bl_hector-0.1.0a2/bl_hector/interfaces/utils.py` & `bl_hector-0.1.0a3/bl_hector/interfaces/utils.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a2/bl_hector/interfaces/validators.py` & `bl_hector-0.1.0a3/bl_hector/interfaces/validators.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,16 +14,22 @@
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 from typing import Any, Callable, Protocol
 
 from werkzeug.datastructures import MultiDict
 
-from bl_hector.domain.collection_management import value_objects as vo
 from bl_hector.domain.collection_management.exceptions import IncorrectValue
+from bl_hector.domain.collection_management.value_objects import (
+    Author,
+    Genre,
+    Isbn,
+    Title,
+    Year,
+)
 from bl_hector.interfaces.l10n import DummyTranslator, Translator
 
 
 class ValidationResult:
     name: str
 
     def __init__(self, name: str, error: str = "", **variables: Any) -> None:
@@ -31,15 +37,15 @@
         self.__error = error
         self.__variables = variables
 
     def __bool__(self) -> bool:
         return not self.__error
 
     def error(self, translator: Translator = DummyTranslator()) -> str:
-        return translator(self.__error, self.__variables)
+        return translator(self.__error, **self.__variables)
 
 
 class Validator(Protocol):
     def __call__(self, name: str, value: str) -> ValidationResult:
         ...
 
 
@@ -59,67 +65,67 @@
         return validator(name, value)
 
     return wrapper
 
 
 def isbn(name: str, value: str) -> ValidationResult:
     try:
-        vo.Isbn.instanciate(value)
+        Isbn.instanciate(value)
         return ValidationResult(name)
     except IncorrectValue:
         return ValidationResult(name, "incorrect-value")
 
 
 def year(name: str, value: str) -> ValidationResult:
     try:
-        vo.Year.instanciate(int(value))
+        Year.instanciate(int(value))
         return ValidationResult(name)
     except ValueError:
         return ValidationResult(name, "incorrect-value")
     except IncorrectValue:
         return ValidationResult(name, "incorrect-value")
 
 
 def title(name: str, value: str) -> ValidationResult:
     try:
-        vo.Title.instanciate(value)
+        Title.instanciate(value)
         return ValidationResult(name)
     except IncorrectValue:
         return ValidationResult(name, "incorrect-value")
 
 
 def author(name: str, value: str) -> ValidationResult:
     try:
-        vo.Author.instanciate(value)
+        Author.instanciate(value)
         return ValidationResult(name)
     except IncorrectValue:
         return ValidationResult(name, "incorrect-value")
 
 
 def authors(name: str, value: str) -> ValidationResult:
     try:
         for d in [d.strip() for d in value.strip().strip(",").split(",")]:
-            vo.Author.instanciate(d)
+            Author.instanciate(d)
         return ValidationResult(name)
     except IncorrectValue:
         return ValidationResult(name, "incorrect-value")
 
 
 def genre(name: str, value: str) -> ValidationResult:
     try:
-        vo.Genre.instanciate(value)
+        Genre.instanciate(value)
         return ValidationResult(name)
     except IncorrectValue:
         return ValidationResult(name, "incorrect-value")
 
 
 def genres(name: str, value: str) -> ValidationResult:
     try:
         for d in [d.strip() for d in value.strip().strip(",").split(",")]:
-            vo.Genre.instanciate(d)
+            Genre.instanciate(d)
         return ValidationResult(name)
     except IncorrectValue:
         return ValidationResult(name, "incorrect-value")
 
 
 class DataValidator:
     VALIDATORS: list[tuple[str, Callable[[str, str], ValidationResult]]] = []
```

### Comparing `bl_hector-0.1.0a2/pyproject.toml` & `bl_hector-0.1.0a3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bl_hector"
-version = "0.1.0-alpha.2"
+version = "0.1.0-alpha.3"
 description = "A collection manager."
 authors = ["Tanguy Le Carrour <tanguy@bioneland.org>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 
 exclude = [
     "**/*_spec.py",
@@ -25,15 +25,15 @@
 bl-seth = "^0.1.2"
 isbnlib = "^3.10.14"
 jinja2-fragments = "^0.3.0"
 SQLAlchemy = "^2.0.15"
 typer = "^0.9.0"
 bl3d = "^0.3.0"
 "fluent.runtime" = "^0.4.0"
-webauthn = "^1.8.1"
+webauthn = {version = "^1.8.1", optional = true}
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3.1"
 robber = "^1.1.5"
 invoke = "^2.1.1"
 flake8 = "^6.0.0"
 black = "^23.3.0"
@@ -42,14 +42,17 @@
 termcolor = "^2.3.0"
 types-setuptools = "^67.7.0"
 mamba = "^0.11.2"
 beautifulsoup4 = "^4.12.2"
 types-beautifulsoup4 = "^4.12.0"
 behave = "^1.2.6"
 
+[tool.poetry.extras]
+webauthn = ["webauthn"]
+
 [tool.isort]
 profile = "black"
 multi_line_output = 3
 
 [tool.black]
 line-length = 89
```

### Comparing `bl_hector-0.1.0a2/setup.py` & `bl_hector-0.1.0a3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,14 +8,15 @@
  'bl_hector.configuration',
  'bl_hector.domain',
  'bl_hector.domain.administration',
  'bl_hector.domain.collection_management',
  'bl_hector.infrastructure',
  'bl_hector.infrastructure.flask',
  'bl_hector.infrastructure.flask.aliases',
+ 'bl_hector.infrastructure.flask.auth',
  'bl_hector.infrastructure.flask.books',
  'bl_hector.infrastructure.flask.webauthn',
  'bl_hector.infrastructure.isbnlib',
  'bl_hector.infrastructure.sqlalchemy',
  'bl_hector.infrastructure.typer',
  'bl_hector.interfaces',
  'bl_hector.interfaces.l10n',
@@ -29,46 +30,50 @@
  'bl_hector.infrastructure.flask': ['static/*',
                                     'static/css/*',
                                     'static/img/placeholders/*',
                                     'static/js/*',
                                     'static/webfonts/*'],
  'bl_hector.interfaces.l10n': ['en-GB/*', 'fr-FR/*'],
  'bl_hector.interfaces.to_http.as_html': ['templates/*',
+                                          'templates/auth/*',
                                           'templates/books/*',
                                           'templates/books/mixins/*',
                                           'templates/mixins/*',
                                           'templates/webauthn/*']}
 
 install_requires = \
 ['Flask>=2.3.2,<3.0.0',
  'SQLAlchemy>=2.0.15,<3.0.0',
  'bl-seth>=0.1.2,<0.2.0',
  'bl3d>=0.3.0,<0.4.0',
  'fluent.runtime>=0.4.0,<0.5.0',
  'isbnlib>=3.10.14,<4.0.0',
  'jinja2-fragments>=0.3.0,<0.4.0',
  'pypugjs>=5.9.12,<6.0.0',
- 'typer>=0.9.0,<0.10.0',
- 'webauthn>=1.8.1,<2.0.0']
+ 'typer>=0.9.0,<0.10.0']
+
+extras_require = \
+{'webauthn': ['webauthn>=1.8.1,<2.0.0']}
 
 entry_points = \
 {'console_scripts': ['hector = bl_hector.configuration.cli:cli']}
 
 setup_kwargs = {
     'name': 'bl-hector',
-    'version': '0.1.0a2',
+    'version': '0.1.0a3',
     'description': 'A collection manager.',
-    'long_description': '# Hector — a collection manager\n\n## Install\n\nFor the time being, Hector cannot be installed from PyPI.\nSee [CONTRIBUTING.md]() to set up a development environment.\n\n\n## Configure\n\nHector is configured using environment variables.\nAll the variable names are prefixed with `HECTOR_`.\n\n```console\n$ export HECTOR_SECRET_KEY="XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"\n$ export HECTOR_DSN="sqlite:///data.sqlite"\n```\n\nThe secret can be generated using the `token_hex()` function from\nthe Python\'s `secrets` module.\n\nAdditional Python database drivers might be required depending on the DSN.\n\nSee [the `settings` module](bl_hector/infrastructure/settings.py) for\na comprehensive list of configuration variables.\n\n\n## Initialise\n\nOnce configured, you must initialise Hector\'s database with the dedicated command:\n\n```console\n$ hector init-db\n```\n\n\n## Run\n\nHector being a Flask application, it can be run using any WSGI server,\nfor instance, with [Gunicorn](https://gunicorn.org):\n\n```console\n$ gunicorn --access-logfile="-" -w 4 -b 127.0.0.1:3000 "bl_hector.configuration.wsgi:app()"\n```\n',
+    'long_description': '# Hector — a collection manager\n\n## Install\n\nFor the time being, Hector cannot be installed from PyPI.\nSee [CONTRIBUTING.md]() to set up a development environment.\n\n\n## Configure\n\nHector is configured using environment variables.\nAll the variable names are prefixed with `HECTOR_`.\n\n```console\n$ export HECTOR_SECRET_KEY="XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"\n$ export HECTOR_DSN="sqlite:///data.sqlite"\n```\n\nThe secret can be generated using the `token_hex()` function from\nthe Python\'s `secrets` module.\n\nAdditional Python database drivers might be required depending on the DSN.\n\nSee [the `settings` module](bl_hector/infrastructure/settings.py) for\na comprehensive list of configuration variables.\n\n\n## Authentication\n\nTo enable WebAuthn authentication, you must install extra dependencies (`bl-hector[webauthn]`)\nand enable it explicitly:\n\n```console\n$ export HECTOR_WEBAUTHN=1\n```\n\n\n## Initialise\n\nOnce configured, you must initialise Hector\'s database with the dedicated command:\n\n```console\n$ hector init-db\n```\n\n\n## Run\n\nHector being a Flask application, it can be run using any WSGI server,\nfor instance, with [Gunicorn](https://gunicorn.org):\n\n```console\n$ gunicorn --access-logfile="-" -w 4 -b 127.0.0.1:3000 "bl_hector.configuration.wsgi:app()"\n```\n',
     'author': 'Tanguy Le Carrour',
     'author_email': 'tanguy@bioneland.org',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
+    'extras_require': extras_require,
     'entry_points': entry_points,
     'python_requires': '>=3.9,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `bl_hector-0.1.0a2/PKG-INFO` & `bl_hector-0.1.0a3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: bl-hector
-Version: 0.1.0a2
+Version: 0.1.0a3
 Summary: A collection manager.
 License: AGPL-3.0-or-later
 Author: Tanguy Le Carrour
 Author-email: tanguy@bioneland.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
+Provides-Extra: webauthn
 Requires-Dist: Flask (>=2.3.2,<3.0.0)
 Requires-Dist: SQLAlchemy (>=2.0.15,<3.0.0)
 Requires-Dist: bl-seth (>=0.1.2,<0.2.0)
 Requires-Dist: bl3d (>=0.3.0,<0.4.0)
 Requires-Dist: fluent.runtime (>=0.4.0,<0.5.0)
 Requires-Dist: isbnlib (>=3.10.14,<4.0.0)
 Requires-Dist: jinja2-fragments (>=0.3.0,<0.4.0)
 Requires-Dist: pypugjs (>=5.9.12,<6.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
-Requires-Dist: webauthn (>=1.8.1,<2.0.0)
+Requires-Dist: webauthn (>=1.8.1,<2.0.0); extra == "webauthn"
 Description-Content-Type: text/markdown
 
 # Hector — a collection manager
 
 ## Install
 
 For the time being, Hector cannot be installed from PyPI.
@@ -45,14 +46,24 @@
 
 Additional Python database drivers might be required depending on the DSN.
 
 See [the `settings` module](bl_hector/infrastructure/settings.py) for
 a comprehensive list of configuration variables.
 
 
+## Authentication
+
+To enable WebAuthn authentication, you must install extra dependencies (`bl-hector[webauthn]`)
+and enable it explicitly:
+
+```console
+$ export HECTOR_WEBAUTHN=1
+```
+
+
 ## Initialise
 
 Once configured, you must initialise Hector's database with the dedicated command:
 
 ```console
 $ hector init-db
 ```
```

