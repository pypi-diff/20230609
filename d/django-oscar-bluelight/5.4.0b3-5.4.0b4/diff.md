# Comparing `tmp/django-oscar-bluelight-5.4.0b3.tar.gz` & `tmp/django-oscar-bluelight-5.4.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-oscar-bluelight-5.4.0b3.tar", last modified: Thu Jun  8 19:18:27 2023, max compression
+gzip compressed data, was "django-oscar-bluelight-5.4.0b4.tar", last modified: Fri Jun  9 14:43:49 2023, max compression
```

## Comparing `django-oscar-bluelight-5.4.0b3.tar` & `django-oscar-bluelight-5.4.0b4.tar`

### file list

```diff
@@ -1,195 +1,195 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:18:27.314821 django-oscar-bluelight-5.4.0b3/
--rw-rw-rw-   0 root         (0) root         (0)      740 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      223 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    15745 2023-06-08 19:18:27.314821 django-oscar-bluelight-5.4.0b3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    14997 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/README.md
--rw-rw-rw-   0 root         (0) root         (0)      126 2023-06-08 19:18:27.314821 django-oscar-bluelight-5.4.0b3/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2028 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:18:27.283821 django-oscar-bluelight-5.4.0b3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:18:27.287821 django-oscar-bluelight-5.4.0b3/src/django_oscar_bluelight.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15745 2023-06-08 19:18:27.000000 django-oscar-bluelight-5.4.0b3/src/django_oscar_bluelight.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8920 2023-06-08 19:18:27.000000 django-oscar-bluelight-5.4.0b3/src/django_oscar_bluelight.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 19:18:27.000000 django-oscar-bluelight-5.4.0b3/src/django_oscar_bluelight.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      347 2023-06-08 19:18:27.000000 django-oscar-bluelight-5.4.0b3/src/django_oscar_bluelight.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-08 19:18:27.000000 django-oscar-bluelight-5.4.0b3/src/django_oscar_bluelight.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:18:27.288821 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3965 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/basket_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2923 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/caching.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:18:27.288821 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/dashboard/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/dashboard/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:18:27.290821 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/dashboard/offers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/dashboard/offers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      390 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/dashboard/offers/api_views.py
--rw-rw-rw-   0 root         (0) root         (0)     4469 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/dashboard/offers/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     8885 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/dashboard/offers/forms.py
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/dashboard/offers/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1734 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/dashboard/offers/reports.py
--rw-rw-rw-   0 root         (0) root         (0)     2628 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/dashboard/offers/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)    15037 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/dashboard/offers/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:18:27.291821 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/dashboard/ranges/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/dashboard/ranges/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1082 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/dashboard/ranges/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     3985 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/dashboard/ranges/forms.py
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/dashboard/ranges/models.py
--rw-rw-rw-   0 root         (0) root         (0)     5764 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/dashboard/ranges/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:18:27.292821 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/dashboard/vouchers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/dashboard/vouchers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2867 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/dashboard/vouchers/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     4450 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/dashboard/vouchers/forms.py
--rw-rw-rw-   0 root         (0) root         (0)    15136 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/dashboard/vouchers/views.py
--rw-rw-rw-   0 root         (0) root         (0)     3809 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/defaults.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:18:27.283821 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:18:27.283821 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/locale/es/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:18:27.292821 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/locale/es/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      380 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/locale/es/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)    37748 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/locale/es/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)      380 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/locale/es/LC_MESSAGES/djangojs.mo
--rw-rw-rw-   0 root         (0) root         (0)     2145 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/locale/es/LC_MESSAGES/djangojs.po
--rw-rw-rw-   0 root         (0) root         (0)    12939 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/mixins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:18:27.295821 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/
--rw-rw-rw-   0 root         (0) root         (0)       47 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1984 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/admin.py
--rw-rw-rw-   0 root         (0) root         (0)     9493 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/applicator.py
--rw-rw-rw-   0 root         (0) root         (0)      248 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/apps.py
--rw-rw-rw-   0 root         (0) root         (0)    27667 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/benefits.py
--rw-rw-rw-   0 root         (0) root         (0)    15451 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/conditions.py
--rw-rw-rw-   0 root         (0) root         (0)      195 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     4735 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/groups.py
--rw-rw-rw-   0 root         (0) root         (0)     3028 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/handlers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:18:27.300821 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/migrations/
--rw-rw-rw-   0 root         (0) root         (0)    25223 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      540 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/migrations/0002_auto_20151210_1053.py
--rw-rw-rw-   0 root         (0) root         (0)     1538 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/migrations/0002_compoundcondition.py
--rw-rw-rw-   0 root         (0) root         (0)      327 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/migrations/0003_merge.py
--rw-rw-rw-   0 root         (0) root         (0)      583 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/migrations/0004_conditionaloffer_groups.py
--rw-rw-rw-   0 root         (0) root         (0)     3547 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/migrations/0005_auto_20160719_1238.py
--rw-rw-rw-   0 root         (0) root         (0)     8828 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/migrations/0006_bluelightabsolutediscountbenefit_bluelightcountcondition_bluelightcoveragecondition_bluelightfixedpr.py
--rw-rw-rw-   0 root         (0) root         (0)     1734 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/migrations/0007_auto_20170417_1354.py
--rw-rw-rw-   0 root         (0) root         (0)     1708 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/migrations/0008_auto_20170512_1049.py
--rw-rw-rw-   0 root         (0) root         (0)      815 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/migrations/0009_auto_20170517_1605.py
--rw-rw-rw-   0 root         (0) root         (0)      460 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/migrations/0009_auto_20200801_0817.py
--rw-rw-rw-   0 root         (0) root         (0)      989 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/migrations/0010_auto_20170613_1245.py
--rw-rw-rw-   0 root         (0) root         (0)      697 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/migrations/0010_conditionaloffer_combinations.py
--rw-rw-rw-   0 root         (0) root         (0)     1991 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/migrations/0011_auto_20170710_1442.py
--rw-rw-rw-   0 root         (0) root         (0)      703 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/migrations/0011_conditionaloffer_affects_cosmetic_pricing.py
--rw-rw-rw-   0 root         (0) root         (0)     1312 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/migrations/0012_auto_20180514_1142.py
--rw-rw-rw-   0 root         (0) root         (0)     1167 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/migrations/0012_auto_20211020_1037.py
--rw-rw-rw-   0 root         (0) root         (0)      637 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/migrations/0013_alter_offergroup_slug.py
--rw-rw-rw-   0 root         (0) root         (0)      559 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/migrations/0013_conditionaloffer_exclusive.py
--rw-rw-rw-   0 root         (0) root         (0)      879 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/migrations/0014_auto_20181017_1151.py
--rw-rw-rw-   0 root         (0) root         (0)     3434 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/migrations/0014_drop_triggers.py
--rw-rw-rw-   0 root         (0) root         (0)      903 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/migrations/0015_auto_20181018_1220.py
--rw-rw-rw-   0 root         (0) root         (0)      355 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/migrations/0016_remove_conditionaloffer_apply_to_displayed_prices.py
--rw-rw-rw-   0 root         (0) root         (0)     2921 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/migrations/0017_auto_20190705_1245.py
--rw-rw-rw-   0 root         (0) root         (0)     1404 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/migrations/0017_compoundbenefit.py
--rw-rw-rw-   0 root         (0) root         (0)      262 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/migrations/0018_merge_20190705_1247.py
--rw-rw-rw-   0 root         (0) root         (0)      833 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/migrations/0019_auto_20190926_1547.py
--rw-rw-rw-   0 root         (0) root         (0)      332 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/migrations/0020_remove_range_cache_version.py
--rw-rw-rw-   0 root         (0) root         (0)      719 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/migrations/0021_rangeproductset.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15316 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/models.py
--rw-rw-rw-   0 root         (0) root         (0)     2400 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/reports.py
--rw-rw-rw-   0 root         (0) root         (0)     1984 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/results.py
--rw-rw-rw-   0 root         (0) root         (0)      646 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/signals.py
--rw-rw-rw-   0 root         (0) root         (0)     7204 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/sql.py
--rw-rw-rw-   0 root         (0) root         (0)     1817 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     3994 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/upsells.py
--rw-rw-rw-   0 root         (0) root         (0)      432 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:18:27.284821 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:18:27.302821 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/static/oscarbluelight/
--rw-rw-rw-   0 root         (0) root         (0)     1388 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/static/oscarbluelight/offergroups.css
--rw-rw-rw-   0 root         (0) root         (0)     1936 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/static/oscarbluelight/offergroups.css.map
--rw-rw-rw-   0 root         (0) root         (0)     6571 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/static/oscarbluelight/offergroups.js
--rw-rw-rw-   0 root         (0) root         (0)    24756 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/static/oscarbluelight/offergroups.js.map
--rw-rw-rw-   0 root         (0) root         (0)   210646 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/static/oscarbluelight/vendor.js
--rw-rw-rw-   0 root         (0) root         (0)   778250 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/static/oscarbluelight/vendor.js.map
--rw-rw-rw-   0 root         (0) root         (0)     1293 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/static/oscarbluelight/webpack-stats.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:18:27.284821 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:18:27.284821 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:18:27.284821 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/catalogue/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:18:27.303821 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/catalogue/partials/
--rw-rw-rw-   0 root         (0) root         (0)     1869 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/catalogue/partials/stock_record.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:18:27.285821 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:18:27.305821 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/offers/
--rw-rw-rw-   0 root         (0) root         (0)     1992 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/offers/benefit_delete.html
--rw-rw-rw-   0 root         (0) root         (0)     5482 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/offers/benefit_edit.html
--rw-rw-rw-   0 root         (0) root         (0)      321 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/offers/benefit_edit_compound.html
--rw-rw-rw-   0 root         (0) root         (0)     5404 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/offers/benefit_list.html
--rw-rw-rw-   0 root         (0) root         (0)      787 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/offers/benefit_selection_form.html
--rw-rw-rw-   0 root         (0) root         (0)     1997 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/offers/condition_delete.html
--rw-rw-rw-   0 root         (0) root         (0)     5389 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/offers/condition_edit.html
--rw-rw-rw-   0 root         (0) root         (0)      563 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/offers/condition_edit_compound.html
--rw-rw-rw-   0 root         (0) root         (0)     5391 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/offers/condition_list.html
--rw-rw-rw-   0 root         (0) root         (0)      793 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/offers/condition_selection_form.html
--rw-rw-rw-   0 root         (0) root         (0)     1959 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/offers/image_form.html
--rw-rw-rw-   0 root         (0) root         (0)     9218 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/offers/offer_detail.html
--rw-rw-rw-   0 root         (0) root         (0)     5691 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/offers/offer_list.html
--rw-rw-rw-   0 root         (0) root         (0)     1924 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/offers/offergroup_delete.html
--rw-rw-rw-   0 root         (0) root         (0)     3944 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/offers/offergroup_edit.html
--rw-rw-rw-   0 root         (0) root         (0)     1547 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/offers/offergroup_list.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:18:27.305821 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/offers/partials/
--rw-rw-rw-   0 root         (0) root         (0)      317 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/offers/partials/offer_thumbnail.html
--rw-rw-rw-   0 root         (0) root         (0)      494 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/offers/restrictions_form.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:18:27.306821 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/ranges/
--rw-rw-rw-   0 root         (0) root         (0)     1793 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/ranges/range_excluded_products.html
--rw-rw-rw-   0 root         (0) root         (0)     5266 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/ranges/range_list.html
--rw-rw-rw-   0 root         (0) root         (0)     8583 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/ranges/range_price_list.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:18:27.307821 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/vouchers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:18:27.307821 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/vouchers/partials/
--rw-rw-rw-   0 root         (0) root         (0)     4162 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/vouchers/partials/voucher_details_table.html
--rw-rw-rw-   0 root         (0) root         (0)     2792 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_add_children.html
--rw-rw-rw-   0 root         (0) root         (0)     7389 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_detail.html
--rw-rw-rw-   0 root         (0) root         (0)     2773 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_export_children.html
--rw-rw-rw-   0 root         (0) root         (0)     2257 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_form.html
--rw-rw-rw-   0 root         (0) root         (0)     3599 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_list.html
--rw-rw-rw-   0 root         (0) root         (0)     6453 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_list_children.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:18:27.307821 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templatetags/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templatetags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      214 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templatetags/oscarbluelight_tags.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:18:27.307821 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:18:27.310821 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/tests/offer/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/tests/offer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1422 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/tests/offer/base.py
--rw-rw-rw-   0 root         (0) root         (0)    19887 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/tests/offer/test_benefit_absolute.py
--rw-rw-rw-   0 root         (0) root         (0)    11153 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/tests/offer/test_benefit_compound.py
--rw-rw-rw-   0 root         (0) root         (0)     8276 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/tests/offer/test_benefit_fixed_price.py
--rw-rw-rw-   0 root         (0) root         (0)     8234 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/tests/offer/test_benefit_fixed_price_per_item.py
--rw-rw-rw-   0 root         (0) root         (0)     6558 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/tests/offer/test_benefit_multibuy.py
--rw-rw-rw-   0 root         (0) root         (0)    15250 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/tests/offer/test_benefit_percentage.py
--rw-rw-rw-   0 root         (0) root         (0)    37853 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/tests/offer/test_conditions.py
--rw-rw-rw-   0 root         (0) root         (0)     2862 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/tests/offer/test_cosmetic_prices.py
--rw-rw-rw-   0 root         (0) root         (0)    54267 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/tests/offer/test_offer_groups.py
--rw-rw-rw-   0 root         (0) root         (0)    10397 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/tests/offer/test_range.py
--rw-rw-rw-   0 root         (0) root         (0)    12352 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/tests/offer/test_recalculate_offer_application_totals.py
--rw-rw-rw-   0 root         (0) root         (0)     6926 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/tests/offer/test_system_groups.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:18:27.310821 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/tests/voucher/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/tests/voucher/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7817 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/tests/voucher/test_rules.py
--rw-rw-rw-   0 root         (0) root         (0)    17769 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/tests/voucher/test_vouchers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:18:27.312821 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/voucher/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/voucher/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1045 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/voucher/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      115 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/voucher/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:18:27.313821 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/voucher/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     5397 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/voucher/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      729 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/voucher/migrations/0002_auto_20160503_1138.py
--rw-rw-rw-   0 root         (0) root         (0)      625 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/voucher/migrations/0003_voucher_parent.py
--rw-rw-rw-   0 root         (0) root         (0)      525 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/voucher/migrations/0004_auto_20161115_1115.py
--rw-rw-rw-   0 root         (0) root         (0)      573 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/voucher/migrations/0005_auto_20170613_1245.py
--rw-rw-rw-   0 root         (0) root         (0)      977 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/voucher/migrations/0006_auto_20170710_1442.py
--rw-rw-rw-   0 root         (0) root         (0)     2850 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/voucher/migrations/0007_auto_20180601_1348.py
--rw-rw-rw-   0 root         (0) root         (0)      623 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/voucher/migrations/0008_auto_20190926_1547.py
--rw-rw-rw-   0 root         (0) root         (0)     1703 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/voucher/migrations/0008_auto_20200801_0817.py
--rw-rw-rw-   0 root         (0) root         (0)      557 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/voucher/migrations/0009_auto_20210216_1327.py
--rw-rw-rw-   0 root         (0) root         (0)     2620 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/voucher/migrations/0010_auto_20210526_1410.py
--rw-rw-rw-   0 root         (0) root         (0)      652 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/voucher/migrations/0011_auto_20220615_1024.py
--rw-rw-rw-   0 root         (0) root         (0)      455 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/voucher/migrations/0012_voucher_status.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/voucher/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11548 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/voucher/models.py
--rw-rw-rw-   0 root         (0) root         (0)     3017 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/voucher/reports.py
--rw-rw-rw-   0 root         (0) root         (0)     4250 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/voucher/rules.py
--rw-rw-rw-   0 root         (0) root         (0)     3229 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/voucher/sql.py
--rw-rw-rw-   0 root         (0) root         (0)      772 2023-06-08 19:18:16.000000 django-oscar-bluelight-5.4.0b3/src/oscarbluelight/voucher/tasks.py
--rw-r--r--   0 root         (0) root         (0)        9 2023-06-08 19:18:27.000000 django-oscar-bluelight-5.4.0b3/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:43:49.146284 django-oscar-bluelight-5.4.0b4/
+-rw-rw-rw-   0 root         (0) root         (0)      740 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      223 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    15745 2023-06-09 14:43:49.146284 django-oscar-bluelight-5.4.0b4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    14997 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      126 2023-06-09 14:43:49.146284 django-oscar-bluelight-5.4.0b4/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2028 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:43:49.121284 django-oscar-bluelight-5.4.0b4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:43:49.124284 django-oscar-bluelight-5.4.0b4/src/django_oscar_bluelight.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15745 2023-06-09 14:43:49.000000 django-oscar-bluelight-5.4.0b4/src/django_oscar_bluelight.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8920 2023-06-09 14:43:49.000000 django-oscar-bluelight-5.4.0b4/src/django_oscar_bluelight.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 14:43:49.000000 django-oscar-bluelight-5.4.0b4/src/django_oscar_bluelight.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      347 2023-06-09 14:43:49.000000 django-oscar-bluelight-5.4.0b4/src/django_oscar_bluelight.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-09 14:43:49.000000 django-oscar-bluelight-5.4.0b4/src/django_oscar_bluelight.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:43:49.125284 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3965 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/basket_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2923 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/caching.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:43:49.125284 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/dashboard/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/dashboard/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:43:49.126284 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/dashboard/offers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/dashboard/offers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      390 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/dashboard/offers/api_views.py
+-rw-rw-rw-   0 root         (0) root         (0)     4469 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/dashboard/offers/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     8885 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/dashboard/offers/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/dashboard/offers/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1734 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/dashboard/offers/reports.py
+-rw-rw-rw-   0 root         (0) root         (0)     2628 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/dashboard/offers/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)    15037 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/dashboard/offers/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:43:49.127284 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/dashboard/ranges/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/dashboard/ranges/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1082 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/dashboard/ranges/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     3985 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/dashboard/ranges/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/dashboard/ranges/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     5764 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/dashboard/ranges/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:43:49.127284 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/dashboard/vouchers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/dashboard/vouchers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2867 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/dashboard/vouchers/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     4450 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/dashboard/vouchers/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)    15136 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/dashboard/vouchers/views.py
+-rw-rw-rw-   0 root         (0) root         (0)     3809 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/defaults.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:43:49.121284 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:43:49.121284 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/locale/es/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:43:49.128284 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/locale/es/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      380 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/locale/es/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)    37748 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/locale/es/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)      380 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/locale/es/LC_MESSAGES/djangojs.mo
+-rw-rw-rw-   0 root         (0) root         (0)     2145 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/locale/es/LC_MESSAGES/djangojs.po
+-rw-rw-rw-   0 root         (0) root         (0)    12939 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/mixins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:43:49.130284 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1984 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)     9493 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/applicator.py
+-rw-rw-rw-   0 root         (0) root         (0)      248 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)    27667 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/benefits.py
+-rw-rw-rw-   0 root         (0) root         (0)    15451 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/conditions.py
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     4735 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/groups.py
+-rw-rw-rw-   0 root         (0) root         (0)     3028 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/handlers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:43:49.134284 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)    25223 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      540 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/migrations/0002_auto_20151210_1053.py
+-rw-rw-rw-   0 root         (0) root         (0)     1538 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/migrations/0002_compoundcondition.py
+-rw-rw-rw-   0 root         (0) root         (0)      327 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/migrations/0003_merge.py
+-rw-rw-rw-   0 root         (0) root         (0)      583 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/migrations/0004_conditionaloffer_groups.py
+-rw-rw-rw-   0 root         (0) root         (0)     3547 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/migrations/0005_auto_20160719_1238.py
+-rw-rw-rw-   0 root         (0) root         (0)     8828 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/migrations/0006_bluelightabsolutediscountbenefit_bluelightcountcondition_bluelightcoveragecondition_bluelightfixedpr.py
+-rw-rw-rw-   0 root         (0) root         (0)     1734 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/migrations/0007_auto_20170417_1354.py
+-rw-rw-rw-   0 root         (0) root         (0)     1708 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/migrations/0008_auto_20170512_1049.py
+-rw-rw-rw-   0 root         (0) root         (0)      815 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/migrations/0009_auto_20170517_1605.py
+-rw-rw-rw-   0 root         (0) root         (0)      460 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/migrations/0009_auto_20200801_0817.py
+-rw-rw-rw-   0 root         (0) root         (0)      989 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/migrations/0010_auto_20170613_1245.py
+-rw-rw-rw-   0 root         (0) root         (0)      697 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/migrations/0010_conditionaloffer_combinations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1991 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/migrations/0011_auto_20170710_1442.py
+-rw-rw-rw-   0 root         (0) root         (0)      703 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/migrations/0011_conditionaloffer_affects_cosmetic_pricing.py
+-rw-rw-rw-   0 root         (0) root         (0)     1312 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/migrations/0012_auto_20180514_1142.py
+-rw-rw-rw-   0 root         (0) root         (0)     1167 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/migrations/0012_auto_20211020_1037.py
+-rw-rw-rw-   0 root         (0) root         (0)      637 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/migrations/0013_alter_offergroup_slug.py
+-rw-rw-rw-   0 root         (0) root         (0)      559 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/migrations/0013_conditionaloffer_exclusive.py
+-rw-rw-rw-   0 root         (0) root         (0)      879 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/migrations/0014_auto_20181017_1151.py
+-rw-rw-rw-   0 root         (0) root         (0)     3442 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/migrations/0014_drop_triggers.py
+-rw-rw-rw-   0 root         (0) root         (0)      903 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/migrations/0015_auto_20181018_1220.py
+-rw-rw-rw-   0 root         (0) root         (0)      355 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/migrations/0016_remove_conditionaloffer_apply_to_displayed_prices.py
+-rw-rw-rw-   0 root         (0) root         (0)     2921 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/migrations/0017_auto_20190705_1245.py
+-rw-rw-rw-   0 root         (0) root         (0)     1404 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/migrations/0017_compoundbenefit.py
+-rw-rw-rw-   0 root         (0) root         (0)      262 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/migrations/0018_merge_20190705_1247.py
+-rw-rw-rw-   0 root         (0) root         (0)      833 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/migrations/0019_auto_20190926_1547.py
+-rw-rw-rw-   0 root         (0) root         (0)      332 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/migrations/0020_remove_range_cache_version.py
+-rw-rw-rw-   0 root         (0) root         (0)      719 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/migrations/0021_rangeproductset.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15316 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     2400 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/reports.py
+-rw-rw-rw-   0 root         (0) root         (0)     1984 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/results.py
+-rw-rw-rw-   0 root         (0) root         (0)      646 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/signals.py
+-rw-rw-rw-   0 root         (0) root         (0)     7204 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/sql.py
+-rw-rw-rw-   0 root         (0) root         (0)     1817 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     3994 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/upsells.py
+-rw-rw-rw-   0 root         (0) root         (0)      432 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:43:49.122284 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:43:49.136284 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/static/oscarbluelight/
+-rw-rw-rw-   0 root         (0) root         (0)     1388 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/static/oscarbluelight/offergroups.css
+-rw-rw-rw-   0 root         (0) root         (0)     1936 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/static/oscarbluelight/offergroups.css.map
+-rw-rw-rw-   0 root         (0) root         (0)     6571 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/static/oscarbluelight/offergroups.js
+-rw-rw-rw-   0 root         (0) root         (0)    24756 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/static/oscarbluelight/offergroups.js.map
+-rw-rw-rw-   0 root         (0) root         (0)   210646 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/static/oscarbluelight/vendor.js
+-rw-rw-rw-   0 root         (0) root         (0)   778250 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/static/oscarbluelight/vendor.js.map
+-rw-rw-rw-   0 root         (0) root         (0)     1293 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/static/oscarbluelight/webpack-stats.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:43:49.122284 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:43:49.122284 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:43:49.122284 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/catalogue/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:43:49.136284 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/catalogue/partials/
+-rw-rw-rw-   0 root         (0) root         (0)     1869 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/catalogue/partials/stock_record.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:43:49.122284 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:43:49.138284 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/offers/
+-rw-rw-rw-   0 root         (0) root         (0)     1992 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/offers/benefit_delete.html
+-rw-rw-rw-   0 root         (0) root         (0)     5482 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/offers/benefit_edit.html
+-rw-rw-rw-   0 root         (0) root         (0)      321 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/offers/benefit_edit_compound.html
+-rw-rw-rw-   0 root         (0) root         (0)     5404 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/offers/benefit_list.html
+-rw-rw-rw-   0 root         (0) root         (0)      787 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/offers/benefit_selection_form.html
+-rw-rw-rw-   0 root         (0) root         (0)     1997 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/offers/condition_delete.html
+-rw-rw-rw-   0 root         (0) root         (0)     5389 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/offers/condition_edit.html
+-rw-rw-rw-   0 root         (0) root         (0)      563 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/offers/condition_edit_compound.html
+-rw-rw-rw-   0 root         (0) root         (0)     5391 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/offers/condition_list.html
+-rw-rw-rw-   0 root         (0) root         (0)      793 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/offers/condition_selection_form.html
+-rw-rw-rw-   0 root         (0) root         (0)     1959 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/offers/image_form.html
+-rw-rw-rw-   0 root         (0) root         (0)     9218 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/offers/offer_detail.html
+-rw-rw-rw-   0 root         (0) root         (0)     5691 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/offers/offer_list.html
+-rw-rw-rw-   0 root         (0) root         (0)     1924 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/offers/offergroup_delete.html
+-rw-rw-rw-   0 root         (0) root         (0)     3944 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/offers/offergroup_edit.html
+-rw-rw-rw-   0 root         (0) root         (0)     1547 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/offers/offergroup_list.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:43:49.138284 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/offers/partials/
+-rw-rw-rw-   0 root         (0) root         (0)      317 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/offers/partials/offer_thumbnail.html
+-rw-rw-rw-   0 root         (0) root         (0)      494 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/offers/restrictions_form.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:43:49.139284 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/ranges/
+-rw-rw-rw-   0 root         (0) root         (0)     1793 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/ranges/range_excluded_products.html
+-rw-rw-rw-   0 root         (0) root         (0)     5266 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/ranges/range_list.html
+-rw-rw-rw-   0 root         (0) root         (0)     8583 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/ranges/range_price_list.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:43:49.140284 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/vouchers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:43:49.140284 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/vouchers/partials/
+-rw-rw-rw-   0 root         (0) root         (0)     4162 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/vouchers/partials/voucher_details_table.html
+-rw-rw-rw-   0 root         (0) root         (0)     2792 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_add_children.html
+-rw-rw-rw-   0 root         (0) root         (0)     7389 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_detail.html
+-rw-rw-rw-   0 root         (0) root         (0)     2773 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_export_children.html
+-rw-rw-rw-   0 root         (0) root         (0)     2257 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_form.html
+-rw-rw-rw-   0 root         (0) root         (0)     3599 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_list.html
+-rw-rw-rw-   0 root         (0) root         (0)     6453 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_list_children.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:43:49.140284 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templatetags/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templatetags/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      214 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templatetags/oscarbluelight_tags.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:43:49.140284 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:43:49.142284 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/tests/offer/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/tests/offer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1422 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/tests/offer/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    19887 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/tests/offer/test_benefit_absolute.py
+-rw-rw-rw-   0 root         (0) root         (0)    11153 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/tests/offer/test_benefit_compound.py
+-rw-rw-rw-   0 root         (0) root         (0)     8276 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/tests/offer/test_benefit_fixed_price.py
+-rw-rw-rw-   0 root         (0) root         (0)     8234 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/tests/offer/test_benefit_fixed_price_per_item.py
+-rw-rw-rw-   0 root         (0) root         (0)     6558 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/tests/offer/test_benefit_multibuy.py
+-rw-rw-rw-   0 root         (0) root         (0)    15250 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/tests/offer/test_benefit_percentage.py
+-rw-rw-rw-   0 root         (0) root         (0)    37853 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/tests/offer/test_conditions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2862 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/tests/offer/test_cosmetic_prices.py
+-rw-rw-rw-   0 root         (0) root         (0)    54267 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/tests/offer/test_offer_groups.py
+-rw-rw-rw-   0 root         (0) root         (0)    10397 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/tests/offer/test_range.py
+-rw-rw-rw-   0 root         (0) root         (0)    12352 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/tests/offer/test_recalculate_offer_application_totals.py
+-rw-rw-rw-   0 root         (0) root         (0)     6926 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/tests/offer/test_system_groups.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:43:49.143284 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/tests/voucher/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/tests/voucher/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7817 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/tests/voucher/test_rules.py
+-rw-rw-rw-   0 root         (0) root         (0)    17769 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/tests/voucher/test_vouchers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:43:49.144284 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/voucher/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/voucher/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1045 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/voucher/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      115 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/voucher/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 14:43:49.146284 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/voucher/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     5397 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/voucher/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      729 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/voucher/migrations/0002_auto_20160503_1138.py
+-rw-rw-rw-   0 root         (0) root         (0)      625 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/voucher/migrations/0003_voucher_parent.py
+-rw-rw-rw-   0 root         (0) root         (0)      525 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/voucher/migrations/0004_auto_20161115_1115.py
+-rw-rw-rw-   0 root         (0) root         (0)      573 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/voucher/migrations/0005_auto_20170613_1245.py
+-rw-rw-rw-   0 root         (0) root         (0)      977 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/voucher/migrations/0006_auto_20170710_1442.py
+-rw-rw-rw-   0 root         (0) root         (0)     2850 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/voucher/migrations/0007_auto_20180601_1348.py
+-rw-rw-rw-   0 root         (0) root         (0)      623 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/voucher/migrations/0008_auto_20190926_1547.py
+-rw-rw-rw-   0 root         (0) root         (0)     1703 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/voucher/migrations/0008_auto_20200801_0817.py
+-rw-rw-rw-   0 root         (0) root         (0)      557 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/voucher/migrations/0009_auto_20210216_1327.py
+-rw-rw-rw-   0 root         (0) root         (0)     2620 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/voucher/migrations/0010_auto_20210526_1410.py
+-rw-rw-rw-   0 root         (0) root         (0)      652 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/voucher/migrations/0011_auto_20220615_1024.py
+-rw-rw-rw-   0 root         (0) root         (0)      455 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/voucher/migrations/0012_voucher_status.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/voucher/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11548 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/voucher/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     3017 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/voucher/reports.py
+-rw-rw-rw-   0 root         (0) root         (0)     4250 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/voucher/rules.py
+-rw-rw-rw-   0 root         (0) root         (0)     3229 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/voucher/sql.py
+-rw-rw-rw-   0 root         (0) root         (0)      772 2023-06-09 14:43:38.000000 django-oscar-bluelight-5.4.0b4/src/oscarbluelight/voucher/tasks.py
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-09 14:43:49.000000 django-oscar-bluelight-5.4.0b4/version.txt
```

### Comparing `django-oscar-bluelight-5.4.0b3/LICENSE` & `django-oscar-bluelight-5.4.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/PKG-INFO` & `django-oscar-bluelight-5.4.0b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-oscar-bluelight
-Version: 5.4.0b3
+Version: 5.4.0b4
 Summary: Bluelight Specials - Enhancements to the offer and vouchers features for Django Oscar.
 Home-page: https://gitlab.com/thelabnyc/django-oscar-bluelight
 Author: thelabnyc
 Author-email: thelabdev@thelabnyc.com
 License: ISC
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `django-oscar-bluelight-5.4.0b3/README.md` & `django-oscar-bluelight-5.4.0b4/README.md`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/setup.py` & `django-oscar-bluelight-5.4.0b4/setup.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/django_oscar_bluelight.egg-info/PKG-INFO` & `django-oscar-bluelight-5.4.0b4/src/django_oscar_bluelight.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-oscar-bluelight
-Version: 5.4.0b3
+Version: 5.4.0b4
 Summary: Bluelight Specials - Enhancements to the offer and vouchers features for Django Oscar.
 Home-page: https://gitlab.com/thelabnyc/django-oscar-bluelight
 Author: thelabnyc
 Author-email: thelabdev@thelabnyc.com
 License: ISC
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `django-oscar-bluelight-5.4.0b3/src/django_oscar_bluelight.egg-info/SOURCES.txt` & `django-oscar-bluelight-5.4.0b4/src/django_oscar_bluelight.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/basket_utils.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/basket_utils.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/caching.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/caching.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/dashboard/offers/apps.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/dashboard/offers/apps.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/dashboard/offers/forms.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/dashboard/offers/forms.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/dashboard/offers/reports.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/dashboard/offers/reports.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/dashboard/offers/serializers.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/dashboard/offers/serializers.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/dashboard/offers/views.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/dashboard/offers/views.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/dashboard/ranges/apps.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/dashboard/ranges/apps.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/dashboard/ranges/forms.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/dashboard/ranges/forms.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/dashboard/ranges/views.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/dashboard/ranges/views.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/dashboard/vouchers/apps.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/dashboard/vouchers/apps.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/dashboard/vouchers/forms.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/dashboard/vouchers/forms.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/dashboard/vouchers/views.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/dashboard/vouchers/views.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/defaults.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/defaults.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/locale/es/LC_MESSAGES/django.po` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/locale/es/LC_MESSAGES/djangojs.po` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/locale/es/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/mixins.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/mixins.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/admin.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/admin.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/applicator.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/applicator.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/benefits.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/benefits.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/conditions.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/conditions.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/groups.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/groups.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/handlers.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/handlers.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/migrations/0001_initial.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/migrations/0002_auto_20151210_1053.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/migrations/0002_auto_20151210_1053.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/migrations/0002_compoundcondition.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/migrations/0002_compoundcondition.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/migrations/0004_conditionaloffer_groups.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/migrations/0004_conditionaloffer_groups.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/migrations/0005_auto_20160719_1238.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/migrations/0005_auto_20160719_1238.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/migrations/0006_bluelightabsolutediscountbenefit_bluelightcountcondition_bluelightcoveragecondition_bluelightfixedpr.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/migrations/0006_bluelightabsolutediscountbenefit_bluelightcountcondition_bluelightcoveragecondition_bluelightfixedpr.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/migrations/0007_auto_20170417_1354.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/migrations/0007_auto_20170417_1354.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/migrations/0008_auto_20170512_1049.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/migrations/0008_auto_20170512_1049.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/migrations/0009_auto_20170517_1605.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/migrations/0009_auto_20170517_1605.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/migrations/0010_auto_20170613_1245.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/migrations/0010_auto_20170613_1245.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/migrations/0010_conditionaloffer_combinations.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/migrations/0010_conditionaloffer_combinations.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/migrations/0011_auto_20170710_1442.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/migrations/0011_auto_20170710_1442.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/migrations/0011_conditionaloffer_affects_cosmetic_pricing.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/migrations/0011_conditionaloffer_affects_cosmetic_pricing.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/migrations/0012_auto_20180514_1142.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/migrations/0012_auto_20180514_1142.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/migrations/0012_auto_20211020_1037.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/migrations/0012_auto_20211020_1037.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/migrations/0013_alter_offergroup_slug.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/migrations/0013_alter_offergroup_slug.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/migrations/0013_conditionaloffer_exclusive.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/migrations/0013_conditionaloffer_exclusive.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/migrations/0014_auto_20181017_1151.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/migrations/0014_auto_20181017_1151.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/migrations/0014_drop_triggers.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/migrations/0014_drop_triggers.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "offer_range",
     "offer_range_classes",
     "offer_range_excluded_products",
     "offer_range_included_categories",
     "offer_rangeproduct",
 ]
 
-drop_triggers = ["DROP FUNCTION IF EXISTS refresh_offer_rangeproductset();"]
+drop_triggers = ["DROP FUNCTION IF EXISTS refresh_offer_rangeproductset() CASCADE;"]
 for table in range_product_trigger_tables:
     for event in "INSERT", "UPDATE", "DELETE":
         drop_triggers.append(
             f"DROP TRIGGER IF EXISTS refresh_refresh_offer_rangeproductset_{event} ON {table} CASCADE;"
         )
```

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/migrations/0015_auto_20181018_1220.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/migrations/0015_auto_20181018_1220.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/migrations/0017_auto_20190705_1245.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/migrations/0017_auto_20190705_1245.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/migrations/0017_compoundbenefit.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/migrations/0017_compoundbenefit.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/migrations/0019_auto_20190926_1547.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/migrations/0019_auto_20190926_1547.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/migrations/0021_rangeproductset.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/migrations/0021_rangeproductset.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/models.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/models.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/reports.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/reports.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/results.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/results.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/signals.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/signals.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/sql.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/sql.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/tasks.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/tasks.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/offer/upsells.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/offer/upsells.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/static/oscarbluelight/offergroups.css` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/static/oscarbluelight/offergroups.css`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/static/oscarbluelight/offergroups.css.map` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/static/oscarbluelight/offergroups.css.map`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/static/oscarbluelight/offergroups.js` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/static/oscarbluelight/offergroups.js`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/static/oscarbluelight/offergroups.js.map` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/static/oscarbluelight/offergroups.js.map`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/static/oscarbluelight/vendor.js` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/static/oscarbluelight/vendor.js`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/static/oscarbluelight/vendor.js.map` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/static/oscarbluelight/vendor.js.map`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/static/oscarbluelight/webpack-stats.json` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/static/oscarbluelight/webpack-stats.json`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/catalogue/partials/stock_record.html` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/catalogue/partials/stock_record.html`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/offers/benefit_delete.html` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/offers/benefit_delete.html`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/offers/benefit_edit.html` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/offers/benefit_edit.html`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/offers/benefit_list.html` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/offers/benefit_list.html`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/offers/benefit_selection_form.html` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/offers/benefit_selection_form.html`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/offers/condition_delete.html` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/offers/condition_delete.html`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/offers/condition_edit.html` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/offers/condition_edit.html`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/offers/condition_edit_compound.html` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/offers/condition_edit_compound.html`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/offers/condition_list.html` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/offers/condition_list.html`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/offers/condition_selection_form.html` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/offers/condition_selection_form.html`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/offers/image_form.html` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/offers/image_form.html`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/offers/offer_detail.html` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/offers/offer_detail.html`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/offers/offer_list.html` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/offers/offer_list.html`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/offers/offergroup_delete.html` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/offers/offergroup_delete.html`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/offers/offergroup_edit.html` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/offers/offergroup_edit.html`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/offers/offergroup_list.html` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/offers/offergroup_list.html`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/ranges/range_excluded_products.html` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/ranges/range_excluded_products.html`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/ranges/range_list.html` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/ranges/range_list.html`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/ranges/range_price_list.html` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/ranges/range_price_list.html`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/vouchers/partials/voucher_details_table.html` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/vouchers/partials/voucher_details_table.html`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_add_children.html` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_add_children.html`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_detail.html` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_detail.html`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_export_children.html` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_export_children.html`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_form.html` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_form.html`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_list.html` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_list.html`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_list_children.html` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_list_children.html`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/tests/offer/base.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/tests/offer/base.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/tests/offer/test_benefit_absolute.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/tests/offer/test_benefit_absolute.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/tests/offer/test_benefit_compound.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/tests/offer/test_benefit_compound.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/tests/offer/test_benefit_fixed_price.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/tests/offer/test_benefit_fixed_price.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/tests/offer/test_benefit_fixed_price_per_item.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/tests/offer/test_benefit_fixed_price_per_item.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/tests/offer/test_benefit_multibuy.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/tests/offer/test_benefit_multibuy.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/tests/offer/test_benefit_percentage.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/tests/offer/test_benefit_percentage.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/tests/offer/test_conditions.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/tests/offer/test_conditions.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/tests/offer/test_cosmetic_prices.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/tests/offer/test_cosmetic_prices.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/tests/offer/test_offer_groups.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/tests/offer/test_offer_groups.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/tests/offer/test_range.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/tests/offer/test_range.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/tests/offer/test_recalculate_offer_application_totals.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/tests/offer/test_recalculate_offer_application_totals.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/tests/offer/test_system_groups.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/tests/offer/test_system_groups.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/tests/voucher/test_rules.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/tests/voucher/test_rules.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/tests/voucher/test_vouchers.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/tests/voucher/test_vouchers.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/voucher/admin.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/voucher/admin.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/voucher/migrations/0001_initial.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/voucher/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/voucher/migrations/0002_auto_20160503_1138.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/voucher/migrations/0002_auto_20160503_1138.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/voucher/migrations/0003_voucher_parent.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/voucher/migrations/0003_voucher_parent.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/voucher/migrations/0004_auto_20161115_1115.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/voucher/migrations/0004_auto_20161115_1115.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/voucher/migrations/0005_auto_20170613_1245.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/voucher/migrations/0005_auto_20170613_1245.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/voucher/migrations/0006_auto_20170710_1442.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/voucher/migrations/0006_auto_20170710_1442.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/voucher/migrations/0007_auto_20180601_1348.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/voucher/migrations/0007_auto_20180601_1348.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/voucher/migrations/0008_auto_20190926_1547.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/voucher/migrations/0008_auto_20190926_1547.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/voucher/migrations/0008_auto_20200801_0817.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/voucher/migrations/0008_auto_20200801_0817.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/voucher/migrations/0009_auto_20210216_1327.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/voucher/migrations/0009_auto_20210216_1327.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/voucher/migrations/0010_auto_20210526_1410.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/voucher/migrations/0010_auto_20210526_1410.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/voucher/migrations/0011_auto_20220615_1024.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/voucher/migrations/0011_auto_20220615_1024.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/voucher/models.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/voucher/models.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/voucher/reports.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/voucher/reports.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/voucher/rules.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/voucher/rules.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/voucher/sql.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/voucher/sql.py`

 * *Files identical despite different names*

### Comparing `django-oscar-bluelight-5.4.0b3/src/oscarbluelight/voucher/tasks.py` & `django-oscar-bluelight-5.4.0b4/src/oscarbluelight/voucher/tasks.py`

 * *Files identical despite different names*

