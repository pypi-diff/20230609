# Comparing `tmp/Flaskel-3.1.0rc3.tar.gz` & `tmp/Flaskel-3.1.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flaskel-3.1.0rc3.tar", last modified: Mon Jun  5 00:39:53 2023, max compression
+gzip compressed data, was "Flaskel-3.1.0rc4.tar", last modified: Thu Jun  8 23:44:37 2023, max compression
```

## Comparing `Flaskel-3.1.0rc3.tar` & `Flaskel-3.1.0rc4.tar`

### file list

```diff
@@ -1,225 +1,225 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.035697 Flaskel-3.1.0rc3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.011697 Flaskel-3.1.0rc3/Flaskel.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15616 2023-06-05 00:39:52.000000 Flaskel-3.1.0rc3/Flaskel.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6189 2023-06-05 00:39:52.000000 Flaskel-3.1.0rc3/Flaskel.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 00:39:52.000000 Flaskel-3.1.0rc3/Flaskel.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2023-06-05 00:39:52.000000 Flaskel-3.1.0rc3/Flaskel.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 00:39:52.000000 Flaskel-3.1.0rc3/Flaskel.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      352 2023-06-05 00:39:52.000000 Flaskel-3.1.0rc3/Flaskel.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-05 00:39:52.000000 Flaskel-3.1.0rc3/Flaskel.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      146 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    15616 2023-06-05 00:39:53.035697 Flaskel-3.1.0rc3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    14795 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.013697 Flaskel-3.1.0rc3/flaskel/
--rw-rw-rw-   0 root         (0) root         (0)      709 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12101 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/builder.py
--rw-rw-rw-   0 root         (0) root         (0)     9072 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/config.py
--rw-rw-rw-   0 root         (0) root         (0)     1188 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/converters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.014697 Flaskel-3.1.0rc3/flaskel/ext/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7359 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/auth.py
--rw-rw-rw-   0 root         (0) root         (0)     4245 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/caching.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.014697 Flaskel-3.1.0rc3/flaskel/ext/cloudflare/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/cloudflare/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4239 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/cloudflare/remote.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.015697 Flaskel-3.1.0rc3/flaskel/ext/crypto/
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/crypto/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1710 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/crypto/argon.py
--rw-rw-rw-   0 root         (0) root         (0)      818 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/datetime.py
--rw-rw-rw-   0 root         (0) root         (0)     1200 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/default.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.015697 Flaskel-3.1.0rc3/flaskel/ext/errors/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/errors/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1954 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/errors/dispatchers.py
--rw-rw-rw-   0 root         (0) root         (0)     4349 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/errors/exception.py
--rw-rw-rw-   0 root         (0) root         (0)     7822 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/errors/handler.py
--rw-rw-rw-   0 root         (0) root         (0)     4499 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/errors/normalize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.016697 Flaskel-3.1.0rc3/flaskel/ext/healthcheck/
--rw-rw-rw-   0 root         (0) root         (0)      203 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/healthcheck/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6601 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/healthcheck/checkers.py
--rw-rw-rw-   0 root         (0) root         (0)     4889 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/healthcheck/health.py
--rw-rw-rw-   0 root         (0) root         (0)     7775 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/ipban.py
--rw-rw-rw-   0 root         (0) root         (0)     5351 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/jobs.py
--rw-rw-rw-   0 root         (0) root         (0)     1309 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/limit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.016697 Flaskel-3.1.0rc3/flaskel/ext/logging/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/logging/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.017697 Flaskel-3.1.0rc3/flaskel/ext/logging/builders/
--rw-rw-rw-   0 root         (0) root         (0)      295 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/logging/builders/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1744 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/logging/builders/base.py
--rw-rw-rw-   0 root         (0) root         (0)     2993 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/logging/builders/json.py
--rw-rw-rw-   0 root         (0) root         (0)     2864 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/logging/builders/text.py
--rw-rw-rw-   0 root         (0) root         (0)      951 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/logging/filters.py
--rw-rw-rw-   0 root         (0) root         (0)     1357 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/logging/formatters.py
--rw-rw-rw-   0 root         (0) root         (0)     1795 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/logging/handlers.py
--rw-rw-rw-   0 root         (0) root         (0)     4279 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/logging/logging.py
--rw-rw-rw-   0 root         (0) root         (0)     6005 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/mongo.py
--rw-rw-rw-   0 root         (0) root         (0)      978 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/redis.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.018697 Flaskel-3.1.0rc3/flaskel/ext/response/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/response/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7380 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/response/builder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.019697 Flaskel-3.1.0rc3/flaskel/ext/response/builders/
--rw-rw-rw-   0 root         (0) root         (0)      180 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/response/builders/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      768 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/response/builders/base64.py
--rw-rw-rw-   0 root         (0) root         (0)     1845 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/response/builders/builder.py
--rw-rw-rw-   0 root         (0) root         (0)     1973 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/response/builders/csv.py
--rw-rw-rw-   0 root         (0) root         (0)     1121 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/response/builders/html.py
--rw-rw-rw-   0 root         (0) root         (0)     1750 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/response/builders/json.py
--rw-rw-rw-   0 root         (0) root         (0)      740 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/response/builders/xml.py
--rw-rw-rw-   0 root         (0) root         (0)      906 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/response/builders/yaml.py
--rw-rw-rw-   0 root         (0) root         (0)     1648 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/response/config.py
--rw-rw-rw-   0 root         (0) root         (0)     1490 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/response/dictutils.py
--rw-rw-rw-   0 root         (0) root         (0)     1538 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/sendmail.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.019697 Flaskel-3.1.0rc3/flaskel/ext/sqlalchemy/
--rw-rw-rw-   0 root         (0) root         (0)       83 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/sqlalchemy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2414 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/sqlalchemy/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.019697 Flaskel-3.1.0rc3/flaskel/ext/templating/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/templating/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      367 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/templating/default.py
--rw-rw-rw-   0 root         (0) root         (0)     1646 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/templating/filters.py
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/templating/functions.py
--rw-rw-rw-   0 root         (0) root         (0)     2067 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/templating/support.py
--rw-rw-rw-   0 root         (0) root         (0)      953 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/useragent.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.020697 Flaskel-3.1.0rc3/flaskel/ext/websocket/
--rw-rw-rw-   0 root         (0) root         (0)      526 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/websocket/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.020697 Flaskel-3.1.0rc3/flaskel/extra/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/extra/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8975 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/extra/account.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.020697 Flaskel-3.1.0rc3/flaskel/extra/apidoc/
--rw-rw-rw-   0 root         (0) root         (0)       54 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/extra/apidoc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2521 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/extra/apidoc/template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.021697 Flaskel-3.1.0rc3/flaskel/extra/media/
--rw-rw-rw-   0 root         (0) root         (0)      111 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/extra/media/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       82 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/extra/media/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2127 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/extra/media/repo.py
--rw-rw-rw-   0 root         (0) root         (0)     2214 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/extra/media/service.py
--rw-rw-rw-   0 root         (0) root         (0)     1144 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/extra/media/view.py
--rw-rw-rw-   0 root         (0) root         (0)    11461 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/extra/mobile_support.py
--rw-rw-rw-   0 root         (0) root         (0)     5218 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/extra/notification.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.021697 Flaskel-3.1.0rc3/flaskel/extra/payments/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/extra/payments/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.022697 Flaskel-3.1.0rc3/flaskel/extra/payments/stripe/
--rw-rw-rw-   0 root         (0) root         (0)      135 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/extra/payments/stripe/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3498 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/extra/payments/stripe/handler.py
--rw-rw-rw-   0 root         (0) root         (0)     2831 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/extra/payments/stripe/repo.py
--rw-rw-rw-   0 root         (0) root         (0)     1374 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/extra/payments/stripe/view.py
--rw-rw-rw-   0 root         (0) root         (0)     4943 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/flaskel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.022697 Flaskel-3.1.0rc3/flaskel/http/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/http/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2223 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/http/client.py
--rw-rw-rw-   0 root         (0) root         (0)     9008 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/http/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     7220 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/middlewares.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.023697 Flaskel-3.1.0rc3/flaskel/scripts/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      253 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1425 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/init_app.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.010697 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.024697 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/resources/
--rw-rw-rw-   0 root         (0) root         (0)      305 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/resources/Caddyfile.example
--rw-rw-rw-   0 root         (0) root         (0)      532 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/resources/conf.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2271 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/resources/log.yaml
--rw-rw-rw-   0 root         (0) root         (0)      757 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/resources/manage.sh
--rw-rw-rw-   0 root         (0) root         (0)      414 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/resources/nginx.example
--rw-rw-rw-   0 root         (0) root         (0)     1561 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/resources/nuisances.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1325 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/resources/schemas.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1775 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/resources/settings.ini.sample
--rw-rw-rw-   0 root         (0) root         (0)      492 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/resources/supervisor.example
--rw-rw-rw-   0 root         (0) root         (0)    14323 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/resources/swagger.yaml
--rw-rw-rw-   0 root         (0) root         (0)      139 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/resources/uwsgi.yaml.example
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.024697 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.025697 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/ext/
--rw-rw-rw-   0 root         (0) root         (0)     1768 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/ext/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      434 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/ext/auth.py
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/ext/database.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.025697 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/forms/
--rw-rw-rw-   0 root         (0) root         (0)      330 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/forms/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.025697 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/models/
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      189 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/models/user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.026697 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/scripts/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/scripts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      685 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/scripts/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      504 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/scripts/config.py
--rw-rw-rw-   0 root         (0) root         (0)      915 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/scripts/ws.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.026697 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/tasks/
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      252 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.026697 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/
--rw-rw-rw-   0 root         (0) root         (0)      856 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1010 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/blueprints.py
--rw-rw-rw-   0 root         (0) root         (0)     1672 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.009697 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.026697 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/static/css/
--rw-rw-rw-   0 root         (0) root         (0)      190 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/static/css/main.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.027697 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/static/img/
--rw-rw-rw-   0 root         (0) root         (0)      318 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/static/img/favicon.ico
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.027697 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/static/js/
--rw-rw-rw-   0 root         (0) root         (0)       35 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/static/js/main.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.027697 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.027697 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/templates/core/
--rw-rw-rw-   0 root         (0) root         (0)      206 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/templates/core/error.html
--rw-rw-rw-   0 root         (0) root         (0)     1103 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/templates/core/head.html
--rw-rw-rw-   0 root         (0) root         (0)      655 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/templates/core/scripts.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.028697 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/templates/emails/
--rw-rw-rw-   0 root         (0) root         (0)      220 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/templates/emails/forgot.html
--rw-rw-rw-   0 root         (0) root         (0)      225 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/templates/emails/registration.html
--rw-rw-rw-   0 root         (0) root         (0)    13479 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/templates/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.028697 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/templates/layout/
--rw-rw-rw-   0 root         (0) root         (0)      458 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/templates/layout/base.html
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/templates/layout/container.html
--rw-rw-rw-   0 root         (0) root         (0)       20 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/templates/layout/footer.html
--rw-rw-rw-   0 root         (0) root         (0)       20 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/templates/layout/header.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.029697 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2434 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)      190 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/tests/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     2180 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/tests/test_smoke.py
--rw-rw-rw-   0 root         (0) root         (0)     5361 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/standalone.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.029697 Flaskel-3.1.0rc3/flaskel/tester/
--rw-rw-rw-   0 root         (0) root         (0)       31 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/tester/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1432 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/tester/client.py
--rw-rw-rw-   0 root         (0) root         (0)     7428 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/tester/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.030697 Flaskel-3.1.0rc3/flaskel/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2551 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/utils/datastruct.py
--rw-rw-rw-   0 root         (0) root         (0)     3513 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/utils/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.030697 Flaskel-3.1.0rc3/flaskel/utils/schemas/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/utils/schemas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5018 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/utils/schemas/default.py
--rw-rw-rw-   0 root         (0) root         (0)    34444 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/utils/schemas/openapi3.py
--rw-rw-rw-   0 root         (0) root         (0)     1420 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/utils/validator.py
--rw-rw-rw-   0 root         (0) root         (0)     2812 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/utils/webargs.py
--rw-rw-rw-   0 root         (0) root         (0)      256 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.031697 Flaskel-3.1.0rc3/flaskel/views/
--rw-rw-rw-   0 root         (0) root         (0)      105 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7046 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/views/base.py
--rw-rw-rw-   0 root         (0) root         (0)     9148 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/views/proxy.py
--rw-rw-rw-   0 root         (0) root         (0)     7866 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/views/resource.py
--rw-rw-rw-   0 root         (0) root         (0)     5689 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/views/rpc.py
--rw-rw-rw-   0 root         (0) root         (0)     1210 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/views/static.py
--rw-rw-rw-   0 root         (0) root         (0)     1185 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/views/template.py
--rw-rw-rw-   0 root         (0) root         (0)     2826 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/views/token.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.032697 Flaskel-3.1.0rc3/flaskel/wsgi/
--rw-rw-rw-   0 root         (0) root         (0)      102 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/wsgi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      861 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/wsgi/base.py
--rw-rw-rw-   0 root         (0) root         (0)      790 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/wsgi/factory.py
--rw-rw-rw-   0 root         (0) root         (0)      584 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/wsgi/wsgi_gevent.py
--rw-rw-rw-   0 root         (0) root         (0)     4389 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/wsgi/wsgi_gunicorn.py
--rw-rw-rw-   0 root         (0) root         (0)      656 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/wsgi/wsgi_tornado.py
--rw-rw-rw-   0 root         (0) root         (0)      856 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/wsgi/wsgi_twisted.py
--rw-rw-rw-   0 root         (0) root         (0)      411 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/wsgi/wsgi_waitress.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.034697 Flaskel-3.1.0rc3/requirements/
--rw-rw-rw-   0 root         (0) root         (0)       93 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/requirements/requirements-all.in
--rw-rw-rw-   0 root         (0) root         (0)    10050 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/requirements/requirements-all.txt
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/requirements/requirements-build.in
--rw-rw-rw-   0 root         (0) root         (0)     3256 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/requirements/requirements-build.txt
--rw-rw-rw-   0 root         (0) root         (0)      413 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/requirements/requirements-dev.in
--rw-rw-rw-   0 root         (0) root         (0)     6727 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/requirements/requirements-dev.txt
--rw-rw-rw-   0 root         (0) root         (0)      139 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/requirements/requirements-extra.in
--rw-rw-rw-   0 root         (0) root         (0)     3155 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/requirements/requirements-extra.txt
--rw-rw-rw-   0 root         (0) root         (0)       84 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/requirements/requirements-test.in
--rw-rw-rw-   0 root         (0) root         (0)     1417 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/requirements/requirements-test.txt
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/requirements/requirements-wsgi.in
--rw-rw-rw-   0 root         (0) root         (0)     1141 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/requirements/requirements-wsgi.txt
--rw-rw-rw-   0 root         (0) root         (0)      182 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/requirements/requirements.in
--rw-rw-rw-   0 root         (0) root         (0)     4329 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/requirements/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-05 00:39:53.035697 Flaskel-3.1.0rc3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     4682 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 23:44:37.632580 Flaskel-3.1.0rc4/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 23:44:37.598581 Flaskel-3.1.0rc4/Flaskel.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15616 2023-06-08 23:44:37.000000 Flaskel-3.1.0rc4/Flaskel.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6189 2023-06-08 23:44:37.000000 Flaskel-3.1.0rc4/Flaskel.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 23:44:37.000000 Flaskel-3.1.0rc4/Flaskel.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2023-06-08 23:44:37.000000 Flaskel-3.1.0rc4/Flaskel.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 23:44:37.000000 Flaskel-3.1.0rc4/Flaskel.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      349 2023-06-08 23:44:37.000000 Flaskel-3.1.0rc4/Flaskel.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-08 23:44:37.000000 Flaskel-3.1.0rc4/Flaskel.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      146 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    15616 2023-06-08 23:44:37.631580 Flaskel-3.1.0rc4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    14795 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 23:44:37.600581 Flaskel-3.1.0rc4/flaskel/
+-rw-rw-rw-   0 root         (0) root         (0)      709 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12101 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/builder.py
+-rw-rw-rw-   0 root         (0) root         (0)     9072 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1188 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/converters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 23:44:37.602581 Flaskel-3.1.0rc4/flaskel/ext/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/ext/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7359 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/ext/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)     4245 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/ext/caching.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 23:44:37.603581 Flaskel-3.1.0rc4/flaskel/ext/cloudflare/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/ext/cloudflare/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4239 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/ext/cloudflare/remote.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 23:44:37.603581 Flaskel-3.1.0rc4/flaskel/ext/crypto/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/ext/crypto/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1710 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/ext/crypto/argon.py
+-rw-rw-rw-   0 root         (0) root         (0)      818 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/ext/datetime.py
+-rw-rw-rw-   0 root         (0) root         (0)     1200 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/ext/default.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 23:44:37.604581 Flaskel-3.1.0rc4/flaskel/ext/errors/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/ext/errors/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1954 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/ext/errors/dispatchers.py
+-rw-rw-rw-   0 root         (0) root         (0)     4349 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/ext/errors/exception.py
+-rw-rw-rw-   0 root         (0) root         (0)     7822 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/ext/errors/handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     4499 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/ext/errors/normalize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 23:44:37.605581 Flaskel-3.1.0rc4/flaskel/ext/healthcheck/
+-rw-rw-rw-   0 root         (0) root         (0)      203 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/ext/healthcheck/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6601 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/ext/healthcheck/checkers.py
+-rw-rw-rw-   0 root         (0) root         (0)     4889 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/ext/healthcheck/health.py
+-rw-rw-rw-   0 root         (0) root         (0)     7775 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/ext/ipban.py
+-rw-rw-rw-   0 root         (0) root         (0)     5351 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/ext/jobs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1309 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/ext/limit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 23:44:37.606581 Flaskel-3.1.0rc4/flaskel/ext/logging/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/ext/logging/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 23:44:37.606581 Flaskel-3.1.0rc4/flaskel/ext/logging/builders/
+-rw-rw-rw-   0 root         (0) root         (0)      295 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/ext/logging/builders/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1744 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/ext/logging/builders/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2993 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/ext/logging/builders/json.py
+-rw-rw-rw-   0 root         (0) root         (0)     2864 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/ext/logging/builders/text.py
+-rw-rw-rw-   0 root         (0) root         (0)      951 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/ext/logging/filters.py
+-rw-rw-rw-   0 root         (0) root         (0)     1357 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/ext/logging/formatters.py
+-rw-rw-rw-   0 root         (0) root         (0)     1795 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/ext/logging/handlers.py
+-rw-rw-rw-   0 root         (0) root         (0)     4279 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/ext/logging/logging.py
+-rw-rw-rw-   0 root         (0) root         (0)     6005 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/ext/mongo.py
+-rw-rw-rw-   0 root         (0) root         (0)      978 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/ext/redis.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 23:44:37.607581 Flaskel-3.1.0rc4/flaskel/ext/response/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/ext/response/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7380 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/ext/response/builder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 23:44:37.609581 Flaskel-3.1.0rc4/flaskel/ext/response/builders/
+-rw-rw-rw-   0 root         (0) root         (0)      180 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/ext/response/builders/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      768 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/ext/response/builders/base64.py
+-rw-rw-rw-   0 root         (0) root         (0)     1845 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/ext/response/builders/builder.py
+-rw-rw-rw-   0 root         (0) root         (0)     1973 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/ext/response/builders/csv.py
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/ext/response/builders/html.py
+-rw-rw-rw-   0 root         (0) root         (0)     1750 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/ext/response/builders/json.py
+-rw-rw-rw-   0 root         (0) root         (0)      740 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/ext/response/builders/xml.py
+-rw-rw-rw-   0 root         (0) root         (0)      906 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/ext/response/builders/yaml.py
+-rw-rw-rw-   0 root         (0) root         (0)     1648 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/ext/response/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1490 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/ext/response/dictutils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1538 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/ext/sendmail.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 23:44:37.609581 Flaskel-3.1.0rc4/flaskel/ext/sqlalchemy/
+-rw-rw-rw-   0 root         (0) root         (0)       83 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/ext/sqlalchemy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2414 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/ext/sqlalchemy/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 23:44:37.610581 Flaskel-3.1.0rc4/flaskel/ext/templating/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/ext/templating/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      367 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/ext/templating/default.py
+-rw-rw-rw-   0 root         (0) root         (0)     1646 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/ext/templating/filters.py
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/ext/templating/functions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2067 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/ext/templating/support.py
+-rw-rw-rw-   0 root         (0) root         (0)      953 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/ext/useragent.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 23:44:37.611581 Flaskel-3.1.0rc4/flaskel/ext/websocket/
+-rw-rw-rw-   0 root         (0) root         (0)      526 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/ext/websocket/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 23:44:37.611581 Flaskel-3.1.0rc4/flaskel/extra/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/extra/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8975 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/extra/account.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 23:44:37.612581 Flaskel-3.1.0rc4/flaskel/extra/apidoc/
+-rw-rw-rw-   0 root         (0) root         (0)       54 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/extra/apidoc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2521 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/extra/apidoc/template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 23:44:37.613581 Flaskel-3.1.0rc4/flaskel/extra/media/
+-rw-rw-rw-   0 root         (0) root         (0)      111 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/extra/media/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       82 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/extra/media/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2127 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/extra/media/repo.py
+-rw-rw-rw-   0 root         (0) root         (0)     2214 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/extra/media/service.py
+-rw-rw-rw-   0 root         (0) root         (0)     1144 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/extra/media/view.py
+-rw-rw-rw-   0 root         (0) root         (0)    11461 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/extra/mobile_support.py
+-rw-rw-rw-   0 root         (0) root         (0)     5218 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/extra/notification.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 23:44:37.613581 Flaskel-3.1.0rc4/flaskel/extra/payments/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/extra/payments/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 23:44:37.614580 Flaskel-3.1.0rc4/flaskel/extra/payments/stripe/
+-rw-rw-rw-   0 root         (0) root         (0)      135 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/extra/payments/stripe/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3498 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/extra/payments/stripe/handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     2831 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/extra/payments/stripe/repo.py
+-rw-rw-rw-   0 root         (0) root         (0)     1374 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/extra/payments/stripe/view.py
+-rw-rw-rw-   0 root         (0) root         (0)     4943 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/flaskel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 23:44:37.615581 Flaskel-3.1.0rc4/flaskel/http/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/http/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2223 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/http/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     9008 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/http/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     7220 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/middlewares.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 23:44:37.615581 Flaskel-3.1.0rc4/flaskel/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/scripts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      253 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/scripts/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1425 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/scripts/init_app.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 23:44:37.596581 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 23:44:37.617581 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/resources/
+-rw-rw-rw-   0 root         (0) root         (0)      305 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/resources/Caddyfile.example
+-rw-rw-rw-   0 root         (0) root         (0)      532 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/resources/conf.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2271 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/resources/log.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      757 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/resources/manage.sh
+-rw-rw-rw-   0 root         (0) root         (0)      414 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/resources/nginx.example
+-rw-rw-rw-   0 root         (0) root         (0)     1561 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/resources/nuisances.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1325 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/resources/schemas.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1775 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/resources/settings.ini.sample
+-rw-rw-rw-   0 root         (0) root         (0)      492 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/resources/supervisor.example
+-rw-rw-rw-   0 root         (0) root         (0)    14323 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/resources/swagger.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      139 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/resources/uwsgi.yaml.example
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 23:44:37.617581 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/skel/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 23:44:37.618580 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/skel/ext/
+-rw-rw-rw-   0 root         (0) root         (0)     1768 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/skel/ext/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      434 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/skel/ext/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/skel/ext/database.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 23:44:37.618580 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/skel/forms/
+-rw-rw-rw-   0 root         (0) root         (0)      330 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/skel/forms/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 23:44:37.619581 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/skel/models/
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/skel/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      189 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/skel/models/user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 23:44:37.619581 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/skel/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/skel/scripts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      685 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/skel/scripts/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      504 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/skel/scripts/config.py
+-rw-rw-rw-   0 root         (0) root         (0)      915 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/skel/scripts/ws.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 23:44:37.620581 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/skel/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/skel/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      252 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/skel/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 23:44:37.620581 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/skel/views/
+-rw-rw-rw-   0 root         (0) root         (0)      856 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/skel/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1010 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/skel/views/blueprints.py
+-rw-rw-rw-   0 root         (0) root         (0)     1672 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/skel/views/common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 23:44:37.596581 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/skel/views/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 23:44:37.620581 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/skel/views/static/css/
+-rw-rw-rw-   0 root         (0) root         (0)      190 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/skel/views/static/css/main.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 23:44:37.621580 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/skel/views/static/img/
+-rw-rw-rw-   0 root         (0) root         (0)      318 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/skel/views/static/img/favicon.ico
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 23:44:37.621580 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/skel/views/static/js/
+-rw-rw-rw-   0 root         (0) root         (0)       35 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/skel/views/static/js/main.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 23:44:37.621580 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/skel/views/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 23:44:37.622580 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/skel/views/templates/core/
+-rw-rw-rw-   0 root         (0) root         (0)      206 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/skel/views/templates/core/error.html
+-rw-rw-rw-   0 root         (0) root         (0)     1103 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/skel/views/templates/core/head.html
+-rw-rw-rw-   0 root         (0) root         (0)      655 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/skel/views/templates/core/scripts.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 23:44:37.622580 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/skel/views/templates/emails/
+-rw-rw-rw-   0 root         (0) root         (0)      220 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/skel/views/templates/emails/forgot.html
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/skel/views/templates/emails/registration.html
+-rw-rw-rw-   0 root         (0) root         (0)    13479 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/skel/views/templates/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 23:44:37.623581 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/skel/views/templates/layout/
+-rw-rw-rw-   0 root         (0) root         (0)      458 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/skel/views/templates/layout/base.html
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/skel/views/templates/layout/container.html
+-rw-rw-rw-   0 root         (0) root         (0)       20 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/skel/views/templates/layout/footer.html
+-rw-rw-rw-   0 root         (0) root         (0)       20 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/skel/views/templates/layout/header.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 23:44:37.624580 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2434 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)      190 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/tests/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2180 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/scripts/skeleton/tests/test_smoke.py
+-rw-rw-rw-   0 root         (0) root         (0)     5361 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/standalone.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 23:44:37.624580 Flaskel-3.1.0rc4/flaskel/tester/
+-rw-rw-rw-   0 root         (0) root         (0)       31 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/tester/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1432 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/tester/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     7428 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/tester/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 23:44:37.625580 Flaskel-3.1.0rc4/flaskel/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2551 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/utils/datastruct.py
+-rw-rw-rw-   0 root         (0) root         (0)     3513 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/utils/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 23:44:37.626581 Flaskel-3.1.0rc4/flaskel/utils/schemas/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/utils/schemas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5018 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/utils/schemas/default.py
+-rw-rw-rw-   0 root         (0) root         (0)    34444 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/utils/schemas/openapi3.py
+-rw-rw-rw-   0 root         (0) root         (0)     1420 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/utils/validator.py
+-rw-rw-rw-   0 root         (0) root         (0)     2812 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/utils/webargs.py
+-rw-rw-rw-   0 root         (0) root         (0)      256 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 23:44:37.627581 Flaskel-3.1.0rc4/flaskel/views/
+-rw-rw-rw-   0 root         (0) root         (0)      105 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7046 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/views/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     9148 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/views/proxy.py
+-rw-rw-rw-   0 root         (0) root         (0)     7866 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/views/resource.py
+-rw-rw-rw-   0 root         (0) root         (0)     5689 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/views/rpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1210 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/views/static.py
+-rw-rw-rw-   0 root         (0) root         (0)     1185 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/views/template.py
+-rw-rw-rw-   0 root         (0) root         (0)     2826 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/views/token.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 23:44:37.629580 Flaskel-3.1.0rc4/flaskel/wsgi/
+-rw-rw-rw-   0 root         (0) root         (0)      102 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/wsgi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      861 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/wsgi/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      790 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/wsgi/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)      584 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/wsgi/wsgi_gevent.py
+-rw-rw-rw-   0 root         (0) root         (0)     4389 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/wsgi/wsgi_gunicorn.py
+-rw-rw-rw-   0 root         (0) root         (0)      656 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/wsgi/wsgi_tornado.py
+-rw-rw-rw-   0 root         (0) root         (0)      856 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/wsgi/wsgi_twisted.py
+-rw-rw-rw-   0 root         (0) root         (0)      411 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/flaskel/wsgi/wsgi_waitress.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 23:44:37.631580 Flaskel-3.1.0rc4/requirements/
+-rw-rw-rw-   0 root         (0) root         (0)       93 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/requirements/requirements-all.in
+-rw-rw-rw-   0 root         (0) root         (0)    10047 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/requirements/requirements-all.txt
+-rw-rw-rw-   0 root         (0) root         (0)       16 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/requirements/requirements-build.in
+-rw-rw-rw-   0 root         (0) root         (0)     2040 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/requirements/requirements-build.txt
+-rw-rw-rw-   0 root         (0) root         (0)      413 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/requirements/requirements-dev.in
+-rw-rw-rw-   0 root         (0) root         (0)     6727 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/requirements/requirements-dev.txt
+-rw-rw-rw-   0 root         (0) root         (0)      139 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/requirements/requirements-extra.in
+-rw-rw-rw-   0 root         (0) root         (0)     3155 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/requirements/requirements-extra.txt
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/requirements/requirements-test.in
+-rw-rw-rw-   0 root         (0) root         (0)     1417 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/requirements/requirements-test.txt
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/requirements/requirements-wsgi.in
+-rw-rw-rw-   0 root         (0) root         (0)     1141 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/requirements/requirements-wsgi.txt
+-rw-rw-rw-   0 root         (0) root         (0)      206 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/requirements/requirements.in
+-rw-rw-rw-   0 root         (0) root         (0)     5111 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/requirements/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-08 23:44:37.632580 Flaskel-3.1.0rc4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     4682 2023-06-08 23:44:25.000000 Flaskel-3.1.0rc4/setup.py
```

### Comparing `Flaskel-3.1.0rc3/Flaskel.egg-info/PKG-INFO` & `Flaskel-3.1.0rc4/Flaskel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flaskel
-Version: 3.1.0rc3
+Version: 3.1.0rc4
 Summary: Skeleton for flask applications
 Home-page: https://github.com/cs91chris/flaskel
 Author: cs91chris
 Author-email: cs91chris@voidbrain.me
 License: MIT
 Platform: any
 Classifier: Environment :: Web Environment
```

### Comparing `Flaskel-3.1.0rc3/Flaskel.egg-info/SOURCES.txt` & `Flaskel-3.1.0rc4/Flaskel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/PKG-INFO` & `Flaskel-3.1.0rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flaskel
-Version: 3.1.0rc3
+Version: 3.1.0rc4
 Summary: Skeleton for flask applications
 Home-page: https://github.com/cs91chris/flaskel
 Author: cs91chris
 Author-email: cs91chris@voidbrain.me
 License: MIT
 Platform: any
 Classifier: Environment :: Web Environment
```

### Comparing `Flaskel-3.1.0rc3/README.md` & `Flaskel-3.1.0rc4/README.md`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/__init__.py` & `Flaskel-3.1.0rc4/flaskel/__init__.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/builder.py` & `Flaskel-3.1.0rc4/flaskel/builder.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/config.py` & `Flaskel-3.1.0rc4/flaskel/config.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/converters.py` & `Flaskel-3.1.0rc4/flaskel/converters.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/ext/auth.py` & `Flaskel-3.1.0rc4/flaskel/ext/auth.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/ext/caching.py` & `Flaskel-3.1.0rc4/flaskel/ext/caching.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/ext/cloudflare/remote.py` & `Flaskel-3.1.0rc4/flaskel/ext/cloudflare/remote.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/ext/crypto/argon.py` & `Flaskel-3.1.0rc4/flaskel/ext/crypto/argon.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/ext/datetime.py` & `Flaskel-3.1.0rc4/flaskel/ext/datetime.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/ext/default.py` & `Flaskel-3.1.0rc4/flaskel/ext/default.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/ext/errors/dispatchers.py` & `Flaskel-3.1.0rc4/flaskel/ext/errors/dispatchers.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/ext/errors/exception.py` & `Flaskel-3.1.0rc4/flaskel/ext/errors/exception.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/ext/errors/handler.py` & `Flaskel-3.1.0rc4/flaskel/ext/errors/handler.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/ext/errors/normalize.py` & `Flaskel-3.1.0rc4/flaskel/ext/errors/normalize.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/ext/healthcheck/checkers.py` & `Flaskel-3.1.0rc4/flaskel/ext/healthcheck/checkers.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/ext/healthcheck/health.py` & `Flaskel-3.1.0rc4/flaskel/ext/healthcheck/health.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/ext/ipban.py` & `Flaskel-3.1.0rc4/flaskel/ext/ipban.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/ext/jobs.py` & `Flaskel-3.1.0rc4/flaskel/ext/jobs.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/ext/limit.py` & `Flaskel-3.1.0rc4/flaskel/ext/limit.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/ext/logging/builders/base.py` & `Flaskel-3.1.0rc4/flaskel/ext/logging/builders/base.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/ext/logging/builders/json.py` & `Flaskel-3.1.0rc4/flaskel/ext/logging/builders/json.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/ext/logging/builders/text.py` & `Flaskel-3.1.0rc4/flaskel/ext/logging/builders/text.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/ext/logging/filters.py` & `Flaskel-3.1.0rc4/flaskel/ext/logging/filters.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/ext/logging/formatters.py` & `Flaskel-3.1.0rc4/flaskel/ext/logging/formatters.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/ext/logging/handlers.py` & `Flaskel-3.1.0rc4/flaskel/ext/logging/handlers.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/ext/logging/logging.py` & `Flaskel-3.1.0rc4/flaskel/ext/logging/logging.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/ext/mongo.py` & `Flaskel-3.1.0rc4/flaskel/ext/mongo.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/ext/redis.py` & `Flaskel-3.1.0rc4/flaskel/ext/redis.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/ext/response/builder.py` & `Flaskel-3.1.0rc4/flaskel/ext/response/builder.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/ext/response/builders/base64.py` & `Flaskel-3.1.0rc4/flaskel/ext/response/builders/base64.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/ext/response/builders/builder.py` & `Flaskel-3.1.0rc4/flaskel/ext/response/builders/builder.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/ext/response/builders/csv.py` & `Flaskel-3.1.0rc4/flaskel/ext/response/builders/csv.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/ext/response/builders/html.py` & `Flaskel-3.1.0rc4/flaskel/ext/response/builders/html.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/ext/response/builders/json.py` & `Flaskel-3.1.0rc4/flaskel/ext/response/builders/json.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/ext/response/builders/xml.py` & `Flaskel-3.1.0rc4/flaskel/ext/response/builders/xml.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/ext/response/builders/yaml.py` & `Flaskel-3.1.0rc4/flaskel/ext/response/builders/yaml.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/ext/response/config.py` & `Flaskel-3.1.0rc4/flaskel/ext/response/config.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/ext/response/dictutils.py` & `Flaskel-3.1.0rc4/flaskel/ext/response/dictutils.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/ext/sendmail.py` & `Flaskel-3.1.0rc4/flaskel/ext/sendmail.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/ext/sqlalchemy/model.py` & `Flaskel-3.1.0rc4/flaskel/ext/sqlalchemy/model.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/ext/templating/filters.py` & `Flaskel-3.1.0rc4/flaskel/ext/templating/filters.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/ext/templating/support.py` & `Flaskel-3.1.0rc4/flaskel/ext/templating/support.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/ext/useragent.py` & `Flaskel-3.1.0rc4/flaskel/ext/useragent.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/ext/websocket/__init__.py` & `Flaskel-3.1.0rc4/flaskel/ext/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/extra/account.py` & `Flaskel-3.1.0rc4/flaskel/extra/account.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/extra/apidoc/template.py` & `Flaskel-3.1.0rc4/flaskel/extra/apidoc/template.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/extra/media/repo.py` & `Flaskel-3.1.0rc4/flaskel/extra/media/repo.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/extra/media/service.py` & `Flaskel-3.1.0rc4/flaskel/extra/media/service.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/extra/media/view.py` & `Flaskel-3.1.0rc4/flaskel/extra/media/view.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/extra/mobile_support.py` & `Flaskel-3.1.0rc4/flaskel/extra/mobile_support.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/extra/notification.py` & `Flaskel-3.1.0rc4/flaskel/extra/notification.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/extra/payments/stripe/handler.py` & `Flaskel-3.1.0rc4/flaskel/extra/payments/stripe/handler.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/extra/payments/stripe/repo.py` & `Flaskel-3.1.0rc4/flaskel/extra/payments/stripe/repo.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/extra/payments/stripe/view.py` & `Flaskel-3.1.0rc4/flaskel/extra/payments/stripe/view.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/flaskel.py` & `Flaskel-3.1.0rc4/flaskel/flaskel.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/http/client.py` & `Flaskel-3.1.0rc4/flaskel/http/client.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/http/exceptions.py` & `Flaskel-3.1.0rc4/flaskel/http/exceptions.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/middlewares.py` & `Flaskel-3.1.0rc4/flaskel/middlewares.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/scripts/init_app.py` & `Flaskel-3.1.0rc4/flaskel/scripts/init_app.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/scripts/skeleton/resources/conf.yaml` & `Flaskel-3.1.0rc4/flaskel/scripts/skeleton/resources/conf.yaml`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/scripts/skeleton/resources/log.yaml` & `Flaskel-3.1.0rc4/flaskel/scripts/skeleton/resources/log.yaml`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/scripts/skeleton/resources/manage.sh` & `Flaskel-3.1.0rc4/flaskel/scripts/skeleton/resources/manage.sh`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/scripts/skeleton/resources/nuisances.yaml` & `Flaskel-3.1.0rc4/flaskel/scripts/skeleton/resources/nuisances.yaml`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/scripts/skeleton/resources/schemas.yaml` & `Flaskel-3.1.0rc4/flaskel/scripts/skeleton/resources/schemas.yaml`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/scripts/skeleton/resources/settings.ini.sample` & `Flaskel-3.1.0rc4/flaskel/scripts/skeleton/resources/settings.ini.sample`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/scripts/skeleton/resources/swagger.yaml` & `Flaskel-3.1.0rc4/flaskel/scripts/skeleton/resources/swagger.yaml`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/ext/__init__.py` & `Flaskel-3.1.0rc4/flaskel/scripts/skeleton/skel/ext/__init__.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/scripts/cli.py` & `Flaskel-3.1.0rc4/flaskel/scripts/skeleton/skel/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/scripts/ws.py` & `Flaskel-3.1.0rc4/flaskel/scripts/skeleton/skel/scripts/ws.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/__init__.py` & `Flaskel-3.1.0rc4/flaskel/scripts/skeleton/skel/views/__init__.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/blueprints.py` & `Flaskel-3.1.0rc4/flaskel/scripts/skeleton/skel/views/blueprints.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/common.py` & `Flaskel-3.1.0rc4/flaskel/scripts/skeleton/skel/views/common.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/templates/core/head.html` & `Flaskel-3.1.0rc4/flaskel/scripts/skeleton/skel/views/templates/core/head.html`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/templates/core/scripts.html` & `Flaskel-3.1.0rc4/flaskel/scripts/skeleton/skel/views/templates/core/scripts.html`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/templates/index.html` & `Flaskel-3.1.0rc4/flaskel/scripts/skeleton/skel/views/templates/index.html`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/scripts/skeleton/tests/conftest.py` & `Flaskel-3.1.0rc4/flaskel/scripts/skeleton/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/scripts/skeleton/tests/test_smoke.py` & `Flaskel-3.1.0rc4/flaskel/scripts/skeleton/tests/test_smoke.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/standalone.py` & `Flaskel-3.1.0rc4/flaskel/standalone.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/tester/client.py` & `Flaskel-3.1.0rc4/flaskel/tester/client.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/tester/helpers.py` & `Flaskel-3.1.0rc4/flaskel/tester/helpers.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/utils/datastruct.py` & `Flaskel-3.1.0rc4/flaskel/utils/datastruct.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/utils/logger.py` & `Flaskel-3.1.0rc4/flaskel/utils/logger.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/utils/schemas/default.py` & `Flaskel-3.1.0rc4/flaskel/utils/schemas/default.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/utils/schemas/openapi3.py` & `Flaskel-3.1.0rc4/flaskel/utils/schemas/openapi3.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/utils/validator.py` & `Flaskel-3.1.0rc4/flaskel/utils/validator.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/utils/webargs.py` & `Flaskel-3.1.0rc4/flaskel/utils/webargs.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/views/base.py` & `Flaskel-3.1.0rc4/flaskel/views/base.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/views/proxy.py` & `Flaskel-3.1.0rc4/flaskel/views/proxy.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/views/resource.py` & `Flaskel-3.1.0rc4/flaskel/views/resource.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/views/rpc.py` & `Flaskel-3.1.0rc4/flaskel/views/rpc.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/views/static.py` & `Flaskel-3.1.0rc4/flaskel/views/static.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/views/template.py` & `Flaskel-3.1.0rc4/flaskel/views/template.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/views/token.py` & `Flaskel-3.1.0rc4/flaskel/views/token.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/wsgi/base.py` & `Flaskel-3.1.0rc4/flaskel/wsgi/base.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/wsgi/factory.py` & `Flaskel-3.1.0rc4/flaskel/wsgi/factory.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/wsgi/wsgi_gevent.py` & `Flaskel-3.1.0rc4/flaskel/wsgi/wsgi_gevent.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/wsgi/wsgi_gunicorn.py` & `Flaskel-3.1.0rc4/flaskel/wsgi/wsgi_gunicorn.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/wsgi/wsgi_tornado.py` & `Flaskel-3.1.0rc4/flaskel/wsgi/wsgi_tornado.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/flaskel/wsgi/wsgi_twisted.py` & `Flaskel-3.1.0rc4/flaskel/wsgi/wsgi_twisted.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc3/requirements/requirements-all.txt` & `Flaskel-3.1.0rc4/requirements/requirements-all.txt`

 * *Files 1% similar despite different names*

```diff
@@ -204,15 +204,15 @@
     # via
     #   -r requirements/requirements.txt
     #   flask-limiter
 markdown-it-py==2.2.0
     # via
     #   -r requirements/requirements.txt
     #   rich
-markupsafe==2.1.2
+markupsafe==2.1.3
     # via
     #   -r requirements/requirements-extra.txt
     #   -r requirements/requirements.txt
     #   jinja2
     #   werkzeug
 marshmallow==3.19.0
     # via
@@ -328,15 +328,15 @@
 requests==2.31.0
     # via
     #   -r requirements/requirements-extra.txt
     #   -r requirements/requirements.txt
     #   pyfcm
     #   stripe
     #   vbcore
-rich==13.3.5
+rich==13.4.1
     # via
     #   -r requirements/requirements.txt
     #   flask-limiter
 rule-engine==3.5.1
     # via
     #   -r requirements/requirements.txt
     #   vbcore
@@ -354,43 +354,43 @@
     #   vbcore
 sqlalchemy-schemadisplay==1.3
     # via
     #   -r requirements/requirements.txt
     #   vbcore
 stripe==5.4.0
     # via -r requirements/requirements-extra.txt
-typing-extensions==4.6.2
+typing-extensions==4.6.3
     # via
     #   -r requirements/requirements.txt
     #   flask-limiter
     #   limits
 tzlocal==5.0.1
     # via
     #   -r requirements/requirements-extra.txt
     #   -r requirements/requirements.txt
     #   apscheduler
 ua-parser==0.16.1
     # via
     #   -r requirements/requirements.txt
     #   user-agents
-urllib3==2.0.2
+urllib3==2.0.3
     # via
     #   -r requirements/requirements-extra.txt
     #   -r requirements/requirements.txt
     #   pyfcm
     #   requests
 user-agents==2.2.0
     # via
     #   -r requirements/requirements.txt
     #   vbcore
-vbcore[all]==2.0.0rc4
+vbcore[all]==2.0.0
     # via -r requirements/requirements.txt
 webargs==8.2.0
     # via -r requirements/requirements.txt
-werkzeug==2.3.4
+werkzeug==2.3.6
     # via
     #   -r requirements/requirements-extra.txt
     #   -r requirements/requirements.txt
     #   flask
     #   flask-jwt-extended
 wrapt==1.15.0
     # via
```

### Comparing `Flaskel-3.1.0rc3/requirements/requirements-build.txt` & `Flaskel-3.1.0rc4/requirements/requirements-extra.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,147 +1,130 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --no-emit-index-url --no-emit-trusted-host --output-file=requirements/requirements-build.txt --resolver=backtracking requirements/requirements-build.in
+#    pip-compile --no-emit-index-url --no-emit-trusted-host --output-file=requirements/requirements-extra.txt --resolver=backtracking requirements/requirements-extra.in
 #
-bleach==6.0.0
-    # via readme-renderer
-cachetools==5.3.1
+apscheduler==3.10.1
     # via
-    #   -c requirements/requirements-dev.txt
-    #   tox
+    #   -c requirements/requirements.txt
+    #   flask-apscheduler
+async-timeout==4.0.2
+    # via
+    #   -c requirements/requirements.txt
+    #   redis
+bidict==0.22.1
+    # via python-socketio
+blinker==1.6.2
+    # via flask-mail
 certifi==2023.5.7
     # via
-    #   -c requirements/requirements-dev.txt
+    #   -c requirements/requirements.txt
     #   requests
-cffi==1.15.1
-    # via
-    #   -c requirements/requirements-dev.txt
-    #   cryptography
-chardet==5.1.0
-    # via
-    #   -c requirements/requirements-dev.txt
-    #   tox
 charset-normalizer==3.1.0
     # via
-    #   -c requirements/requirements-dev.txt
+    #   -c requirements/requirements.txt
     #   requests
-colorama==0.4.6
+click==8.1.3
     # via
-    #   -c requirements/requirements-dev.txt
-    #   tox
-cryptography==41.0.1
-    # via
-    #   -c requirements/requirements-dev.txt
-    #   secretstorage
-distlib==0.3.6
-    # via
-    #   -c requirements/requirements-dev.txt
-    #   virtualenv
-docutils==0.20.1
-    # via readme-renderer
-filelock==3.12.0
-    # via
-    #   -c requirements/requirements-dev.txt
-    #   tox
-    #   virtualenv
+    #   -c requirements/requirements.txt
+    #   flask
+dnspython==2.3.0
+    # via
+    #   -c requirements/requirements.txt
+    #   pymongo
+flask==2.2.5
+    # via
+    #   -c requirements/requirements.txt
+    #   flask-apscheduler
+    #   flask-mail
+    #   flask-pymongo
+    #   flask-socketio
+flask-apscheduler==1.12.4
+    # via -r requirements/requirements-extra.in
+flask-mail==0.9.1
+    # via -r requirements/requirements-extra.in
+flask-pymongo==2.3.0
+    # via -r requirements/requirements-extra.in
+flask-socketio==5.3.4
+    # via -r requirements/requirements-extra.in
+gevent==22.10.2
+    # via
+    #   -r requirements/requirements-extra.in
+    #   gevent-websocket
+gevent-websocket==0.10.1
+    # via -r requirements/requirements-extra.in
+greenlet==2.0.2
+    # via
+    #   -c requirements/requirements.txt
+    #   gevent
+gunicorn==20.1.0
+    # via -r requirements/requirements-extra.in
+hiredis==2.2.3
+    # via -r requirements/requirements-extra.in
 idna==3.4
     # via
-    #   -c requirements/requirements-dev.txt
+    #   -c requirements/requirements.txt
     #   requests
-importlib-metadata==6.6.0
+itsdangerous==2.1.2
     # via
-    #   keyring
-    #   twine
-jaraco-classes==3.2.3
-    # via keyring
-jeepney==0.8.0
-    # via
-    #   keyring
-    #   secretstorage
-keyring==23.13.1
-    # via twine
-markdown-it-py==2.2.0
-    # via
-    #   -c requirements/requirements-dev.txt
-    #   rich
-mdurl==0.1.2
-    # via
-    #   -c requirements/requirements-dev.txt
-    #   markdown-it-py
-more-itertools==9.1.0
-    # via jaraco-classes
-packaging==23.1
-    # via
-    #   -c requirements/requirements-dev.txt
-    #   pyproject-api
-    #   tox
-pkginfo==1.9.6
-    # via twine
-platformdirs==3.5.1
-    # via
-    #   -c requirements/requirements-dev.txt
-    #   tox
-    #   virtualenv
-pluggy==1.0.0
-    # via
-    #   -c requirements/requirements-dev.txt
-    #   tox
-pycparser==2.21
-    # via
-    #   -c requirements/requirements-dev.txt
-    #   cffi
-pygments==2.15.1
-    # via
-    #   -c requirements/requirements-dev.txt
-    #   readme-renderer
-    #   rich
-pyproject-api==1.5.1
-    # via
-    #   -c requirements/requirements-dev.txt
-    #   tox
-readme-renderer==37.3
-    # via twine
+    #   -c requirements/requirements.txt
+    #   flask
+jinja2==3.1.2
+    # via
+    #   -c requirements/requirements.txt
+    #   flask
+markupsafe==2.1.3
+    # via
+    #   -c requirements/requirements.txt
+    #   jinja2
+    #   werkzeug
+pyfcm==1.5.4
+    # via -r requirements/requirements-extra.in
+pymongo==4.3.3
+    # via flask-pymongo
+python-dateutil==2.8.2
+    # via
+    #   -c requirements/requirements.txt
+    #   flask-apscheduler
+python-engineio==4.4.1
+    # via python-socketio
+python-socketio==5.8.0
+    # via flask-socketio
+pytz==2023.3
+    # via
+    #   -c requirements/requirements.txt
+    #   apscheduler
+redis==4.5.5
+    # via -r requirements/requirements-extra.in
 requests==2.31.0
     # via
-    #   -c requirements/requirements-dev.txt
-    #   requests-toolbelt
-    #   twine
-requests-toolbelt==1.0.0
-    # via twine
-rfc3986==2.0.0
-    # via twine
-rich==13.3.5
-    # via
-    #   -c requirements/requirements-dev.txt
-    #   twine
-secretstorage==3.3.3
-    # via keyring
+    #   -c requirements/requirements.txt
+    #   pyfcm
+    #   stripe
 six==1.16.0
     # via
-    #   -c requirements/requirements-dev.txt
-    #   bleach
-tomli==2.0.1
-    # via
-    #   -c requirements/requirements-dev.txt
-    #   pyproject-api
-    #   tox
-tox==4.5.2
-    # via -r requirements/requirements-build.in
-twine==4.0.2
-    # via -r requirements/requirements-build.in
-urllib3==2.0.2
+    #   -c requirements/requirements.txt
+    #   apscheduler
+    #   python-dateutil
+stripe==5.4.0
+    # via -r requirements/requirements-extra.in
+tzlocal==5.0.1
+    # via
+    #   -c requirements/requirements.txt
+    #   apscheduler
+urllib3==2.0.3
     # via
-    #   -c requirements/requirements-dev.txt
+    #   -c requirements/requirements.txt
+    #   pyfcm
     #   requests
-    #   twine
-virtualenv==20.23.0
+werkzeug==2.3.6
     # via
-    #   -c requirements/requirements-dev.txt
-    #   tox
-webencodings==0.5.1
-    # via bleach
-wheel==0.40.0
-    # via -r requirements/requirements-build.in
-zipp==3.15.0
-    # via importlib-metadata
+    #   -c requirements/requirements.txt
+    #   flask
+zope-event==4.6
+    # via gevent
+zope-interface==6.0
+    # via gevent
+
+# The following packages are considered to be unsafe in a requirements file:
+# setuptools
```

### Comparing `Flaskel-3.1.0rc3/requirements/requirements-dev.txt` & `Flaskel-3.1.0rc4/requirements/requirements-dev.txt`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     # via
     #   tox
     #   virtualenv
 flake8==6.0.0
     # via
     #   -r requirements/requirements-dev.in
     #   flake8-bugbear
-flake8-bugbear==23.5.9
+flake8-bugbear==23.6.5
     # via -r requirements/requirements-dev.in
 flask==2.2.5
     # via
     #   -c requirements/requirements.txt
     #   flask-sqlalchemy
 flask-sqlalchemy==3.0.3
     # via
@@ -116,15 +116,15 @@
     # via -r requirements/requirements-dev.in
 mando==0.7.1
     # via radon
 markdown-it-py==2.2.0
     # via
     #   -c requirements/requirements.txt
     #   rich
-markupsafe==2.1.2
+markupsafe==2.1.3
     # via
     #   -c requirements/requirements.txt
     #   jinja2
     #   werkzeug
 mccabe==0.7.0
     # via
     #   flake8
@@ -152,15 +152,15 @@
     #   tox
 pathspec==0.11.1
     # via black
 pbr==5.11.1
     # via stevedore
 pip-tools==6.13.0
     # via -r requirements/requirements-dev.in
-pipdeptree==2.7.1
+pipdeptree==2.9.0
     # via -r requirements/requirements-dev.in
 platformdirs==3.5.1
     # via
     #   black
     #   pylint
     #   tox
     #   virtualenv
@@ -204,19 +204,19 @@
     #   bandit
 radon==6.0.1
     # via -r requirements/requirements-dev.in
 requests==2.31.0
     # via
     #   -c requirements/requirements-test.txt
     #   safety
-rich==13.3.5
+rich==13.4.1
     # via
     #   -c requirements/requirements.txt
     #   bandit
-ruamel-yaml==0.17.28
+ruamel-yaml==0.17.31
     # via safety
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 safety==2.3.4
     # via -r requirements/requirements-dev.in
 semantic-version==2.10.0
     # via liccheck
@@ -247,51 +247,51 @@
     #   mypy
     #   pylint
     #   pyproject-api
     #   pyproject-hooks
     #   tox
 tomlkit==0.11.8
     # via pylint
-tox==4.5.2
+tox==4.6.0
     # via -r requirements/requirements-dev.in
 types-cryptography==3.3.23.2
     # via -r requirements/requirements-dev.in
-types-pyopenssl==23.1.0.3
+types-pyopenssl==23.2.0.0
     # via
     #   -r requirements/requirements-dev.in
     #   types-redis
 types-python-dateutil==2.8.19.13
     # via -r requirements/requirements-dev.in
 types-redis==4.5.5.2
     # via -r requirements/requirements-dev.in
-types-requests==2.31.0.0
+types-requests==2.31.0.1
     # via -r requirements/requirements-dev.in
 types-setuptools==57.4.16
     # via -r requirements/requirements-dev.in
 types-urllib3==1.26.25.13
     # via
     #   -r requirements/requirements-dev.in
     #   types-requests
 types-waitress==2.1.4.8
     # via -r requirements/requirements-dev.in
 types-xmltodict==0.13.0.2
     # via -r requirements/requirements-dev.in
-typing-extensions==4.6.2
+typing-extensions==4.6.3
     # via
     #   -c requirements/requirements.txt
     #   astroid
     #   mypy
     #   sqlalchemy-stubs
-urllib3==2.0.2
+urllib3==2.0.3
     # via
     #   -c requirements/requirements-test.txt
     #   requests
 virtualenv==20.23.0
     # via tox
-werkzeug==2.3.4
+werkzeug==2.3.6
     # via
     #   -c requirements/requirements.txt
     #   flask
 wheel==0.40.0
     # via pip-tools
 wrapt==1.15.0
     # via
```

### Comparing `Flaskel-3.1.0rc3/requirements/requirements-test.txt` & `Flaskel-3.1.0rc4/requirements/requirements-test.txt`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     # via
     #   -c requirements/requirements-extra.txt
     #   requests
 charset-normalizer==3.1.0
     # via
     #   -c requirements/requirements-extra.txt
     #   requests
-coverage[toml]==7.2.6
+coverage[toml]==7.2.7
     # via
     #   -r requirements/requirements-test.in
     #   pytest-cov
 exceptiongroup==1.1.1
     # via pytest
 idna==3.4
     # via
@@ -48,12 +48,12 @@
     # via -r requirements/requirements-test.in
 tomli==2.0.1
     # via
     #   coverage
     #   pytest
 types-pyyaml==6.0.12.10
     # via responses
-urllib3==2.0.2
+urllib3==2.0.3
     # via
     #   -c requirements/requirements-extra.txt
     #   requests
     #   responses
```

### Comparing `Flaskel-3.1.0rc3/requirements/requirements-wsgi.txt` & `Flaskel-3.1.0rc4/requirements/requirements-wsgi.txt`

 * *Files 7% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     # via
     #   -c requirements/requirements-extra.txt
     #   automat
 tornado==6.3.2
     # via -r requirements/requirements-wsgi.in
 twisted==22.10.0
     # via -r requirements/requirements-wsgi.in
-typing-extensions==4.6.2
+typing-extensions==4.6.3
     # via
     #   -c requirements/requirements.txt
     #   twisted
 waitress==2.1.2
     # via -r requirements/requirements-wsgi.in
 zope-interface==6.0
     # via
```

### Comparing `Flaskel-3.1.0rc3/setup.py` & `Flaskel-3.1.0rc4/setup.py`

 * *Files identical despite different names*

