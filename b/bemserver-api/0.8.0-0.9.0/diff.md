# Comparing `tmp/bemserver-api-0.8.0.tar.gz` & `tmp/bemserver-api-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bemserver-api-0.8.0.tar", last modified: Wed Jan 11 10:38:14 2023, max compression
+gzip compressed data, was "bemserver-api-0.9.0.tar", last modified: Thu Jan 12 09:49:39 2023, max compression
```

## Comparing `bemserver-api-0.8.0.tar` & `bemserver-api-0.9.0.tar`

### file list

```diff
@@ -1,313 +1,313 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.629971 bemserver-api-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-01-11 10:38:14.629971 bemserver-api-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.597969 bemserver-api-0.8.0/bemserver_api/
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.597969 bemserver-api-0.8.0/bemserver_api/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/extensions/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/extensions/integrity_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/extensions/ma_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/extensions/smorest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8826 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/extensions/timezones.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.597969 bemserver-api-0.8.0/bemserver_api/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.597969 bemserver-api-0.8.0/bemserver_api/resources/about/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/about/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/about/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/about/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.597969 bemserver-api-0.8.0/bemserver_api/resources/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.597969 bemserver-api-0.8.0/bemserver_api/resources/analysis/completeness/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/analysis/completeness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/analysis/completeness/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/analysis/completeness/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.597969 bemserver-api-0.8.0/bemserver_api/resources/analysis/energy_consumption/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/analysis/energy_consumption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/analysis/energy_consumption/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/analysis/energy_consumption/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.597969 bemserver-api-0.8.0/bemserver_api/resources/building_properties/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/building_properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/building_properties/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/building_properties/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.601969 bemserver-api-0.8.0/bemserver_api/resources/building_property_data/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/building_property_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/building_property_data/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/building_property_data/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.601969 bemserver-api-0.8.0/bemserver_api/resources/buildings/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/buildings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/buildings/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/buildings/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.601969 bemserver-api-0.8.0/bemserver_api/resources/campaign_scopes/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/campaign_scopes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/campaign_scopes/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/campaign_scopes/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.601969 bemserver-api-0.8.0/bemserver_api/resources/campaigns/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/campaigns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/campaigns/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/campaigns/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.601969 bemserver-api-0.8.0/bemserver_api/resources/energy_consumption_timeseries_by_buildings/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/energy_consumption_timeseries_by_buildings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/energy_consumption_timeseries_by_buildings/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/energy_consumption_timeseries_by_buildings/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.601969 bemserver-api-0.8.0/bemserver_api/resources/energy_consumption_timeseries_by_sites/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/energy_consumption_timeseries_by_sites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/energy_consumption_timeseries_by_sites/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/energy_consumption_timeseries_by_sites/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.601969 bemserver-api-0.8.0/bemserver_api/resources/energy_end_uses/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/energy_end_uses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/energy_end_uses/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/energy_end_uses/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.601969 bemserver-api-0.8.0/bemserver_api/resources/energy_sources/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/energy_sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/energy_sources/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/energy_sources/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.601969 bemserver-api-0.8.0/bemserver_api/resources/event_categories/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/event_categories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/event_categories/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/event_categories/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.601969 bemserver-api-0.8.0/bemserver_api/resources/event_categories_by_users/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/event_categories_by_users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/event_categories_by_users/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/event_categories_by_users/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.601969 bemserver-api-0.8.0/bemserver_api/resources/events/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/events/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/events/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.601969 bemserver-api-0.8.0/bemserver_api/resources/events_by_buildings/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/events_by_buildings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/events_by_buildings/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/events_by_buildings/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.601969 bemserver-api-0.8.0/bemserver_api/resources/events_by_sites/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/events_by_sites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/events_by_sites/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/events_by_sites/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.601969 bemserver-api-0.8.0/bemserver_api/resources/events_by_spaces/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/events_by_spaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/events_by_spaces/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/events_by_spaces/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.605970 bemserver-api-0.8.0/bemserver_api/resources/events_by_storeys/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/events_by_storeys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/events_by_storeys/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/events_by_storeys/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.605970 bemserver-api-0.8.0/bemserver_api/resources/events_by_zones/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/events_by_zones/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/events_by_zones/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/events_by_zones/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.605970 bemserver-api-0.8.0/bemserver_api/resources/input_output/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/input_output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/input_output/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/input_output/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.605970 bemserver-api-0.8.0/bemserver_api/resources/notifications/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/notifications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/notifications/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/notifications/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.605970 bemserver-api-0.8.0/bemserver_api/resources/site_properties/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/site_properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/site_properties/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/site_properties/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.605970 bemserver-api-0.8.0/bemserver_api/resources/site_property_data/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/site_property_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/site_property_data/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/site_property_data/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.605970 bemserver-api-0.8.0/bemserver_api/resources/sites/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/sites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/sites/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/sites/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.605970 bemserver-api-0.8.0/bemserver_api/resources/space_properties/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/space_properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/space_properties/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/space_properties/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.605970 bemserver-api-0.8.0/bemserver_api/resources/space_property_data/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/space_property_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/space_property_data/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/space_property_data/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.605970 bemserver-api-0.8.0/bemserver_api/resources/spaces/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/spaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/spaces/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/spaces/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.605970 bemserver-api-0.8.0/bemserver_api/resources/st_check_missings_by_campaigns/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/st_check_missings_by_campaigns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/st_check_missings_by_campaigns/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/st_check_missings_by_campaigns/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.605970 bemserver-api-0.8.0/bemserver_api/resources/st_cleanups_by_campaigns/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/st_cleanups_by_campaigns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/st_cleanups_by_campaigns/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/st_cleanups_by_campaigns/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.605970 bemserver-api-0.8.0/bemserver_api/resources/st_cleanups_by_timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/st_cleanups_by_timeseries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/st_cleanups_by_timeseries/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/st_cleanups_by_timeseries/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.609970 bemserver-api-0.8.0/bemserver_api/resources/storey_properties/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/storey_properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/storey_properties/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/storey_properties/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.609970 bemserver-api-0.8.0/bemserver_api/resources/storey_property_data/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/storey_property_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/storey_property_data/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/storey_property_data/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.609970 bemserver-api-0.8.0/bemserver_api/resources/storeys/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/storeys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/storeys/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/storeys/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.609970 bemserver-api-0.8.0/bemserver_api/resources/structural_element_properties/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/structural_element_properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/structural_element_properties/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/structural_element_properties/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.609970 bemserver-api-0.8.0/bemserver_api/resources/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/timeseries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/timeseries/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/timeseries/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.609970 bemserver-api-0.8.0/bemserver_api/resources/timeseries_by_buildings/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/timeseries_by_buildings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/timeseries_by_buildings/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/timeseries_by_buildings/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.609970 bemserver-api-0.8.0/bemserver_api/resources/timeseries_by_events/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/timeseries_by_events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/timeseries_by_events/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/timeseries_by_events/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.609970 bemserver-api-0.8.0/bemserver_api/resources/timeseries_by_sites/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/timeseries_by_sites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/timeseries_by_sites/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/timeseries_by_sites/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.609970 bemserver-api-0.8.0/bemserver_api/resources/timeseries_by_spaces/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/timeseries_by_spaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/timeseries_by_spaces/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/timeseries_by_spaces/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.609970 bemserver-api-0.8.0/bemserver_api/resources/timeseries_by_storeys/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/timeseries_by_storeys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/timeseries_by_storeys/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/timeseries_by_storeys/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.609970 bemserver-api-0.8.0/bemserver_api/resources/timeseries_by_zones/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/timeseries_by_zones/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/timeseries_by_zones/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/timeseries_by_zones/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.609970 bemserver-api-0.8.0/bemserver_api/resources/timeseries_data/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/timeseries_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15665 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/timeseries_data/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/timeseries_data/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.609970 bemserver-api-0.8.0/bemserver_api/resources/timeseries_data_states/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/timeseries_data_states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/timeseries_data_states/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/timeseries_data_states/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.613970 bemserver-api-0.8.0/bemserver_api/resources/timeseries_properties/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/timeseries_properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/timeseries_properties/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/timeseries_properties/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.613970 bemserver-api-0.8.0/bemserver_api/resources/timeseries_property_data/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/timeseries_property_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/timeseries_property_data/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/timeseries_property_data/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.613970 bemserver-api-0.8.0/bemserver_api/resources/user_groups/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/user_groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/user_groups/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/user_groups/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.613970 bemserver-api-0.8.0/bemserver_api/resources/user_groups_by_campaign_scopes/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/user_groups_by_campaign_scopes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/user_groups_by_campaign_scopes/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/user_groups_by_campaign_scopes/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.617970 bemserver-api-0.8.0/bemserver_api/resources/user_groups_by_campaigns/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/user_groups_by_campaigns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/user_groups_by_campaigns/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/user_groups_by_campaigns/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.617970 bemserver-api-0.8.0/bemserver_api/resources/users/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/users/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/users/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.617970 bemserver-api-0.8.0/bemserver_api/resources/users_by_user_groups/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/users_by_user_groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/users_by_user_groups/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/users_by_user_groups/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.617970 bemserver-api-0.8.0/bemserver_api/resources/zone_properties/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/zone_properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/zone_properties/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/zone_properties/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.621971 bemserver-api-0.8.0/bemserver_api/resources/zone_property_data/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/zone_property_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/zone_property_data/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/zone_property_data/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.621971 bemserver-api-0.8.0/bemserver_api/resources/zones/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/zones/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/zones/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/resources/zones/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/bemserver_api/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.597969 bemserver-api-0.8.0/bemserver_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-01-11 10:38:14.000000 bemserver-api-0.8.0/bemserver_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11877 2023-01-11 10:38:14.000000 bemserver-api-0.8.0/bemserver_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 10:38:14.000000 bemserver-api-0.8.0/bemserver_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-01-11 10:38:14.000000 bemserver-api-0.8.0/bemserver_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-01-11 10:38:14.000000 bemserver-api-0.8.0/bemserver_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.621971 bemserver-api-0.8.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/requirements/install.txt
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/requirements/tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-01-11 10:38:14.633971 bemserver-api-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.621971 bemserver-api-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    24189 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.621971 bemserver-api-0.8.0/tests/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/extensions/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/extensions/test_integrity_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/extensions/test_ma_fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.629971 bemserver-api-0.8.0/tests/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:38:14.629971 bemserver-api-0.8.0/tests/resources/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/resources/analysis/test_completeness.py
--rw-r--r--   0 runner    (1001) docker     (123)    15076 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/resources/analysis/test_energy_consumption.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/resources/test_about.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/resources/test_building_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     9303 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/resources/test_building_property_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8100 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/resources/test_buildings.py
--rw-r--r--   0 runner    (1001) docker     (123)     8051 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/resources/test_campaign_scopes.py
--rw-r--r--   0 runner    (1001) docker     (123)    10596 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/resources/test_campaigns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/resources/test_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10215 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/resources/test_energy_consumption_timeseries_by_buildings.py
--rw-r--r--   0 runner    (1001) docker     (123)     9781 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/resources/test_energy_consumption_timeseries_by_sites.py
--rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/resources/test_event_categories.py
--rw-r--r--   0 runner    (1001) docker     (123)     8732 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/resources/test_event_categories_by_users.py
--rw-r--r--   0 runner    (1001) docker     (123)    13374 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/resources/test_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     6796 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/resources/test_events_by_buildings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/resources/test_events_by_sites.py
--rw-r--r--   0 runner    (1001) docker     (123)     6873 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/resources/test_events_by_spaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     6865 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/resources/test_events_by_storeys.py
--rw-r--r--   0 runner    (1001) docker     (123)     6725 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/resources/test_events_by_zones.py
--rw-r--r--   0 runner    (1001) docker     (123)    12933 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/resources/test_input_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     7973 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/resources/test_notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/resources/test_site_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     8869 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/resources/test_site_property_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7467 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/resources/test_sites.py
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/resources/test_space_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/resources/test_space_property_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8240 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/resources/test_spaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     9598 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/resources/test_st_check_missings_by_campaigns.py
--rw-r--r--   0 runner    (1001) docker     (123)     9341 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/resources/test_st_cleanups_by_campaigns.py
--rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/resources/test_st_cleanups_by_timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/resources/test_storey_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     9079 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/resources/test_storey_property_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8159 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/resources/test_storeys.py
--rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/resources/test_structural_element_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    13684 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/resources/test_timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/resources/test_timeseries_by_buildings.py
--rw-r--r--   0 runner    (1001) docker     (123)     7117 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/resources/test_timeseries_by_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/resources/test_timeseries_by_sites.py
--rw-r--r--   0 runner    (1001) docker     (123)     8189 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/resources/test_timeseries_by_spaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     8260 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/resources/test_timeseries_by_storeys.py
--rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/resources/test_timeseries_by_zones.py
--rw-r--r--   0 runner    (1001) docker     (123)    36342 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/resources/test_timeseries_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6282 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/resources/test_timeseries_data_states.py
--rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/resources/test_timeseries_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     8337 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/resources/test_timeseries_property_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/resources/test_user_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     7931 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/resources/test_user_groups_by_campaigns.py
--rw-r--r--   0 runner    (1001) docker     (123)     8242 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/resources/test_user_groups_by_campaigns_scopes.py
--rw-r--r--   0 runner    (1001) docker     (123)    10168 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/resources/test_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     7548 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/resources/test_users_by_user_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/resources/test_zone_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/resources/test_zone_property_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7467 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/resources/test_zones.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-01-11 10:38:02.000000 bemserver-api-0.8.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.155100 bemserver-api-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-01-12 09:49:39.155100 bemserver-api-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.135100 bemserver-api-0.9.0/bemserver_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.135100 bemserver-api-0.9.0/bemserver_api/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/extensions/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/extensions/integrity_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/extensions/ma_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/extensions/smorest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8826 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/extensions/timezones.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.135100 bemserver-api-0.9.0/bemserver_api/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.135100 bemserver-api-0.9.0/bemserver_api/resources/about/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/about/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/about/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/about/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.135100 bemserver-api-0.9.0/bemserver_api/resources/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.135100 bemserver-api-0.9.0/bemserver_api/resources/analysis/completeness/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/analysis/completeness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/analysis/completeness/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/analysis/completeness/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.135100 bemserver-api-0.9.0/bemserver_api/resources/analysis/energy_consumption/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/analysis/energy_consumption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/analysis/energy_consumption/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/analysis/energy_consumption/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.135100 bemserver-api-0.9.0/bemserver_api/resources/building_properties/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/building_properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/building_properties/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/building_properties/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.135100 bemserver-api-0.9.0/bemserver_api/resources/building_property_data/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/building_property_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/building_property_data/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/building_property_data/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.135100 bemserver-api-0.9.0/bemserver_api/resources/buildings/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/buildings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/buildings/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/buildings/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.139100 bemserver-api-0.9.0/bemserver_api/resources/campaign_scopes/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/campaign_scopes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/campaign_scopes/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/campaign_scopes/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.139100 bemserver-api-0.9.0/bemserver_api/resources/campaigns/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/campaigns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/campaigns/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/campaigns/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.139100 bemserver-api-0.9.0/bemserver_api/resources/energy_consumption_timeseries_by_buildings/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/energy_consumption_timeseries_by_buildings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/energy_consumption_timeseries_by_buildings/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/energy_consumption_timeseries_by_buildings/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.139100 bemserver-api-0.9.0/bemserver_api/resources/energy_consumption_timeseries_by_sites/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/energy_consumption_timeseries_by_sites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/energy_consumption_timeseries_by_sites/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/energy_consumption_timeseries_by_sites/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.139100 bemserver-api-0.9.0/bemserver_api/resources/energy_end_uses/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/energy_end_uses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/energy_end_uses/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/energy_end_uses/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.139100 bemserver-api-0.9.0/bemserver_api/resources/energy_sources/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/energy_sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/energy_sources/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/energy_sources/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.139100 bemserver-api-0.9.0/bemserver_api/resources/event_categories/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/event_categories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/event_categories/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/event_categories/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.139100 bemserver-api-0.9.0/bemserver_api/resources/event_categories_by_users/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/event_categories_by_users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/event_categories_by_users/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/event_categories_by_users/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.139100 bemserver-api-0.9.0/bemserver_api/resources/events/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/events/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/events/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.139100 bemserver-api-0.9.0/bemserver_api/resources/events_by_buildings/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/events_by_buildings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/events_by_buildings/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/events_by_buildings/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.139100 bemserver-api-0.9.0/bemserver_api/resources/events_by_sites/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/events_by_sites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/events_by_sites/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/events_by_sites/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.139100 bemserver-api-0.9.0/bemserver_api/resources/events_by_spaces/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/events_by_spaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/events_by_spaces/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/events_by_spaces/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.139100 bemserver-api-0.9.0/bemserver_api/resources/events_by_storeys/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/events_by_storeys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/events_by_storeys/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/events_by_storeys/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.139100 bemserver-api-0.9.0/bemserver_api/resources/events_by_zones/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/events_by_zones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/events_by_zones/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/events_by_zones/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.139100 bemserver-api-0.9.0/bemserver_api/resources/input_output/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/input_output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/input_output/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/input_output/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.139100 bemserver-api-0.9.0/bemserver_api/resources/notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/notifications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/notifications/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/notifications/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.139100 bemserver-api-0.9.0/bemserver_api/resources/site_properties/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/site_properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/site_properties/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/site_properties/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.143100 bemserver-api-0.9.0/bemserver_api/resources/site_property_data/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/site_property_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/site_property_data/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/site_property_data/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.143100 bemserver-api-0.9.0/bemserver_api/resources/sites/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/sites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/sites/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/sites/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.143100 bemserver-api-0.9.0/bemserver_api/resources/space_properties/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/space_properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/space_properties/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/space_properties/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.143100 bemserver-api-0.9.0/bemserver_api/resources/space_property_data/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/space_property_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/space_property_data/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/space_property_data/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.143100 bemserver-api-0.9.0/bemserver_api/resources/spaces/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/spaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/spaces/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/spaces/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.143100 bemserver-api-0.9.0/bemserver_api/resources/st_check_missings_by_campaigns/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/st_check_missings_by_campaigns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/st_check_missings_by_campaigns/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/st_check_missings_by_campaigns/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.143100 bemserver-api-0.9.0/bemserver_api/resources/st_cleanups_by_campaigns/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/st_cleanups_by_campaigns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/st_cleanups_by_campaigns/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/st_cleanups_by_campaigns/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.143100 bemserver-api-0.9.0/bemserver_api/resources/st_cleanups_by_timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/st_cleanups_by_timeseries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/st_cleanups_by_timeseries/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/st_cleanups_by_timeseries/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.143100 bemserver-api-0.9.0/bemserver_api/resources/storey_properties/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/storey_properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/storey_properties/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/storey_properties/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.143100 bemserver-api-0.9.0/bemserver_api/resources/storey_property_data/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/storey_property_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/storey_property_data/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/storey_property_data/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.143100 bemserver-api-0.9.0/bemserver_api/resources/storeys/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/storeys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/storeys/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/storeys/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.143100 bemserver-api-0.9.0/bemserver_api/resources/structural_element_properties/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/structural_element_properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/structural_element_properties/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/structural_element_properties/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.143100 bemserver-api-0.9.0/bemserver_api/resources/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/timeseries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/timeseries/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/timeseries/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.143100 bemserver-api-0.9.0/bemserver_api/resources/timeseries_by_buildings/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/timeseries_by_buildings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/timeseries_by_buildings/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/timeseries_by_buildings/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.143100 bemserver-api-0.9.0/bemserver_api/resources/timeseries_by_events/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/timeseries_by_events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/timeseries_by_events/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/timeseries_by_events/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.143100 bemserver-api-0.9.0/bemserver_api/resources/timeseries_by_sites/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/timeseries_by_sites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/timeseries_by_sites/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/timeseries_by_sites/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.143100 bemserver-api-0.9.0/bemserver_api/resources/timeseries_by_spaces/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/timeseries_by_spaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/timeseries_by_spaces/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/timeseries_by_spaces/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.147100 bemserver-api-0.9.0/bemserver_api/resources/timeseries_by_storeys/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/timeseries_by_storeys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/timeseries_by_storeys/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/timeseries_by_storeys/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.147100 bemserver-api-0.9.0/bemserver_api/resources/timeseries_by_zones/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/timeseries_by_zones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/timeseries_by_zones/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/timeseries_by_zones/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.147100 bemserver-api-0.9.0/bemserver_api/resources/timeseries_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/timeseries_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15665 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/timeseries_data/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/timeseries_data/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.147100 bemserver-api-0.9.0/bemserver_api/resources/timeseries_data_states/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/timeseries_data_states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/timeseries_data_states/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/timeseries_data_states/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.147100 bemserver-api-0.9.0/bemserver_api/resources/timeseries_properties/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/timeseries_properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/timeseries_properties/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/timeseries_properties/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.147100 bemserver-api-0.9.0/bemserver_api/resources/timeseries_property_data/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/timeseries_property_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/timeseries_property_data/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/timeseries_property_data/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.147100 bemserver-api-0.9.0/bemserver_api/resources/user_groups/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/user_groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/user_groups/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/user_groups/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.147100 bemserver-api-0.9.0/bemserver_api/resources/user_groups_by_campaign_scopes/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/user_groups_by_campaign_scopes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/user_groups_by_campaign_scopes/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/user_groups_by_campaign_scopes/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.147100 bemserver-api-0.9.0/bemserver_api/resources/user_groups_by_campaigns/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/user_groups_by_campaigns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/user_groups_by_campaigns/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/user_groups_by_campaigns/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.147100 bemserver-api-0.9.0/bemserver_api/resources/users/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/users/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/users/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.147100 bemserver-api-0.9.0/bemserver_api/resources/users_by_user_groups/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/users_by_user_groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/users_by_user_groups/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/users_by_user_groups/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.147100 bemserver-api-0.9.0/bemserver_api/resources/zone_properties/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/zone_properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/zone_properties/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/zone_properties/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.147100 bemserver-api-0.9.0/bemserver_api/resources/zone_property_data/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/zone_property_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/zone_property_data/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/zone_property_data/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.147100 bemserver-api-0.9.0/bemserver_api/resources/zones/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/zones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/zones/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/resources/zones/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/bemserver_api/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.135100 bemserver-api-0.9.0/bemserver_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-01-12 09:49:39.000000 bemserver-api-0.9.0/bemserver_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11877 2023-01-12 09:49:39.000000 bemserver-api-0.9.0/bemserver_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 09:49:39.000000 bemserver-api-0.9.0/bemserver_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-01-12 09:49:39.000000 bemserver-api-0.9.0/bemserver_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-01-12 09:49:39.000000 bemserver-api-0.9.0/bemserver_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.147100 bemserver-api-0.9.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/requirements/install.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/requirements/tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-01-12 09:49:39.155100 bemserver-api-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.147100 bemserver-api-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24189 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.151100 bemserver-api-0.9.0/tests/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/extensions/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/extensions/test_integrity_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/extensions/test_ma_fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.155100 bemserver-api-0.9.0/tests/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 09:49:39.155100 bemserver-api-0.9.0/tests/resources/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/resources/analysis/test_completeness.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15076 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/resources/analysis/test_energy_consumption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/resources/test_about.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/resources/test_building_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9303 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/resources/test_building_property_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8100 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/resources/test_buildings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8051 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/resources/test_campaign_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10596 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/resources/test_campaigns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/resources/test_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10215 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/resources/test_energy_consumption_timeseries_by_buildings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9781 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/resources/test_energy_consumption_timeseries_by_sites.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/resources/test_event_categories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8732 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/resources/test_event_categories_by_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13374 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/resources/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6950 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/resources/test_events_by_buildings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/resources/test_events_by_sites.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/resources/test_events_by_spaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/resources/test_events_by_storeys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/resources/test_events_by_zones.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12933 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/resources/test_input_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7231 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/resources/test_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/resources/test_site_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8869 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/resources/test_site_property_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7467 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/resources/test_sites.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/resources/test_space_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/resources/test_space_property_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8240 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/resources/test_spaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9598 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/resources/test_st_check_missings_by_campaigns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9341 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/resources/test_st_cleanups_by_campaigns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/resources/test_st_cleanups_by_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5313 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/resources/test_storey_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9079 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/resources/test_storey_property_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8159 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/resources/test_storeys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/resources/test_structural_element_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13684 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/resources/test_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/resources/test_timeseries_by_buildings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6893 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/resources/test_timeseries_by_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/resources/test_timeseries_by_sites.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/resources/test_timeseries_by_spaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6118 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/resources/test_timeseries_by_storeys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/resources/test_timeseries_by_zones.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36342 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/resources/test_timeseries_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6282 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/resources/test_timeseries_data_states.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/resources/test_timeseries_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8337 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/resources/test_timeseries_property_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/resources/test_user_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7831 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/resources/test_user_groups_by_campaigns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/resources/test_user_groups_by_campaigns_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10168 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/resources/test_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/resources/test_users_by_user_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/resources/test_zone_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/resources/test_zone_property_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7467 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/resources/test_zones.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-01-12 09:49:31.000000 bemserver-api-0.9.0/tox.ini
```

### Comparing `bemserver-api-0.8.0/LICENSE` & `bemserver-api-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/PKG-INFO` & `bemserver-api-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bemserver-api
-Version: 0.8.0
+Version: 0.9.0
 Summary: BEMServer API
 Home-page: https://github.com/BEMServer/bemserver-api
 Author: Nobatek/INEF4
 Author-email: jlafrechoux@nobatek.inef4.com
 License: AGPLv3+
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `bemserver-api-0.8.0/README.rst` & `bemserver-api-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/__init__.py` & `bemserver-api-0.9.0/bemserver_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     SQLCursorPage,
     SortField,
     authentication,
 )
 from .resources import register_blueprints
 
 
-__version__ = "0.8.0"
+__version__ = "0.9.0"
 
 API_VERSION = __version__
 OPENAPI_VERSION = "3.1.0"
 
 
 def create_app(config_override=None):
     """Create application
```

### Comparing `bemserver-api-0.8.0/bemserver_api/extensions/authentication.py` & `bemserver-api-0.9.0/bemserver_api/extensions/authentication.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/extensions/integrity_error.py` & `bemserver-api-0.9.0/bemserver_api/extensions/integrity_error.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/extensions/ma_fields.py` & `bemserver-api-0.9.0/bemserver_api/extensions/ma_fields.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/extensions/smorest.py` & `bemserver-api-0.9.0/bemserver_api/extensions/smorest.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/extensions/timezones.json` & `bemserver-api-0.9.0/bemserver_api/extensions/timezones.json`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/__init__.py` & `bemserver-api-0.9.0/bemserver_api/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/about/routes.py` & `bemserver-api-0.9.0/bemserver_api/resources/about/routes.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/analysis/completeness/routes.py` & `bemserver-api-0.9.0/bemserver_api/resources/analysis/completeness/routes.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/analysis/completeness/schemas.py` & `bemserver-api-0.9.0/bemserver_api/resources/analysis/completeness/schemas.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/analysis/energy_consumption/routes.py` & `bemserver-api-0.9.0/bemserver_api/resources/analysis/energy_consumption/routes.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/analysis/energy_consumption/schemas.py` & `bemserver-api-0.9.0/bemserver_api/resources/analysis/energy_consumption/schemas.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/building_properties/routes.py` & `bemserver-api-0.9.0/bemserver_api/resources/building_properties/routes.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,37 +20,34 @@
     description="Operations on building properties",
 )
 
 
 @blp.route("/")
 class BuildingPropertyViews(MethodView):
     @blp.login_required
-    @blp.etag
     @blp.arguments(BuildingPropertyQueryArgsSchema, location="query")
     @blp.response(200, BuildingPropertySchema(many=True))
     def get(self, args):
         """List building properties"""
         return BuildingProperty.get(**args)
 
     @blp.login_required
-    @blp.etag
     @blp.arguments(BuildingPropertySchema)
     @blp.response(201, BuildingPropertySchema)
     @blp.catch_integrity_error
     def post(self, new_item):
         """Add a new building property"""
         item = BuildingProperty.new(**new_item)
         db.session.commit()
         return item
 
 
 @blp.route("/<int:item_id>")
 class BuildingPropertyByIdViews(MethodView):
     @blp.login_required
-    @blp.etag
     @blp.response(200, BuildingPropertySchema)
     def get(self, item_id):
         """Get building property by ID"""
         item = BuildingProperty.get_by_id(item_id)
         if item is None:
             abort(404)
         return item
```

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/building_properties/schemas.py` & `bemserver-api-0.9.0/bemserver_api/resources/building_properties/schemas.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/building_property_data/routes.py` & `bemserver-api-0.9.0/bemserver_api/resources/building_property_data/routes.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/buildings/routes.py` & `bemserver-api-0.9.0/bemserver_api/resources/buildings/routes.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/buildings/schemas.py` & `bemserver-api-0.9.0/bemserver_api/resources/buildings/schemas.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/campaign_scopes/routes.py` & `bemserver-api-0.9.0/bemserver_api/resources/campaign_scopes/routes.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/campaign_scopes/schemas.py` & `bemserver-api-0.9.0/bemserver_api/resources/campaign_scopes/schemas.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/campaigns/routes.py` & `bemserver-api-0.9.0/bemserver_api/resources/campaigns/routes.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/campaigns/schemas.py` & `bemserver-api-0.9.0/bemserver_api/resources/campaigns/schemas.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/energy_consumption_timeseries_by_buildings/routes.py` & `bemserver-api-0.9.0/bemserver_api/resources/energy_consumption_timeseries_by_buildings/routes.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/energy_consumption_timeseries_by_buildings/schemas.py` & `bemserver-api-0.9.0/bemserver_api/resources/energy_consumption_timeseries_by_buildings/schemas.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/energy_consumption_timeseries_by_sites/routes.py` & `bemserver-api-0.9.0/bemserver_api/resources/energy_consumption_timeseries_by_sites/routes.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/energy_consumption_timeseries_by_sites/schemas.py` & `bemserver-api-0.9.0/bemserver_api/resources/energy_consumption_timeseries_by_sites/schemas.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/energy_end_uses/routes.py` & `bemserver-api-0.9.0/bemserver_api/resources/energy_end_uses/routes.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/energy_sources/routes.py` & `bemserver-api-0.9.0/bemserver_api/resources/energy_sources/routes.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/event_categories/routes.py` & `bemserver-api-0.9.0/bemserver_api/resources/event_categories/routes.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/event_categories_by_users/routes.py` & `bemserver-api-0.9.0/bemserver_api/resources/event_categories_by_users/routes.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/event_categories_by_users/schemas.py` & `bemserver-api-0.9.0/bemserver_api/resources/event_categories_by_users/schemas.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/events/routes.py` & `bemserver-api-0.9.0/bemserver_api/resources/events/routes.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/events/schemas.py` & `bemserver-api-0.9.0/bemserver_api/resources/events/schemas.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/events_by_buildings/routes.py` & `bemserver-api-0.9.0/bemserver_api/resources/events_by_buildings/routes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Events by buildings resources"""
 from flask.views import MethodView
 from flask_smorest import abort
 
 from bemserver_core.model import EventByBuilding
 from bemserver_core.exceptions import BEMServerCoreCampaignError
 
-from bemserver_api import Blueprint
+from bemserver_api import Blueprint, SQLCursorPage
 from bemserver_api.database import db
 
 from .schemas import (
     EventByBuildingSchema,
     EventByBuildingQueryArgsSchema,
 )
 
@@ -21,23 +21,22 @@
     description="Operations on event x building associations",
 )
 
 
 @blp.route("/")
 class EventByBuildingViews(MethodView):
     @blp.login_required
-    @blp.etag
     @blp.arguments(EventByBuildingQueryArgsSchema, location="query")
     @blp.response(200, EventByBuildingSchema(many=True))
+    @blp.paginate(SQLCursorPage)
     def get(self, args):
         """List event x building associations"""
         return EventByBuilding.get(**args)
 
     @blp.login_required
-    @blp.etag
     @blp.arguments(EventByBuildingSchema)
     @blp.response(201, EventByBuildingSchema)
     @blp.catch_integrity_error
     def post(self, new_item):
         """Add a new event x building association"""
         item = EventByBuilding.new(**new_item)
         try:
@@ -46,15 +45,14 @@
             abort(422, errors={"json": {"_schema": str(exc)}})
         return item
 
 
 @blp.route("/<int:item_id>")
 class EventByBuildingByIdViews(MethodView):
     @blp.login_required
-    @blp.etag
     @blp.response(200, EventByBuildingSchema)
     def get(self, item_id):
         """Get event x building association by ID"""
         item = EventByBuilding.get_by_id(item_id)
         if item is None:
             abort(404)
         return item
```

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/events_by_sites/routes.py` & `bemserver-api-0.9.0/bemserver_api/resources/events_by_sites/routes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Events by sites resources"""
 from flask.views import MethodView
 from flask_smorest import abort
 
 from bemserver_core.model import EventBySite
 from bemserver_core.exceptions import BEMServerCoreCampaignError
 
-from bemserver_api import Blueprint
+from bemserver_api import Blueprint, SQLCursorPage
 from bemserver_api.database import db
 
 from .schemas import (
     EventBySiteSchema,
     EventBySiteQueryArgsSchema,
 )
 
@@ -21,23 +21,22 @@
     description="Operations on event x site associations",
 )
 
 
 @blp.route("/")
 class EventBySiteViews(MethodView):
     @blp.login_required
-    @blp.etag
     @blp.arguments(EventBySiteQueryArgsSchema, location="query")
     @blp.response(200, EventBySiteSchema(many=True))
+    @blp.paginate(SQLCursorPage)
     def get(self, args):
         """List event x site associations"""
         return EventBySite.get(**args)
 
     @blp.login_required
-    @blp.etag
     @blp.arguments(EventBySiteSchema)
     @blp.response(201, EventBySiteSchema)
     @blp.catch_integrity_error
     def post(self, new_item):
         """Add a new event x site association"""
         item = EventBySite.new(**new_item)
         try:
@@ -46,15 +45,14 @@
             abort(422, errors={"json": {"_schema": str(exc)}})
         return item
 
 
 @blp.route("/<int:item_id>")
 class EventBySiteByIdViews(MethodView):
     @blp.login_required
-    @blp.etag
     @blp.response(200, EventBySiteSchema)
     def get(self, item_id):
         """Get event x site association by ID"""
         item = EventBySite.get_by_id(item_id)
         if item is None:
             abort(404)
         return item
```

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/events_by_spaces/routes.py` & `bemserver-api-0.9.0/bemserver_api/resources/events_by_spaces/routes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Events by spaces resources"""
 from flask.views import MethodView
 from flask_smorest import abort
 
 from bemserver_core.model import EventBySpace
 from bemserver_core.exceptions import BEMServerCoreCampaignError
 
-from bemserver_api import Blueprint
+from bemserver_api import Blueprint, SQLCursorPage
 from bemserver_api.database import db
 
 from .schemas import (
     EventBySpaceSchema,
     EventBySpaceQueryArgsSchema,
 )
 
@@ -21,23 +21,22 @@
     description="Operations on event x space associations",
 )
 
 
 @blp.route("/")
 class EventBySpaceViews(MethodView):
     @blp.login_required
-    @blp.etag
     @blp.arguments(EventBySpaceQueryArgsSchema, location="query")
     @blp.response(200, EventBySpaceSchema(many=True))
+    @blp.paginate(SQLCursorPage)
     def get(self, args):
         """List event x space associations"""
         return EventBySpace.get(**args)
 
     @blp.login_required
-    @blp.etag
     @blp.arguments(EventBySpaceSchema)
     @blp.response(201, EventBySpaceSchema)
     @blp.catch_integrity_error
     def post(self, new_item):
         """Add a new event x space association"""
         item = EventBySpace.new(**new_item)
         try:
@@ -46,15 +45,14 @@
             abort(422, errors={"json": {"_schema": str(exc)}})
         return item
 
 
 @blp.route("/<int:item_id>")
 class EventBySpaceByIdViews(MethodView):
     @blp.login_required
-    @blp.etag
     @blp.response(200, EventBySpaceSchema)
     def get(self, item_id):
         """Get event x space association by ID"""
         item = EventBySpace.get_by_id(item_id)
         if item is None:
             abort(404)
         return item
```

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/events_by_storeys/routes.py` & `bemserver-api-0.9.0/bemserver_api/resources/events_by_storeys/routes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Events by storeys resources"""
 from flask.views import MethodView
 from flask_smorest import abort
 
 from bemserver_core.model import EventByStorey
 from bemserver_core.exceptions import BEMServerCoreCampaignError
 
-from bemserver_api import Blueprint
+from bemserver_api import Blueprint, SQLCursorPage
 from bemserver_api.database import db
 
 from .schemas import (
     EventByStoreySchema,
     EventByStoreyQueryArgsSchema,
 )
 
@@ -21,23 +21,22 @@
     description="Operations on event x storey associations",
 )
 
 
 @blp.route("/")
 class EventByStoreyViews(MethodView):
     @blp.login_required
-    @blp.etag
     @blp.arguments(EventByStoreyQueryArgsSchema, location="query")
     @blp.response(200, EventByStoreySchema(many=True))
+    @blp.paginate(SQLCursorPage)
     def get(self, args):
         """List event x storey associations"""
         return EventByStorey.get(**args)
 
     @blp.login_required
-    @blp.etag
     @blp.arguments(EventByStoreySchema)
     @blp.response(201, EventByStoreySchema)
     @blp.catch_integrity_error
     def post(self, new_item):
         """Add a new event x storey association"""
         item = EventByStorey.new(**new_item)
         try:
@@ -46,15 +45,14 @@
             abort(422, errors={"json": {"_schema": str(exc)}})
         return item
 
 
 @blp.route("/<int:item_id>")
 class EventByStoreyByIdViews(MethodView):
     @blp.login_required
-    @blp.etag
     @blp.response(200, EventByStoreySchema)
     def get(self, item_id):
         """Get event x storey association by ID"""
         item = EventByStorey.get_by_id(item_id)
         if item is None:
             abort(404)
         return item
```

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/events_by_zones/routes.py` & `bemserver-api-0.9.0/bemserver_api/resources/events_by_zones/routes.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Events by zones resources"""
 from flask.views import MethodView
 from flask_smorest import abort
 
 from bemserver_core.model import EventByZone
 from bemserver_core.exceptions import BEMServerCoreCampaignError
 
-from bemserver_api import Blueprint
+from bemserver_api import Blueprint, SQLCursorPage
 from bemserver_api.database import db
 
 from .schemas import (
     EventByZoneSchema,
     EventByZoneQueryArgsSchema,
 )
 
@@ -21,23 +21,22 @@
     description="Operations on event x zone associations",
 )
 
 
 @blp.route("/")
 class EventByZoneViews(MethodView):
     @blp.login_required
-    @blp.etag
     @blp.arguments(EventByZoneQueryArgsSchema, location="query")
     @blp.response(200, EventByZoneSchema(many=True))
+    @blp.paginate(SQLCursorPage)
     def get(self, args):
         """List event x zone associations"""
         return EventByZone.get(**args)
 
     @blp.login_required
-    @blp.etag
     @blp.arguments(EventByZoneSchema)
     @blp.response(201, EventByZoneSchema)
     @blp.catch_integrity_error
     def post(self, new_item):
         """Add a new event x zone association"""
         item = EventByZone.new(**new_item)
         try:
@@ -46,15 +45,14 @@
             abort(422, errors={"json": {"_schema": str(exc)}})
         return item
 
 
 @blp.route("/<int:item_id>")
 class EventByZoneByIdViews(MethodView):
     @blp.login_required
-    @blp.etag
     @blp.response(200, EventByZoneSchema)
     def get(self, item_id):
         """Get event x zone association by ID"""
         item = EventByZone.get_by_id(item_id)
         if item is None:
             abort(404)
         return item
```

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/input_output/routes.py` & `bemserver-api-0.9.0/bemserver_api/resources/input_output/routes.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/input_output/schemas.py` & `bemserver-api-0.9.0/bemserver_api/resources/input_output/schemas.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/notifications/routes.py` & `bemserver-api-0.9.0/bemserver_api/resources/notifications/routes.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Notifications resources"""
 
 from flask.views import MethodView
 from flask_smorest import abort
 
 from bemserver_core.model import Notification
 
-from bemserver_api import Blueprint
+from bemserver_api import Blueprint, SQLCursorPage
 from bemserver_api.database import db
 
 from .schemas import (
     NotificationSchema,
     NotificationPutSchema,
     NotificationsQueryArgsSchema,
 )
@@ -25,14 +25,15 @@
 
 @blp.route("/")
 class NotificationsViews(MethodView):
     @blp.login_required
     @blp.etag
     @blp.arguments(NotificationsQueryArgsSchema, location="query")
     @blp.response(200, NotificationSchema(many=True))
+    @blp.paginate(SQLCursorPage)
     def get(self, args):
         """List notifications"""
         return Notification.get(**args)
 
     @blp.login_required
     @blp.etag
     @blp.arguments(NotificationSchema)
@@ -54,32 +55,28 @@
         """Get a notification by its by ID"""
         item = Notification.get_by_id(item_id)
         if item is None:
             abort(404)
         return item
 
     @blp.login_required
-    @blp.etag
     @blp.arguments(NotificationPutSchema)
     @blp.response(200, NotificationSchema)
     @blp.catch_integrity_error
     def put(self, new_item, item_id):
         """Update an existing notification"""
         item = Notification.get_by_id(item_id)
         if item is None:
             abort(404)
-        blp.check_etag(item, NotificationSchema)
         item.update(**new_item)
         db.session.commit()
         return item
 
     @blp.login_required
-    @blp.etag
     @blp.response(204)
     def delete(self, item_id):
         """Delete a notification"""
         item = Notification.get_by_id(item_id)
         if item is None:
             abort(404)
-        blp.check_etag(item, NotificationSchema)
         item.delete()
         db.session.commit()
```

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/notifications/schemas.py` & `bemserver-api-0.9.0/bemserver_api/resources/notifications/schemas.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/site_properties/routes.py` & `bemserver-api-0.9.0/bemserver_api/resources/site_properties/routes.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,37 +20,34 @@
     description="Operations on site properties",
 )
 
 
 @blp.route("/")
 class SitePropertyViews(MethodView):
     @blp.login_required
-    @blp.etag
     @blp.arguments(SitePropertyQueryArgsSchema, location="query")
     @blp.response(200, SitePropertySchema(many=True))
     def get(self, args):
         """List site properties"""
         return SiteProperty.get(**args)
 
     @blp.login_required
-    @blp.etag
     @blp.arguments(SitePropertySchema)
     @blp.response(201, SitePropertySchema)
     @blp.catch_integrity_error
     def post(self, new_item):
         """Add a new site property"""
         item = SiteProperty.new(**new_item)
         db.session.commit()
         return item
 
 
 @blp.route("/<int:item_id>")
 class SitePropertyByIdViews(MethodView):
     @blp.login_required
-    @blp.etag
     @blp.response(200, SitePropertySchema)
     def get(self, item_id):
         """Get site property by ID"""
         item = SiteProperty.get_by_id(item_id)
         if item is None:
             abort(404)
         return item
```

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/site_properties/schemas.py` & `bemserver-api-0.9.0/bemserver_api/resources/site_properties/schemas.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/site_property_data/routes.py` & `bemserver-api-0.9.0/bemserver_api/resources/site_property_data/routes.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/sites/routes.py` & `bemserver-api-0.9.0/bemserver_api/resources/sites/routes.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/sites/schemas.py` & `bemserver-api-0.9.0/bemserver_api/resources/sites/schemas.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/space_properties/routes.py` & `bemserver-api-0.9.0/bemserver_api/resources/spaces/routes.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,66 +1,77 @@
-"""Space properties resources"""
+"""Space resources"""
 from flask.views import MethodView
 from flask_smorest import abort
 
-from bemserver_core.model import SpaceProperty
+from bemserver_core.model import Space
 
 from bemserver_api import Blueprint
 from bemserver_api.database import db
 
-from .schemas import (
-    SpacePropertySchema,
-    SpacePropertyQueryArgsSchema,
-)
+from .schemas import SpaceSchema, SpacePutSchema, SpaceQueryArgsSchema
 
 
 blp = Blueprint(
-    "SpaceProperty",
-    __name__,
-    url_prefix="/space_properties",
-    description="Operations on space properties",
+    "Space", __name__, url_prefix="/spaces", description="Operations on spaces"
 )
 
 
 @blp.route("/")
-class SpacePropertyViews(MethodView):
+class SpaceViews(MethodView):
     @blp.login_required
     @blp.etag
-    @blp.arguments(SpacePropertyQueryArgsSchema, location="query")
-    @blp.response(200, SpacePropertySchema(many=True))
+    @blp.arguments(SpaceQueryArgsSchema, location="query")
+    @blp.response(200, SpaceSchema(many=True))
     def get(self, args):
-        """List space properties"""
-        return SpaceProperty.get(**args)
+        """List spaces"""
+        return Space.get(**args)
 
     @blp.login_required
     @blp.etag
-    @blp.arguments(SpacePropertySchema)
-    @blp.response(201, SpacePropertySchema)
+    @blp.arguments(SpaceSchema)
+    @blp.response(201, SpaceSchema)
     @blp.catch_integrity_error
     def post(self, new_item):
-        """Add a new space property"""
-        item = SpaceProperty.new(**new_item)
+        """Add a new space"""
+        item = Space.new(**new_item)
         db.session.commit()
         return item
 
 
 @blp.route("/<int:item_id>")
-class SpacePropertyByIdViews(MethodView):
+class SpaceByIdViews(MethodView):
     @blp.login_required
     @blp.etag
-    @blp.response(200, SpacePropertySchema)
+    @blp.response(200, SpaceSchema)
     def get(self, item_id):
-        """Get space property by ID"""
-        item = SpaceProperty.get_by_id(item_id)
+        """Get space by ID"""
+        item = Space.get_by_id(item_id)
+        if item is None:
+            abort(404)
+        return item
+
+    @blp.login_required
+    @blp.etag
+    @blp.arguments(SpacePutSchema)
+    @blp.response(200, SpaceSchema)
+    @blp.catch_integrity_error
+    def put(self, new_item, item_id):
+        """Update an existing space"""
+        item = Space.get_by_id(item_id)
         if item is None:
             abort(404)
+        blp.check_etag(item, SpaceSchema)
+        item.update(**new_item)
+        db.session.commit()
         return item
 
     @blp.login_required
+    @blp.etag
     @blp.response(204)
     def delete(self, item_id):
-        """Delete a space property"""
-        item = SpaceProperty.get_by_id(item_id)
+        """Delete a space"""
+        item = Space.get_by_id(item_id)
         if item is None:
             abort(404)
+        blp.check_etag(item, SpaceSchema)
         item.delete()
         db.session.commit()
```

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/space_properties/schemas.py` & `bemserver-api-0.9.0/bemserver_api/resources/space_properties/schemas.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/space_property_data/routes.py` & `bemserver-api-0.9.0/bemserver_api/resources/space_property_data/routes.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/spaces/routes.py` & `bemserver-api-0.9.0/bemserver_api/resources/users/routes.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,77 +1,115 @@
-"""Space resources"""
+"""Users resources"""
 from flask.views import MethodView
 from flask_smorest import abort
 
-from bemserver_core.model import Space
+from bemserver_core.model import User
 
 from bemserver_api import Blueprint
 from bemserver_api.database import db
 
-from .schemas import SpaceSchema, SpacePutSchema, SpaceQueryArgsSchema
+from .schemas import UserSchema, UserQueryArgsSchema, BooleanValueSchema
 
 
 blp = Blueprint(
-    "Space", __name__, url_prefix="/spaces", description="Operations on spaces"
+    "User", __name__, url_prefix="/users", description="Operations on users"
 )
 
 
 @blp.route("/")
-class SpaceViews(MethodView):
+class UserViews(MethodView):
     @blp.login_required
     @blp.etag
-    @blp.arguments(SpaceQueryArgsSchema, location="query")
-    @blp.response(200, SpaceSchema(many=True))
+    @blp.arguments(UserQueryArgsSchema, location="query")
+    @blp.response(200, UserSchema(many=True))
     def get(self, args):
-        """List spaces"""
-        return Space.get(**args)
+        """List users"""
+        return User.get(**args)
 
     @blp.login_required
     @blp.etag
-    @blp.arguments(SpaceSchema)
-    @blp.response(201, SpaceSchema)
+    @blp.arguments(UserSchema)
+    @blp.response(201, UserSchema)
     @blp.catch_integrity_error
     def post(self, new_item):
-        """Add a new space"""
-        item = Space.new(**new_item)
+        """Add a new user"""
+        password = new_item.pop("password")
+        item = User.new(**new_item)
+        item.set_password(password)
+        item.is_admin = False
+        item.is_active = True
         db.session.commit()
         return item
 
 
 @blp.route("/<int:item_id>")
-class SpaceByIdViews(MethodView):
+class UserByIdViews(MethodView):
     @blp.login_required
     @blp.etag
-    @blp.response(200, SpaceSchema)
+    @blp.response(200, UserSchema)
     def get(self, item_id):
-        """Get space by ID"""
-        item = Space.get_by_id(item_id)
+        """Get user by ID"""
+        item = User.get_by_id(item_id)
         if item is None:
             abort(404)
         return item
 
     @blp.login_required
     @blp.etag
-    @blp.arguments(SpacePutSchema)
-    @blp.response(200, SpaceSchema)
+    @blp.arguments(UserSchema)
+    @blp.response(200, UserSchema)
     @blp.catch_integrity_error
     def put(self, new_item, item_id):
-        """Update an existing space"""
-        item = Space.get_by_id(item_id)
+        """Update an existing user"""
+        item = User.get_by_id(item_id)
         if item is None:
             abort(404)
-        blp.check_etag(item, SpaceSchema)
+        blp.check_etag(item, UserSchema)
+        password = new_item.pop("password")
         item.update(**new_item)
+        item.set_password(password)
         db.session.commit()
         return item
 
     @blp.login_required
     @blp.etag
     @blp.response(204)
     def delete(self, item_id):
-        """Delete a space"""
-        item = Space.get_by_id(item_id)
+        """Delete a user"""
+        item = User.get_by_id(item_id)
         if item is None:
             abort(404)
-        blp.check_etag(item, SpaceSchema)
+        blp.check_etag(item, UserSchema)
         item.delete()
         db.session.commit()
+
+
+@blp.route("/<int:item_id>/set_admin", methods=("PUT",))
+@blp.login_required
+@blp.etag
+@blp.arguments(BooleanValueSchema)
+@blp.response(204)
+def set_admin(args, item_id):
+    """Set / unset admin"""
+    item = User.get_by_id(item_id)
+    if item is None:
+        abort(404)
+    blp.check_etag(item, UserSchema)
+    item.is_admin = args["value"]
+    db.session.commit()
+    blp.set_etag(item, UserSchema)
+
+
+@blp.route("/<int:item_id>/set_active", methods=("PUT",))
+@blp.login_required
+@blp.etag
+@blp.arguments(BooleanValueSchema)
+@blp.response(204)
+def set_active(args, item_id):
+    """Set / unset active"""
+    item = User.get_by_id(item_id)
+    if item is None:
+        abort(404)
+    blp.check_etag(item, UserSchema)
+    item.is_active = args["value"]
+    db.session.commit()
+    blp.set_etag(item, UserSchema)
```

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/spaces/schemas.py` & `bemserver-api-0.9.0/bemserver_api/resources/spaces/schemas.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/st_check_missings_by_campaigns/routes.py` & `bemserver-api-0.9.0/bemserver_api/resources/st_check_missings_by_campaigns/routes.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/st_check_missings_by_campaigns/schemas.py` & `bemserver-api-0.9.0/bemserver_api/resources/st_check_missings_by_campaigns/schemas.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/st_cleanups_by_campaigns/routes.py` & `bemserver-api-0.9.0/bemserver_api/resources/st_cleanups_by_campaigns/routes.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/st_cleanups_by_campaigns/schemas.py` & `bemserver-api-0.9.0/bemserver_api/resources/st_cleanups_by_campaigns/schemas.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/st_cleanups_by_timeseries/routes.py` & `bemserver-api-0.9.0/bemserver_api/resources/st_cleanups_by_timeseries/routes.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/st_cleanups_by_timeseries/schemas.py` & `bemserver-api-0.9.0/bemserver_api/resources/st_cleanups_by_timeseries/schemas.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/storey_properties/routes.py` & `bemserver-api-0.9.0/bemserver_api/resources/storey_properties/routes.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,37 +20,34 @@
     description="Operations on storey properties",
 )
 
 
 @blp.route("/")
 class StoreyPropertyViews(MethodView):
     @blp.login_required
-    @blp.etag
     @blp.arguments(StoreyPropertyQueryArgsSchema, location="query")
     @blp.response(200, StoreyPropertySchema(many=True))
     def get(self, args):
         """List storey properties"""
         return StoreyProperty.get(**args)
 
     @blp.login_required
-    @blp.etag
     @blp.arguments(StoreyPropertySchema)
     @blp.response(201, StoreyPropertySchema)
     @blp.catch_integrity_error
     def post(self, new_item):
         """Add a new storey property"""
         item = StoreyProperty.new(**new_item)
         db.session.commit()
         return item
 
 
 @blp.route("/<int:item_id>")
 class StoreyPropertyByIdViews(MethodView):
     @blp.login_required
-    @blp.etag
     @blp.response(200, StoreyPropertySchema)
     def get(self, item_id):
         """Get storey property by ID"""
         item = StoreyProperty.get_by_id(item_id)
         if item is None:
             abort(404)
         return item
```

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/storey_properties/schemas.py` & `bemserver-api-0.9.0/bemserver_api/resources/storey_properties/schemas.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/storey_property_data/routes.py` & `bemserver-api-0.9.0/bemserver_api/resources/storey_property_data/routes.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/storeys/routes.py` & `bemserver-api-0.9.0/bemserver_api/resources/storeys/routes.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/storeys/schemas.py` & `bemserver-api-0.9.0/bemserver_api/resources/storeys/schemas.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/structural_element_properties/routes.py` & `bemserver-api-0.9.0/bemserver_api/resources/structural_element_properties/routes.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/structural_element_properties/schemas.py` & `bemserver-api-0.9.0/bemserver_api/resources/structural_element_properties/schemas.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/timeseries/routes.py` & `bemserver-api-0.9.0/bemserver_api/resources/timeseries/routes.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/timeseries/schemas.py` & `bemserver-api-0.9.0/bemserver_api/resources/timeseries/schemas.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/timeseries_by_buildings/routes.py` & `bemserver-api-0.9.0/bemserver_api/resources/timeseries_by_buildings/routes.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Timeseries by buildings resources"""
 from flask.views import MethodView
 from flask_smorest import abort
 
 from bemserver_core.model import TimeseriesByBuilding
 
-from bemserver_api import Blueprint
+from bemserver_api import Blueprint, SQLCursorPage
 from bemserver_api.database import db
 
 from .schemas import (
     TimeseriesByBuildingSchema,
     TimeseriesByBuildingQueryArgsSchema,
 )
 
@@ -20,64 +20,45 @@
     description="Operations on timeseries x building associations",
 )
 
 
 @blp.route("/")
 class TimeseriesByBuildingViews(MethodView):
     @blp.login_required
-    @blp.etag
     @blp.arguments(TimeseriesByBuildingQueryArgsSchema, location="query")
     @blp.response(200, TimeseriesByBuildingSchema(many=True))
+    @blp.paginate(SQLCursorPage)
     def get(self, args):
         """List timeseries x building associations"""
         return TimeseriesByBuilding.get(**args)
 
     @blp.login_required
-    @blp.etag
     @blp.arguments(TimeseriesByBuildingSchema)
     @blp.response(201, TimeseriesByBuildingSchema)
     @blp.catch_integrity_error
     def post(self, new_item):
         """Add a new timeseries x building association"""
         item = TimeseriesByBuilding.new(**new_item)
         db.session.commit()
         return item
 
 
 @blp.route("/<int:item_id>")
 class TimeseriesByBuildingByIdViews(MethodView):
     @blp.login_required
-    @blp.etag
     @blp.response(200, TimeseriesByBuildingSchema)
     def get(self, item_id):
         """Get timeseries x building association by ID"""
         item = TimeseriesByBuilding.get_by_id(item_id)
         if item is None:
             abort(404)
         return item
 
     @blp.login_required
-    @blp.etag
-    @blp.arguments(TimeseriesByBuildingSchema)
-    @blp.response(200, TimeseriesByBuildingSchema)
-    @blp.catch_integrity_error
-    def put(self, new_item, item_id):
-        """Update an existing timeseries x building association"""
-        item = TimeseriesByBuilding.get_by_id(item_id)
-        if item is None:
-            abort(404)
-        blp.check_etag(item, TimeseriesByBuildingSchema)
-        item.update(**new_item)
-        db.session.commit()
-        return item
-
-    @blp.login_required
-    @blp.etag
     @blp.response(204)
     def delete(self, item_id):
         """Delete a timeseries x building association"""
         item = TimeseriesByBuilding.get_by_id(item_id)
         if item is None:
             abort(404)
-        blp.check_etag(item, TimeseriesByBuildingSchema)
         item.delete()
         db.session.commit()
```

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/timeseries_by_events/routes.py` & `bemserver-api-0.9.0/bemserver_api/resources/timeseries_by_events/routes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Timeseries by events resources"""
 from flask.views import MethodView
 from flask_smorest import abort
 
 from bemserver_core.model import TimeseriesByEvent
 from bemserver_core.exceptions import BEMServerCoreCampaignScopeError
 
-from bemserver_api import Blueprint
+from bemserver_api import Blueprint, SQLCursorPage
 from bemserver_api.database import db
 
 from .schemas import (
     TimeseriesByEventSchema,
     TimeseriesByEventQueryArgsSchema,
 )
 
@@ -21,23 +21,22 @@
     description="Operations on timeseries x event associations",
 )
 
 
 @blp.route("/")
 class TimeseriesByEventViews(MethodView):
     @blp.login_required
-    @blp.etag
     @blp.arguments(TimeseriesByEventQueryArgsSchema, location="query")
     @blp.response(200, TimeseriesByEventSchema(many=True))
+    @blp.paginate(SQLCursorPage)
     def get(self, args):
         """List timeseries x event associations"""
         return TimeseriesByEvent.get(**args)
 
     @blp.login_required
-    @blp.etag
     @blp.arguments(TimeseriesByEventSchema)
     @blp.response(201, TimeseriesByEventSchema)
     @blp.catch_integrity_error
     def post(self, new_item):
         """Add a new timeseries x event association"""
         item = TimeseriesByEvent.new(**new_item)
         try:
@@ -46,15 +45,14 @@
             abort(422, errors={"json": {"_schema": str(exc)}})
         return item
 
 
 @blp.route("/<int:item_id>")
 class TimeseriesByEventByIdViews(MethodView):
     @blp.login_required
-    @blp.etag
     @blp.response(200, TimeseriesByEventSchema)
     def get(self, item_id):
         """Get timeseries x event association by ID"""
         item = TimeseriesByEvent.get_by_id(item_id)
         if item is None:
             abort(404)
         return item
```

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/timeseries_by_sites/routes.py` & `bemserver-api-0.9.0/bemserver_api/resources/timeseries_by_spaces/routes.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,83 +1,64 @@
-"""Timeseries by sites resources"""
+"""Timeseries by spaces resources"""
 from flask.views import MethodView
 from flask_smorest import abort
 
-from bemserver_core.model import TimeseriesBySite
+from bemserver_core.model import TimeseriesBySpace
 
-from bemserver_api import Blueprint
+from bemserver_api import Blueprint, SQLCursorPage
 from bemserver_api.database import db
 
 from .schemas import (
-    TimeseriesBySiteSchema,
-    TimeseriesBySiteQueryArgsSchema,
+    TimeseriesBySpaceSchema,
+    TimeseriesBySpaceQueryArgsSchema,
 )
 
 
 blp = Blueprint(
-    "TimeseriesBySite",
+    "TimeseriesBySpace",
     __name__,
-    url_prefix="/timeseries_by_sites",
-    description="Operations on timeseries x site associations",
+    url_prefix="/timeseries_by_spaces",
+    description="Operations on timeseries x space associations",
 )
 
 
 @blp.route("/")
-class TimeseriesBySiteViews(MethodView):
+class TimeseriesBySpaceViews(MethodView):
     @blp.login_required
-    @blp.etag
-    @blp.arguments(TimeseriesBySiteQueryArgsSchema, location="query")
-    @blp.response(200, TimeseriesBySiteSchema(many=True))
+    @blp.arguments(TimeseriesBySpaceQueryArgsSchema, location="query")
+    @blp.response(200, TimeseriesBySpaceSchema(many=True))
+    @blp.paginate(SQLCursorPage)
     def get(self, args):
-        """List timeseries x site associations"""
-        return TimeseriesBySite.get(**args)
+        """List timeseries x space associations"""
+        return TimeseriesBySpace.get(**args)
 
     @blp.login_required
-    @blp.etag
-    @blp.arguments(TimeseriesBySiteSchema)
-    @blp.response(201, TimeseriesBySiteSchema)
+    @blp.arguments(TimeseriesBySpaceSchema)
+    @blp.response(201, TimeseriesBySpaceSchema)
     @blp.catch_integrity_error
     def post(self, new_item):
-        """Add a new timeseries x site association"""
-        item = TimeseriesBySite.new(**new_item)
+        """Add a new timeseries x space association"""
+        item = TimeseriesBySpace.new(**new_item)
         db.session.commit()
         return item
 
 
 @blp.route("/<int:item_id>")
-class TimeseriesBySiteByIdViews(MethodView):
+class TimeseriesBySpaceByIdViews(MethodView):
     @blp.login_required
-    @blp.etag
-    @blp.response(200, TimeseriesBySiteSchema)
+    @blp.response(200, TimeseriesBySpaceSchema)
     def get(self, item_id):
-        """Get timeseries x site association by ID"""
-        item = TimeseriesBySite.get_by_id(item_id)
+        """Get timeseries x space association by ID"""
+        item = TimeseriesBySpace.get_by_id(item_id)
         if item is None:
             abort(404)
         return item
 
     @blp.login_required
-    @blp.etag
-    @blp.arguments(TimeseriesBySiteSchema)
-    @blp.response(200, TimeseriesBySiteSchema)
-    @blp.catch_integrity_error
-    def put(self, new_item, item_id):
-        """Update an existing timeseries x site association"""
-        item = TimeseriesBySite.get_by_id(item_id)
-        if item is None:
-            abort(404)
-        blp.check_etag(item, TimeseriesBySiteSchema)
-        item.update(**new_item)
-        db.session.commit()
-        return item
-
-    @blp.login_required
-    @blp.etag
     @blp.response(204)
     def delete(self, item_id):
-        """Delete a timeseries x site association"""
-        item = TimeseriesBySite.get_by_id(item_id)
+        """Delete a timeseries x space association"""
+        item = TimeseriesBySpace.get_by_id(item_id)
         if item is None:
             abort(404)
-        blp.check_etag(item, TimeseriesBySiteSchema)
         item.delete()
         db.session.commit()
```

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/timeseries_by_spaces/routes.py` & `bemserver-api-0.9.0/bemserver_api/resources/timeseries_by_storeys/routes.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,83 +1,64 @@
-"""Timeseries by spaces resources"""
+"""Timeseries by storeys resources"""
 from flask.views import MethodView
 from flask_smorest import abort
 
-from bemserver_core.model import TimeseriesBySpace
+from bemserver_core.model import TimeseriesByStorey
 
-from bemserver_api import Blueprint
+from bemserver_api import Blueprint, SQLCursorPage
 from bemserver_api.database import db
 
 from .schemas import (
-    TimeseriesBySpaceSchema,
-    TimeseriesBySpaceQueryArgsSchema,
+    TimeseriesByStoreySchema,
+    TimeseriesByStoreyQueryArgsSchema,
 )
 
 
 blp = Blueprint(
-    "TimeseriesBySpace",
+    "TimeseriesByStorey",
     __name__,
-    url_prefix="/timeseries_by_spaces",
-    description="Operations on timeseries x space associations",
+    url_prefix="/timeseries_by_storeys",
+    description="Operations on timeseries x storey associations",
 )
 
 
 @blp.route("/")
-class TimeseriesBySpaceViews(MethodView):
+class TimeseriesByStoreyViews(MethodView):
     @blp.login_required
-    @blp.etag
-    @blp.arguments(TimeseriesBySpaceQueryArgsSchema, location="query")
-    @blp.response(200, TimeseriesBySpaceSchema(many=True))
+    @blp.arguments(TimeseriesByStoreyQueryArgsSchema, location="query")
+    @blp.response(200, TimeseriesByStoreySchema(many=True))
+    @blp.paginate(SQLCursorPage)
     def get(self, args):
-        """List timeseries x space associations"""
-        return TimeseriesBySpace.get(**args)
+        """List timeseries x storey associations"""
+        return TimeseriesByStorey.get(**args)
 
     @blp.login_required
-    @blp.etag
-    @blp.arguments(TimeseriesBySpaceSchema)
-    @blp.response(201, TimeseriesBySpaceSchema)
+    @blp.arguments(TimeseriesByStoreySchema)
+    @blp.response(201, TimeseriesByStoreySchema)
     @blp.catch_integrity_error
     def post(self, new_item):
-        """Add a new timeseries x space association"""
-        item = TimeseriesBySpace.new(**new_item)
+        """Add a new timeseries x storey association"""
+        item = TimeseriesByStorey.new(**new_item)
         db.session.commit()
         return item
 
 
 @blp.route("/<int:item_id>")
-class TimeseriesBySpaceByIdViews(MethodView):
+class TimeseriesByStoreyByIdViews(MethodView):
     @blp.login_required
-    @blp.etag
-    @blp.response(200, TimeseriesBySpaceSchema)
+    @blp.response(200, TimeseriesByStoreySchema)
     def get(self, item_id):
-        """Get timeseries x space association by ID"""
-        item = TimeseriesBySpace.get_by_id(item_id)
+        """Get timeseries x storey association by ID"""
+        item = TimeseriesByStorey.get_by_id(item_id)
         if item is None:
             abort(404)
         return item
 
     @blp.login_required
-    @blp.etag
-    @blp.arguments(TimeseriesBySpaceSchema)
-    @blp.response(200, TimeseriesBySpaceSchema)
-    @blp.catch_integrity_error
-    def put(self, new_item, item_id):
-        """Update an existing timeseries x space association"""
-        item = TimeseriesBySpace.get_by_id(item_id)
-        if item is None:
-            abort(404)
-        blp.check_etag(item, TimeseriesBySpaceSchema)
-        item.update(**new_item)
-        db.session.commit()
-        return item
-
-    @blp.login_required
-    @blp.etag
     @blp.response(204)
     def delete(self, item_id):
-        """Delete a timeseries x space association"""
-        item = TimeseriesBySpace.get_by_id(item_id)
+        """Delete a timeseries x storey association"""
+        item = TimeseriesByStorey.get_by_id(item_id)
         if item is None:
             abort(404)
-        blp.check_etag(item, TimeseriesBySpaceSchema)
         item.delete()
         db.session.commit()
```

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/timeseries_by_storeys/routes.py` & `bemserver-api-0.9.0/bemserver_api/resources/timeseries_by_zones/routes.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,83 +1,64 @@
-"""Timeseries by storeys resources"""
+"""Timeseries by zones resources"""
 from flask.views import MethodView
 from flask_smorest import abort
 
-from bemserver_core.model import TimeseriesByStorey
+from bemserver_core.model import TimeseriesByZone
 
-from bemserver_api import Blueprint
+from bemserver_api import Blueprint, SQLCursorPage
 from bemserver_api.database import db
 
 from .schemas import (
-    TimeseriesByStoreySchema,
-    TimeseriesByStoreyQueryArgsSchema,
+    TimeseriesByZoneSchema,
+    TimeseriesByZoneQueryArgsSchema,
 )
 
 
 blp = Blueprint(
-    "TimeseriesByStorey",
+    "TimeseriesByZone",
     __name__,
-    url_prefix="/timeseries_by_storeys",
-    description="Operations on timeseries x storey associations",
+    url_prefix="/timeseries_by_zones",
+    description="Operations on timeseries x zone associations",
 )
 
 
 @blp.route("/")
-class TimeseriesByStoreyViews(MethodView):
+class TimeseriesByZoneViews(MethodView):
     @blp.login_required
-    @blp.etag
-    @blp.arguments(TimeseriesByStoreyQueryArgsSchema, location="query")
-    @blp.response(200, TimeseriesByStoreySchema(many=True))
+    @blp.arguments(TimeseriesByZoneQueryArgsSchema, location="query")
+    @blp.response(200, TimeseriesByZoneSchema(many=True))
+    @blp.paginate(SQLCursorPage)
     def get(self, args):
-        """List timeseries x storey associations"""
-        return TimeseriesByStorey.get(**args)
+        """List timeseries x zone associations"""
+        return TimeseriesByZone.get(**args)
 
     @blp.login_required
-    @blp.etag
-    @blp.arguments(TimeseriesByStoreySchema)
-    @blp.response(201, TimeseriesByStoreySchema)
+    @blp.arguments(TimeseriesByZoneSchema)
+    @blp.response(201, TimeseriesByZoneSchema)
     @blp.catch_integrity_error
     def post(self, new_item):
-        """Add a new timeseries x storey association"""
-        item = TimeseriesByStorey.new(**new_item)
+        """Add a new timeseries x zone association"""
+        item = TimeseriesByZone.new(**new_item)
         db.session.commit()
         return item
 
 
 @blp.route("/<int:item_id>")
-class TimeseriesByStoreyByIdViews(MethodView):
+class TimeseriesByZoneByIdViews(MethodView):
     @blp.login_required
-    @blp.etag
-    @blp.response(200, TimeseriesByStoreySchema)
+    @blp.response(200, TimeseriesByZoneSchema)
     def get(self, item_id):
-        """Get timeseries x storey association by ID"""
-        item = TimeseriesByStorey.get_by_id(item_id)
+        """Get timeseries x zone association by ID"""
+        item = TimeseriesByZone.get_by_id(item_id)
         if item is None:
             abort(404)
         return item
 
     @blp.login_required
-    @blp.etag
-    @blp.arguments(TimeseriesByStoreySchema)
-    @blp.response(200, TimeseriesByStoreySchema)
-    @blp.catch_integrity_error
-    def put(self, new_item, item_id):
-        """Update an existing timeseries x storey association"""
-        item = TimeseriesByStorey.get_by_id(item_id)
-        if item is None:
-            abort(404)
-        blp.check_etag(item, TimeseriesByStoreySchema)
-        item.update(**new_item)
-        db.session.commit()
-        return item
-
-    @blp.login_required
-    @blp.etag
     @blp.response(204)
     def delete(self, item_id):
-        """Delete a timeseries x storey association"""
-        item = TimeseriesByStorey.get_by_id(item_id)
+        """Delete a timeseries x zone association"""
+        item = TimeseriesByZone.get_by_id(item_id)
         if item is None:
             abort(404)
-        blp.check_etag(item, TimeseriesByStoreySchema)
         item.delete()
         db.session.commit()
```

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/timeseries_by_zones/routes.py` & `bemserver-api-0.9.0/bemserver_api/resources/timeseries_by_sites/routes.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,83 +1,64 @@
-"""Timeseries by zones resources"""
+"""Timeseries by sites resources"""
 from flask.views import MethodView
 from flask_smorest import abort
 
-from bemserver_core.model import TimeseriesByZone
+from bemserver_core.model import TimeseriesBySite
 
-from bemserver_api import Blueprint
+from bemserver_api import Blueprint, SQLCursorPage
 from bemserver_api.database import db
 
 from .schemas import (
-    TimeseriesByZoneSchema,
-    TimeseriesByZoneQueryArgsSchema,
+    TimeseriesBySiteSchema,
+    TimeseriesBySiteQueryArgsSchema,
 )
 
 
 blp = Blueprint(
-    "TimeseriesByZone",
+    "TimeseriesBySite",
     __name__,
-    url_prefix="/timeseries_by_zones",
-    description="Operations on timeseries x zone associations",
+    url_prefix="/timeseries_by_sites",
+    description="Operations on timeseries x site associations",
 )
 
 
 @blp.route("/")
-class TimeseriesByZoneViews(MethodView):
+class TimeseriesBySiteViews(MethodView):
     @blp.login_required
-    @blp.etag
-    @blp.arguments(TimeseriesByZoneQueryArgsSchema, location="query")
-    @blp.response(200, TimeseriesByZoneSchema(many=True))
+    @blp.arguments(TimeseriesBySiteQueryArgsSchema, location="query")
+    @blp.response(200, TimeseriesBySiteSchema(many=True))
+    @blp.paginate(SQLCursorPage)
     def get(self, args):
-        """List timeseries x zone associations"""
-        return TimeseriesByZone.get(**args)
+        """List timeseries x site associations"""
+        return TimeseriesBySite.get(**args)
 
     @blp.login_required
-    @blp.etag
-    @blp.arguments(TimeseriesByZoneSchema)
-    @blp.response(201, TimeseriesByZoneSchema)
+    @blp.arguments(TimeseriesBySiteSchema)
+    @blp.response(201, TimeseriesBySiteSchema)
     @blp.catch_integrity_error
     def post(self, new_item):
-        """Add a new timeseries x zone association"""
-        item = TimeseriesByZone.new(**new_item)
+        """Add a new timeseries x site association"""
+        item = TimeseriesBySite.new(**new_item)
         db.session.commit()
         return item
 
 
 @blp.route("/<int:item_id>")
-class TimeseriesByZoneByIdViews(MethodView):
+class TimeseriesBySiteByIdViews(MethodView):
     @blp.login_required
-    @blp.etag
-    @blp.response(200, TimeseriesByZoneSchema)
+    @blp.response(200, TimeseriesBySiteSchema)
     def get(self, item_id):
-        """Get timeseries x zone association by ID"""
-        item = TimeseriesByZone.get_by_id(item_id)
+        """Get timeseries x site association by ID"""
+        item = TimeseriesBySite.get_by_id(item_id)
         if item is None:
             abort(404)
         return item
 
     @blp.login_required
-    @blp.etag
-    @blp.arguments(TimeseriesByZoneSchema)
-    @blp.response(200, TimeseriesByZoneSchema)
-    @blp.catch_integrity_error
-    def put(self, new_item, item_id):
-        """Update an existing timeseries x zone association"""
-        item = TimeseriesByZone.get_by_id(item_id)
-        if item is None:
-            abort(404)
-        blp.check_etag(item, TimeseriesByZoneSchema)
-        item.update(**new_item)
-        db.session.commit()
-        return item
-
-    @blp.login_required
-    @blp.etag
     @blp.response(204)
     def delete(self, item_id):
-        """Delete a timeseries x zone association"""
-        item = TimeseriesByZone.get_by_id(item_id)
+        """Delete a timeseries x site association"""
+        item = TimeseriesBySite.get_by_id(item_id)
         if item is None:
             abort(404)
-        blp.check_etag(item, TimeseriesByZoneSchema)
         item.delete()
         db.session.commit()
```

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/timeseries_data/routes.py` & `bemserver-api-0.9.0/bemserver_api/resources/timeseries_data/routes.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/timeseries_data/schemas.py` & `bemserver-api-0.9.0/bemserver_api/resources/timeseries_data/schemas.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/timeseries_data_states/routes.py` & `bemserver-api-0.9.0/bemserver_api/resources/timeseries_data_states/routes.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     description="Operations on timeseries data states",
 )
 
 
 @blp.route("/")
 class TimeseriesDataStatesViews(MethodView):
     @blp.login_required
+    @blp.etag
     @blp.response(200, TimeseriesDataStateSchema(many=True))
     def get(self):
         """List timeseries data states"""
         return TimeseriesDataState.get()
 
     @blp.login_required
     @blp.etag
```

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/timeseries_properties/routes.py` & `bemserver-api-0.9.0/bemserver_api/resources/timeseries_properties/routes.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     description="Operations on timeseries properties",
 )
 
 
 @blp.route("/")
 class TimeseriesPropertiesViews(MethodView):
     @blp.login_required
+    @blp.etag
     @blp.arguments(TimeseriesPropertyQueryArgsSchema, location="query")
     @blp.response(200, TimeseriesPropertySchema(many=True))
     def get(self, args):
         """List timeseries properties"""
         return TimeseriesProperty.get(**args)
 
     @blp.login_required
```

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/timeseries_properties/schemas.py` & `bemserver-api-0.9.0/bemserver_api/resources/timeseries_properties/schemas.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/timeseries_property_data/routes.py` & `bemserver-api-0.9.0/bemserver_api/resources/timeseries_property_data/routes.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/user_groups/routes.py` & `bemserver-api-0.9.0/bemserver_api/resources/user_groups/routes.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/user_groups_by_campaign_scopes/routes.py` & `bemserver-api-0.9.0/bemserver_api/resources/user_groups_by_campaign_scopes/routes.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,37 +20,34 @@
     description="Operations on user group x campaign scope associations",
 )
 
 
 @blp.route("/")
 class UserGroupByCampaignScopeViews(MethodView):
     @blp.login_required
-    @blp.etag
     @blp.arguments(UserGroupByCampaignScopeQueryArgsSchema, location="query")
     @blp.response(200, UserGroupByCampaignScopeSchema(many=True))
     def get(self, args):
         """List user group x campaign scope associations"""
         return UserGroupByCampaignScope.get(**args)
 
     @blp.login_required
-    @blp.etag
     @blp.arguments(UserGroupByCampaignScopeSchema)
     @blp.response(201, UserGroupByCampaignScopeSchema)
     @blp.catch_integrity_error
     def post(self, new_item):
         """Add a new user group x campaign scope association"""
         item = UserGroupByCampaignScope.new(**new_item)
         db.session.commit()
         return item
 
 
 @blp.route("/<int:item_id>")
 class UserGroupByCampaignScopeByIdViews(MethodView):
     @blp.login_required
-    @blp.etag
     @blp.response(200, UserGroupByCampaignScopeSchema)
     def get(self, item_id):
         """Get user group x campaign scope association by ID"""
         item = UserGroupByCampaignScope.get_by_id(item_id)
         if item is None:
             abort(404)
         return item
```

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/user_groups_by_campaign_scopes/schemas.py` & `bemserver-api-0.9.0/bemserver_api/resources/user_groups_by_campaign_scopes/schemas.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/user_groups_by_campaigns/routes.py` & `bemserver-api-0.9.0/bemserver_api/resources/user_groups_by_campaigns/routes.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,37 +17,34 @@
     description="Operations on user group x campaign associations",
 )
 
 
 @blp.route("/")
 class UserGroupByCampaignViews(MethodView):
     @blp.login_required
-    @blp.etag
     @blp.arguments(UserGroupByCampaignQueryArgsSchema, location="query")
     @blp.response(200, UserGroupByCampaignSchema(many=True))
     def get(self, args):
         """List user group x campaign associations"""
         return UserGroupByCampaign.get(**args)
 
     @blp.login_required
-    @blp.etag
     @blp.arguments(UserGroupByCampaignSchema)
     @blp.response(201, UserGroupByCampaignSchema)
     @blp.catch_integrity_error
     def post(self, new_item):
         """Add a new user group x campaign association"""
         item = UserGroupByCampaign.new(**new_item)
         db.session.commit()
         return item
 
 
 @blp.route("/<int:item_id>")
 class UserGroupByCampaignByIdViews(MethodView):
     @blp.login_required
-    @blp.etag
     @blp.response(200, UserGroupByCampaignSchema)
     def get(self, item_id):
         """Get user group x campaign association by ID"""
         item = UserGroupByCampaign.get_by_id(item_id)
         if item is None:
             abort(404)
         return item
```

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/users/schemas.py` & `bemserver-api-0.9.0/bemserver_api/resources/users/schemas.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/users_by_user_groups/routes.py` & `bemserver-api-0.9.0/bemserver_api/resources/users_by_user_groups/routes.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,37 +17,34 @@
     description="Operations on users x user groups associations",
 )
 
 
 @blp.route("/")
 class UserByUserGroupViews(MethodView):
     @blp.login_required
-    @blp.etag
     @blp.arguments(UserByUserGroupQueryArgsSchema, location="query")
     @blp.response(200, UserByUserGroupSchema(many=True))
     def get(self, args):
         """List user x user group associations"""
         return UserByUserGroup.get(**args)
 
     @blp.login_required
-    @blp.etag
     @blp.arguments(UserByUserGroupSchema)
     @blp.response(201, UserByUserGroupSchema)
     @blp.catch_integrity_error
     def post(self, new_item):
         """Add a new user x user group association"""
         item = UserByUserGroup.new(**new_item)
         db.session.commit()
         return item
 
 
 @blp.route("/<int:item_id>")
 class UserByUserGroupByIdViews(MethodView):
     @blp.login_required
-    @blp.etag
     @blp.response(200, UserByUserGroupSchema)
     def get(self, item_id):
         """Get user x user group association by ID"""
         item = UserByUserGroup.get_by_id(item_id)
         if item is None:
             abort(404)
         return item
```

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/zone_properties/routes.py` & `bemserver-api-0.9.0/bemserver_api/resources/zone_properties/routes.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,37 +20,34 @@
     description="Operations on zone properties",
 )
 
 
 @blp.route("/")
 class ZonePropertyViews(MethodView):
     @blp.login_required
-    @blp.etag
     @blp.arguments(ZonePropertyQueryArgsSchema, location="query")
     @blp.response(200, ZonePropertySchema(many=True))
     def get(self, args):
         """List zone properties"""
         return ZoneProperty.get(**args)
 
     @blp.login_required
-    @blp.etag
     @blp.arguments(ZonePropertySchema)
     @blp.response(201, ZonePropertySchema)
     @blp.catch_integrity_error
     def post(self, new_item):
         """Add a new zone property"""
         item = ZoneProperty.new(**new_item)
         db.session.commit()
         return item
 
 
 @blp.route("/<int:item_id>")
 class ZonePropertyByIdViews(MethodView):
     @blp.login_required
-    @blp.etag
     @blp.response(200, ZonePropertySchema)
     def get(self, item_id):
         """Get zone property by ID"""
         item = ZoneProperty.get_by_id(item_id)
         if item is None:
             abort(404)
         return item
```

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/zone_properties/schemas.py` & `bemserver-api-0.9.0/bemserver_api/resources/zone_properties/schemas.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/zone_property_data/routes.py` & `bemserver-api-0.9.0/bemserver_api/resources/zone_property_data/routes.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/zones/routes.py` & `bemserver-api-0.9.0/bemserver_api/resources/zones/routes.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/resources/zones/schemas.py` & `bemserver-api-0.9.0/bemserver_api/resources/zones/schemas.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api/settings.py` & `bemserver-api-0.9.0/bemserver_api/settings.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/bemserver_api.egg-info/PKG-INFO` & `bemserver-api-0.9.0/bemserver_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bemserver-api
-Version: 0.8.0
+Version: 0.9.0
 Summary: BEMServer API
 Home-page: https://github.com/BEMServer/bemserver-api
 Author: Nobatek/INEF4
 Author-email: jlafrechoux@nobatek.inef4.com
 License: AGPLv3+
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `bemserver-api-0.8.0/bemserver_api.egg-info/SOURCES.txt` & `bemserver-api-0.9.0/bemserver_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/requirements/dev.txt` & `bemserver-api-0.9.0/requirements/dev.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,56 +1,60 @@
 #
 # This file is autogenerated by pip-compile with python 3.9
 # To update, run:
 #
 #    pip-compile requirements/dev.in
 #
-attrs==22.1.0
+attrs==22.2.0
     # via pytest
 bump2version==1.0.1
     # via -r requirements/dev.in
 cfgv==3.3.1
     # via pre-commit
-coverage[toml]==6.5.0
+coverage[toml]==7.0.5
     # via pytest-cov
 distlib==0.3.6
     # via virtualenv
-filelock==3.8.0
+exceptiongroup==1.1.0
+    # via pytest
+filelock==3.9.0
     # via virtualenv
-identify==2.5.8
+identify==2.5.13
     # via pre-commit
-iniconfig==1.1.1
+iniconfig==2.0.0
     # via pytest
 mirakuru==2.4.2
     # via pytest-postgresql
 nodeenv==1.7.0
     # via pre-commit
-packaging==21.3
+packaging==23.0
     # via pytest
-platformdirs==2.5.4
+platformdirs==2.6.2
     # via virtualenv
 pluggy==1.0.0
     # via pytest
-port-for==0.6.2
+port-for==0.6.3
     # via pytest-postgresql
 pre-commit==2.21.0
     # via -r requirements/dev.in
 psutil==5.9.4
     # via mirakuru
-pyparsing==3.0.9
-    # via packaging
 pytest==7.2.0
     # via
     #   -r requirements/tests.in
     #   pytest-cov
     #   pytest-postgresql
 pytest-cov==4.0.0
     # via -r requirements/tests.in
 pytest-postgresql==3.1.3
     # via -r requirements/tests.in
 pyyaml==6.0
     # via pre-commit
-virtualenv==20.16.7
+tomli==2.0.1
+    # via
+    #   coverage
+    #   pytest
+virtualenv==20.17.1
     # via pre-commit
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `bemserver-api-0.8.0/requirements/install.txt` & `bemserver-api-0.9.0/requirements/install.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #
 # This file is autogenerated by pip-compile with python 3.9
 # To update, run:
 #
 #    pip-compile --output-file=requirements/install.txt setup.py
 #
-alembic==1.8.1
+alembic==1.9.1
     # via bemserver-core
 amqp==5.1.1
     # via kombu
 apispec[marshmallow]==6.0.2
     # via flask-smorest
 argon2-cffi==21.3.0
     # via bemserver-core
@@ -36,28 +36,26 @@
     #   flask
 click-didyoumean==0.3.0
     # via celery
 click-plugins==1.1.1
     # via celery
 click-repl==0.2.0
     # via celery
-deprecated==1.2.13
-    # via redis
 flask==2.2.2
     # via
     #   bemserver-api (setup.py)
     #   flask-httpauth
     #   flask-smorest
 flask-httpauth==4.7.0
     # via bemserver-api (setup.py)
 flask-smorest==0.40.0
     # via bemserver-api (setup.py)
 greenlet==2.0.1
     # via sqlalchemy
-importlib-metadata==5.0.0
+importlib-metadata==6.0.0
     # via flask
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via flask
 kombu==5.2.4
     # via celery
@@ -73,52 +71,49 @@
     #   apispec
     #   bemserver-api (setup.py)
     #   flask-smorest
     #   marshmallow-sqlalchemy
     #   webargs
 marshmallow-sqlalchemy==0.28.1
     # via bemserver-api (setup.py)
-numpy==1.23.4
+numpy==1.24.1
     # via pandas
 oso==0.26.4
     # via bemserver-core
-packaging==21.3
+packaging==23.0
     # via
     #   apispec
     #   marshmallow
     #   marshmallow-sqlalchemy
-    #   redis
     #   webargs
-pandas==1.5.1
+pandas==1.5.2
     # via bemserver-core
 passlib==1.7.4
     # via bemserver-core
-prompt-toolkit==3.0.32
+prompt-toolkit==3.0.36
     # via click-repl
 psycopg2==2.9.5
     # via bemserver-core
 pycparser==2.21
     # via cffi
-pyparsing==3.0.9
-    # via packaging
 python-dateutil==2.8.2
     # via pandas
 python-dotenv==0.21.0
     # via bemserver-api (setup.py)
-pytz==2022.6
+pytz==2022.7
     # via
     #   celery
     #   pandas
-redis==4.3.4
+redis==4.4.2
     # via bemserver-core
 six==1.16.0
     # via
     #   click-repl
     #   python-dateutil
-sqlalchemy==1.4.44
+sqlalchemy==1.4.46
     # via
     #   alembic
     #   bemserver-core
     #   marshmallow-sqlalchemy
 vine==5.0.0
     # via
     #   amqp
@@ -128,11 +123,9 @@
     # via prompt-toolkit
 webargs==8.2.0
     # via flask-smorest
 werkzeug==2.2.2
     # via
     #   flask
     #   flask-smorest
-wrapt==1.14.1
-    # via deprecated
-zipp==3.10.0
+zipp==3.11.0
     # via importlib-metadata
```

### Comparing `bemserver-api-0.8.0/requirements/tests.txt` & `bemserver-api-0.9.0/requirements/tests.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 #
 # This file is autogenerated by pip-compile with python 3.9
 # To update, run:
 #
 #    pip-compile requirements/tests.in
 #
-attrs==22.1.0
+attrs==22.2.0
     # via pytest
-coverage[toml]==6.5.0
+coverage[toml]==7.0.5
     # via pytest-cov
-exceptiongroup==1.0.4
+exceptiongroup==1.1.0
     # via pytest
-iniconfig==1.1.1
+iniconfig==2.0.0
     # via pytest
 mirakuru==2.4.2
     # via pytest-postgresql
-packaging==21.3
+packaging==23.0
     # via pytest
 pluggy==1.0.0
     # via pytest
-port-for==0.6.2
+port-for==0.6.3
     # via pytest-postgresql
 psutil==5.9.4
     # via mirakuru
-pyparsing==3.0.9
-    # via packaging
 pytest==7.2.0
     # via
     #   -r requirements/tests.in
     #   pytest-cov
     #   pytest-postgresql
 pytest-cov==4.0.0
     # via -r requirements/tests.in
```

### Comparing `bemserver-api-0.8.0/setup.py` & `bemserver-api-0.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Get the long description from the README file
 with open("README.rst", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="bemserver-api",
-    version="0.8.0",
+    version="0.9.0",
     description="BEMServer API",
     long_description=long_description,
     url="https://github.com/BEMServer/bemserver-api",
     author="Nobatek/INEF4",
     author_email="jlafrechoux@nobatek.inef4.com",
     license="AGPLv3+",
     classifiers=[
```

### Comparing `bemserver-api-0.8.0/tests/conftest.py` & `bemserver-api-0.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/tests/extensions/test_authentication.py` & `bemserver-api-0.9.0/tests/extensions/test_authentication.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/tests/extensions/test_integrity_error.py` & `bemserver-api-0.9.0/tests/extensions/test_integrity_error.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/tests/resources/analysis/test_completeness.py` & `bemserver-api-0.9.0/tests/resources/analysis/test_completeness.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/tests/resources/analysis/test_energy_consumption.py` & `bemserver-api-0.9.0/tests/resources/analysis/test_energy_consumption.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/tests/resources/test_about.py` & `bemserver-api-0.9.0/tests/resources/test_about.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/tests/resources/test_building_properties.py` & `bemserver-api-0.9.0/tests/resources/test_building_properties.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,14 @@
             building_p_1 = {
                 "structural_element_property_id": sep_1_id,
             }
             ret = client.post(BUILDING_PROPERTIES_URL, json=building_p_1)
             assert ret.status_code == 201
             ret_val = ret.json
             building_p_1_id = ret_val.pop("id")
-            building_p_1_etag = ret.headers["ETag"]
             sep = ret_val.pop("structural_element_property")
             assert sep == {"name": "Area", "value_type": "integer"}
             assert ret_val == building_p_1
 
             # POST violating unique constraint
             ret = client.post(BUILDING_PROPERTIES_URL, json=building_p_1)
             assert ret.status_code == 409
@@ -46,15 +45,14 @@
             ret_val = ret.json
             assert len(ret_val) == 1
             assert ret_val[0]["id"] == building_p_1_id
 
             # GET by id
             ret = client.get(f"{BUILDING_PROPERTIES_URL}{building_p_1_id}")
             assert ret.status_code == 200
-            assert ret.headers["ETag"] == building_p_1_etag
             ret_val = ret.json
             ret_val.pop("id")
             ret_val.pop("structural_element_property")
             assert ret_val == building_p_1
 
             # POST sep 2
             building_p_2 = {
```

### Comparing `bemserver-api-0.8.0/tests/resources/test_building_property_data.py` & `bemserver-api-0.9.0/tests/resources/test_building_property_data.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/tests/resources/test_buildings.py` & `bemserver-api-0.9.0/tests/resources/test_buildings.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/tests/resources/test_campaign_scopes.py` & `bemserver-api-0.9.0/tests/resources/test_campaign_scopes.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/tests/resources/test_campaigns.py` & `bemserver-api-0.9.0/tests/resources/test_campaigns.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/tests/resources/test_energy.py` & `bemserver-api-0.9.0/tests/resources/test_energy.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/tests/resources/test_energy_consumption_timeseries_by_buildings.py` & `bemserver-api-0.9.0/tests/resources/test_energy_consumption_timeseries_by_buildings.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/tests/resources/test_energy_consumption_timeseries_by_sites.py` & `bemserver-api-0.9.0/tests/resources/test_energy_consumption_timeseries_by_sites.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/tests/resources/test_event_categories.py` & `bemserver-api-0.9.0/tests/resources/test_event_categories.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/tests/resources/test_event_categories_by_users.py` & `bemserver-api-0.9.0/tests/resources/test_event_categories_by_users.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/tests/resources/test_events.py` & `bemserver-api-0.9.0/tests/resources/test_events.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/tests/resources/test_events_by_buildings.py` & `bemserver-api-0.9.0/tests/resources/test_events_by_buildings.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,16 @@
                 "event_id": event_1_id,
                 "building_id": building_1_id,
             }
             ret = client.post(EVENTS_BY_BUILDINGS_URL, json=ebb_1)
             assert ret.status_code == 201
             ret_val = ret.json
             ebb_1_id = ret_val.pop("id")
-            ebb_1_etag = ret.headers["ETag"]
+            assert ret_val.pop("site")["name"] == "Site 1"
+            assert ret_val.pop("building")["name"] == "Building 1"
             assert ret_val == ebb_1
 
             # POST violating unique constraint
             ret = client.post(EVENTS_BY_BUILDINGS_URL, json=ebb_1)
             assert ret.status_code == 409
 
             # POST event + building from different campaigns
@@ -62,17 +63,18 @@
             ret_val = ret.json
             assert len(ret_val) == 1
             assert ret_val[0]["id"] == ebb_1_id
 
             # GET by id
             ret = client.get(f"{EVENTS_BY_BUILDINGS_URL}{ebb_1_id}")
             assert ret.status_code == 200
-            assert ret.headers["ETag"] == ebb_1_etag
             ret_val = ret.json
             ret_val.pop("id")
+            assert ret_val.pop("site")["name"] == "Site 1"
+            assert ret_val.pop("building")["name"] == "Building 1"
             assert ret_val == ebb_1
 
             # POST
             ebb_2 = {
                 "event_id": event_2_id,
                 "building_id": building_2_id,
             }
```

### Comparing `bemserver-api-0.8.0/tests/resources/test_events_by_sites.py` & `bemserver-api-0.9.0/tests/resources/test_events_by_sites.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,15 +33,15 @@
                 "event_id": event_1_id,
                 "site_id": site_1_id,
             }
             ret = client.post(EVENTS_BY_SITES_URL, json=ebs_1)
             assert ret.status_code == 201
             ret_val = ret.json
             ebs_1_id = ret_val.pop("id")
-            ebs_1_etag = ret.headers["ETag"]
+            assert ret_val.pop("site")["name"] == "Site 1"
             assert ret_val == ebs_1
 
             # POST violating unique constraint
             ret = client.post(EVENTS_BY_SITES_URL, json=ebs_1)
             assert ret.status_code == 409
 
             # POST event + site from different campaigns
@@ -62,17 +62,17 @@
             ret_val = ret.json
             assert len(ret_val) == 1
             assert ret_val[0]["id"] == ebs_1_id
 
             # GET by id
             ret = client.get(f"{EVENTS_BY_SITES_URL}{ebs_1_id}")
             assert ret.status_code == 200
-            assert ret.headers["ETag"] == ebs_1_etag
             ret_val = ret.json
             ret_val.pop("id")
+            assert ret_val.pop("site")["name"] == "Site 1"
             assert ret_val == ebs_1
 
             # POST
             ebs_2 = {
                 "event_id": event_2_id,
                 "site_id": site_2_id,
             }
```

### Comparing `bemserver-api-0.8.0/tests/resources/test_events_by_spaces.py` & `bemserver-api-0.9.0/tests/resources/test_events_by_storeys.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,218 +1,215 @@
-"""Events by spaces routes tests"""
+"""Events by storeys routes tests"""
 import pytest
 
 from tests.common import AuthHeader
 
 
 DUMMY_ID = "69"
 
-EVENTS_BY_SPACES_URL = "/events_by_spaces/"
+EVENTS_BY_STOREYS_URL = "/events_by_storeys/"
 EVENTS_URL = "/events/"
 
 
-class TestEventBySpaceApi:
-    def test_events_by_spaces_api(self, app, users, spaces, events):
+class TestEventByStoreyApi:
+    def test_events_by_storeys_api(self, app, users, storeys, events):
 
         creds = users["Chuck"]["creds"]
         event_1_id = events[0]
         event_2_id = events[1]
-        space_1_id = spaces[0]
-        space_2_id = spaces[1]
+        storey_1_id = storeys[0]
+        storey_2_id = storeys[1]
 
         client = app.test_client()
 
         with AuthHeader(creds):
 
             # GET list
-            ret = client.get(EVENTS_BY_SPACES_URL)
+            ret = client.get(EVENTS_BY_STOREYS_URL)
             assert ret.status_code == 200
             assert ret.json == []
 
             # POST
             ebs_1 = {
                 "event_id": event_1_id,
-                "space_id": space_1_id,
+                "storey_id": storey_1_id,
             }
-            ret = client.post(EVENTS_BY_SPACES_URL, json=ebs_1)
+            ret = client.post(EVENTS_BY_STOREYS_URL, json=ebs_1)
             assert ret.status_code == 201
             ret_val = ret.json
             ebs_1_id = ret_val.pop("id")
-            ebs_1_etag = ret.headers["ETag"]
+            assert ret_val.pop("site")["name"] == "Site 1"
+            assert ret_val.pop("building")["name"] == "Building 1"
+            assert ret_val.pop("storey")["name"] == "Storey 1"
             assert ret_val == ebs_1
 
             # POST violating unique constraint
-            ret = client.post(EVENTS_BY_SPACES_URL, json=ebs_1)
+            ret = client.post(EVENTS_BY_STOREYS_URL, json=ebs_1)
             assert ret.status_code == 409
 
-            # POST event + space from different campaigns
+            # POST event + storey from different campaigns
             ebs = {
                 "event_id": event_2_id,
-                "space_id": space_1_id,
+                "storey_id": storey_1_id,
             }
-            ret = client.post(EVENTS_BY_SPACES_URL, json=ebs)
+            ret = client.post(EVENTS_BY_STOREYS_URL, json=ebs)
             assert ret.status_code == 422
             ret_val = ret.json
             assert ret_val["errors"]["json"]["_schema"] == (
-                "Event and space must be in same campaign"
+                "Event and storey must be in same campaign"
             )
 
             # GET list
-            ret = client.get(EVENTS_BY_SPACES_URL)
+            ret = client.get(EVENTS_BY_STOREYS_URL)
             assert ret.status_code == 200
             ret_val = ret.json
             assert len(ret_val) == 1
             assert ret_val[0]["id"] == ebs_1_id
 
             # GET by id
-            ret = client.get(f"{EVENTS_BY_SPACES_URL}{ebs_1_id}")
+            ret = client.get(f"{EVENTS_BY_STOREYS_URL}{ebs_1_id}")
             assert ret.status_code == 200
-            assert ret.headers["ETag"] == ebs_1_etag
             ret_val = ret.json
             ret_val.pop("id")
+            assert ret_val.pop("site")["name"] == "Site 1"
+            assert ret_val.pop("building")["name"] == "Building 1"
+            assert ret_val.pop("storey")["name"] == "Storey 1"
             assert ret_val == ebs_1
 
             # POST
             ebs_2 = {
                 "event_id": event_2_id,
-                "space_id": space_2_id,
+                "storey_id": storey_2_id,
             }
-            ret = client.post(EVENTS_BY_SPACES_URL, json=ebs_2)
+            ret = client.post(EVENTS_BY_STOREYS_URL, json=ebs_2)
             ret_val = ret.json
             ebs_2_id = ret_val.pop("id")
 
             # GET list
-            ret = client.get(EVENTS_BY_SPACES_URL)
+            ret = client.get(EVENTS_BY_STOREYS_URL)
             assert ret.status_code == 200
             ret_val = ret.json
             assert len(ret_val) == 2
 
             # GET list with filters
             ret = client.get(
-                EVENTS_BY_SPACES_URL,
+                EVENTS_BY_STOREYS_URL,
                 query_string={"event_id": event_1_id},
             )
             assert ret.status_code == 200
             ret_val = ret.json
             assert len(ret_val) == 1
             assert ret_val[0]["id"] == ebs_1_id
 
             # DELETE wrong ID -> 404
-            ret = client.delete(f"{EVENTS_BY_SPACES_URL}{DUMMY_ID}")
+            ret = client.delete(f"{EVENTS_BY_STOREYS_URL}{DUMMY_ID}")
             assert ret.status_code == 404
 
             # DELETE event cascade
             ret = client.get(f"{EVENTS_URL}{event_1_id}")
             event_1_etag = ret.headers["ETag"]
             ret = client.delete(
                 f"{EVENTS_URL}{event_1_id}", headers={"If-Match": event_1_etag}
             )
             assert ret.status_code == 204
 
             # DELETE
-            ret = client.delete(f"{EVENTS_BY_SPACES_URL}{ebs_1_id}")
+            ret = client.delete(f"{EVENTS_BY_STOREYS_URL}{ebs_1_id}")
             assert ret.status_code == 404
-            ret = client.delete(f"{EVENTS_BY_SPACES_URL}{ebs_2_id}")
+            ret = client.delete(f"{EVENTS_BY_STOREYS_URL}{ebs_2_id}")
             assert ret.status_code == 204
 
             # GET list
-            ret = client.get(EVENTS_BY_SPACES_URL)
+            ret = client.get(EVENTS_BY_STOREYS_URL)
             assert ret.status_code == 200
             ret_val = ret.json
             assert len(ret_val) == 0
 
             # GET by id -> 404
-            ret = client.get(f"{EVENTS_BY_SPACES_URL}{ebs_1_id}")
+            ret = client.get(f"{EVENTS_BY_STOREYS_URL}{ebs_1_id}")
             assert ret.status_code == 404
 
     @pytest.mark.usefixtures("users_by_user_groups")
     @pytest.mark.usefixtures("user_groups_by_campaigns")
     @pytest.mark.usefixtures("user_groups_by_campaign_scopes")
-    def test_events_by_spaces_as_user_api(
-        self, app, users, spaces, events, events_by_spaces
+    def test_events_by_storeys_as_user_api(
+        self, app, users, storeys, events, events_by_storeys
     ):
 
         user_creds = users["Active"]["creds"]
         event_1_id = events[0]
         event_2_id = events[1]
-        space_1_id = spaces[0]
-        space_2_id = spaces[1]
-        ebs_1_id = events_by_spaces[0]
-        ebs_2_id = events_by_spaces[1]
+        storey_1_id = storeys[0]
+        storey_2_id = storeys[1]
+        ebs_1_id = events_by_storeys[0]
+        ebs_2_id = events_by_storeys[1]
 
         client = app.test_client()
 
         with AuthHeader(user_creds):
 
             # GET list
-            ret = client.get(EVENTS_BY_SPACES_URL)
+            ret = client.get(EVENTS_BY_STOREYS_URL)
             assert ret.status_code == 200
             ret_val = ret.json
             assert len(ret_val) == 1
             ebs_1 = ret_val[0]
             assert ebs_1.pop("id") == ebs_1_id
 
             # GET by id
-            ret = client.get(f"{EVENTS_BY_SPACES_URL}{ebs_1_id}")
+            ret = client.get(f"{EVENTS_BY_STOREYS_URL}{ebs_1_id}")
             assert ret.status_code == 200
-            ebs_1_etag = ret.headers["ETag"]
 
             # GET by id not in campaign scope
-            ret = client.get(f"{EVENTS_BY_SPACES_URL}{ebs_2_id}")
+            ret = client.get(f"{EVENTS_BY_STOREYS_URL}{ebs_2_id}")
             assert ret.status_code == 403
 
             # DELETE
-            ret = client.delete(
-                f"{EVENTS_BY_SPACES_URL}{ebs_1_id}",
-                headers={"If-Match": ebs_1_etag},
-            )
+            ret = client.delete(f"{EVENTS_BY_STOREYS_URL}{ebs_1_id}")
             assert ret.status_code == 204
 
             # POST
             ebs_3 = {
                 "event_id": event_1_id,
-                "space_id": space_1_id,
+                "storey_id": storey_1_id,
             }
-            ret = client.post(EVENTS_BY_SPACES_URL, json=ebs_3)
+            ret = client.post(EVENTS_BY_STOREYS_URL, json=ebs_3)
             assert ret.status_code == 201
             ret_val = ret.json
 
             # POST not in campaign scope
             ebs = {
                 "event_id": event_2_id,
-                "space_id": space_2_id,
+                "storey_id": storey_2_id,
             }
-            ret = client.post(EVENTS_BY_SPACES_URL, json=ebs)
+            ret = client.post(EVENTS_BY_STOREYS_URL, json=ebs)
             assert ret.status_code == 403
 
-    def test_events_by_spaces_as_anonym_api(
-        self, app, spaces, events, events_by_spaces
+    def test_events_by_storeys_as_anonym_api(
+        self, app, storeys, events, events_by_storeys
     ):
         event_1_id = events[0]
-        space_2_id = spaces[1]
-        ebs_1_id = events_by_spaces[0]
+        storey_2_id = storeys[1]
+        ebs_1_id = events_by_storeys[0]
 
         client = app.test_client()
 
         # GET list
-        ret = client.get(EVENTS_BY_SPACES_URL)
+        ret = client.get(EVENTS_BY_STOREYS_URL)
         assert ret.status_code == 401
 
         # POST
         ebs_3 = {
             "event_id": event_1_id,
-            "space_id": space_2_id,
+            "storey_id": storey_2_id,
         }
-        ret = client.post(EVENTS_BY_SPACES_URL, json=ebs_3)
+        ret = client.post(EVENTS_BY_STOREYS_URL, json=ebs_3)
         assert ret.status_code == 401
 
         # GET by id
-        ret = client.get(f"{EVENTS_BY_SPACES_URL}{ebs_1_id}")
+        ret = client.get(f"{EVENTS_BY_STOREYS_URL}{ebs_1_id}")
         assert ret.status_code == 401
 
         # DELETE
-        ret = client.delete(
-            f"{EVENTS_BY_SPACES_URL}{ebs_1_id}",
-            headers={"If-Match": "Dummy-Etag"},
-        )
+        ret = client.delete(f"{EVENTS_BY_STOREYS_URL}{ebs_1_id}")
         # ETag is wrong but we get rejected before ETag check anyway
         assert ret.status_code == 401
```

### Comparing `bemserver-api-0.8.0/tests/resources/test_events_by_storeys.py` & `bemserver-api-0.9.0/tests/resources/test_events_by_zones.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,215 +1,209 @@
-"""Events by storeys routes tests"""
+"""Events by zones routes tests"""
 import pytest
 
 from tests.common import AuthHeader
 
 
 DUMMY_ID = "69"
 
-EVENTS_BY_STOREYS_URL = "/events_by_storeys/"
+EVENTS_BY_ZONES_URL = "/events_by_zones/"
 EVENTS_URL = "/events/"
 
 
-class TestEventByStoreyApi:
-    def test_events_by_storeys_api(self, app, users, storeys, events):
+class TestEventByZoneApi:
+    def test_events_by_zones_api(self, app, users, zones, events):
 
         creds = users["Chuck"]["creds"]
         event_1_id = events[0]
         event_2_id = events[1]
-        storey_1_id = storeys[0]
-        storey_2_id = storeys[1]
+        zone_1_id = zones[0]
+        zone_2_id = zones[1]
 
         client = app.test_client()
 
         with AuthHeader(creds):
 
             # GET list
-            ret = client.get(EVENTS_BY_STOREYS_URL)
+            ret = client.get(EVENTS_BY_ZONES_URL)
             assert ret.status_code == 200
             assert ret.json == []
 
             # POST
-            ebs_1 = {
+            ebz_1 = {
                 "event_id": event_1_id,
-                "storey_id": storey_1_id,
+                "zone_id": zone_1_id,
             }
-            ret = client.post(EVENTS_BY_STOREYS_URL, json=ebs_1)
+            ret = client.post(EVENTS_BY_ZONES_URL, json=ebz_1)
             assert ret.status_code == 201
             ret_val = ret.json
-            ebs_1_id = ret_val.pop("id")
-            ebs_1_etag = ret.headers["ETag"]
-            assert ret_val == ebs_1
+            ebz_1_id = ret_val.pop("id")
+            assert ret_val.pop("zone")["name"] == "Zone 1"
+            assert ret_val == ebz_1
 
             # POST violating unique constraint
-            ret = client.post(EVENTS_BY_STOREYS_URL, json=ebs_1)
+            ret = client.post(EVENTS_BY_ZONES_URL, json=ebz_1)
             assert ret.status_code == 409
 
-            # POST event + storey from different campaigns
-            ebs = {
+            # POST event + zone from different campaigns
+            ebz = {
                 "event_id": event_2_id,
-                "storey_id": storey_1_id,
+                "zone_id": zone_1_id,
             }
-            ret = client.post(EVENTS_BY_STOREYS_URL, json=ebs)
+            ret = client.post(EVENTS_BY_ZONES_URL, json=ebz)
             assert ret.status_code == 422
             ret_val = ret.json
             assert ret_val["errors"]["json"]["_schema"] == (
-                "Event and storey must be in same campaign"
+                "Event and zone must be in same campaign"
             )
 
             # GET list
-            ret = client.get(EVENTS_BY_STOREYS_URL)
+            ret = client.get(EVENTS_BY_ZONES_URL)
             assert ret.status_code == 200
             ret_val = ret.json
             assert len(ret_val) == 1
-            assert ret_val[0]["id"] == ebs_1_id
+            assert ret_val[0]["id"] == ebz_1_id
 
             # GET by id
-            ret = client.get(f"{EVENTS_BY_STOREYS_URL}{ebs_1_id}")
+            ret = client.get(f"{EVENTS_BY_ZONES_URL}{ebz_1_id}")
             assert ret.status_code == 200
-            assert ret.headers["ETag"] == ebs_1_etag
             ret_val = ret.json
             ret_val.pop("id")
-            assert ret_val == ebs_1
+            assert ret_val.pop("zone")["name"] == "Zone 1"
+            assert ret_val == ebz_1
 
             # POST
-            ebs_2 = {
+            ebz_2 = {
                 "event_id": event_2_id,
-                "storey_id": storey_2_id,
+                "zone_id": zone_2_id,
             }
-            ret = client.post(EVENTS_BY_STOREYS_URL, json=ebs_2)
+            ret = client.post(EVENTS_BY_ZONES_URL, json=ebz_2)
             ret_val = ret.json
-            ebs_2_id = ret_val.pop("id")
+            ebz_2_id = ret_val.pop("id")
 
             # GET list
-            ret = client.get(EVENTS_BY_STOREYS_URL)
+            ret = client.get(EVENTS_BY_ZONES_URL)
             assert ret.status_code == 200
             ret_val = ret.json
             assert len(ret_val) == 2
 
             # GET list with filters
             ret = client.get(
-                EVENTS_BY_STOREYS_URL,
+                EVENTS_BY_ZONES_URL,
                 query_string={"event_id": event_1_id},
             )
             assert ret.status_code == 200
             ret_val = ret.json
             assert len(ret_val) == 1
-            assert ret_val[0]["id"] == ebs_1_id
+            assert ret_val[0]["id"] == ebz_1_id
 
             # DELETE wrong ID -> 404
-            ret = client.delete(f"{EVENTS_BY_STOREYS_URL}{DUMMY_ID}")
+            ret = client.delete(f"{EVENTS_BY_ZONES_URL}{DUMMY_ID}")
             assert ret.status_code == 404
 
             # DELETE event cascade
             ret = client.get(f"{EVENTS_URL}{event_1_id}")
             event_1_etag = ret.headers["ETag"]
             ret = client.delete(
                 f"{EVENTS_URL}{event_1_id}", headers={"If-Match": event_1_etag}
             )
             assert ret.status_code == 204
 
             # DELETE
-            ret = client.delete(f"{EVENTS_BY_STOREYS_URL}{ebs_1_id}")
+            ret = client.delete(f"{EVENTS_BY_ZONES_URL}{ebz_1_id}")
             assert ret.status_code == 404
-            ret = client.delete(f"{EVENTS_BY_STOREYS_URL}{ebs_2_id}")
+            ret = client.delete(f"{EVENTS_BY_ZONES_URL}{ebz_2_id}")
             assert ret.status_code == 204
 
             # GET list
-            ret = client.get(EVENTS_BY_STOREYS_URL)
+            ret = client.get(EVENTS_BY_ZONES_URL)
             assert ret.status_code == 200
             ret_val = ret.json
             assert len(ret_val) == 0
 
             # GET by id -> 404
-            ret = client.get(f"{EVENTS_BY_STOREYS_URL}{ebs_1_id}")
+            ret = client.get(f"{EVENTS_BY_ZONES_URL}{ebz_1_id}")
             assert ret.status_code == 404
 
     @pytest.mark.usefixtures("users_by_user_groups")
     @pytest.mark.usefixtures("user_groups_by_campaigns")
     @pytest.mark.usefixtures("user_groups_by_campaign_scopes")
-    def test_events_by_storeys_as_user_api(
-        self, app, users, storeys, events, events_by_storeys
+    def test_events_by_zones_as_user_api(
+        self, app, users, zones, events, events_by_zones
     ):
 
         user_creds = users["Active"]["creds"]
         event_1_id = events[0]
         event_2_id = events[1]
-        storey_1_id = storeys[0]
-        storey_2_id = storeys[1]
-        ebs_1_id = events_by_storeys[0]
-        ebs_2_id = events_by_storeys[1]
+        zone_1_id = zones[0]
+        zone_2_id = zones[1]
+        ebz_1_id = events_by_zones[0]
+        ebz_2_id = events_by_zones[1]
 
         client = app.test_client()
 
         with AuthHeader(user_creds):
 
             # GET list
-            ret = client.get(EVENTS_BY_STOREYS_URL)
+            ret = client.get(EVENTS_BY_ZONES_URL)
             assert ret.status_code == 200
             ret_val = ret.json
             assert len(ret_val) == 1
-            ebs_1 = ret_val[0]
-            assert ebs_1.pop("id") == ebs_1_id
+            ebz_1 = ret_val[0]
+            assert ebz_1.pop("id") == ebz_1_id
 
             # GET by id
-            ret = client.get(f"{EVENTS_BY_STOREYS_URL}{ebs_1_id}")
+            ret = client.get(f"{EVENTS_BY_ZONES_URL}{ebz_1_id}")
             assert ret.status_code == 200
-            ebs_1_etag = ret.headers["ETag"]
 
             # GET by id not in campaign scope
-            ret = client.get(f"{EVENTS_BY_STOREYS_URL}{ebs_2_id}")
+            ret = client.get(f"{EVENTS_BY_ZONES_URL}{ebz_2_id}")
             assert ret.status_code == 403
 
             # DELETE
-            ret = client.delete(
-                f"{EVENTS_BY_STOREYS_URL}{ebs_1_id}",
-                headers={"If-Match": ebs_1_etag},
-            )
+            ret = client.delete(f"{EVENTS_BY_ZONES_URL}{ebz_1_id}")
             assert ret.status_code == 204
 
             # POST
-            ebs_3 = {
+            ebz_3 = {
                 "event_id": event_1_id,
-                "storey_id": storey_1_id,
+                "zone_id": zone_1_id,
             }
-            ret = client.post(EVENTS_BY_STOREYS_URL, json=ebs_3)
+            ret = client.post(EVENTS_BY_ZONES_URL, json=ebz_3)
             assert ret.status_code == 201
             ret_val = ret.json
 
             # POST not in campaign scope
-            ebs = {
+            ebz = {
                 "event_id": event_2_id,
-                "storey_id": storey_2_id,
+                "zone_id": zone_2_id,
             }
-            ret = client.post(EVENTS_BY_STOREYS_URL, json=ebs)
+            ret = client.post(EVENTS_BY_ZONES_URL, json=ebz)
             assert ret.status_code == 403
 
-    def test_events_by_storeys_as_anonym_api(
-        self, app, storeys, events, events_by_storeys
-    ):
+    def test_events_by_zones_as_anonym_api(self, app, zones, events, events_by_zones):
         event_1_id = events[0]
-        storey_2_id = storeys[1]
-        ebs_1_id = events_by_storeys[0]
+        zone_2_id = zones[1]
+        ebz_1_id = events_by_zones[0]
 
         client = app.test_client()
 
         # GET list
-        ret = client.get(EVENTS_BY_STOREYS_URL)
+        ret = client.get(EVENTS_BY_ZONES_URL)
         assert ret.status_code == 401
 
         # POST
-        ebs_3 = {
+        ebz_3 = {
             "event_id": event_1_id,
-            "storey_id": storey_2_id,
+            "zone_id": zone_2_id,
         }
-        ret = client.post(EVENTS_BY_STOREYS_URL, json=ebs_3)
+        ret = client.post(EVENTS_BY_ZONES_URL, json=ebz_3)
         assert ret.status_code == 401
 
         # GET by id
-        ret = client.get(f"{EVENTS_BY_STOREYS_URL}{ebs_1_id}")
+        ret = client.get(f"{EVENTS_BY_ZONES_URL}{ebz_1_id}")
         assert ret.status_code == 401
 
         # DELETE
-        ret = client.delete(f"{EVENTS_BY_STOREYS_URL}{ebs_1_id}")
+        ret = client.delete(f"{EVENTS_BY_ZONES_URL}{ebz_1_id}")
         # ETag is wrong but we get rejected before ETag check anyway
         assert ret.status_code == 401
```

### Comparing `bemserver-api-0.8.0/tests/resources/test_events_by_zones.py` & `bemserver-api-0.9.0/tests/resources/test_events_by_spaces.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,213 +1,220 @@
-"""Events by zones routes tests"""
+"""Events by spaces routes tests"""
 import pytest
 
 from tests.common import AuthHeader
 
 
 DUMMY_ID = "69"
 
-EVENTS_BY_ZONES_URL = "/events_by_zones/"
+EVENTS_BY_SPACES_URL = "/events_by_spaces/"
 EVENTS_URL = "/events/"
 
 
-class TestEventByZoneApi:
-    def test_events_by_zones_api(self, app, users, zones, events):
+class TestEventBySpaceApi:
+    def test_events_by_spaces_api(self, app, users, spaces, events):
 
         creds = users["Chuck"]["creds"]
         event_1_id = events[0]
         event_2_id = events[1]
-        zone_1_id = zones[0]
-        zone_2_id = zones[1]
+        space_1_id = spaces[0]
+        space_2_id = spaces[1]
 
         client = app.test_client()
 
         with AuthHeader(creds):
 
             # GET list
-            ret = client.get(EVENTS_BY_ZONES_URL)
+            ret = client.get(EVENTS_BY_SPACES_URL)
             assert ret.status_code == 200
             assert ret.json == []
 
             # POST
-            ebz_1 = {
+            ebs_1 = {
                 "event_id": event_1_id,
-                "zone_id": zone_1_id,
+                "space_id": space_1_id,
             }
-            ret = client.post(EVENTS_BY_ZONES_URL, json=ebz_1)
+            ret = client.post(EVENTS_BY_SPACES_URL, json=ebs_1)
             assert ret.status_code == 201
             ret_val = ret.json
-            ebz_1_id = ret_val.pop("id")
-            ebz_1_etag = ret.headers["ETag"]
-            assert ret_val == ebz_1
+            ebs_1_id = ret_val.pop("id")
+            assert ret_val.pop("site")["name"] == "Site 1"
+            assert ret_val.pop("building")["name"] == "Building 1"
+            assert ret_val.pop("storey")["name"] == "Storey 1"
+            assert ret_val.pop("space")["name"] == "Space 1"
+            assert ret_val == ebs_1
 
             # POST violating unique constraint
-            ret = client.post(EVENTS_BY_ZONES_URL, json=ebz_1)
+            ret = client.post(EVENTS_BY_SPACES_URL, json=ebs_1)
             assert ret.status_code == 409
 
-            # POST event + zone from different campaigns
-            ebz = {
+            # POST event + space from different campaigns
+            ebs = {
                 "event_id": event_2_id,
-                "zone_id": zone_1_id,
+                "space_id": space_1_id,
             }
-            ret = client.post(EVENTS_BY_ZONES_URL, json=ebz)
+            ret = client.post(EVENTS_BY_SPACES_URL, json=ebs)
             assert ret.status_code == 422
             ret_val = ret.json
             assert ret_val["errors"]["json"]["_schema"] == (
-                "Event and zone must be in same campaign"
+                "Event and space must be in same campaign"
             )
 
             # GET list
-            ret = client.get(EVENTS_BY_ZONES_URL)
+            ret = client.get(EVENTS_BY_SPACES_URL)
             assert ret.status_code == 200
             ret_val = ret.json
             assert len(ret_val) == 1
-            assert ret_val[0]["id"] == ebz_1_id
+            assert ret_val[0]["id"] == ebs_1_id
 
             # GET by id
-            ret = client.get(f"{EVENTS_BY_ZONES_URL}{ebz_1_id}")
+            ret = client.get(f"{EVENTS_BY_SPACES_URL}{ebs_1_id}")
             assert ret.status_code == 200
-            assert ret.headers["ETag"] == ebz_1_etag
             ret_val = ret.json
             ret_val.pop("id")
-            assert ret_val == ebz_1
+            assert ret_val.pop("site")["name"] == "Site 1"
+            assert ret_val.pop("building")["name"] == "Building 1"
+            assert ret_val.pop("storey")["name"] == "Storey 1"
+            assert ret_val.pop("space")["name"] == "Space 1"
+            assert ret_val == ebs_1
 
             # POST
-            ebz_2 = {
+            ebs_2 = {
                 "event_id": event_2_id,
-                "zone_id": zone_2_id,
+                "space_id": space_2_id,
             }
-            ret = client.post(EVENTS_BY_ZONES_URL, json=ebz_2)
+            ret = client.post(EVENTS_BY_SPACES_URL, json=ebs_2)
             ret_val = ret.json
-            ebz_2_id = ret_val.pop("id")
-            ebz_2_etag = ret.headers["ETag"]
+            ebs_2_id = ret_val.pop("id")
 
             # GET list
-            ret = client.get(EVENTS_BY_ZONES_URL)
+            ret = client.get(EVENTS_BY_SPACES_URL)
             assert ret.status_code == 200
             ret_val = ret.json
             assert len(ret_val) == 2
 
             # GET list with filters
             ret = client.get(
-                EVENTS_BY_ZONES_URL,
+                EVENTS_BY_SPACES_URL,
                 query_string={"event_id": event_1_id},
             )
             assert ret.status_code == 200
             ret_val = ret.json
             assert len(ret_val) == 1
-            assert ret_val[0]["id"] == ebz_1_id
+            assert ret_val[0]["id"] == ebs_1_id
 
             # DELETE wrong ID -> 404
-            ret = client.delete(f"{EVENTS_BY_ZONES_URL}{DUMMY_ID}")
+            ret = client.delete(f"{EVENTS_BY_SPACES_URL}{DUMMY_ID}")
             assert ret.status_code == 404
 
             # DELETE event cascade
             ret = client.get(f"{EVENTS_URL}{event_1_id}")
             event_1_etag = ret.headers["ETag"]
             ret = client.delete(
                 f"{EVENTS_URL}{event_1_id}", headers={"If-Match": event_1_etag}
             )
             assert ret.status_code == 204
 
             # DELETE
-            ret = client.delete(f"{EVENTS_BY_ZONES_URL}{ebz_1_id}")
+            ret = client.delete(f"{EVENTS_BY_SPACES_URL}{ebs_1_id}")
             assert ret.status_code == 404
-            ret = client.delete(
-                f"{EVENTS_BY_ZONES_URL}{ebz_2_id}",
-                headers={"If-Match": ebz_2_etag},
-            )
+            ret = client.delete(f"{EVENTS_BY_SPACES_URL}{ebs_2_id}")
             assert ret.status_code == 204
 
             # GET list
-            ret = client.get(EVENTS_BY_ZONES_URL)
+            ret = client.get(EVENTS_BY_SPACES_URL)
             assert ret.status_code == 200
             ret_val = ret.json
             assert len(ret_val) == 0
 
             # GET by id -> 404
-            ret = client.get(f"{EVENTS_BY_ZONES_URL}{ebz_1_id}")
+            ret = client.get(f"{EVENTS_BY_SPACES_URL}{ebs_1_id}")
             assert ret.status_code == 404
 
     @pytest.mark.usefixtures("users_by_user_groups")
     @pytest.mark.usefixtures("user_groups_by_campaigns")
     @pytest.mark.usefixtures("user_groups_by_campaign_scopes")
-    def test_events_by_zones_as_user_api(
-        self, app, users, zones, events, events_by_zones
+    def test_events_by_spaces_as_user_api(
+        self, app, users, spaces, events, events_by_spaces
     ):
 
         user_creds = users["Active"]["creds"]
         event_1_id = events[0]
         event_2_id = events[1]
-        zone_1_id = zones[0]
-        zone_2_id = zones[1]
-        ebz_1_id = events_by_zones[0]
-        ebz_2_id = events_by_zones[1]
+        space_1_id = spaces[0]
+        space_2_id = spaces[1]
+        ebs_1_id = events_by_spaces[0]
+        ebs_2_id = events_by_spaces[1]
 
         client = app.test_client()
 
         with AuthHeader(user_creds):
 
             # GET list
-            ret = client.get(EVENTS_BY_ZONES_URL)
+            ret = client.get(EVENTS_BY_SPACES_URL)
             assert ret.status_code == 200
             ret_val = ret.json
             assert len(ret_val) == 1
-            ebz_1 = ret_val[0]
-            assert ebz_1.pop("id") == ebz_1_id
+            ebs_1 = ret_val[0]
+            assert ebs_1.pop("id") == ebs_1_id
 
             # GET by id
-            ret = client.get(f"{EVENTS_BY_ZONES_URL}{ebz_1_id}")
+            ret = client.get(f"{EVENTS_BY_SPACES_URL}{ebs_1_id}")
             assert ret.status_code == 200
 
             # GET by id not in campaign scope
-            ret = client.get(f"{EVENTS_BY_ZONES_URL}{ebz_2_id}")
+            ret = client.get(f"{EVENTS_BY_SPACES_URL}{ebs_2_id}")
             assert ret.status_code == 403
 
             # DELETE
-            ret = client.delete(f"{EVENTS_BY_ZONES_URL}{ebz_1_id}")
+            ret = client.delete(f"{EVENTS_BY_SPACES_URL}{ebs_1_id}")
             assert ret.status_code == 204
 
             # POST
-            ebz_3 = {
+            ebs_3 = {
                 "event_id": event_1_id,
-                "zone_id": zone_1_id,
+                "space_id": space_1_id,
             }
-            ret = client.post(EVENTS_BY_ZONES_URL, json=ebz_3)
+            ret = client.post(EVENTS_BY_SPACES_URL, json=ebs_3)
             assert ret.status_code == 201
             ret_val = ret.json
 
             # POST not in campaign scope
-            ebz = {
+            ebs = {
                 "event_id": event_2_id,
-                "zone_id": zone_2_id,
+                "space_id": space_2_id,
             }
-            ret = client.post(EVENTS_BY_ZONES_URL, json=ebz)
+            ret = client.post(EVENTS_BY_SPACES_URL, json=ebs)
             assert ret.status_code == 403
 
-    def test_events_by_zones_as_anonym_api(self, app, zones, events, events_by_zones):
+    def test_events_by_spaces_as_anonym_api(
+        self, app, spaces, events, events_by_spaces
+    ):
         event_1_id = events[0]
-        zone_2_id = zones[1]
-        ebz_1_id = events_by_zones[0]
+        space_2_id = spaces[1]
+        ebs_1_id = events_by_spaces[0]
 
         client = app.test_client()
 
         # GET list
-        ret = client.get(EVENTS_BY_ZONES_URL)
+        ret = client.get(EVENTS_BY_SPACES_URL)
         assert ret.status_code == 401
 
         # POST
-        ebz_3 = {
+        ebs_3 = {
             "event_id": event_1_id,
-            "zone_id": zone_2_id,
+            "space_id": space_2_id,
         }
-        ret = client.post(EVENTS_BY_ZONES_URL, json=ebz_3)
+        ret = client.post(EVENTS_BY_SPACES_URL, json=ebs_3)
         assert ret.status_code == 401
 
         # GET by id
-        ret = client.get(f"{EVENTS_BY_ZONES_URL}{ebz_1_id}")
+        ret = client.get(f"{EVENTS_BY_SPACES_URL}{ebs_1_id}")
         assert ret.status_code == 401
 
         # DELETE
-        ret = client.delete(f"{EVENTS_BY_ZONES_URL}{ebz_1_id}")
+        ret = client.delete(
+            f"{EVENTS_BY_SPACES_URL}{ebs_1_id}",
+            headers={"If-Match": "Dummy-Etag"},
+        )
         # ETag is wrong but we get rejected before ETag check anyway
         assert ret.status_code == 401
```

### Comparing `bemserver-api-0.8.0/tests/resources/test_input_output.py` & `bemserver-api-0.9.0/tests/resources/test_input_output.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/tests/resources/test_notifications.py` & `bemserver-api-0.9.0/tests/resources/test_notifications.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,52 +36,44 @@
                 "user_id": user_1_id,
                 "timestamp": dt_1,
             }
             ret = client.post(NOTIFICATIONS_URL, json=notif_1)
             assert ret.status_code == 201
             ret_val = ret.json
             notif_1_id = ret_val.pop("id")
-            notif_1_etag = ret.headers["ETag"]
 
             # GET list
             ret = client.get(NOTIFICATIONS_URL)
             assert ret.status_code == 200
             ret_val = ret.json
             assert len(ret_val) == 1
 
             # GET by id
             ret = client.get(f"{NOTIFICATIONS_URL}{notif_1_id}")
             assert ret.status_code == 200
-            assert ret.headers["ETag"] == notif_1_etag
             ret_val = ret.json
             ret_val.pop("id")
             assert ret_val.pop("read") is False
             assert ret_val == notif_1
 
             # PUT wrong ID -> 404
             notif_1_put = {
                 "read": True,
             }
-            ret = client.put(
-                f"{NOTIFICATIONS_URL}{DUMMY_ID}",
-                json=notif_1_put,
-                headers={"If-Match": notif_1_etag},
-            )
+            ret = client.put(f"{NOTIFICATIONS_URL}{DUMMY_ID}", json=notif_1_put)
             assert ret.status_code == 404
 
             # PUT
             notif_1["read"] = True
             ret = client.put(
                 f"{NOTIFICATIONS_URL}{notif_1_id}",
                 json=notif_1_put,
-                headers={"If-Match": notif_1_etag},
             )
             assert ret.status_code == 200
             ret_val = ret.json
-            notif_1_etag = ret.headers["ETag"]
 
             # POST
             notif_2 = {
                 "event_id": event_1_id,
                 "user_id": user_2_id,
                 "timestamp": dt_2,
             }
@@ -126,25 +118,19 @@
             ret = client.get(NOTIFICATIONS_URL, query_string={"sort": "-timestamp"})
             assert ret.status_code == 200
             ret_val = ret.json
             assert len(ret_val) == 2
             assert ret_val[1]["id"] == notif_1_id
 
             # DELETE wrong ID -> 404
-            ret = client.delete(
-                f"{NOTIFICATIONS_URL}{DUMMY_ID}",
-                headers={"If-Match": notif_1_etag},
-            )
+            ret = client.delete(f"{NOTIFICATIONS_URL}{DUMMY_ID}")
             assert ret.status_code == 404
 
             # DELETE
-            ret = client.delete(
-                f"{NOTIFICATIONS_URL}{notif_1_id}",
-                headers={"If-Match": notif_1_etag},
-            )
+            ret = client.delete(f"{NOTIFICATIONS_URL}{notif_1_id}")
             assert ret.status_code == 204
 
             # GET list
             ret = client.get(NOTIFICATIONS_URL)
             assert ret.status_code == 200
             ret_val = ret.json
             assert len(ret_val) == 1
@@ -183,36 +169,27 @@
             # GET by id
             ret = client.get(f"{NOTIFICATIONS_URL}{notif_1_id}")
             assert ret.status_code == 200
             ret_val = ret.json
             ret_val.pop("id")
             notif_1 = ret_val
             assert notif_1["read"] is False
-            notif_1_etag = ret.headers["ETag"]
 
             ret = client.get(f"{NOTIFICATIONS_URL}{notif_2_id}")
             assert ret.status_code == 403
 
             # PUT - set read status
             notif_1_put = {
                 "read": True,
             }
-            ret = client.put(
-                f"{NOTIFICATIONS_URL}{notif_1_id}",
-                json=notif_1_put,
-                headers={"If-Match": notif_1_etag},
-            )
+            ret = client.put(f"{NOTIFICATIONS_URL}{notif_1_id}", json=notif_1_put)
             assert ret.status_code == 200
-            notif_1_etag = ret.headers["ETag"]
 
             # DELETE
-            ret = client.delete(
-                f"{NOTIFICATIONS_URL}{notif_1_id}",
-                headers={"If-Match": notif_1_etag},
-            )
+            ret = client.delete(f"{NOTIFICATIONS_URL}{notif_1_id}")
             assert ret.status_code == 403
 
     def test_notifications_as_anonym_api(self, app, users, events, notifications):
 
         user_1_id = users["Active"]["id"]
         event_1_id = events[0]
         notif_1_id = notifications[0]
```

### Comparing `bemserver-api-0.8.0/tests/resources/test_site_properties.py` & `bemserver-api-0.9.0/tests/resources/test_site_properties.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,14 @@
             site_p_1 = {
                 "structural_element_property_id": sep_1_id,
             }
             ret = client.post(SITE_PROPERTIES_URL, json=site_p_1)
             assert ret.status_code == 201
             ret_val = ret.json
             site_p_1_id = ret_val.pop("id")
-            site_p_1_etag = ret.headers["ETag"]
             sep = ret_val.pop("structural_element_property")
             assert sep == {"name": "Area", "value_type": "integer"}
             assert ret_val == site_p_1
 
             # POST violating unique constraint
             ret = client.post(SITE_PROPERTIES_URL, json=site_p_1)
             assert ret.status_code == 409
@@ -46,15 +45,14 @@
             ret_val = ret.json
             assert len(ret_val) == 1
             assert ret_val[0]["id"] == site_p_1_id
 
             # GET by id
             ret = client.get(f"{SITE_PROPERTIES_URL}{site_p_1_id}")
             assert ret.status_code == 200
-            assert ret.headers["ETag"] == site_p_1_etag
             ret_val = ret.json
             ret_val.pop("id")
             ret_val.pop("structural_element_property")
             assert ret_val == site_p_1
 
             # POST sep 2
             site_p_2 = {
```

### Comparing `bemserver-api-0.8.0/tests/resources/test_site_property_data.py` & `bemserver-api-0.9.0/tests/resources/test_site_property_data.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/tests/resources/test_sites.py` & `bemserver-api-0.9.0/tests/resources/test_sites.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/tests/resources/test_space_properties.py` & `bemserver-api-0.9.0/tests/resources/test_space_properties.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,14 @@
             space_p_1 = {
                 "structural_element_property_id": sep_1_id,
             }
             ret = client.post(SPACE_PROPERTIES_URL, json=space_p_1)
             assert ret.status_code == 201
             ret_val = ret.json
             space_p_1_id = ret_val.pop("id")
-            space_p_1_etag = ret.headers["ETag"]
             sep = ret_val.pop("structural_element_property")
             assert sep == {"name": "Area", "value_type": "integer"}
             assert ret_val == space_p_1
 
             # POST violating unique constraint
             ret = client.post(SPACE_PROPERTIES_URL, json=space_p_1)
             assert ret.status_code == 409
@@ -46,15 +45,14 @@
             ret_val = ret.json
             assert len(ret_val) == 1
             assert ret_val[0]["id"] == space_p_1_id
 
             # GET by id
             ret = client.get(f"{SPACE_PROPERTIES_URL}{space_p_1_id}")
             assert ret.status_code == 200
-            assert ret.headers["ETag"] == space_p_1_etag
             ret_val = ret.json
             ret_val.pop("id")
             ret_val.pop("structural_element_property")
             assert ret_val == space_p_1
 
             # POST sep 2
             space_p_2 = {
```

### Comparing `bemserver-api-0.8.0/tests/resources/test_space_property_data.py` & `bemserver-api-0.9.0/tests/resources/test_space_property_data.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/tests/resources/test_spaces.py` & `bemserver-api-0.9.0/tests/resources/test_spaces.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/tests/resources/test_st_check_missings_by_campaigns.py` & `bemserver-api-0.9.0/tests/resources/test_st_check_missings_by_campaigns.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/tests/resources/test_st_cleanups_by_campaigns.py` & `bemserver-api-0.9.0/tests/resources/test_st_cleanups_by_campaigns.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/tests/resources/test_st_cleanups_by_timeseries.py` & `bemserver-api-0.9.0/tests/resources/test_st_cleanups_by_timeseries.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/tests/resources/test_storey_properties.py` & `bemserver-api-0.9.0/tests/resources/test_storey_properties.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,14 @@
             storey_p_1 = {
                 "structural_element_property_id": sep_1_id,
             }
             ret = client.post(STOREY_PROPERTIES_URL, json=storey_p_1)
             assert ret.status_code == 201
             ret_val = ret.json
             storey_p_1_id = ret_val.pop("id")
-            storey_p_1_etag = ret.headers["ETag"]
             sep = ret_val.pop("structural_element_property")
             assert sep == {"name": "Area", "value_type": "integer"}
             assert ret_val == storey_p_1
 
             # POST violating unique constraint
             ret = client.post(STOREY_PROPERTIES_URL, json=storey_p_1)
             assert ret.status_code == 409
@@ -46,15 +45,14 @@
             ret_val = ret.json
             assert len(ret_val) == 1
             assert ret_val[0]["id"] == storey_p_1_id
 
             # GET by id
             ret = client.get(f"{STOREY_PROPERTIES_URL}{storey_p_1_id}")
             assert ret.status_code == 200
-            assert ret.headers["ETag"] == storey_p_1_etag
             ret_val = ret.json
             ret_val.pop("id")
             ret_val.pop("structural_element_property")
             assert ret_val == storey_p_1
 
             # POST sep 2
             storey_p_2 = {
```

### Comparing `bemserver-api-0.8.0/tests/resources/test_storey_property_data.py` & `bemserver-api-0.9.0/tests/resources/test_storey_property_data.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/tests/resources/test_storeys.py` & `bemserver-api-0.9.0/tests/resources/test_storeys.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/tests/resources/test_structural_element_properties.py` & `bemserver-api-0.9.0/tests/resources/test_structural_element_properties.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/tests/resources/test_timeseries.py` & `bemserver-api-0.9.0/tests/resources/test_timeseries.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/tests/resources/test_timeseries_by_buildings.py` & `bemserver-api-0.9.0/tests/resources/test_timeseries_by_events.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,256 +1,211 @@
-"""Timeseries by buildings routes tests"""
+"""Timeseries by events routes tests"""
 import pytest
 
 from tests.common import AuthHeader
 
 
 DUMMY_ID = "69"
 
-TIMESERIES_BY_BUILDINGS_URL = "/timeseries_by_buildings/"
-BUILDINGS_URL = "/buildings/"
+TIMESERIES_BY_EVENTS_URL = "/timeseries_by_events/"
+EVENTS_URL = "/events/"
 
 
-class TestTimeseriesByBuildingApi:
-    def test_timeseries_by_buildings_api(self, app, users, buildings, timeseries):
+class TestTimeseriesByEventApi:
+    @pytest.mark.parametrize("timeseries", (4,), indirect=True)
+    def test_timeseries_by_events_api(self, app, users, events, timeseries):
 
         creds = users["Chuck"]["creds"]
-        building_1_id = buildings[0]
-        building_2_id = buildings[1]
+        event_1_id = events[0]
+        event_2_id = events[1]
         ts_1_id = timeseries[0]
         ts_2_id = timeseries[1]
 
         client = app.test_client()
 
         with AuthHeader(creds):
 
             # GET list
-            ret = client.get(TIMESERIES_BY_BUILDINGS_URL)
+            ret = client.get(TIMESERIES_BY_EVENTS_URL)
             assert ret.status_code == 200
             assert ret.json == []
 
             # POST
-            tbb_1 = {
-                "building_id": building_1_id,
+            tbs_1 = {
+                "event_id": event_1_id,
                 "timeseries_id": ts_1_id,
             }
-            ret = client.post(TIMESERIES_BY_BUILDINGS_URL, json=tbb_1)
+            ret = client.post(TIMESERIES_BY_EVENTS_URL, json=tbs_1)
             assert ret.status_code == 201
             ret_val = ret.json
-            tbb_1_id = ret_val.pop("id")
-            tbb_1_etag = ret.headers["ETag"]
-            assert ret_val == tbb_1
+            tbs_1_id = ret_val.pop("id")
+            assert ret_val == tbs_1
 
             # POST violating unique constraint
-            ret = client.post(TIMESERIES_BY_BUILDINGS_URL, json=tbb_1)
+            ret = client.post(TIMESERIES_BY_EVENTS_URL, json=tbs_1)
             assert ret.status_code == 409
 
+            # POST event + TS from different campaign scopes
+            tbs = {
+                "event_id": event_2_id,
+                "timeseries_id": ts_1_id,
+            }
+            ret = client.post(TIMESERIES_BY_EVENTS_URL, json=tbs)
+            assert ret.status_code == 422
+            ret_val = ret.json
+            assert ret_val["errors"]["json"]["_schema"] == (
+                "Event and timeseries must be in same campaign scope"
+            )
+
             # GET list
-            ret = client.get(TIMESERIES_BY_BUILDINGS_URL)
+            ret = client.get(TIMESERIES_BY_EVENTS_URL)
             assert ret.status_code == 200
             ret_val = ret.json
             assert len(ret_val) == 1
             assert ret_val[0]["id"] == ts_1_id
 
             # GET by id
-            ret = client.get(f"{TIMESERIES_BY_BUILDINGS_URL}{tbb_1_id}")
-            assert ret.status_code == 200
-            assert ret.headers["ETag"] == tbb_1_etag
-            ret_val = ret.json
-            ret_val.pop("id")
-            assert ret_val == tbb_1
-
-            # PUT
-            tbb_1["timeseries_id"] = ts_2_id
-            ret = client.put(
-                f"{TIMESERIES_BY_BUILDINGS_URL}{tbb_1_id}",
-                json=tbb_1,
-                headers={"If-Match": tbb_1_etag},
-            )
+            ret = client.get(f"{TIMESERIES_BY_EVENTS_URL}{tbs_1_id}")
             assert ret.status_code == 200
             ret_val = ret.json
             ret_val.pop("id")
-            tbb_1_etag = ret.headers["ETag"]
-            assert ret_val == tbb_1
+            assert ret_val == tbs_1
 
-            # PUT wrong ID -> 404
-            ret = client.put(
-                f"{TIMESERIES_BY_BUILDINGS_URL}{DUMMY_ID}",
-                json=tbb_1,
-                headers={"If-Match": tbb_1_etag},
-            )
-            assert ret.status_code == 404
-
-            # POST sep 2
-            tbb_2 = {
-                "building_id": building_2_id,
+            # POST
+            tbs_2 = {
+                "event_id": event_2_id,
                 "timeseries_id": ts_2_id,
             }
-            ret = client.post(TIMESERIES_BY_BUILDINGS_URL, json=tbb_2)
+            ret = client.post(TIMESERIES_BY_EVENTS_URL, json=tbs_2)
             ret_val = ret.json
-            tbb_2_id = ret_val.pop("id")
-            tbb_2_etag = ret.headers["ETag"]
-
-            # PUT violating unique constraint
-            tbb_1["building_id"] = tbb_2["building_id"]
-            tbb_1["timeseries_id"] = tbb_2["timeseries_id"]
-            ret = client.put(
-                f"{TIMESERIES_BY_BUILDINGS_URL}{tbb_1_id}",
-                json=tbb_1,
-                headers={"If-Match": tbb_1_etag},
-            )
-            assert ret.status_code == 409
+            tbs_2_id = ret_val.pop("id")
 
             # GET list
-            ret = client.get(TIMESERIES_BY_BUILDINGS_URL)
+            ret = client.get(TIMESERIES_BY_EVENTS_URL)
             assert ret.status_code == 200
             ret_val = ret.json
             assert len(ret_val) == 2
 
             # GET list with filters
             ret = client.get(
-                TIMESERIES_BY_BUILDINGS_URL,
-                query_string={"building_id": building_1_id},
+                TIMESERIES_BY_EVENTS_URL,
+                query_string={"event_id": event_1_id},
             )
             assert ret.status_code == 200
             ret_val = ret.json
             assert len(ret_val) == 1
-            assert ret_val[0]["id"] == tbb_1_id
+            assert ret_val[0]["id"] == tbs_1_id
 
             # DELETE wrong ID -> 404
-            ret = client.delete(
-                f"{TIMESERIES_BY_BUILDINGS_URL}{DUMMY_ID}",
-                headers={"If-Match": tbb_1_etag},
-            )
+            ret = client.delete(f"{TIMESERIES_BY_EVENTS_URL}{DUMMY_ID}")
             assert ret.status_code == 404
 
-            # DELETE building cascade
-            ret = client.get(f"{BUILDINGS_URL}{building_1_id}")
-            building_1_etag = ret.headers["ETag"]
+            # DELETE event cascade
+            ret = client.get(f"{EVENTS_URL}{event_1_id}")
+            event_1_etag = ret.headers["ETag"]
             ret = client.delete(
-                f"{BUILDINGS_URL}{building_1_id}", headers={"If-Match": building_1_etag}
+                f"{EVENTS_URL}{event_1_id}", headers={"If-Match": event_1_etag}
             )
             assert ret.status_code == 204
 
             # DELETE
-            ret = client.delete(
-                f"{TIMESERIES_BY_BUILDINGS_URL}{tbb_1_id}",
-                headers={"If-Match": tbb_1_etag},
-            )
+            ret = client.delete(f"{TIMESERIES_BY_EVENTS_URL}{tbs_1_id}")
             assert ret.status_code == 404
-            ret = client.delete(
-                f"{TIMESERIES_BY_BUILDINGS_URL}{tbb_2_id}",
-                headers={"If-Match": tbb_2_etag},
-            )
+            ret = client.delete(f"{TIMESERIES_BY_EVENTS_URL}{tbs_2_id}")
             assert ret.status_code == 204
 
             # GET list
-            ret = client.get(TIMESERIES_BY_BUILDINGS_URL)
+            ret = client.get(TIMESERIES_BY_EVENTS_URL)
             assert ret.status_code == 200
             ret_val = ret.json
             assert len(ret_val) == 0
 
             # GET by id -> 404
-            ret = client.get(f"{TIMESERIES_BY_BUILDINGS_URL}{tbb_1_id}")
+            ret = client.get(f"{TIMESERIES_BY_EVENTS_URL}{tbs_1_id}")
             assert ret.status_code == 404
 
     @pytest.mark.usefixtures("users_by_user_groups")
     @pytest.mark.usefixtures("user_groups_by_campaigns")
     @pytest.mark.usefixtures("user_groups_by_campaign_scopes")
     @pytest.mark.parametrize("timeseries", (4,), indirect=True)
-    def test_timeseries_by_buildings_as_user_api(
-        self, app, users, buildings, timeseries, timeseries_by_buildings
+    def test_timeseries_by_events_as_user_api(
+        self, app, users, events, timeseries, timeseries_by_events
     ):
 
         user_creds = users["Active"]["creds"]
-        building_1_id = buildings[0]
-        ts_1_id = timeseries[0]
+        event_1_id = events[0]
+        event_2_id = events[1]
+        ts_2_id = timeseries[1]
         ts_3_id = timeseries[2]
-        tbb_1_id = timeseries_by_buildings[0]
+        tbs_1_id = timeseries_by_events[0]
+        tbs_2_id = timeseries_by_events[1]
 
         client = app.test_client()
 
         with AuthHeader(user_creds):
 
             # GET list
-            ret = client.get(TIMESERIES_BY_BUILDINGS_URL)
+            ret = client.get(TIMESERIES_BY_EVENTS_URL)
             assert ret.status_code == 200
             ret_val = ret.json
             assert len(ret_val) == 1
-            tbb_1 = ret_val[0]
-            assert tbb_1.pop("id") == tbb_1_id
+            tbs_1 = ret_val[0]
+            assert tbs_1.pop("id") == tbs_1_id
 
             # POST
-            tbb_3 = {
-                "building_id": building_1_id,
-                "timeseries_id": ts_1_id,
+            tbs_3 = {
+                "event_id": event_1_id,
+                "timeseries_id": ts_3_id,
+            }
+            ret = client.post(TIMESERIES_BY_EVENTS_URL, json=tbs_3)
+            assert ret.status_code == 201
+            ret_val = ret.json
+
+            # POST not in campaign scope
+            tbs = {
+                "event_id": event_2_id,
+                "timeseries_id": ts_2_id,
             }
-            ret = client.post(TIMESERIES_BY_BUILDINGS_URL, json=tbb_3)
+            ret = client.post(TIMESERIES_BY_EVENTS_URL, json=tbs)
             assert ret.status_code == 403
 
             # GET by id
-            ret = client.get(f"{TIMESERIES_BY_BUILDINGS_URL}{tbb_1_id}")
+            ret = client.get(f"{TIMESERIES_BY_EVENTS_URL}{tbs_1_id}")
             assert ret.status_code == 200
-            tbb_1_etag = ret.headers["ETag"]
 
-            # PUT
-            tbb_1["timeseries_id"] = ts_3_id
-            ret = client.put(
-                f"{TIMESERIES_BY_BUILDINGS_URL}{tbb_1_id}",
-                json=tbb_1,
-                headers={"If-Match": tbb_1_etag},
-            )
+            # GET by id not in campaign scope
+            ret = client.get(f"{TIMESERIES_BY_EVENTS_URL}{tbs_2_id}")
             assert ret.status_code == 403
 
             # DELETE
-            ret = client.delete(
-                f"{TIMESERIES_BY_BUILDINGS_URL}{tbb_1_id}",
-                headers={"If-Match": tbb_1_etag},
-            )
-            assert ret.status_code == 403
+            ret = client.delete(f"{TIMESERIES_BY_EVENTS_URL}{tbs_1_id}")
+            assert ret.status_code == 204
 
-    def test_timeseries_by_buildings_as_anonym_api(
-        self, app, buildings, timeseries, timeseries_by_buildings
+    def test_timeseries_by_events_as_anonym_api(
+        self, app, events, timeseries, timeseries_by_events
     ):
-        building_1_id = buildings[0]
-        ts_1_id = timeseries[0]
+        event_1_id = events[0]
         ts_2_id = timeseries[1]
-        tbb_1_id = timeseries_by_buildings[0]
+        tbs_1_id = timeseries_by_events[0]
 
         client = app.test_client()
 
         # GET list
-        ret = client.get(TIMESERIES_BY_BUILDINGS_URL)
+        ret = client.get(TIMESERIES_BY_EVENTS_URL)
         assert ret.status_code == 401
 
         # POST
-        tbb_3 = {
-            "building_id": building_1_id,
+        tbs_3 = {
+            "event_id": event_1_id,
             "timeseries_id": ts_2_id,
         }
-        ret = client.post(TIMESERIES_BY_BUILDINGS_URL, json=tbb_3)
+        ret = client.post(TIMESERIES_BY_EVENTS_URL, json=tbs_3)
         assert ret.status_code == 401
 
         # GET by id
-        ret = client.get(f"{TIMESERIES_BY_BUILDINGS_URL}{tbb_1_id}")
-        assert ret.status_code == 401
-
-        # PUT
-        tbb_1 = {
-            "building_id": building_1_id,
-            "timeseries_id": ts_1_id,
-        }
-        ret = client.put(
-            f"{TIMESERIES_BY_BUILDINGS_URL}{tbb_1_id}",
-            json=tbb_1,
-            headers={"If-Match": "Dummy-ETag"},
-        )
-        # ETag is wrong but we get rejected before ETag check anyway
+        ret = client.get(f"{TIMESERIES_BY_EVENTS_URL}{tbs_1_id}")
         assert ret.status_code == 401
 
         # DELETE
-        ret = client.delete(
-            f"{TIMESERIES_BY_BUILDINGS_URL}{tbb_1_id}",
-            headers={"If-Match": "Dummy-Etag"},
-        )
+        ret = client.delete(f"{TIMESERIES_BY_EVENTS_URL}{tbs_1_id}")
         # ETag is wrong but we get rejected before ETag check anyway
         assert ret.status_code == 401
```

### Comparing `bemserver-api-0.8.0/tests/resources/test_timeseries_by_events.py` & `bemserver-api-0.9.0/tests/resources/test_zones.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,217 +1,243 @@
-"""Timeseries by events routes tests"""
+"""Zones routes tests"""
 import pytest
 
 from tests.common import AuthHeader
 
 
 DUMMY_ID = "69"
 
-TIMESERIES_BY_EVENTS_URL = "/timeseries_by_events/"
-EVENTS_URL = "/events/"
+ZONES_URL = "/zones/"
 
 
-class TestTimeseriesByEventApi:
-    @pytest.mark.parametrize("timeseries", (4,), indirect=True)
-    def test_timeseries_by_events_api(self, app, users, events, timeseries):
+class TestZonesApi:
+    def test_zones_api(self, app, users, campaigns):
 
         creds = users["Chuck"]["creds"]
-        event_1_id = events[0]
-        event_2_id = events[1]
-        ts_1_id = timeseries[0]
-        ts_2_id = timeseries[1]
+        campaign_1_id = campaigns[0]
 
         client = app.test_client()
 
         with AuthHeader(creds):
 
             # GET list
-            ret = client.get(TIMESERIES_BY_EVENTS_URL)
+            ret = client.get(ZONES_URL)
             assert ret.status_code == 200
             assert ret.json == []
 
             # POST
-            tbs_1 = {
-                "event_id": event_1_id,
-                "timeseries_id": ts_1_id,
+            zone_1 = {
+                "name": "Zone 1",
+                "campaign_id": campaign_1_id,
             }
-            ret = client.post(TIMESERIES_BY_EVENTS_URL, json=tbs_1)
+            ret = client.post(ZONES_URL, json=zone_1)
             assert ret.status_code == 201
             ret_val = ret.json
-            tbs_1_id = ret_val.pop("id")
-            tbs_1_etag = ret.headers["ETag"]
-            assert ret_val == tbs_1
+            zone_1_id = ret_val.pop("id")
+            zone_1_etag = ret.headers["ETag"]
+            assert ret_val == zone_1
 
             # POST violating unique constraint
-            ret = client.post(TIMESERIES_BY_EVENTS_URL, json=tbs_1)
+            ret = client.post(ZONES_URL, json=zone_1)
             assert ret.status_code == 409
 
-            # POST event + TS from different campaign scopes
-            tbs = {
-                "event_id": event_2_id,
-                "timeseries_id": ts_1_id,
-            }
-            ret = client.post(TIMESERIES_BY_EVENTS_URL, json=tbs)
-            assert ret.status_code == 422
-            ret_val = ret.json
-            assert ret_val["errors"]["json"]["_schema"] == (
-                "Event and timeseries must be in same campaign scope"
-            )
-
             # GET list
-            ret = client.get(TIMESERIES_BY_EVENTS_URL)
+            ret = client.get(ZONES_URL)
             assert ret.status_code == 200
             ret_val = ret.json
             assert len(ret_val) == 1
-            assert ret_val[0]["id"] == ts_1_id
+            assert ret_val[0]["id"] == zone_1_id
 
             # GET by id
-            ret = client.get(f"{TIMESERIES_BY_EVENTS_URL}{tbs_1_id}")
+            ret = client.get(f"{ZONES_URL}{zone_1_id}")
             assert ret.status_code == 200
-            assert ret.headers["ETag"] == tbs_1_etag
+            assert ret.headers["ETag"] == zone_1_etag
             ret_val = ret.json
             ret_val.pop("id")
-            assert ret_val == tbs_1
+            assert ret_val == zone_1
 
-            # POST
-            tbs_2 = {
-                "event_id": event_2_id,
-                "timeseries_id": ts_2_id,
+            # PUT
+            zone_1["description"] = "Fantastic zone"
+            zone_1_put = zone_1.copy()
+            del zone_1_put["campaign_id"]
+            ret = client.put(
+                f"{ZONES_URL}{zone_1_id}",
+                json=zone_1_put,
+                headers={"If-Match": zone_1_etag},
+            )
+            assert ret.status_code == 200
+            ret_val = ret.json
+            ret_val.pop("id")
+            zone_1_etag = ret.headers["ETag"]
+            assert ret_val == zone_1
+
+            # PUT wrong ID -> 404
+            ret = client.put(
+                f"{ZONES_URL}{DUMMY_ID}",
+                json=zone_1_put,
+                headers={"If-Match": zone_1_etag},
+            )
+            assert ret.status_code == 404
+
+            # POST zone 2
+            zone_2 = {
+                "name": "Zone 2",
+                "campaign_id": campaign_1_id,
             }
-            ret = client.post(TIMESERIES_BY_EVENTS_URL, json=tbs_2)
+            ret = client.post(ZONES_URL, json=zone_2)
             ret_val = ret.json
-            tbs_2_id = ret_val.pop("id")
+            zone_2_id = ret_val.pop("id")
+            zone_2_etag = ret.headers["ETag"]
+
+            # PUT violating unique constraint
+            zone_1_put["name"] = zone_2["name"]
+            ret = client.put(
+                f"{ZONES_URL}{zone_1_id}",
+                json=zone_1_put,
+                headers={"If-Match": zone_1_etag},
+            )
+            assert ret.status_code == 409
 
             # GET list
-            ret = client.get(TIMESERIES_BY_EVENTS_URL)
+            ret = client.get(ZONES_URL)
             assert ret.status_code == 200
             ret_val = ret.json
             assert len(ret_val) == 2
 
             # GET list with filters
-            ret = client.get(
-                TIMESERIES_BY_EVENTS_URL,
-                query_string={"event_id": event_1_id},
-            )
+            ret = client.get(ZONES_URL, query_string={"name": "Zone 1"})
             assert ret.status_code == 200
             ret_val = ret.json
             assert len(ret_val) == 1
-            assert ret_val[0]["id"] == tbs_1_id
+            assert ret_val[0]["id"] == zone_1_id
 
             # DELETE wrong ID -> 404
-            ret = client.delete(f"{TIMESERIES_BY_EVENTS_URL}{DUMMY_ID}")
+            ret = client.delete(
+                f"{ZONES_URL}{DUMMY_ID}", headers={"If-Match": zone_1_etag}
+            )
             assert ret.status_code == 404
 
-            # DELETE event cascade
-            ret = client.get(f"{EVENTS_URL}{event_1_id}")
-            event_1_etag = ret.headers["ETag"]
+            # DELETE
             ret = client.delete(
-                f"{EVENTS_URL}{event_1_id}", headers={"If-Match": event_1_etag}
+                f"{ZONES_URL}{zone_1_id}", headers={"If-Match": zone_1_etag}
             )
             assert ret.status_code == 204
-
-            # DELETE
-            ret = client.delete(f"{TIMESERIES_BY_EVENTS_URL}{tbs_1_id}")
-            assert ret.status_code == 404
-            ret = client.delete(f"{TIMESERIES_BY_EVENTS_URL}{tbs_2_id}")
+            ret = client.delete(
+                f"{ZONES_URL}{zone_2_id}", headers={"If-Match": zone_2_etag}
+            )
             assert ret.status_code == 204
 
             # GET list
-            ret = client.get(TIMESERIES_BY_EVENTS_URL)
+            ret = client.get(ZONES_URL)
             assert ret.status_code == 200
             ret_val = ret.json
             assert len(ret_val) == 0
 
             # GET by id -> 404
-            ret = client.get(f"{TIMESERIES_BY_EVENTS_URL}{tbs_1_id}")
+            ret = client.get(f"{ZONES_URL}{zone_1_id}")
             assert ret.status_code == 404
 
     @pytest.mark.usefixtures("users_by_user_groups")
     @pytest.mark.usefixtures("user_groups_by_campaigns")
-    @pytest.mark.usefixtures("user_groups_by_campaign_scopes")
-    @pytest.mark.parametrize("timeseries", (4,), indirect=True)
-    def test_timeseries_by_events_as_user_api(
-        self, app, users, events, timeseries, timeseries_by_events
-    ):
+    def test_zones_as_user_api(self, app, users, campaigns, zones):
 
         user_creds = users["Active"]["creds"]
-        event_1_id = events[0]
-        event_2_id = events[1]
-        ts_2_id = timeseries[1]
-        ts_3_id = timeseries[2]
-        tbs_1_id = timeseries_by_events[0]
-        tbs_2_id = timeseries_by_events[1]
+        campaign_2_id = campaigns[1]
+        zone_1_id = zones[0]
+        zone_2_id = zones[1]
 
         client = app.test_client()
 
         with AuthHeader(user_creds):
 
             # GET list
-            ret = client.get(TIMESERIES_BY_EVENTS_URL)
+            ret = client.get(ZONES_URL)
             assert ret.status_code == 200
             ret_val = ret.json
             assert len(ret_val) == 1
-            tbs_1 = ret_val[0]
-            assert tbs_1.pop("id") == tbs_1_id
+            zone_1 = ret_val[0]
+            assert zone_1.pop("id") == zone_1_id
 
-            # POST
-            tbs_3 = {
-                "event_id": event_1_id,
-                "timeseries_id": ts_3_id,
-            }
-            ret = client.post(TIMESERIES_BY_EVENTS_URL, json=tbs_3)
-            assert ret.status_code == 201
+            # GET list with filters
+            ret = client.get(ZONES_URL, query_string={"name": "Zone 1"})
+            assert ret.status_code == 200
             ret_val = ret.json
+            assert len(ret_val) == 1
+            assert ret_val[0]["id"] == zone_1_id
+            ret = client.get(ZONES_URL, query_string={"name": "Zone 2"})
+            assert ret.status_code == 200
+            assert not ret.json
 
-            # POST not in campaign scope
-            tbs = {
-                "event_id": event_2_id,
-                "timeseries_id": ts_2_id,
+            # POST
+            zone_3 = {
+                "name": "Zone 3",
+                "campaign_id": campaign_2_id,
             }
-            ret = client.post(TIMESERIES_BY_EVENTS_URL, json=tbs)
+            ret = client.post(ZONES_URL, json=zone_3)
             assert ret.status_code == 403
 
             # GET by id
-            ret = client.get(f"{TIMESERIES_BY_EVENTS_URL}{tbs_1_id}")
+            ret = client.get(f"{ZONES_URL}{zone_1_id}")
             assert ret.status_code == 200
-            tbs_1_etag = ret.headers["ETag"]
+            zone_1_etag = ret.headers["ETag"]
 
-            # GET by id not in campaign scope
-            ret = client.get(f"{TIMESERIES_BY_EVENTS_URL}{tbs_2_id}")
+            ret = client.get(f"{ZONES_URL}{zone_2_id}")
+            assert ret.status_code == 403
+
+            # PUT
+            zone_1["description"] = "Fantastic zone"
+            zone_1_put = zone_1.copy()
+            del zone_1_put["campaign_id"]
+            ret = client.put(
+                f"{ZONES_URL}{zone_1_id}",
+                json=zone_1_put,
+                headers={"If-Match": zone_1_etag},
+            )
             assert ret.status_code == 403
 
             # DELETE
             ret = client.delete(
-                f"{TIMESERIES_BY_EVENTS_URL}{tbs_1_id}",
-                headers={"If-Match": tbs_1_etag},
+                f"{ZONES_URL}{zone_1_id}", headers={"If-Match": zone_1_etag}
             )
-            assert ret.status_code == 204
+            assert ret.status_code == 403
 
-    def test_timeseries_by_events_as_anonym_api(
-        self, app, events, timeseries, timeseries_by_events
-    ):
-        event_1_id = events[0]
-        ts_2_id = timeseries[1]
-        tbs_1_id = timeseries_by_events[0]
+    def test_zones_as_anonym_api(self, app, zones, campaigns):
+
+        zone_1_id = zones[0]
+        campaign_1_id = campaigns[0]
 
         client = app.test_client()
 
         # GET list
-        ret = client.get(TIMESERIES_BY_EVENTS_URL)
+        ret = client.get(ZONES_URL)
         assert ret.status_code == 401
 
         # POST
-        tbs_3 = {
-            "event_id": event_1_id,
-            "timeseries_id": ts_2_id,
+        zone_3 = {
+            "name": "Zone 3",
+            "campaign_id": campaign_1_id,
         }
-        ret = client.post(TIMESERIES_BY_EVENTS_URL, json=tbs_3)
+        ret = client.post(ZONES_URL, json=zone_3)
         assert ret.status_code == 401
 
         # GET by id
-        ret = client.get(f"{TIMESERIES_BY_EVENTS_URL}{tbs_1_id}")
+        ret = client.get(f"{ZONES_URL}{zone_1_id}")
+        assert ret.status_code == 401
+
+        # PUT
+        zone_1 = {
+            "name": "Super Zone 1",
+        }
+        ret = client.put(
+            f"{ZONES_URL}{zone_1_id}",
+            json=zone_1,
+            headers={"If-Match": "Dummy-ETag"},
+        )
+        # ETag is wrong but we get rejected before ETag check anyway
         assert ret.status_code == 401
 
         # DELETE
-        ret = client.delete(f"{TIMESERIES_BY_EVENTS_URL}{tbs_1_id}")
+        ret = client.delete(
+            f"{ZONES_URL}{zone_1_id}", headers={"If-Match": "Dummy-Etag"}
+        )
         # ETag is wrong but we get rejected before ETag check anyway
         assert ret.status_code == 401
```

### Comparing `bemserver-api-0.8.0/tests/resources/test_timeseries_by_sites.py` & `bemserver-api-0.9.0/tests/resources/test_timeseries_by_sites.py`

 * *Files 22% similar despite different names*

```diff
@@ -33,15 +33,15 @@
                 "site_id": site_1_id,
                 "timeseries_id": ts_1_id,
             }
             ret = client.post(TIMESERIES_BY_SITES_URL, json=tbs_1)
             assert ret.status_code == 201
             ret_val = ret.json
             tbs_1_id = ret_val.pop("id")
-            tbs_1_etag = ret.headers["ETag"]
+            assert ret_val.pop("site")["name"] == "Site 1"
             assert ret_val == tbs_1
 
             # POST violating unique constraint
             ret = client.post(TIMESERIES_BY_SITES_URL, json=tbs_1)
             assert ret.status_code == 409
 
             # GET list
@@ -50,59 +50,27 @@
             ret_val = ret.json
             assert len(ret_val) == 1
             assert ret_val[0]["id"] == ts_1_id
 
             # GET by id
             ret = client.get(f"{TIMESERIES_BY_SITES_URL}{tbs_1_id}")
             assert ret.status_code == 200
-            assert ret.headers["ETag"] == tbs_1_etag
             ret_val = ret.json
             ret_val.pop("id")
+            assert ret_val.pop("site")["name"] == "Site 1"
             assert ret_val == tbs_1
 
-            # PUT
-            tbs_1["timeseries_id"] = ts_2_id
-            ret = client.put(
-                f"{TIMESERIES_BY_SITES_URL}{tbs_1_id}",
-                json=tbs_1,
-                headers={"If-Match": tbs_1_etag},
-            )
-            assert ret.status_code == 200
-            ret_val = ret.json
-            ret_val.pop("id")
-            tbs_1_etag = ret.headers["ETag"]
-            assert ret_val == tbs_1
-
-            # PUT wrong ID -> 404
-            ret = client.put(
-                f"{TIMESERIES_BY_SITES_URL}{DUMMY_ID}",
-                json=tbs_1,
-                headers={"If-Match": tbs_1_etag},
-            )
-            assert ret.status_code == 404
-
             # POST sep 2
             tbs_2 = {
                 "site_id": site_2_id,
                 "timeseries_id": ts_2_id,
             }
             ret = client.post(TIMESERIES_BY_SITES_URL, json=tbs_2)
             ret_val = ret.json
             tbs_2_id = ret_val.pop("id")
-            tbs_2_etag = ret.headers["ETag"]
-
-            # PUT violating unique constraint
-            tbs_1["site_id"] = tbs_2["site_id"]
-            tbs_1["timeseries_id"] = tbs_2["timeseries_id"]
-            ret = client.put(
-                f"{TIMESERIES_BY_SITES_URL}{tbs_1_id}",
-                json=tbs_1,
-                headers={"If-Match": tbs_1_etag},
-            )
-            assert ret.status_code == 409
 
             # GET list
             ret = client.get(TIMESERIES_BY_SITES_URL)
             assert ret.status_code == 200
             ret_val = ret.json
             assert len(ret_val) == 2
 
@@ -115,36 +83,29 @@
             ret_val = ret.json
             assert len(ret_val) == 1
             assert ret_val[0]["id"] == tbs_1_id
 
             # DELETE wrong ID -> 404
             ret = client.delete(
                 f"{TIMESERIES_BY_SITES_URL}{DUMMY_ID}",
-                headers={"If-Match": tbs_1_etag},
             )
             assert ret.status_code == 404
 
             # DELETE site cascade
             ret = client.get(f"{SITES_URL}{site_1_id}")
             site_1_etag = ret.headers["ETag"]
             ret = client.delete(
                 f"{SITES_URL}{site_1_id}", headers={"If-Match": site_1_etag}
             )
             assert ret.status_code == 204
 
             # DELETE
-            ret = client.delete(
-                f"{TIMESERIES_BY_SITES_URL}{tbs_1_id}",
-                headers={"If-Match": tbs_1_etag},
-            )
+            ret = client.delete(f"{TIMESERIES_BY_SITES_URL}{tbs_1_id}")
             assert ret.status_code == 404
-            ret = client.delete(
-                f"{TIMESERIES_BY_SITES_URL}{tbs_2_id}",
-                headers={"If-Match": tbs_2_etag},
-            )
+            ret = client.delete(f"{TIMESERIES_BY_SITES_URL}{tbs_2_id}")
             assert ret.status_code == 204
 
             # GET list
             ret = client.get(TIMESERIES_BY_SITES_URL)
             assert ret.status_code == 200
             ret_val = ret.json
             assert len(ret_val) == 0
@@ -152,23 +113,21 @@
             # GET by id -> 404
             ret = client.get(f"{TIMESERIES_BY_SITES_URL}{tbs_1_id}")
             assert ret.status_code == 404
 
     @pytest.mark.usefixtures("users_by_user_groups")
     @pytest.mark.usefixtures("user_groups_by_campaigns")
     @pytest.mark.usefixtures("user_groups_by_campaign_scopes")
-    @pytest.mark.parametrize("timeseries", (4,), indirect=True)
     def test_timeseries_by_sites_as_user_api(
         self, app, users, sites, timeseries, timeseries_by_sites
     ):
 
         user_creds = users["Active"]["creds"]
         site_1_id = sites[0]
         ts_1_id = timeseries[0]
-        ts_3_id = timeseries[2]
         tbs_1_id = timeseries_by_sites[0]
 
         client = app.test_client()
 
         with AuthHeader(user_creds):
 
             # GET list
@@ -186,37 +145,23 @@
             }
             ret = client.post(TIMESERIES_BY_SITES_URL, json=tbs_3)
             assert ret.status_code == 403
 
             # GET by id
             ret = client.get(f"{TIMESERIES_BY_SITES_URL}{tbs_1_id}")
             assert ret.status_code == 200
-            tbs_1_etag = ret.headers["ETag"]
-
-            # PUT
-            tbs_1["timeseries_id"] = ts_3_id
-            ret = client.put(
-                f"{TIMESERIES_BY_SITES_URL}{tbs_1_id}",
-                json=tbs_1,
-                headers={"If-Match": tbs_1_etag},
-            )
-            assert ret.status_code == 403
 
             # DELETE
-            ret = client.delete(
-                f"{TIMESERIES_BY_SITES_URL}{tbs_1_id}",
-                headers={"If-Match": tbs_1_etag},
-            )
+            ret = client.delete(f"{TIMESERIES_BY_SITES_URL}{tbs_1_id}")
             assert ret.status_code == 403
 
     def test_timeseries_by_sites_as_anonym_api(
         self, app, sites, timeseries, timeseries_by_sites
     ):
         site_1_id = sites[0]
-        ts_1_id = timeseries[0]
         ts_2_id = timeseries[1]
         tbs_1_id = timeseries_by_sites[0]
 
         client = app.test_client()
 
         # GET list
         ret = client.get(TIMESERIES_BY_SITES_URL)
@@ -230,27 +175,10 @@
         ret = client.post(TIMESERIES_BY_SITES_URL, json=tbs_3)
         assert ret.status_code == 401
 
         # GET by id
         ret = client.get(f"{TIMESERIES_BY_SITES_URL}{tbs_1_id}")
         assert ret.status_code == 401
 
-        # PUT
-        tbs_1 = {
-            "site_id": site_1_id,
-            "timeseries_id": ts_1_id,
-        }
-        ret = client.put(
-            f"{TIMESERIES_BY_SITES_URL}{tbs_1_id}",
-            json=tbs_1,
-            headers={"If-Match": "Dummy-ETag"},
-        )
-        # ETag is wrong but we get rejected before ETag check anyway
-        assert ret.status_code == 401
-
         # DELETE
-        ret = client.delete(
-            f"{TIMESERIES_BY_SITES_URL}{tbs_1_id}",
-            headers={"If-Match": "Dummy-Etag"},
-        )
-        # ETag is wrong but we get rejected before ETag check anyway
+        ret = client.delete(f"{TIMESERIES_BY_SITES_URL}{tbs_1_id}")
         assert ret.status_code == 401
```

### Comparing `bemserver-api-0.8.0/tests/resources/test_timeseries_by_storeys.py` & `bemserver-api-0.9.0/tests/resources/test_timeseries_properties.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,256 +1,254 @@
-"""Timeseries by storeys routes tests"""
-import pytest
+"""Timeseries properties tests"""
+import copy
 
 from tests.common import AuthHeader
 
 
 DUMMY_ID = "69"
 
-TIMESERIES_BY_STOREYS_URL = "/timeseries_by_storeys/"
-STOREYS_URL = "/storeys/"
+TIMESERIES_PROPERTIES_URL = "/timeseries_properties/"
 
 
-class TestTimeseriesByStoreyApi:
-    def test_timeseries_by_storeys_api(self, app, users, storeys, timeseries):
+class TestTimeseriesDataStatesApi:
+    def test_timeseries_properties_api(self, app, users):
 
         creds = users["Chuck"]["creds"]
-        storey_1_id = storeys[0]
-        storey_2_id = storeys[1]
-        ts_1_id = timeseries[0]
-        ts_2_id = timeseries[1]
 
         client = app.test_client()
 
         with AuthHeader(creds):
 
             # GET list
-            ret = client.get(TIMESERIES_BY_STOREYS_URL)
+            ret = client.get(TIMESERIES_PROPERTIES_URL)
             assert ret.status_code == 200
-            assert ret.json == []
+            ret_val = ret.json
+            nb_ts_props = len(ret_val)
+            assert nb_ts_props > 0
+            nb_float = len([x for x in ret_val if x["value_type"] == "float"])
+            nb_bool = len([x for x in ret_val if x["value_type"] == "boolean"])
 
             # POST
-            tbs_1 = {
-                "storey_id": storey_1_id,
-                "timeseries_id": ts_1_id,
+            tsp_1 = {
+                "name": "Deutsche Qualität",
+                "value_type": "float",
+                "unit_symbol": "Qualität unit",
             }
-            ret = client.post(TIMESERIES_BY_STOREYS_URL, json=tbs_1)
+            ret = client.post(TIMESERIES_PROPERTIES_URL, json=tsp_1)
             assert ret.status_code == 201
             ret_val = ret.json
-            tbs_1_id = ret_val.pop("id")
-            tbs_1_etag = ret.headers["ETag"]
-            assert ret_val == tbs_1
+            tsp_1_id = ret_val.pop("id")
+            tsp_1_etag = ret.headers["ETag"]
+            assert ret_val == tsp_1
 
             # POST violating unique constraint
-            ret = client.post(TIMESERIES_BY_STOREYS_URL, json=tbs_1)
+            ret = client.post(TIMESERIES_PROPERTIES_URL, json=tsp_1)
             assert ret.status_code == 409
 
             # GET list
-            ret = client.get(TIMESERIES_BY_STOREYS_URL)
+            ret = client.get(TIMESERIES_PROPERTIES_URL)
             assert ret.status_code == 200
             ret_val = ret.json
-            assert len(ret_val) == 1
-            assert ret_val[0]["id"] == ts_1_id
+            assert len(ret_val) == nb_ts_props + 1
+            assert tsp_1["name"] in [x["name"] for x in ret_val]
 
             # GET by id
-            ret = client.get(f"{TIMESERIES_BY_STOREYS_URL}{tbs_1_id}")
+            ret = client.get(f"{TIMESERIES_PROPERTIES_URL}{tsp_1_id}")
             assert ret.status_code == 200
-            assert ret.headers["ETag"] == tbs_1_etag
+            assert ret.headers["ETag"] == tsp_1_etag
             ret_val = ret.json
             ret_val.pop("id")
-            assert ret_val == tbs_1
+            assert ret_val == tsp_1
 
             # PUT
-            tbs_1["timeseries_id"] = ts_2_id
+            tsp_1["name"] = "Qualität"
+            tsp_1_put = copy.deepcopy(tsp_1)
+            del tsp_1_put["value_type"]
             ret = client.put(
-                f"{TIMESERIES_BY_STOREYS_URL}{tbs_1_id}",
-                json=tbs_1,
-                headers={"If-Match": tbs_1_etag},
+                f"{TIMESERIES_PROPERTIES_URL}{tsp_1_id}",
+                json=tsp_1_put,
+                headers={"If-Match": tsp_1_etag},
             )
             assert ret.status_code == 200
             ret_val = ret.json
             ret_val.pop("id")
-            tbs_1_etag = ret.headers["ETag"]
-            assert ret_val == tbs_1
+            tsp_1_etag = ret.headers["ETag"]
+            assert ret_val == tsp_1
 
             # PUT wrong ID -> 404
             ret = client.put(
-                f"{TIMESERIES_BY_STOREYS_URL}{DUMMY_ID}",
-                json=tbs_1,
-                headers={"If-Match": tbs_1_etag},
+                f"{TIMESERIES_PROPERTIES_URL}{DUMMY_ID}",
+                json=tsp_1_put,
+                headers={"If-Match": tsp_1_etag},
             )
             assert ret.status_code == 404
 
-            # POST sep 2
-            tbs_2 = {
-                "storey_id": storey_2_id,
-                "timeseries_id": ts_2_id,
+            # POST TSP 2
+            tsp_2 = {
+                "name": "Autentica qualità",
+                "value_type": "float",
             }
-            ret = client.post(TIMESERIES_BY_STOREYS_URL, json=tbs_2)
+            ret = client.post(TIMESERIES_PROPERTIES_URL, json=tsp_2)
             ret_val = ret.json
-            tbs_2_id = ret_val.pop("id")
-            tbs_2_etag = ret.headers["ETag"]
+            tsp_2_id = ret_val.pop("id")
+            tsp_2_etag = ret.headers["ETag"]
 
             # PUT violating unique constraint
-            tbs_1["storey_id"] = tbs_2["storey_id"]
-            tbs_1["timeseries_id"] = tbs_2["timeseries_id"]
+            tsp_2_put = copy.deepcopy(tsp_2)
+            del tsp_2_put["value_type"]
+            tsp_2_put["name"] = "Qualität"
             ret = client.put(
-                f"{TIMESERIES_BY_STOREYS_URL}{tbs_1_id}",
-                json=tbs_1,
-                headers={"If-Match": tbs_1_etag},
+                f"{TIMESERIES_PROPERTIES_URL}{tsp_2_id}",
+                json=tsp_2_put,
+                headers={"If-Match": tsp_2_etag},
             )
             assert ret.status_code == 409
 
-            # GET list
-            ret = client.get(TIMESERIES_BY_STOREYS_URL)
-            assert ret.status_code == 200
-            ret_val = ret.json
-            assert len(ret_val) == 2
-
             # GET list with filters
             ret = client.get(
-                TIMESERIES_BY_STOREYS_URL,
-                query_string={"storey_id": storey_1_id},
+                TIMESERIES_PROPERTIES_URL, query_string={"name": "Qualität"}
             )
             assert ret.status_code == 200
             ret_val = ret.json
             assert len(ret_val) == 1
-            assert ret_val[0]["id"] == tbs_1_id
-
-            # DELETE wrong ID -> 404
-            ret = client.delete(
-                f"{TIMESERIES_BY_STOREYS_URL}{DUMMY_ID}",
-                headers={"If-Match": tbs_1_etag},
+            assert ret_val[0]["id"] == tsp_1_id
+            ret = client.get(
+                TIMESERIES_PROPERTIES_URL,
+                query_string={"value_type": "float"},
             )
-            assert ret.status_code == 404
-
-            # DELETE storey cascade
-            ret = client.get(f"{STOREYS_URL}{storey_1_id}")
-            storey_1_etag = ret.headers["ETag"]
-            ret = client.delete(
-                f"{STOREYS_URL}{storey_1_id}", headers={"If-Match": storey_1_etag}
+            assert ret.status_code == 200
+            ret_val = ret.json
+            assert len(ret_val) == nb_float + 2
+            ret = client.get(
+                TIMESERIES_PROPERTIES_URL,
+                query_string={"value_type": "boolean"},
             )
-            assert ret.status_code == 204
+            assert ret.status_code == 200
+            ret_val = ret.json
+            assert len(ret_val) == nb_bool
+            ret = client.get(
+                TIMESERIES_PROPERTIES_URL,
+                query_string={"unit_symbol": "Qualität unit"},
+            )
+            assert ret.status_code == 200
+            ret_val = ret.json
+            assert len(ret_val) == 1
+            ret = client.get(
+                TIMESERIES_PROPERTIES_URL,
+                query_string={"unit_symbol": "Qualità unit"},
+            )
+            assert ret.status_code == 200
+            ret_val = ret.json
+            assert len(ret_val) == 0
 
             # DELETE
             ret = client.delete(
-                f"{TIMESERIES_BY_STOREYS_URL}{tbs_1_id}",
-                headers={"If-Match": tbs_1_etag},
+                f"{TIMESERIES_PROPERTIES_URL}{tsp_1_id}",
+                headers={"If-Match": tsp_1_etag},
             )
-            assert ret.status_code == 404
+            assert ret.status_code == 204
             ret = client.delete(
-                f"{TIMESERIES_BY_STOREYS_URL}{tbs_2_id}",
-                headers={"If-Match": tbs_2_etag},
+                f"{TIMESERIES_PROPERTIES_URL}{tsp_2_id}",
+                headers={"If-Match": tsp_2_etag},
             )
             assert ret.status_code == 204
 
             # GET list
-            ret = client.get(TIMESERIES_BY_STOREYS_URL)
+            ret = client.get(TIMESERIES_PROPERTIES_URL)
             assert ret.status_code == 200
             ret_val = ret.json
-            assert len(ret_val) == 0
+            assert len(ret_val) == nb_ts_props
 
             # GET by id -> 404
-            ret = client.get(f"{TIMESERIES_BY_STOREYS_URL}{tbs_1_id}")
+            ret = client.get(f"{TIMESERIES_PROPERTIES_URL}{tsp_1_id}")
             assert ret.status_code == 404
 
-    @pytest.mark.usefixtures("users_by_user_groups")
-    @pytest.mark.usefixtures("user_groups_by_campaigns")
-    @pytest.mark.usefixtures("user_groups_by_campaign_scopes")
-    @pytest.mark.parametrize("timeseries", (4,), indirect=True)
-    def test_timeseries_by_storeys_as_user_api(
-        self, app, users, storeys, timeseries, timeseries_by_storeys
-    ):
+    def test_timeseries_properties_as_user_api(self, app, users):
+
+        tds_1_id = 1
 
-        user_creds = users["Active"]["creds"]
-        storey_1_id = storeys[0]
-        ts_1_id = timeseries[0]
-        ts_3_id = timeseries[2]
-        tbs_1_id = timeseries_by_storeys[0]
+        creds = users["Active"]["creds"]
 
         client = app.test_client()
 
-        with AuthHeader(user_creds):
+        with AuthHeader(creds):
 
             # GET list
-            ret = client.get(TIMESERIES_BY_STOREYS_URL)
+            ret = client.get(TIMESERIES_PROPERTIES_URL)
             assert ret.status_code == 200
             ret_val = ret.json
-            assert len(ret_val) == 1
-            tbs_1 = ret_val[0]
-            assert tbs_1.pop("id") == tbs_1_id
+            nb_ts_props = len(ret_val)
+            assert nb_ts_props > 0
 
             # POST
-            tbs_3 = {
-                "storey_id": storey_1_id,
-                "timeseries_id": ts_1_id,
+            tds = {
+                "name": "Frequency (test)",
+                "value_type": "integer",
             }
-            ret = client.post(TIMESERIES_BY_STOREYS_URL, json=tbs_3)
+            ret = client.post(TIMESERIES_PROPERTIES_URL, json=tds)
             assert ret.status_code == 403
 
             # GET by id
-            ret = client.get(f"{TIMESERIES_BY_STOREYS_URL}{tbs_1_id}")
+            ret = client.get(f"{TIMESERIES_PROPERTIES_URL}{tds_1_id}")
             assert ret.status_code == 200
-            tbs_1_etag = ret.headers["ETag"]
+            tds_1_etag = ret.headers["ETag"]
+            ret_val = ret.json
+            ret_val.pop("id")
+            tds_1 = ret_val
 
             # PUT
-            tbs_1["timeseries_id"] = ts_3_id
+            tds_1_put = copy.deepcopy(tds_1)
+            del tds_1_put["value_type"]
+            tds_1_put["name"] = "Qualität"
             ret = client.put(
-                f"{TIMESERIES_BY_STOREYS_URL}{tbs_1_id}",
-                json=tbs_1,
-                headers={"If-Match": tbs_1_etag},
+                f"{TIMESERIES_PROPERTIES_URL}{tds_1_id}",
+                json=tds_1_put,
+                headers={"If-Match": tds_1_etag},
             )
             assert ret.status_code == 403
 
             # DELETE
             ret = client.delete(
-                f"{TIMESERIES_BY_STOREYS_URL}{tbs_1_id}",
-                headers={"If-Match": tbs_1_etag},
+                f"{TIMESERIES_PROPERTIES_URL}{tds_1_id}",
+                headers={"If-Match": tds_1_etag},
             )
             assert ret.status_code == 403
 
-    def test_timeseries_by_storeys_as_anonym_api(
-        self, app, storeys, timeseries, timeseries_by_storeys
+    def test_timeseries_properties_as_anonym_api(
+        self, app, users, timeseries_properties
     ):
-        storey_1_id = storeys[0]
-        ts_1_id = timeseries[0]
-        ts_2_id = timeseries[1]
-        tbs_1_id = timeseries_by_storeys[0]
+
+        tsp_1_id = timeseries_properties[0]
 
         client = app.test_client()
 
         # GET list
-        ret = client.get(TIMESERIES_BY_STOREYS_URL)
+        ret = client.get(TIMESERIES_PROPERTIES_URL)
         assert ret.status_code == 401
 
         # POST
-        tbs_3 = {
-            "storey_id": storey_1_id,
-            "timeseries_id": ts_2_id,
+        tds = {
+            "name": "Frequency (test)",
         }
-        ret = client.post(TIMESERIES_BY_STOREYS_URL, json=tbs_3)
+        ret = client.post(TIMESERIES_PROPERTIES_URL, json=tds)
         assert ret.status_code == 401
 
         # GET by id
-        ret = client.get(f"{TIMESERIES_BY_STOREYS_URL}{tbs_1_id}")
+        ret = client.get(f"{TIMESERIES_PROPERTIES_URL}{tsp_1_id}")
         assert ret.status_code == 401
 
         # PUT
-        tbs_1 = {
-            "storey_id": storey_1_id,
-            "timeseries_id": ts_1_id,
-        }
         ret = client.put(
-            f"{TIMESERIES_BY_STOREYS_URL}{tbs_1_id}",
-            json=tbs_1,
+            f"{TIMESERIES_PROPERTIES_URL}{tsp_1_id}",
+            json=tds,
             headers={"If-Match": "Dummy-ETag"},
         )
         # ETag is wrong but we get rejected before ETag check anyway
         assert ret.status_code == 401
 
         # DELETE
         ret = client.delete(
-            f"{TIMESERIES_BY_STOREYS_URL}{tbs_1_id}",
-            headers={"If-Match": "Dummy-Etag"},
+            f"{TIMESERIES_PROPERTIES_URL}{tsp_1_id}",
+            headers={"If-Match": "Dummy-ETag"},
         )
         # ETag is wrong but we get rejected before ETag check anyway
         assert ret.status_code == 401
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bemserver-api-0.8.0/tests/resources/test_timeseries_by_zones.py` & `bemserver-api-0.9.0/tests/resources/test_timeseries_by_zones.py`

 * *Files 18% similar despite different names*

```diff
@@ -33,15 +33,15 @@
                 "zone_id": zone_1_id,
                 "timeseries_id": ts_1_id,
             }
             ret = client.post(TIMESERIES_BY_ZONES_URL, json=tbz_1)
             assert ret.status_code == 201
             ret_val = ret.json
             tbz_1_id = ret_val.pop("id")
-            tbz_1_etag = ret.headers["ETag"]
+            assert ret_val.pop("zone")["name"] == "Zone 1"
             assert ret_val == tbz_1
 
             # POST violating unique constraint
             ret = client.post(TIMESERIES_BY_ZONES_URL, json=tbz_1)
             assert ret.status_code == 409
 
             # GET list
@@ -50,59 +50,27 @@
             ret_val = ret.json
             assert len(ret_val) == 1
             assert ret_val[0]["id"] == ts_1_id
 
             # GET by id
             ret = client.get(f"{TIMESERIES_BY_ZONES_URL}{tbz_1_id}")
             assert ret.status_code == 200
-            assert ret.headers["ETag"] == tbz_1_etag
             ret_val = ret.json
             ret_val.pop("id")
+            assert ret_val.pop("zone")["name"] == "Zone 1"
             assert ret_val == tbz_1
 
-            # PUT
-            tbz_1["timeseries_id"] = ts_2_id
-            ret = client.put(
-                f"{TIMESERIES_BY_ZONES_URL}{tbz_1_id}",
-                json=tbz_1,
-                headers={"If-Match": tbz_1_etag},
-            )
-            assert ret.status_code == 200
-            ret_val = ret.json
-            ret_val.pop("id")
-            tbz_1_etag = ret.headers["ETag"]
-            assert ret_val == tbz_1
-
-            # PUT wrong ID -> 404
-            ret = client.put(
-                f"{TIMESERIES_BY_ZONES_URL}{DUMMY_ID}",
-                json=tbz_1,
-                headers={"If-Match": tbz_1_etag},
-            )
-            assert ret.status_code == 404
-
             # POST sep 2
             tbz_2 = {
                 "zone_id": zone_2_id,
                 "timeseries_id": ts_2_id,
             }
             ret = client.post(TIMESERIES_BY_ZONES_URL, json=tbz_2)
             ret_val = ret.json
             tbz_2_id = ret_val.pop("id")
-            tbz_2_etag = ret.headers["ETag"]
-
-            # PUT violating unique constraint
-            tbz_1["zone_id"] = tbz_2["zone_id"]
-            tbz_1["timeseries_id"] = tbz_2["timeseries_id"]
-            ret = client.put(
-                f"{TIMESERIES_BY_ZONES_URL}{tbz_1_id}",
-                json=tbz_1,
-                headers={"If-Match": tbz_1_etag},
-            )
-            assert ret.status_code == 409
 
             # GET list
             ret = client.get(TIMESERIES_BY_ZONES_URL)
             assert ret.status_code == 200
             ret_val = ret.json
             assert len(ret_val) == 2
 
@@ -113,38 +81,29 @@
             )
             assert ret.status_code == 200
             ret_val = ret.json
             assert len(ret_val) == 1
             assert ret_val[0]["id"] == tbz_1_id
 
             # DELETE wrong ID -> 404
-            ret = client.delete(
-                f"{TIMESERIES_BY_ZONES_URL}{DUMMY_ID}",
-                headers={"If-Match": tbz_1_etag},
-            )
+            ret = client.delete(f"{TIMESERIES_BY_ZONES_URL}{DUMMY_ID}")
             assert ret.status_code == 404
 
             # DELETE zone cascade
             ret = client.get(f"{ZONES_URL}{zone_1_id}")
             zone_1_etag = ret.headers["ETag"]
             ret = client.delete(
                 f"{ZONES_URL}{zone_1_id}", headers={"If-Match": zone_1_etag}
             )
             assert ret.status_code == 204
 
             # DELETE
-            ret = client.delete(
-                f"{TIMESERIES_BY_ZONES_URL}{tbz_1_id}",
-                headers={"If-Match": tbz_1_etag},
-            )
+            ret = client.delete(f"{TIMESERIES_BY_ZONES_URL}{tbz_1_id}")
             assert ret.status_code == 404
-            ret = client.delete(
-                f"{TIMESERIES_BY_ZONES_URL}{tbz_2_id}",
-                headers={"If-Match": tbz_2_etag},
-            )
+            ret = client.delete(f"{TIMESERIES_BY_ZONES_URL}{tbz_2_id}")
             assert ret.status_code == 204
 
             # GET list
             ret = client.get(TIMESERIES_BY_ZONES_URL)
             assert ret.status_code == 200
             ret_val = ret.json
             assert len(ret_val) == 0
@@ -152,23 +111,21 @@
             # GET by id -> 404
             ret = client.get(f"{TIMESERIES_BY_ZONES_URL}{tbz_1_id}")
             assert ret.status_code == 404
 
     @pytest.mark.usefixtures("users_by_user_groups")
     @pytest.mark.usefixtures("user_groups_by_campaigns")
     @pytest.mark.usefixtures("user_groups_by_campaign_scopes")
-    @pytest.mark.parametrize("timeseries", (4,), indirect=True)
     def test_timeseries_by_zones_as_user_api(
         self, app, users, zones, timeseries, timeseries_by_zones
     ):
 
         user_creds = users["Active"]["creds"]
         zone_1_id = zones[0]
         ts_1_id = timeseries[0]
-        ts_3_id = timeseries[2]
         tbz_1_id = timeseries_by_zones[0]
 
         client = app.test_client()
 
         with AuthHeader(user_creds):
 
             # GET list
@@ -186,37 +143,25 @@
             }
             ret = client.post(TIMESERIES_BY_ZONES_URL, json=tbz_3)
             assert ret.status_code == 403
 
             # GET by id
             ret = client.get(f"{TIMESERIES_BY_ZONES_URL}{tbz_1_id}")
             assert ret.status_code == 200
-            tbz_1_etag = ret.headers["ETag"]
-
-            # PUT
-            tbz_1["timeseries_id"] = ts_3_id
-            ret = client.put(
-                f"{TIMESERIES_BY_ZONES_URL}{tbz_1_id}",
-                json=tbz_1,
-                headers={"If-Match": tbz_1_etag},
-            )
-            assert ret.status_code == 403
 
             # DELETE
             ret = client.delete(
                 f"{TIMESERIES_BY_ZONES_URL}{tbz_1_id}",
-                headers={"If-Match": tbz_1_etag},
             )
             assert ret.status_code == 403
 
     def test_timeseries_by_zones_as_anonym_api(
         self, app, zones, timeseries, timeseries_by_zones
     ):
         zone_1_id = zones[0]
-        ts_1_id = timeseries[0]
         ts_2_id = timeseries[1]
         tbz_1_id = timeseries_by_zones[0]
 
         client = app.test_client()
 
         # GET list
         ret = client.get(TIMESERIES_BY_ZONES_URL)
@@ -230,27 +175,11 @@
         ret = client.post(TIMESERIES_BY_ZONES_URL, json=tbz_3)
         assert ret.status_code == 401
 
         # GET by id
         ret = client.get(f"{TIMESERIES_BY_ZONES_URL}{tbz_1_id}")
         assert ret.status_code == 401
 
-        # PUT
-        tbz_1 = {
-            "zone_id": zone_1_id,
-            "timeseries_id": ts_1_id,
-        }
-        ret = client.put(
-            f"{TIMESERIES_BY_ZONES_URL}{tbz_1_id}",
-            json=tbz_1,
-            headers={"If-Match": "Dummy-ETag"},
-        )
-        # ETag is wrong but we get rejected before ETag check anyway
-        assert ret.status_code == 401
-
         # DELETE
-        ret = client.delete(
-            f"{TIMESERIES_BY_ZONES_URL}{tbz_1_id}",
-            headers={"If-Match": "Dummy-Etag"},
-        )
+        ret = client.delete(f"{TIMESERIES_BY_ZONES_URL}{tbz_1_id}")
         # ETag is wrong but we get rejected before ETag check anyway
         assert ret.status_code == 401
```

### Comparing `bemserver-api-0.8.0/tests/resources/test_timeseries_data.py` & `bemserver-api-0.9.0/tests/resources/test_timeseries_data.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/tests/resources/test_timeseries_data_states.py` & `bemserver-api-0.9.0/tests/resources/test_timeseries_data_states.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/tests/resources/test_timeseries_properties.py` & `bemserver-api-0.9.0/tests/resources/test_timeseries_property_data.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,254 +1,263 @@
-"""Timeseries properties tests"""
+"""Timeseries property data tests"""
 import copy
+import pytest
 
 from tests.common import AuthHeader
 
 
 DUMMY_ID = "69"
 
-TIMESERIES_PROPERTIES_URL = "/timeseries_properties/"
+TIMESERIES_PROPERTY_DATA_URL = "/timeseries_property_data/"
 
 
-class TestTimeseriesDataStatesApi:
-    def test_timeseries_properties_api(self, app, users):
+class TestTimeseriesPropertyDataApi:
+    def test_timeseries_property_data_api(
+        self, app, users, timeseries_properties, timeseries
+    ):
+
+        tsp_1_id = timeseries_properties[0]
+        tsp_2_id = timeseries_properties[1]
+        ts_1_id = timeseries[0]
 
         creds = users["Chuck"]["creds"]
 
         client = app.test_client()
 
         with AuthHeader(creds):
 
             # GET list
-            ret = client.get(TIMESERIES_PROPERTIES_URL)
+            ret = client.get(TIMESERIES_PROPERTY_DATA_URL)
             assert ret.status_code == 200
-            ret_val = ret.json
-            nb_ts_props = len(ret_val)
-            assert nb_ts_props > 0
-            nb_float = len([x for x in ret_val if x["value_type"] == "float"])
-            nb_bool = len([x for x in ret_val if x["value_type"] == "boolean"])
+            assert ret.json == []
 
             # POST
-            tsp_1 = {
-                "name": "Deutsche Qualität",
-                "value_type": "float",
-                "unit_symbol": "Qualität unit",
+            tsg_1 = {
+                "timeseries_id": ts_1_id,
+                "property_id": tsp_1_id,
+                "value": "12",
             }
-            ret = client.post(TIMESERIES_PROPERTIES_URL, json=tsp_1)
+            ret = client.post(TIMESERIES_PROPERTY_DATA_URL, json=tsg_1)
             assert ret.status_code == 201
             ret_val = ret.json
-            tsp_1_id = ret_val.pop("id")
-            tsp_1_etag = ret.headers["ETag"]
-            assert ret_val == tsp_1
+            tsg_1_id = ret_val.pop("id")
+            tsg_1_etag = ret.headers["ETag"]
+            assert ret_val == tsg_1
 
             # POST violating unique constraint
-            ret = client.post(TIMESERIES_PROPERTIES_URL, json=tsp_1)
+            ret = client.post(TIMESERIES_PROPERTY_DATA_URL, json=tsg_1)
             assert ret.status_code == 409
 
+            # POST wrong value type
+            tsg_post = {
+                "timeseries_id": ts_1_id,
+                "property_id": tsp_2_id,
+                "value": "wrong type",
+            }
+            ret = client.post(TIMESERIES_PROPERTY_DATA_URL, json=tsg_post)
+            assert ret.status_code == 422
+
             # GET list
-            ret = client.get(TIMESERIES_PROPERTIES_URL)
+            ret = client.get(TIMESERIES_PROPERTY_DATA_URL)
             assert ret.status_code == 200
             ret_val = ret.json
-            assert len(ret_val) == nb_ts_props + 1
-            assert tsp_1["name"] in [x["name"] for x in ret_val]
+            assert len(ret_val) == 1
+            assert ret_val[0]["id"] == tsg_1_id
 
             # GET by id
-            ret = client.get(f"{TIMESERIES_PROPERTIES_URL}{tsp_1_id}")
+            ret = client.get(f"{TIMESERIES_PROPERTY_DATA_URL}{tsg_1_id}")
             assert ret.status_code == 200
-            assert ret.headers["ETag"] == tsp_1_etag
+            assert ret.headers["ETag"] == tsg_1_etag
             ret_val = ret.json
             ret_val.pop("id")
-            assert ret_val == tsp_1
+            assert ret_val == tsg_1
 
             # PUT
-            tsp_1["name"] = "Qualität"
-            tsp_1_put = copy.deepcopy(tsp_1)
-            del tsp_1_put["value_type"]
+            tsg_1["value"] = "42"
             ret = client.put(
-                f"{TIMESERIES_PROPERTIES_URL}{tsp_1_id}",
-                json=tsp_1_put,
-                headers={"If-Match": tsp_1_etag},
+                f"{TIMESERIES_PROPERTY_DATA_URL}{tsg_1_id}",
+                json=tsg_1,
+                headers={"If-Match": tsg_1_etag},
             )
             assert ret.status_code == 200
             ret_val = ret.json
             ret_val.pop("id")
-            tsp_1_etag = ret.headers["ETag"]
-            assert ret_val == tsp_1
+            tsg_1_etag = ret.headers["ETag"]
+            assert ret_val == tsg_1
+
+            # PUT wrong value type
+            tsg_1_put = copy.deepcopy(tsg_1)
+            tsg_1_put["value"] = "wrong type"
+            ret = client.put(
+                f"{TIMESERIES_PROPERTY_DATA_URL}{tsg_1_id}",
+                json=tsg_1_put,
+                headers={"If-Match": tsg_1_etag},
+            )
+            assert ret.status_code == 422
 
             # PUT wrong ID -> 404
             ret = client.put(
-                f"{TIMESERIES_PROPERTIES_URL}{DUMMY_ID}",
-                json=tsp_1_put,
-                headers={"If-Match": tsp_1_etag},
+                f"{TIMESERIES_PROPERTY_DATA_URL}{DUMMY_ID}",
+                json=tsg_1,
+                headers={"If-Match": tsg_1_etag},
             )
             assert ret.status_code == 404
 
-            # POST TSP 2
-            tsp_2 = {
-                "name": "Autentica qualità",
-                "value_type": "float",
+            # POST TSPD 2
+            tsg_2 = {
+                "timeseries_id": ts_1_id,
+                "property_id": tsp_2_id,
+                "value": "42",
             }
-            ret = client.post(TIMESERIES_PROPERTIES_URL, json=tsp_2)
+            ret = client.post(TIMESERIES_PROPERTY_DATA_URL, json=tsg_2)
             ret_val = ret.json
-            tsp_2_id = ret_val.pop("id")
-            tsp_2_etag = ret.headers["ETag"]
+            tsg_2_id = ret_val.pop("id")
+            tsg_2_etag = ret.headers["ETag"]
 
             # PUT violating unique constraint
-            tsp_2_put = copy.deepcopy(tsp_2)
-            del tsp_2_put["value_type"]
-            tsp_2_put["name"] = "Qualität"
+            tsg_2["property_id"] = tsp_1_id
             ret = client.put(
-                f"{TIMESERIES_PROPERTIES_URL}{tsp_2_id}",
-                json=tsp_2_put,
-                headers={"If-Match": tsp_2_etag},
+                f"{TIMESERIES_PROPERTY_DATA_URL}{tsg_2_id}",
+                json=tsg_2,
+                headers={"If-Match": tsg_2_etag},
             )
             assert ret.status_code == 409
 
-            # GET list with filters
-            ret = client.get(
-                TIMESERIES_PROPERTIES_URL, query_string={"name": "Qualität"}
-            )
-            assert ret.status_code == 200
-            ret_val = ret.json
-            assert len(ret_val) == 1
-            assert ret_val[0]["id"] == tsp_1_id
-            ret = client.get(
-                TIMESERIES_PROPERTIES_URL,
-                query_string={"value_type": "float"},
-            )
-            assert ret.status_code == 200
-            ret_val = ret.json
-            assert len(ret_val) == nb_float + 2
-            ret = client.get(
-                TIMESERIES_PROPERTIES_URL,
-                query_string={"value_type": "boolean"},
-            )
-            assert ret.status_code == 200
-            ret_val = ret.json
-            assert len(ret_val) == nb_bool
-            ret = client.get(
-                TIMESERIES_PROPERTIES_URL,
-                query_string={"unit_symbol": "Qualität unit"},
-            )
-            assert ret.status_code == 200
-            ret_val = ret.json
-            assert len(ret_val) == 1
-            ret = client.get(
-                TIMESERIES_PROPERTIES_URL,
-                query_string={"unit_symbol": "Qualità unit"},
-            )
-            assert ret.status_code == 200
-            ret_val = ret.json
-            assert len(ret_val) == 0
-
             # DELETE
             ret = client.delete(
-                f"{TIMESERIES_PROPERTIES_URL}{tsp_1_id}",
-                headers={"If-Match": tsp_1_etag},
+                f"{TIMESERIES_PROPERTY_DATA_URL}{tsg_1_id}",
+                headers={"If-Match": tsg_1_etag},
             )
             assert ret.status_code == 204
             ret = client.delete(
-                f"{TIMESERIES_PROPERTIES_URL}{tsp_2_id}",
-                headers={"If-Match": tsp_2_etag},
+                f"{TIMESERIES_PROPERTY_DATA_URL}{tsg_2_id}",
+                headers={"If-Match": tsg_2_etag},
             )
-            assert ret.status_code == 204
 
             # GET list
-            ret = client.get(TIMESERIES_PROPERTIES_URL)
+            ret = client.get(TIMESERIES_PROPERTY_DATA_URL)
             assert ret.status_code == 200
-            ret_val = ret.json
-            assert len(ret_val) == nb_ts_props
+            assert ret.json == []
 
             # GET by id -> 404
-            ret = client.get(f"{TIMESERIES_PROPERTIES_URL}{tsp_1_id}")
+            ret = client.get(f"{TIMESERIES_PROPERTY_DATA_URL}{tsg_1_id}")
             assert ret.status_code == 404
 
-    def test_timeseries_properties_as_user_api(self, app, users):
+    @pytest.mark.usefixtures("users_by_user_groups")
+    @pytest.mark.usefixtures("user_groups_by_campaign_scopes")
+    def test_timeseries_property_data_as_user_api(
+        self,
+        app,
+        users,
+        timeseries_properties,
+        timeseries,
+        timeseries_property_data,
+    ):
 
-        tds_1_id = 1
+        tsp_1_id = timeseries_properties[0]
+        ts_1_id = timeseries[0]
+        tspd_1_id = timeseries_property_data[0]
+        tspd_3_id = timeseries_property_data[2]
 
         creds = users["Active"]["creds"]
 
         client = app.test_client()
 
         with AuthHeader(creds):
 
             # GET list
-            ret = client.get(TIMESERIES_PROPERTIES_URL)
+            ret = client.get(TIMESERIES_PROPERTY_DATA_URL)
             assert ret.status_code == 200
             ret_val = ret.json
-            nb_ts_props = len(ret_val)
-            assert nb_ts_props > 0
+            assert len(ret_val) == 2
+            assert all([tspd["timeseries_id"] == ts_1_id for tspd in ret_val])
 
             # POST
-            tds = {
-                "name": "Frequency (test)",
-                "value_type": "integer",
+            tspd = {
+                "timeseries_id": ts_1_id,
+                "property_id": tsp_1_id,
+                "value": "12",
             }
-            ret = client.post(TIMESERIES_PROPERTIES_URL, json=tds)
+            ret = client.post(TIMESERIES_PROPERTY_DATA_URL, json=tspd)
+            # This would trigger a unique constraint violation error
+            # but we get rejected before that
             assert ret.status_code == 403
 
             # GET by id
-            ret = client.get(f"{TIMESERIES_PROPERTIES_URL}{tds_1_id}")
+            ret = client.get(f"{TIMESERIES_PROPERTY_DATA_URL}{tspd_1_id}")
             assert ret.status_code == 200
-            tds_1_etag = ret.headers["ETag"]
+            ts_1_etag = ret.headers["ETag"]
             ret_val = ret.json
             ret_val.pop("id")
-            tds_1 = ret_val
+            tspd_1 = ret_val
+
+            # GET by id, user not in group
+            ret = client.get(f"{TIMESERIES_PROPERTY_DATA_URL}{tspd_3_id}")
+            assert ret.status_code == 403
 
             # PUT
-            tds_1_put = copy.deepcopy(tds_1)
-            del tds_1_put["value_type"]
-            tds_1_put["name"] = "Qualität"
+            tspd_1["value"] = "42"
             ret = client.put(
-                f"{TIMESERIES_PROPERTIES_URL}{tds_1_id}",
-                json=tds_1_put,
-                headers={"If-Match": tds_1_etag},
+                f"{TIMESERIES_PROPERTY_DATA_URL}{tspd_1_id}",
+                json=tspd_1,
+                headers={"If-Match": ts_1_etag},
             )
+            # ETag is wrong but we get rejected before ETag check anyway
             assert ret.status_code == 403
 
             # DELETE
             ret = client.delete(
-                f"{TIMESERIES_PROPERTIES_URL}{tds_1_id}",
-                headers={"If-Match": tds_1_etag},
+                f"{TIMESERIES_PROPERTY_DATA_URL}{tspd_1_id}",
+                headers={"If-Match": ts_1_etag},
             )
+            # ETag is wrong but we get rejected before ETag check anyway
             assert ret.status_code == 403
 
-    def test_timeseries_properties_as_anonym_api(
-        self, app, users, timeseries_properties
+    def test_timeseries_property_data_as_anonym_api(
+        self,
+        app,
+        users,
+        timeseries_properties,
+        timeseries,
+        timeseries_property_data,
     ):
 
         tsp_1_id = timeseries_properties[0]
+        ts_1_id = timeseries[0]
+        tspd_1_id = timeseries_property_data[0]
 
         client = app.test_client()
 
         # GET list
-        ret = client.get(TIMESERIES_PROPERTIES_URL)
+        ret = client.get(TIMESERIES_PROPERTY_DATA_URL)
         assert ret.status_code == 401
 
         # POST
-        tds = {
-            "name": "Frequency (test)",
+        tspd = {
+            "timeseries_id": ts_1_id,
+            "property_id": tsp_1_id,
+            "value": "12",
         }
-        ret = client.post(TIMESERIES_PROPERTIES_URL, json=tds)
+        ret = client.post(TIMESERIES_PROPERTY_DATA_URL, json=tspd)
         assert ret.status_code == 401
 
         # GET by id
-        ret = client.get(f"{TIMESERIES_PROPERTIES_URL}{tsp_1_id}")
+        ret = client.get(f"{TIMESERIES_PROPERTY_DATA_URL}{tspd_1_id}")
         assert ret.status_code == 401
 
         # PUT
+        tspd["value"] = "42"
         ret = client.put(
-            f"{TIMESERIES_PROPERTIES_URL}{tsp_1_id}",
-            json=tds,
+            f"{TIMESERIES_PROPERTY_DATA_URL}{tspd_1_id}",
+            json=tspd,
             headers={"If-Match": "Dummy-ETag"},
         )
         # ETag is wrong but we get rejected before ETag check anyway
         assert ret.status_code == 401
 
         # DELETE
         ret = client.delete(
-            f"{TIMESERIES_PROPERTIES_URL}{tsp_1_id}",
+            f"{TIMESERIES_PROPERTY_DATA_URL}{tspd_1_id}",
             headers={"If-Match": "Dummy-ETag"},
         )
         # ETag is wrong but we get rejected before ETag check anyway
         assert ret.status_code == 401
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `bemserver-api-0.8.0/tests/resources/test_user_groups.py` & `bemserver-api-0.9.0/tests/resources/test_user_groups.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/tests/resources/test_user_groups_by_campaigns.py` & `bemserver-api-0.9.0/tests/resources/test_user_groups_by_campaigns.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 
             # POST
             ugbc_1 = {"campaign_id": campaign_1_id, "user_group_id": ug_1_id}
             ret = client.post(USER_GROUPS_BY_CAMPAIGNS_URL, json=ugbc_1)
             assert ret.status_code == 201
             ret_val = ret.json
             ugbc_1_id = ret_val.pop("id")
-            ugbc_1_etag = ret.headers["ETag"]
 
             # POST violating unique constraint
             ret = client.post(USER_GROUPS_BY_CAMPAIGNS_URL, json=ugbc_1)
             assert ret.status_code == 409
 
             # GET list
             ret = client.get(USER_GROUPS_BY_CAMPAIGNS_URL)
@@ -48,15 +47,14 @@
             ret_val = ret.json
             assert len(ret_val) == 1
             assert ret_val[0]["id"] == ugbc_1_id
 
             # GET by id
             ret = client.get(f"{USER_GROUPS_BY_CAMPAIGNS_URL}{ugbc_1_id}")
             assert ret.status_code == 200
-            assert ret.headers["ETag"] == ugbc_1_etag
 
             # POST
             ugbc_2 = {"campaign_id": campaign_2_id, "user_group_id": ug_2_id}
             ret = client.post(USER_GROUPS_BY_CAMPAIGNS_URL, json=ugbc_2)
             assert ret.status_code == 201
             ret_val = ret.json
             ugbc_2_id = ret_val.pop("id")
```

### Comparing `bemserver-api-0.8.0/tests/resources/test_user_groups_by_campaigns_scopes.py` & `bemserver-api-0.9.0/tests/resources/test_user_groups_by_campaigns_scopes.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 
             # POST
             ugbc_1 = {"campaign_scope_id": cs_1_id, "user_group_id": ug_1_id}
             ret = client.post(USER_GROUPS_BY_CAMPAIGN_SCOPES_URL, json=ugbc_1)
             assert ret.status_code == 201
             ret_val = ret.json
             ugbc_1_id = ret_val.pop("id")
-            ugbc_1_etag = ret.headers["ETag"]
 
             # POST violating unique constraint
             ret = client.post(USER_GROUPS_BY_CAMPAIGN_SCOPES_URL, json=ugbc_1)
             assert ret.status_code == 409
 
             # GET list
             ret = client.get(USER_GROUPS_BY_CAMPAIGN_SCOPES_URL)
@@ -50,15 +49,14 @@
             ret_val = ret.json
             assert len(ret_val) == 1
             assert ret_val[0]["id"] == ugbc_1_id
 
             # GET by id
             ret = client.get(f"{USER_GROUPS_BY_CAMPAIGN_SCOPES_URL}{ugbc_1_id}")
             assert ret.status_code == 200
-            assert ret.headers["ETag"] == ugbc_1_etag
 
             # POST
             ugbc_2 = {"campaign_scope_id": cs_2_id, "user_group_id": ug_2_id}
             ret = client.post(USER_GROUPS_BY_CAMPAIGN_SCOPES_URL, json=ugbc_2)
             assert ret.status_code == 201
             ret_val = ret.json
             ugbc_2_id = ret_val.pop("id")
```

### Comparing `bemserver-api-0.8.0/tests/resources/test_users.py` & `bemserver-api-0.9.0/tests/resources/test_users.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/tests/resources/test_users_by_user_groups.py` & `bemserver-api-0.9.0/tests/resources/test_users_by_user_groups.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 
             # POST
             ubug_1 = {"user_group_id": ug_1_id, "user_id": user_1_id}
             ret = client.post(USERS_BY_USER_GROUPS_URL, json=ubug_1)
             assert ret.status_code == 201
             ret_val = ret.json
             ubug_1_id = ret_val.pop("id")
-            ubug_1_etag = ret.headers["ETag"]
 
             # POST violating unique constraint
             ret = client.post(USERS_BY_USER_GROUPS_URL, json=ubug_1)
             assert ret.status_code == 409
 
             # GET list
             ret = client.get(USERS_BY_USER_GROUPS_URL)
@@ -46,15 +45,14 @@
             ret_val = ret.json
             assert len(ret_val) == 1
             assert ret_val[0]["id"] == ubug_1_id
 
             # GET by id
             ret = client.get(f"{USERS_BY_USER_GROUPS_URL}{ubug_1_id}")
             assert ret.status_code == 200
-            assert ret.headers["ETag"] == ubug_1_etag
 
             # POST
             ubug_2 = {"user_group_id": ug_2_id, "user_id": user_2_id}
             ret = client.post(USERS_BY_USER_GROUPS_URL, json=ubug_2)
             assert ret.status_code == 201
             ret_val = ret.json
             ubug_2_id = ret_val.pop("id")
```

### Comparing `bemserver-api-0.8.0/tests/resources/test_zone_properties.py` & `bemserver-api-0.9.0/tests/resources/test_zone_properties.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,14 @@
             zone_p_1 = {
                 "structural_element_property_id": sep_1_id,
             }
             ret = client.post(ZONE_PROPERTIES_URL, json=zone_p_1)
             assert ret.status_code == 201
             ret_val = ret.json
             zone_p_1_id = ret_val.pop("id")
-            zone_p_1_etag = ret.headers["ETag"]
             sep = ret_val.pop("structural_element_property")
             assert sep == {"name": "Area", "value_type": "integer"}
             assert ret_val == zone_p_1
 
             # POST violating unique constraint
             ret = client.post(ZONE_PROPERTIES_URL, json=zone_p_1)
             assert ret.status_code == 409
@@ -46,15 +45,14 @@
             ret_val = ret.json
             assert len(ret_val) == 1
             assert ret_val[0]["id"] == zone_p_1_id
 
             # GET by id
             ret = client.get(f"{ZONE_PROPERTIES_URL}{zone_p_1_id}")
             assert ret.status_code == 200
-            assert ret.headers["ETag"] == zone_p_1_etag
             ret_val = ret.json
             ret_val.pop("id")
             ret_val.pop("structural_element_property")
             assert ret_val == zone_p_1
 
             # POST sep 2
             zone_p_2 = {
```

### Comparing `bemserver-api-0.8.0/tests/resources/test_zone_property_data.py` & `bemserver-api-0.9.0/tests/resources/test_zone_property_data.py`

 * *Files identical despite different names*

### Comparing `bemserver-api-0.8.0/tests/utils.py` & `bemserver-api-0.9.0/tests/utils.py`

 * *Files identical despite different names*

