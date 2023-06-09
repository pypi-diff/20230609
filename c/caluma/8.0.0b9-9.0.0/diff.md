# Comparing `tmp/caluma-8.0.0b9.tar.gz` & `tmp/caluma-9.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caluma-8.0.0b9.tar", max compression
+gzip compressed data, was "caluma-9.0.0.tar", max compression
```

## Comparing `caluma-8.0.0b9.tar` & `caluma-9.0.0.tar`

### file list

```diff
@@ -1,210 +1,213 @@
--rw-r--r--   0        0        0    44302 2022-06-24 12:42:38.651433 caluma-8.0.0b9/CHANGELOG.md
--rw-r--r--   0        0        0    35149 2022-06-24 12:42:38.651433 caluma-8.0.0b9/LICENSE
-drwxr-xr-x   0        0        0        0 2022-06-24 12:42:38.651433 caluma-8.0.0b9/LICENSES/
--rw-r--r--   0        0        0     1957 2022-06-24 12:42:38.651433 caluma-8.0.0b9/README.md
--rw-r--r--   0        0        0        0 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/__init__.py
--rw-r--r--   0        0        0     5442 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_analytics/README.md
--rw-r--r--   0        0        0        0 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_analytics/__init__.py
--rw-r--r--   0        0        0      105 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_analytics/apps.py
--rw-r--r--   0        0        0     3322 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_analytics/conftest.py
--rw-r--r--   0        0        0      797 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_analytics/factories.py
--rw-r--r--   0        0        0     1543 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_analytics/filters.py
--rw-r--r--   0        0        0     3416 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_analytics/management/commands/run_analytics.py
--rw-r--r--   0        0        0    11086 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_analytics/migrations/0001_initial.py
--rw-r--r--   0        0        0     2008 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_analytics/migrations/0002_analytics_pivot_table.py
--rw-r--r--   0        0        0     1026 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_analytics/migrations/0003_starting_objects.py
--rw-r--r--   0        0        0     1383 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_analytics/migrations/0004_simple_history.py
--rw-r--r--   0        0        0        0 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_analytics/migrations/__init__.py
--rw-r--r--   0        0        0     3469 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_analytics/models.py
--rw-r--r--   0        0        0     3666 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_analytics/pivot_table.py
--rw-r--r--   0        0        0     6996 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_analytics/schema.py
--rw-r--r--   0        0        0     3499 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_analytics/serializers.py
--rw-r--r--   0        0        0    32474 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_analytics/simple_table.py
--rw-r--r--   0        0        0    16037 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_analytics/sql.py
--rw-r--r--   0        0        0     1113 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_analytics/visibility.py
--rw-r--r--   0        0        0        0 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_core/__init__.py
--rw-r--r--   0        0        0      975 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_core/apps.py
--rw-r--r--   0        0        0      195 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_core/collections.py
--rw-r--r--   0        0        0    11297 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_core/conftest.py
--rw-r--r--   0        0        0     3074 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_core/events.py
--rw-r--r--   0        0        0      325 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_core/factories.py
--rw-r--r--   0        0        0      485 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_core/faker.py
--rw-r--r--   0        0        0    18433 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_core/filters.py
--rw-r--r--   0        0        0      642 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_core/forms.py
--rw-r--r--   0        0        0     4176 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_core/health_checks.py
--rw-r--r--   0        0        0     7855 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_core/jexl.py
--rw-r--r--   0        0        0        0 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_core/management/__init__.py
--rw-r--r--   0        0        0        0 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_core/management/commands/__init__.py
--rw-r--r--   0        0        0     1824 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_core/management/commands/cleanup_history.py
--rw-r--r--   0        0        0     3803 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_core/management/commands/dump_caluma_config.py
--rw-r--r--   0        0        0      794 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_core/management/commands/migrate.py
--rw-r--r--   0        0        0     4768 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_core/management/commands/migrate_to_prefixed_apps.py
--rw-r--r--   0        0        0     3078 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_core/models.py
--rw-r--r--   0        0        0    11206 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_core/mutation.py
--rw-r--r--   0        0        0     3216 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_core/ordering.py
--rw-r--r--   0        0        0     3195 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_core/pagination.py
--rw-r--r--   0        0        0     4485 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_core/permissions.py
--rw-r--r--   0        0        0     1253 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_core/relay.py
--rw-r--r--   0        0        0     4764 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_core/serializers.py
--rw-r--r--   0        0        0     7577 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_core/types.py
--rw-r--r--   0        0        0      387 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_core/urls.py
--rw-r--r--   0        0        0     2430 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_core/validations.py
--rw-r--r--   0        0        0     1607 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_core/views.py
--rw-r--r--   0        0        0     2937 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_core/visibilities.py
--rw-r--r--   0        0        0        0 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_data_source/__init__.py
--rw-r--r--   0        0        0      107 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_data_source/apps.py
--rw-r--r--   0        0        0     2028 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_data_source/data_source_handlers.py
--rw-r--r--   0        0        0     3104 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_data_source/data_sources.py
--rw-r--r--   0        0        0      989 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_data_source/schema.py
--rw-r--r--   0        0        0      486 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_data_source/utils.py
--rw-r--r--   0        0        0        0 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/__init__.py
--rw-r--r--   0        0        0     2472 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/api.py
--rw-r--r--   0        0        0      100 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/apps.py
--rw-r--r--   0        0        0     8317 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/domain_logic.py
--rw-r--r--   0        0        0     5702 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/factories.py
--rw-r--r--   0        0        0    16457 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/filters.py
--rw-r--r--   0        0        0     3283 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/format_validators.py
--rw-r--r--   0        0        0     7860 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/historical_schema.py
--rw-r--r--   0        0        0     7496 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/jexl.py
--rw-r--r--   0        0        0        0 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/management/__init__.py
--rw-r--r--   0        0        0        0 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/management/commands/__init__.py
--rw-r--r--   0        0        0     1880 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/management/commands/copy_form.py
--rw-r--r--   0        0        0      631 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/management/commands/create_bucket.py
--rw-r--r--   0        0        0    10984 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0001_initial.py
--rw-r--r--   0        0        0     2830 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0002_auto_20181221_1517.py
--rw-r--r--   0        0        0     3863 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0003_auto_20190130_0920.py
--rw-r--r--   0        0        0     1566 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0004_auto_20190207_1405.py
--rw-r--r--   0        0        0      826 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0005_auto_20190208_1016.py
--rw-r--r--   0        0        0      801 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0006_choice_type_conversion.py
--rw-r--r--   0        0        0      630 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0007_auto_20190208_1232.py
--rw-r--r--   0        0        0     1180 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0008_auto_20190319_1720.py
--rw-r--r--   0        0        0     2134 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0009_auto_20190321_1722.py
--rw-r--r--   0        0        0     2303 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0010_auto_20190404_0652.py
--rw-r--r--   0        0        0      605 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0011_auto_20190411_0607.py
--rw-r--r--   0        0        0      789 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0012_auto_20190416_1835.py
--rw-r--r--   0        0        0     1257 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0013_auto_20190418_0733.py
--rw-r--r--   0        0        0     1408 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0014_auto_20190429_0910.py
--rw-r--r--   0        0        0      660 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0015_question_format_validators.py
--rw-r--r--   0        0        0      531 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0016_auto_20190510_0843.py
--rw-r--r--   0        0        0      606 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0017_auto_20190619_1320.py
--rw-r--r--   0        0        0     1860 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0018_remove_answer_value_document_data_migration.py
--rw-r--r--   0        0        0      366 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0019_remove_answer_value_document.py
--rw-r--r--   0        0        0    27840 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0020_historicalanswer_historicalanswerdocument_historicaldocument_historicalfile_historicalform_historica.py
--rw-r--r--   0        0        0     2471 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0021_auto_20190708_0905.py
--rw-r--r--   0        0        0     1454 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0022_add_gin_index_to_jsonfields.py
--rw-r--r--   0        0        0      559 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0023_auto_20190729_1448.py
--rw-r--r--   0        0        0     1088 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0024_auto_20190919_1244.py
--rw-r--r--   0        0        0     4835 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0025_dynamicoption_historicaldynamicoption.py
--rw-r--r--   0        0        0      829 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0026_auto_20191031_0834.py
--rw-r--r--   0        0        0     2088 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0027_auto_20200113_0727.py
--rw-r--r--   0        0        0    12676 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0028_auto_20200210_0929.py
--rw-r--r--   0        0        0     1571 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0029_dynamic_option_unique_together.py
--rw-r--r--   0        0        0     1282 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0030_auto_20200219_1359.py
--rw-r--r--   0        0        0     1702 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0031_auto_20200220_0910.py
--rw-r--r--   0        0        0     1154 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0032_auto_20200220_1311.py
--rw-r--r--   0        0        0     1270 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0033_slugfield_length.py
--rw-r--r--   0        0        0      520 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0034_fix_fk_lengths.py
--rw-r--r--   0        0        0     1688 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0035_historicalanswer_history_question_type.py
--rw-r--r--   0        0        0     1387 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0036_default_answers.py
--rw-r--r--   0        0        0      611 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0037_default_answer_one2one.py
--rw-r--r--   0        0        0     3051 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0038_auto_20201224_0920.py
--rw-r--r--   0        0        0      461 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0038_remove_table_answer_value.py
--rw-r--r--   0        0        0      284 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0039_merge_20210114_0956.py
--rw-r--r--   0        0        0    10394 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0040_add_modified_by_user_group.py
--rw-r--r--   0        0        0     2150 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0041_action_button_question.py
--rw-r--r--   0        0        0      751 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0042_auto_20220110_1051.py
--rw-r--r--   0        0        0     1210 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0043_alter_historicalanswer_history_question_type.py
--rw-r--r--   0        0        0      991 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0044_migrate_format_validators.py
--rw-r--r--   0        0        0     5739 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0045_simple_history.py
--rw-r--r--   0        0        0        0 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/__init__.py
--rw-r--r--   0        0        0    21045 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/models.py
--rw-r--r--   0        0        0     2211 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/ordering.py
--rw-r--r--   0        0        0    36664 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/schema.py
--rw-r--r--   0        0        0    22614 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/serializers.py
--rw-r--r--   0        0        0     7337 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/signals.py
--rw-r--r--   0        0        0     3865 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/storage_clients.py
--rw-r--r--   0        0        0     7813 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/structure.py
--rw-r--r--   0        0        0    17803 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_form/validators.py
--rw-r--r--   0        0        0        0 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_logging/__init__.py
--rw-r--r--   0        0        0      103 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_logging/apps.py
--rw-r--r--   0        0        0      365 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_logging/factories.py
--rw-r--r--   0        0        0        0 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_logging/management/__init__.py
--rw-r--r--   0        0        0        0 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_logging/management/commands/__init__.py
--rw-r--r--   0        0        0     1087 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_logging/management/commands/cleanup_access_log.py
--rw-r--r--   0        0        0     1777 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_logging/middleware.py
--rw-r--r--   0        0        0     1560 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_logging/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_logging/migrations/__init__.py
--rw-r--r--   0        0        0      657 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_logging/models.py
--rw-r--r--   0        0        0        0 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_user/__init__.py
--rw-r--r--   0        0        0      100 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_user/apps.py
--rw-r--r--   0        0        0     1919 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_user/models.py
--rw-r--r--   0        0        0      506 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_user/permissions.py
--rw-r--r--   0        0        0     5012 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_user/views.py
--rw-r--r--   0        0        0      711 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_user/visibilities.py
--rw-r--r--   0        0        0        0 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_workflow/__init__.py
--rw-r--r--   0        0        0     7790 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_workflow/api.py
--rw-r--r--   0        0        0      618 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_workflow/apps.py
--rw-r--r--   0        0        0    20682 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_workflow/domain_logic.py
--rw-r--r--   0        0        0     1606 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_workflow/dynamic_groups.py
--rw-r--r--   0        0        0     1941 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_workflow/dynamic_tasks.py
--rw-r--r--   0        0        0      534 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_workflow/events.py
--rw-r--r--   0        0        0     2674 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_workflow/factories.py
--rw-r--r--   0        0        0     6090 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_workflow/filters.py
--rw-r--r--   0        0        0     6485 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_workflow/jexl.py
--rw-r--r--   0        0        0    11030 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0001_initial.py
--rw-r--r--   0        0        0      666 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0002_auto_20181213_1334.py
--rw-r--r--   0        0        0      756 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0003_auto_20181217_1051.py
--rw-r--r--   0        0        0     1632 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0004_auto_20181218_1352.py
--rw-r--r--   0        0        0     4269 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0005_auto_20181228_1243.py
--rw-r--r--   0        0        0      994 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0006_auto_20190121_1440.py
--rw-r--r--   0        0        0     1035 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0007_auto_20190206_0854.py
--rw-r--r--   0        0        0      687 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0008_auto_20190208_1302.py
--rw-r--r--   0        0        0     1621 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0009_auto_20190213_0939.py
--rw-r--r--   0        0        0      753 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0010_auto_20190213_1050.py
--rw-r--r--   0        0        0     1235 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0011_auto_20190220_1303.py
--rw-r--r--   0        0        0    21985 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0012_historicalcase_historicalflow_historicaltask_historicaltaskflow_historicalworkflow_historicalworkite.py
--rw-r--r--   0        0        0     3459 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0013_auto_20190718_1235.py
--rw-r--r--   0        0        0     1121 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0014_add_gin_index_to_jsonfields.py
--rw-r--r--   0        0        0     1299 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0015_add_work_item_skipped.py
--rw-r--r--   0        0        0     2220 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0016_auto_20200113_0727.py
--rw-r--r--   0        0        0     7594 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0017_auto_20200210_0929.py
--rw-r--r--   0        0        0      925 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0018_auto_20200219_1359.py
--rw-r--r--   0        0        0      925 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0019_slugfield_length.py
--rw-r--r--   0        0        0     2851 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0020_case_families.py
--rw-r--r--   0        0        0     1742 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0021_work_item_controlling_groups.py
--rw-r--r--   0        0        0     2504 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0022_workitem_name_description.py
--rw-r--r--   0        0        0     1064 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0023_auto_20200730_1135.py
--rw-r--r--   0        0        0     2491 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0024_auto_20200901_1026.py
--rw-r--r--   0        0        0     1453 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0025_auto_20200901_1415.py
--rw-r--r--   0        0        0     1337 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0026_auto_20200901_1435.py
--rw-r--r--   0        0        0     6416 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0027_add_modified_by_user_group.py
--rw-r--r--   0        0        0     2619 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0028_redoable_field.py
--rw-r--r--   0        0        0      854 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0029_task_continue_async.py
--rw-r--r--   0        0        0     3681 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0030_remove_choices_char_field.py
--rw-r--r--   0        0        0     3475 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0031_simple_history.py
--rw-r--r--   0        0        0        0 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/__init__.py
--rw-r--r--   0        0        0     9946 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/caluma_workflow/models.py
--rw-r--r--   0        0        0    12372 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/caluma_workflow/schema.py
--rw-r--r--   0        0        0    21121 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/caluma_workflow/serializers.py
--rw-r--r--   0        0        0     4155 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/caluma_workflow/utils.py
--rw-r--r--   0        0        0     1202 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/caluma_workflow/validators.py
--rw-r--r--   0        0        0     2120 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/caluma_workflow/visibilities.py
--rw-r--r--   0        0        0    12222 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/conftest.py
--rw-r--r--   0        0        0        0 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/extensions/__init__.py
--rw-r--r--   0        0        0       53 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/extensions/data_sources.py
--rw-r--r--   0        0        0       39 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/extensions/dynamic_groups.py
--rw-r--r--   0        0        0       40 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/extensions/events.py
--rw-r--r--   0        0        0       58 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/extensions/format_validators.py
--rw-r--r--   0        0        0       52 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/extensions/permissions.py
--rw-r--r--   0        0        0       52 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/extensions/validations.py
--rw-r--r--   0        0        0       52 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/extensions/visibilities.py
--rw-r--r--   0        0        0     2782 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/schema.py
--rw-r--r--   0        0        0        0 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/settings/__init__.py
--rw-r--r--   0        0        0     3609 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/settings/caluma.py
--rw-r--r--   0        0        0     5752 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/settings/django.py
--rw-r--r--   0        0        0      100 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/urls.py
--rw-r--r--   0        0        0     3416 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/utils.py
--rw-r--r--   0        0        0      403 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/wsgi.py
--rw-r--r--   0        0        0     3542 2022-06-24 12:42:38.663433 caluma-8.0.0b9/pyproject.toml
--rw-r--r--   0        0        0     3945 2022-06-24 12:42:56.699962 caluma-8.0.0b9/setup.py
--rw-r--r--   0        0        0     3736 2022-06-24 12:42:56.700354 caluma-8.0.0b9/PKG-INFO
+-rw-r--r--   0        0        0    57525 2023-06-09 11:02:36.308242 caluma-9.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0    35149 2023-06-09 11:02:36.308242 caluma-9.0.0/LICENSE
+drwxr-xr-x   0        0        0        0 2023-06-09 11:02:36.308242 caluma-9.0.0/LICENSES/
+-rw-r--r--   0        0        0     1957 2023-06-09 11:02:36.312242 caluma-9.0.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-09 11:02:36.312242 caluma-9.0.0/caluma/__init__.py
+-rw-r--r--   0        0        0     5442 2023-06-09 11:02:36.312242 caluma-9.0.0/caluma/caluma_analytics/README.md
+-rw-r--r--   0        0        0        0 2023-06-09 11:02:36.312242 caluma-9.0.0/caluma/caluma_analytics/__init__.py
+-rw-r--r--   0        0        0      105 2023-06-09 11:02:36.312242 caluma-9.0.0/caluma/caluma_analytics/apps.py
+-rw-r--r--   0        0        0     3728 2023-06-09 11:02:36.312242 caluma-9.0.0/caluma/caluma_analytics/conftest.py
+-rw-r--r--   0        0        0      797 2023-06-09 11:02:36.312242 caluma-9.0.0/caluma/caluma_analytics/factories.py
+-rw-r--r--   0        0        0     1543 2023-06-09 11:02:36.312242 caluma-9.0.0/caluma/caluma_analytics/filters.py
+-rw-r--r--   0        0        0     3842 2023-06-09 11:02:36.312242 caluma-9.0.0/caluma/caluma_analytics/management/commands/run_analytics.py
+-rw-r--r--   0        0        0    11085 2023-06-09 11:02:36.312242 caluma-9.0.0/caluma/caluma_analytics/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2007 2023-06-09 11:02:36.312242 caluma-9.0.0/caluma/caluma_analytics/migrations/0002_analytics_pivot_table.py
+-rw-r--r--   0        0        0     1025 2023-06-09 11:02:36.312242 caluma-9.0.0/caluma/caluma_analytics/migrations/0003_starting_objects.py
+-rw-r--r--   0        0        0     1382 2023-06-09 11:02:36.312242 caluma-9.0.0/caluma/caluma_analytics/migrations/0004_simple_history.py
+-rw-r--r--   0        0        0      781 2023-06-09 11:02:36.312242 caluma-9.0.0/caluma/caluma_analytics/migrations/0005_analytics_field_ordering.py
+-rw-r--r--   0        0        0      631 2023-06-09 11:02:36.312242 caluma-9.0.0/caluma/caluma_analytics/migrations/0006_rename_form_slug_fields.py
+-rw-r--r--   0        0        0        0 2023-06-09 11:02:36.312242 caluma-9.0.0/caluma/caluma_analytics/migrations/__init__.py
+-rw-r--r--   0        0        0     3593 2023-06-09 11:02:36.312242 caluma-9.0.0/caluma/caluma_analytics/models.py
+-rw-r--r--   0        0        0     4082 2023-06-09 11:02:36.312242 caluma-9.0.0/caluma/caluma_analytics/pivot_table.py
+-rw-r--r--   0        0        0     7235 2023-06-09 11:02:36.312242 caluma-9.0.0/caluma/caluma_analytics/schema.py
+-rw-r--r--   0        0        0     4269 2023-06-09 11:02:36.312242 caluma-9.0.0/caluma/caluma_analytics/serializers.py
+-rw-r--r--   0        0        0    44521 2023-06-09 11:02:36.312242 caluma-9.0.0/caluma/caluma_analytics/simple_table.py
+-rw-r--r--   0        0        0    17612 2023-06-09 11:02:36.312242 caluma-9.0.0/caluma/caluma_analytics/sql.py
+-rw-r--r--   0        0        0     1401 2023-06-09 11:02:36.316242 caluma-9.0.0/caluma/caluma_analytics/visibility.py
+-rw-r--r--   0        0        0        0 2023-06-09 11:02:36.316242 caluma-9.0.0/caluma/caluma_core/__init__.py
+-rw-r--r--   0        0        0      975 2023-06-09 11:02:36.316242 caluma-9.0.0/caluma/caluma_core/apps.py
+-rw-r--r--   0        0        0      195 2023-06-09 11:02:36.316242 caluma-9.0.0/caluma/caluma_core/collections.py
+-rw-r--r--   0        0        0    11331 2023-06-09 11:02:36.316242 caluma-9.0.0/caluma/caluma_core/conftest.py
+-rw-r--r--   0        0        0     2877 2023-06-09 11:02:36.316242 caluma-9.0.0/caluma/caluma_core/events.py
+-rw-r--r--   0        0        0      325 2023-06-09 11:02:36.316242 caluma-9.0.0/caluma/caluma_core/factories.py
+-rw-r--r--   0        0        0      485 2023-06-09 11:02:36.316242 caluma-9.0.0/caluma/caluma_core/faker.py
+-rw-r--r--   0        0        0    18813 2023-06-09 11:02:36.316242 caluma-9.0.0/caluma/caluma_core/filters.py
+-rw-r--r--   0        0        0      642 2023-06-09 11:02:36.316242 caluma-9.0.0/caluma/caluma_core/forms.py
+-rw-r--r--   0        0        0     4176 2023-06-09 11:02:36.316242 caluma-9.0.0/caluma/caluma_core/health_checks.py
+-rw-r--r--   0        0        0     7855 2023-06-09 11:02:36.316242 caluma-9.0.0/caluma/caluma_core/jexl.py
+-rw-r--r--   0        0        0        0 2023-06-09 11:02:36.316242 caluma-9.0.0/caluma/caluma_core/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 11:02:36.316242 caluma-9.0.0/caluma/caluma_core/management/commands/__init__.py
+-rw-r--r--   0        0        0     1824 2023-06-09 11:02:36.316242 caluma-9.0.0/caluma/caluma_core/management/commands/cleanup_history.py
+-rw-r--r--   0        0        0     3803 2023-06-09 11:02:36.316242 caluma-9.0.0/caluma/caluma_core/management/commands/dump_caluma_config.py
+-rw-r--r--   0        0        0      794 2023-06-09 11:02:36.316242 caluma-9.0.0/caluma/caluma_core/management/commands/migrate.py
+-rw-r--r--   0        0        0     4768 2023-06-09 11:02:36.316242 caluma-9.0.0/caluma/caluma_core/management/commands/migrate_to_prefixed_apps.py
+-rw-r--r--   0        0        0     3078 2023-06-09 11:02:36.316242 caluma-9.0.0/caluma/caluma_core/models.py
+-rw-r--r--   0        0        0    11674 2023-06-09 11:02:36.316242 caluma-9.0.0/caluma/caluma_core/mutation.py
+-rw-r--r--   0        0        0     3216 2023-06-09 11:02:36.316242 caluma-9.0.0/caluma/caluma_core/ordering.py
+-rw-r--r--   0        0        0     3195 2023-06-09 11:02:36.316242 caluma-9.0.0/caluma/caluma_core/pagination.py
+-rw-r--r--   0        0        0     4485 2023-06-09 11:02:36.316242 caluma-9.0.0/caluma/caluma_core/permissions.py
+-rw-r--r--   0        0        0     1253 2023-06-09 11:02:36.316242 caluma-9.0.0/caluma/caluma_core/relay.py
+-rw-r--r--   0        0        0     4764 2023-06-09 11:02:36.316242 caluma-9.0.0/caluma/caluma_core/serializers.py
+-rw-r--r--   0        0        0     7577 2023-06-09 11:02:36.316242 caluma-9.0.0/caluma/caluma_core/types.py
+-rw-r--r--   0        0        0      387 2023-06-09 11:02:36.316242 caluma-9.0.0/caluma/caluma_core/urls.py
+-rw-r--r--   0        0        0     2430 2023-06-09 11:02:36.316242 caluma-9.0.0/caluma/caluma_core/validations.py
+-rw-r--r--   0        0        0     1607 2023-06-09 11:02:36.316242 caluma-9.0.0/caluma/caluma_core/views.py
+-rw-r--r--   0        0        0     2937 2023-06-09 11:02:36.316242 caluma-9.0.0/caluma/caluma_core/visibilities.py
+-rw-r--r--   0        0        0        0 2023-06-09 11:02:36.316242 caluma-9.0.0/caluma/caluma_data_source/__init__.py
+-rw-r--r--   0        0        0      107 2023-06-09 11:02:36.316242 caluma-9.0.0/caluma/caluma_data_source/apps.py
+-rw-r--r--   0        0        0     2066 2023-06-09 11:02:36.316242 caluma-9.0.0/caluma/caluma_data_source/data_source_handlers.py
+-rw-r--r--   0        0        0     3231 2023-06-09 11:02:36.316242 caluma-9.0.0/caluma/caluma_data_source/data_sources.py
+-rw-r--r--   0        0        0     1427 2023-06-09 11:02:36.316242 caluma-9.0.0/caluma/caluma_data_source/schema.py
+-rw-r--r--   0        0        0      508 2023-06-09 11:02:36.316242 caluma-9.0.0/caluma/caluma_data_source/utils.py
+-rw-r--r--   0        0        0        0 2023-06-09 11:02:36.316242 caluma-9.0.0/caluma/caluma_form/__init__.py
+-rw-r--r--   0        0        0     2472 2023-06-09 11:02:36.316242 caluma-9.0.0/caluma/caluma_form/api.py
+-rw-r--r--   0        0        0      100 2023-06-09 11:02:36.316242 caluma-9.0.0/caluma/caluma_form/apps.py
+-rw-r--r--   0        0        0    10172 2023-06-09 11:02:36.316242 caluma-9.0.0/caluma/caluma_form/domain_logic.py
+-rw-r--r--   0        0        0     6164 2023-06-09 11:02:36.316242 caluma-9.0.0/caluma/caluma_form/factories.py
+-rw-r--r--   0        0        0    19812 2023-06-09 11:02:36.316242 caluma-9.0.0/caluma/caluma_form/filters.py
+-rw-r--r--   0        0        0     3283 2023-06-09 11:02:36.316242 caluma-9.0.0/caluma/caluma_form/format_validators.py
+-rw-r--r--   0        0        0     7830 2023-06-09 11:02:36.316242 caluma-9.0.0/caluma/caluma_form/historical_schema.py
+-rw-r--r--   0        0        0     7495 2023-06-09 11:02:36.316242 caluma-9.0.0/caluma/caluma_form/jexl.py
+-rw-r--r--   0        0        0        0 2023-06-09 11:02:36.316242 caluma-9.0.0/caluma/caluma_form/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/management/commands/__init__.py
+-rw-r--r--   0        0        0     1880 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/management/commands/copy_form.py
+-rw-r--r--   0        0        0      631 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/management/commands/create_bucket.py
+-rw-r--r--   0        0        0     1194 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/management/commands/recalculate_calc_answers.py
+-rw-r--r--   0        0        0    10983 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2829 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/migrations/0002_auto_20181221_1517.py
+-rw-r--r--   0        0        0     3862 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/migrations/0003_auto_20190130_0920.py
+-rw-r--r--   0        0        0     1565 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/migrations/0004_auto_20190207_1405.py
+-rw-r--r--   0        0        0      825 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/migrations/0005_auto_20190208_1016.py
+-rw-r--r--   0        0        0      800 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/migrations/0006_choice_type_conversion.py
+-rw-r--r--   0        0        0      629 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/migrations/0007_auto_20190208_1232.py
+-rw-r--r--   0        0        0     1179 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/migrations/0008_auto_20190319_1720.py
+-rw-r--r--   0        0        0     2133 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/migrations/0009_auto_20190321_1722.py
+-rw-r--r--   0        0        0     2302 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/migrations/0010_auto_20190404_0652.py
+-rw-r--r--   0        0        0      604 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/migrations/0011_auto_20190411_0607.py
+-rw-r--r--   0        0        0      788 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/migrations/0012_auto_20190416_1835.py
+-rw-r--r--   0        0        0     1256 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/migrations/0013_auto_20190418_0733.py
+-rw-r--r--   0        0        0     1407 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/migrations/0014_auto_20190429_0910.py
+-rw-r--r--   0        0        0      659 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/migrations/0015_question_format_validators.py
+-rw-r--r--   0        0        0      530 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/migrations/0016_auto_20190510_0843.py
+-rw-r--r--   0        0        0      605 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/migrations/0017_auto_20190619_1320.py
+-rw-r--r--   0        0        0     1859 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/migrations/0018_remove_answer_value_document_data_migration.py
+-rw-r--r--   0        0        0      365 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/migrations/0019_remove_answer_value_document.py
+-rw-r--r--   0        0        0    27839 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/migrations/0020_historicalanswer_historicalanswerdocument_historicaldocument_historicalfile_historicalform_historica.py
+-rw-r--r--   0        0        0     2470 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/migrations/0021_auto_20190708_0905.py
+-rw-r--r--   0        0        0     1453 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/migrations/0022_add_gin_index_to_jsonfields.py
+-rw-r--r--   0        0        0      558 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/migrations/0023_auto_20190729_1448.py
+-rw-r--r--   0        0        0     1087 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/migrations/0024_auto_20190919_1244.py
+-rw-r--r--   0        0        0     4834 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/migrations/0025_dynamicoption_historicaldynamicoption.py
+-rw-r--r--   0        0        0      828 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/migrations/0026_auto_20191031_0834.py
+-rw-r--r--   0        0        0     2087 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/migrations/0027_auto_20200113_0727.py
+-rw-r--r--   0        0        0    12675 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/migrations/0028_auto_20200210_0929.py
+-rw-r--r--   0        0        0     1570 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/migrations/0029_dynamic_option_unique_together.py
+-rw-r--r--   0        0        0     1281 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/migrations/0030_auto_20200219_1359.py
+-rw-r--r--   0        0        0     1701 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/migrations/0031_auto_20200220_0910.py
+-rw-r--r--   0        0        0     1153 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/migrations/0032_auto_20200220_1311.py
+-rw-r--r--   0        0        0     1269 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/migrations/0033_slugfield_length.py
+-rw-r--r--   0        0        0      518 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/migrations/0034_fix_fk_lengths.py
+-rw-r--r--   0        0        0     1687 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/migrations/0035_historicalanswer_history_question_type.py
+-rw-r--r--   0        0        0     1386 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/migrations/0036_default_answers.py
+-rw-r--r--   0        0        0      610 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/migrations/0037_default_answer_one2one.py
+-rw-r--r--   0        0        0     3050 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/migrations/0038_auto_20201224_0920.py
+-rw-r--r--   0        0        0      461 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/migrations/0038_remove_table_answer_value.py
+-rw-r--r--   0        0        0      283 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/migrations/0039_merge_20210114_0956.py
+-rw-r--r--   0        0        0    10393 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/migrations/0040_add_modified_by_user_group.py
+-rw-r--r--   0        0        0     2149 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/migrations/0041_action_button_question.py
+-rw-r--r--   0        0        0      750 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/migrations/0042_auto_20220110_1051.py
+-rw-r--r--   0        0        0     1209 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/migrations/0043_alter_historicalanswer_history_question_type.py
+-rw-r--r--   0        0        0      991 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/migrations/0044_migrate_format_validators.py
+-rw-r--r--   0        0        0     5738 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/migrations/0045_simple_history.py
+-rw-r--r--   0        0        0     5998 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/migrations/0046_file_answer_reverse_keys.py
+-rw-r--r--   0        0        0        0 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/migrations/__init__.py
+-rw-r--r--   0        0        0    22969 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/models.py
+-rw-r--r--   0        0        0     2213 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/ordering.py
+-rw-r--r--   0        0        0    37073 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/schema.py
+-rw-r--r--   0        0        0    23003 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/serializers.py
+-rw-r--r--   0        0        0     7471 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/signals.py
+-rw-r--r--   0        0        0     3883 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/storage_clients.py
+-rw-r--r--   0        0        0     8044 2023-06-09 11:02:36.320242 caluma-9.0.0/caluma/caluma_form/structure.py
+-rw-r--r--   0        0        0    18456 2023-06-09 11:02:36.324242 caluma-9.0.0/caluma/caluma_form/validators.py
+-rw-r--r--   0        0        0        0 2023-06-09 11:02:36.324242 caluma-9.0.0/caluma/caluma_logging/__init__.py
+-rw-r--r--   0        0        0      103 2023-06-09 11:02:36.324242 caluma-9.0.0/caluma/caluma_logging/apps.py
+-rw-r--r--   0        0        0      365 2023-06-09 11:02:36.324242 caluma-9.0.0/caluma/caluma_logging/factories.py
+-rw-r--r--   0        0        0        0 2023-06-09 11:02:36.324242 caluma-9.0.0/caluma/caluma_logging/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 11:02:36.324242 caluma-9.0.0/caluma/caluma_logging/management/commands/__init__.py
+-rw-r--r--   0        0        0     1087 2023-06-09 11:02:36.324242 caluma-9.0.0/caluma/caluma_logging/management/commands/cleanup_access_log.py
+-rw-r--r--   0        0        0     1777 2023-06-09 11:02:36.324242 caluma-9.0.0/caluma/caluma_logging/middleware.py
+-rw-r--r--   0        0        0     1559 2023-06-09 11:02:36.324242 caluma-9.0.0/caluma/caluma_logging/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-06-09 11:02:36.324242 caluma-9.0.0/caluma/caluma_logging/migrations/__init__.py
+-rw-r--r--   0        0        0      657 2023-06-09 11:02:36.324242 caluma-9.0.0/caluma/caluma_logging/models.py
+-rw-r--r--   0        0        0        0 2023-06-09 11:02:36.324242 caluma-9.0.0/caluma/caluma_user/__init__.py
+-rw-r--r--   0        0        0      100 2023-06-09 11:02:36.324242 caluma-9.0.0/caluma/caluma_user/apps.py
+-rw-r--r--   0        0        0      982 2023-06-09 11:02:36.324242 caluma-9.0.0/caluma/caluma_user/models.py
+-rw-r--r--   0        0        0      667 2023-06-09 11:02:36.324242 caluma-9.0.0/caluma/caluma_user/permissions.py
+-rw-r--r--   0        0        0     3355 2023-06-09 11:02:36.324242 caluma-9.0.0/caluma/caluma_user/views.py
+-rw-r--r--   0        0        0      711 2023-06-09 11:02:36.324242 caluma-9.0.0/caluma/caluma_user/visibilities.py
+-rw-r--r--   0        0        0        0 2023-06-09 11:02:36.324242 caluma-9.0.0/caluma/caluma_workflow/__init__.py
+-rw-r--r--   0        0        0     7821 2023-06-09 11:02:36.324242 caluma-9.0.0/caluma/caluma_workflow/api.py
+-rw-r--r--   0        0        0      618 2023-06-09 11:02:36.324242 caluma-9.0.0/caluma/caluma_workflow/apps.py
+-rw-r--r--   0        0        0    21249 2023-06-09 11:02:36.324242 caluma-9.0.0/caluma/caluma_workflow/domain_logic.py
+-rw-r--r--   0        0        0     1606 2023-06-09 11:02:36.324242 caluma-9.0.0/caluma/caluma_workflow/dynamic_groups.py
+-rw-r--r--   0        0        0     1941 2023-06-09 11:02:36.324242 caluma-9.0.0/caluma/caluma_workflow/dynamic_tasks.py
+-rw-r--r--   0        0        0      533 2023-06-09 11:02:36.324242 caluma-9.0.0/caluma/caluma_workflow/events.py
+-rw-r--r--   0        0        0     2674 2023-06-09 11:02:36.324242 caluma-9.0.0/caluma/caluma_workflow/factories.py
+-rw-r--r--   0        0        0     6851 2023-06-09 11:02:36.324242 caluma-9.0.0/caluma/caluma_workflow/filters.py
+-rw-r--r--   0        0        0     6485 2023-06-09 11:02:36.324242 caluma-9.0.0/caluma/caluma_workflow/jexl.py
+-rw-r--r--   0        0        0    11029 2023-06-09 11:02:36.324242 caluma-9.0.0/caluma/caluma_workflow/migrations/0001_initial.py
+-rw-r--r--   0        0        0      665 2023-06-09 11:02:36.324242 caluma-9.0.0/caluma/caluma_workflow/migrations/0002_auto_20181213_1334.py
+-rw-r--r--   0        0        0      755 2023-06-09 11:02:36.324242 caluma-9.0.0/caluma/caluma_workflow/migrations/0003_auto_20181217_1051.py
+-rw-r--r--   0        0        0     1631 2023-06-09 11:02:36.324242 caluma-9.0.0/caluma/caluma_workflow/migrations/0004_auto_20181218_1352.py
+-rw-r--r--   0        0        0     4268 2023-06-09 11:02:36.324242 caluma-9.0.0/caluma/caluma_workflow/migrations/0005_auto_20181228_1243.py
+-rw-r--r--   0        0        0      993 2023-06-09 11:02:36.328242 caluma-9.0.0/caluma/caluma_workflow/migrations/0006_auto_20190121_1440.py
+-rw-r--r--   0        0        0     1034 2023-06-09 11:02:36.328242 caluma-9.0.0/caluma/caluma_workflow/migrations/0007_auto_20190206_0854.py
+-rw-r--r--   0        0        0      686 2023-06-09 11:02:36.328242 caluma-9.0.0/caluma/caluma_workflow/migrations/0008_auto_20190208_1302.py
+-rw-r--r--   0        0        0     1620 2023-06-09 11:02:36.328242 caluma-9.0.0/caluma/caluma_workflow/migrations/0009_auto_20190213_0939.py
+-rw-r--r--   0        0        0      752 2023-06-09 11:02:36.328242 caluma-9.0.0/caluma/caluma_workflow/migrations/0010_auto_20190213_1050.py
+-rw-r--r--   0        0        0     1234 2023-06-09 11:02:36.328242 caluma-9.0.0/caluma/caluma_workflow/migrations/0011_auto_20190220_1303.py
+-rw-r--r--   0        0        0    21984 2023-06-09 11:02:36.328242 caluma-9.0.0/caluma/caluma_workflow/migrations/0012_historicalcase_historicalflow_historicaltask_historicaltaskflow_historicalworkflow_historicalworkite.py
+-rw-r--r--   0        0        0     3458 2023-06-09 11:02:36.328242 caluma-9.0.0/caluma/caluma_workflow/migrations/0013_auto_20190718_1235.py
+-rw-r--r--   0        0        0     1120 2023-06-09 11:02:36.328242 caluma-9.0.0/caluma/caluma_workflow/migrations/0014_add_gin_index_to_jsonfields.py
+-rw-r--r--   0        0        0     1298 2023-06-09 11:02:36.328242 caluma-9.0.0/caluma/caluma_workflow/migrations/0015_add_work_item_skipped.py
+-rw-r--r--   0        0        0     2219 2023-06-09 11:02:36.328242 caluma-9.0.0/caluma/caluma_workflow/migrations/0016_auto_20200113_0727.py
+-rw-r--r--   0        0        0     7593 2023-06-09 11:02:36.328242 caluma-9.0.0/caluma/caluma_workflow/migrations/0017_auto_20200210_0929.py
+-rw-r--r--   0        0        0      924 2023-06-09 11:02:36.328242 caluma-9.0.0/caluma/caluma_workflow/migrations/0018_auto_20200219_1359.py
+-rw-r--r--   0        0        0      924 2023-06-09 11:02:36.328242 caluma-9.0.0/caluma/caluma_workflow/migrations/0019_slugfield_length.py
+-rw-r--r--   0        0        0     2849 2023-06-09 11:02:36.328242 caluma-9.0.0/caluma/caluma_workflow/migrations/0020_case_families.py
+-rw-r--r--   0        0        0     1741 2023-06-09 11:02:36.328242 caluma-9.0.0/caluma/caluma_workflow/migrations/0021_work_item_controlling_groups.py
+-rw-r--r--   0        0        0     2503 2023-06-09 11:02:36.328242 caluma-9.0.0/caluma/caluma_workflow/migrations/0022_workitem_name_description.py
+-rw-r--r--   0        0        0     1063 2023-06-09 11:02:36.328242 caluma-9.0.0/caluma/caluma_workflow/migrations/0023_auto_20200730_1135.py
+-rw-r--r--   0        0        0     2490 2023-06-09 11:02:36.328242 caluma-9.0.0/caluma/caluma_workflow/migrations/0024_auto_20200901_1026.py
+-rw-r--r--   0        0        0     1452 2023-06-09 11:02:36.328242 caluma-9.0.0/caluma/caluma_workflow/migrations/0025_auto_20200901_1415.py
+-rw-r--r--   0        0        0     1336 2023-06-09 11:02:36.328242 caluma-9.0.0/caluma/caluma_workflow/migrations/0026_auto_20200901_1435.py
+-rw-r--r--   0        0        0     6415 2023-06-09 11:02:36.328242 caluma-9.0.0/caluma/caluma_workflow/migrations/0027_add_modified_by_user_group.py
+-rw-r--r--   0        0        0     2618 2023-06-09 11:02:36.328242 caluma-9.0.0/caluma/caluma_workflow/migrations/0028_redoable_field.py
+-rw-r--r--   0        0        0      853 2023-06-09 11:02:36.328242 caluma-9.0.0/caluma/caluma_workflow/migrations/0029_task_continue_async.py
+-rw-r--r--   0        0        0     3680 2023-06-09 11:02:36.328242 caluma-9.0.0/caluma/caluma_workflow/migrations/0030_remove_choices_char_field.py
+-rw-r--r--   0        0        0     3474 2023-06-09 11:02:36.328242 caluma-9.0.0/caluma/caluma_workflow/migrations/0031_simple_history.py
+-rw-r--r--   0        0        0        0 2023-06-09 11:02:36.328242 caluma-9.0.0/caluma/caluma_workflow/migrations/__init__.py
+-rw-r--r--   0        0        0     9946 2023-06-09 11:02:36.328242 caluma-9.0.0/caluma/caluma_workflow/models.py
+-rw-r--r--   0        0        0    12709 2023-06-09 11:02:36.328242 caluma-9.0.0/caluma/caluma_workflow/schema.py
+-rw-r--r--   0        0        0    19994 2023-06-09 11:02:36.328242 caluma-9.0.0/caluma/caluma_workflow/serializers.py
+-rw-r--r--   0        0        0     4914 2023-06-09 11:02:36.328242 caluma-9.0.0/caluma/caluma_workflow/utils.py
+-rw-r--r--   0        0        0     1892 2023-06-09 11:02:36.328242 caluma-9.0.0/caluma/caluma_workflow/validators.py
+-rw-r--r--   0        0        0     2120 2023-06-09 11:02:36.328242 caluma-9.0.0/caluma/caluma_workflow/visibilities.py
+-rw-r--r--   0        0        0    13211 2023-06-09 11:02:36.328242 caluma-9.0.0/caluma/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-09 11:02:36.328242 caluma-9.0.0/caluma/extensions/__init__.py
+-rw-r--r--   0        0        0       53 2023-06-09 11:02:36.328242 caluma-9.0.0/caluma/extensions/data_sources.py
+-rw-r--r--   0        0        0       39 2023-06-09 11:02:36.328242 caluma-9.0.0/caluma/extensions/dynamic_groups.py
+-rw-r--r--   0        0        0       40 2023-06-09 11:02:36.328242 caluma-9.0.0/caluma/extensions/events.py
+-rw-r--r--   0        0        0       58 2023-06-09 11:02:36.328242 caluma-9.0.0/caluma/extensions/format_validators.py
+-rw-r--r--   0        0        0       52 2023-06-09 11:02:36.328242 caluma-9.0.0/caluma/extensions/permissions.py
+-rw-r--r--   0        0        0       52 2023-06-09 11:02:36.328242 caluma-9.0.0/caluma/extensions/validations.py
+-rw-r--r--   0        0        0       52 2023-06-09 11:02:36.328242 caluma-9.0.0/caluma/extensions/visibilities.py
+-rw-r--r--   0        0        0     2785 2023-06-09 11:02:36.328242 caluma-9.0.0/caluma/schema.py
+-rw-r--r--   0        0        0        0 2023-06-09 11:02:36.328242 caluma-9.0.0/caluma/settings/__init__.py
+-rw-r--r--   0        0        0     3520 2023-06-09 11:02:36.328242 caluma-9.0.0/caluma/settings/caluma.py
+-rw-r--r--   0        0        0     6014 2023-06-09 11:02:36.328242 caluma-9.0.0/caluma/settings/django.py
+-rw-r--r--   0        0        0      100 2023-06-09 11:02:36.328242 caluma-9.0.0/caluma/urls.py
+-rw-r--r--   0        0        0     3416 2023-06-09 11:02:36.328242 caluma-9.0.0/caluma/utils.py
+-rw-r--r--   0        0        0      403 2023-06-09 11:02:36.328242 caluma-9.0.0/caluma/wsgi.py
+-rw-r--r--   0        0        0     3921 2023-06-09 11:02:36.332242 caluma-9.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3733 1970-01-01 00:00:00.000000 caluma-9.0.0/PKG-INFO
```

### Comparing `caluma-8.0.0b9/CHANGELOG.md` & `caluma-9.0.0/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,245 @@
+# v9.0.0 (9 June 2023)
+
+### Feature
+* **auth:** Only use userinfo for auth (drop introspect) ([`d065ef8`](https://github.com/projectcaluma/caluma/commit/d065ef8fd52f0c09d7c5f660c72441ef1cb3a0a6))
+* **analytics:** Support accessing sub-cases and their parent ([`6dfc4f9`](https://github.com/projectcaluma/caluma/commit/6dfc4f9c5f7eeb92042447e77954639d298a907b))
+
+### Breaking
+* setting the `OIDC_INTROSPECT_*` and `OIDC_CLIENT_AS_USERNAME` env vars is obsolete now. Auth now only calls the userinfo endpoint without any fallback to the introspect endpoint. This will possibly have an impact on the `username` property of the user object. If your extensions depend on that property, please update them if necessary. Additionally, all requests sent to Caluma must include the `openid`-scope. ([`d065ef8`](https://github.com/projectcaluma/caluma/commit/d065ef8fd52f0c09d7c5f660c72441ef1cb3a0a6))
+
+
+# v8.0.0 (12 May 2023)
+
+### Fix
+* **workflow:** Provide context to WorkItemValidator ([`2fb5308`](https://github.com/projectcaluma/caluma/commit/2fb530874869898a0e03ce9af16038003ce1f56a))
+
+**This is the long overdue stable release of Caluma v8. For a detailed description of the changes to v7, please refer to the changelogs of the v8 beta versions.**
+
+
+# v8.0.0-beta.30 (10 May 2023)
+
+### Fix
+
+* **analytics:** Fix aliases exceeding 63 bytes ([`cdca090`](https://github.com/projectcaluma/caluma/commit/cdca090e6a8cafbeb3dde5aad29bb1c866dea518))
+
+
+# v8.0.0-beta.29 (13 April 2023)
+
+### Feature
+
+- **filters:** Add filters for modified_at ([`16fdb73`](https://github.com/projectcaluma/caluma/commit/16fdb732f127fb06038784e87582441f303526de))
+
+
+# v8.0.0-beta.28 (21 March 2023)
+
+### Feature
+* **filters:** Add useful deadline filters to workitems ([`f74d641`](https://github.com/projectcaluma/caluma/commit/f74d641eac81151aa0b7a435f804a43078a952a2))
+
+
+# v8.0.0-beta.27 (10 March 2023)
+
+### Feature
+* **filters:** Support word combinations in SearchAnswersFilter ([`4c3e910`](https://github.com/projectcaluma/caluma/commit/4c3e910db65cc34677856a97b07b812c3db28233))
+* **workflow:** Add case_document_forms filter to work item ([`e351de3`](https://github.com/projectcaluma/caluma/commit/e351de3b9c4c48e70f529295b13a61cc5052daec))
+
+
+# v8.0.0-beta.26 (20 February 2023)
+
+### Fix
+* **form:** Fix validation in document validity graph ([`6b859fa`](https://github.com/projectcaluma/caluma/commit/6b859fa1f76762a8fcfadff7f1010ec4b17d02f4))
+
+
+# v8.0.0-beta.25 (17 February 2023)
+
+This release provides a management command for recalculating calculated Answers that
+contain values from `TableQuestions`. Due to a bug, answers to calculated questions
+were wrong under certain conditions, if they contained values from table rows. This
+command recalculates all of them.
+
+If you use `CalculatedFloatQuestions` in your forms, it is advised to run this command:
+
+```shell
+python manage.py recalculate_calc_answers
+```
+
+### Fix
+* Replace faulty migration for calc answers with a command ([`4a3e85c`](https://github.com/projectcaluma/caluma/commit/4a3e85cf5a1ac105541dde1b04d8081d01a90e12))
+
+
+# v8.0.0-beta.24 (17 February 2023)
+
+### Feature
+* **analytics:** Add support for calculated questions ([`196ab05`](https://github.com/projectcaluma/caluma/commit/196ab054abb94aa4e27900ade6c3920b14829ee6))
+
+### Fix
+* Fix calc answer evaluation when adding new table rows ([`cb668ba`](https://github.com/projectcaluma/caluma/commit/cb668ba88371fe5d48ee4402348ec9182068ee18))
+* **workflow:** Emit post_create_work_item when redo is set to ready ([`5e9744a`](https://github.com/projectcaluma/caluma/commit/5e9744a0b9cbcc2fdbf741f77fa1603b8d3bf69d))
+* **analytics:** Handle missing dates ([`a06181a`](https://github.com/projectcaluma/caluma/commit/a06181a11994a9e40600b419753b83d35557b76e))
+* **analytics:** Properly quote expressions ([`3ff7f36`](https://github.com/projectcaluma/caluma/commit/3ff7f368c87f1f058ad0420fb14e8fda522ccffd))
+
+
+# v8.0.0-beta.23 (26 January 2023)
+
+### Fix
+* **analytics:** Fix form identifier; disable subform form ([`94542ac`](https://github.com/projectcaluma/caluma/commit/94542aca4c9e9d5df26240aee1e465ad01c4db58))
+* Properly quote aliases - small additional fixes ([`535c703`](https://github.com/projectcaluma/caluma/commit/535c7030a019672ce72d2db8efe532cfab492125))
+
+
+# v8.0.0-beta.22 (12 December 2022)
+
+### Feature
+* **analytics:** Add support for form name extraction ([`1df3f53`](https://github.com/projectcaluma/caluma/commit/1df3f536a7968b5d0f6bf0dcc0392af338e36bcb))
+* Allow using client id as user for client-secret auth ([`3e45c61`](https://github.com/projectcaluma/caluma/commit/3e45c61a9feda916fefc06ab6f2764bbe415bf5f))
+
+### Fix
+* Do not crash when django-extensions is missing ([`6028be3`](https://github.com/projectcaluma/caluma/commit/6028be3d297ec76bd0b584553fb56679a85a43b9))
+* **analytics:** Fix commandline output crash with certain aliases ([`1839423`](https://github.com/projectcaluma/caluma/commit/1839423b5ef5559b392138c04881abbb204a2c0e))
+* **analytics:** Do not crash with more complex visibility layers ([`71be082`](https://github.com/projectcaluma/caluma/commit/71be0822e467bfe5edf757b8068c483a91c73f18))
+* **analytics:** Do not output summary for simple tables ([`34205cf`](https://github.com/projectcaluma/caluma/commit/34205cfe9a7ffc6cc9e3d2d4ae807f0a25e59cad))
+
+
+# v8.0.0-beta.21 (17 November 2022)
+
+### Feature
+* **data_source:** Add question and context arguments for data sources ([`cb2739e`](https://github.com/projectcaluma/caluma/commit/cb2739ed40a7afabf95f2ce0386b38dc07d919bb))
+
+### Breaking
+* The method `get_data` on data sources receives two new arguments `question` (caluma question model) and `context` (dict). The method `validate_answer_value` on data sources receives a new argument `context` (dict).  ([`cb2739e`](https://github.com/projectcaluma/caluma/commit/cb2739ed40a7afabf95f2ce0386b38dc07d919bb))
+
+
+# v8.0.0-beta.20 (10 November 2022)
+
+### Feature
+* **workflow:** Include family field on case schema model ([`aea98f9`](https://github.com/projectcaluma/caluma/commit/aea98f9d24e9eba3ae82bb789a1bcb12f62f5324))
+* **filters:** Add `visibleInDocument`-filter for questions ([`9f5caa2`](https://github.com/projectcaluma/caluma/commit/9f5caa2527e27fc4185d7fcca4339a60ec0ccb83))
+* **analytics:** Enable reordering of analytics fields ([`59eadbc`](https://github.com/projectcaluma/caluma/commit/59eadbc799a2486f7606ce6d5d1eac3d12b86398))
+
+### Fix
+* Fix breaking change introduced in 59eadbc ([`34be9bf`](https://github.com/projectcaluma/caluma/commit/34be9bfedfd893e0dd86f117df8b61d011359f53))
+* Remove order_by in field_ordering, refactor test ([`121a433`](https://github.com/projectcaluma/caluma/commit/121a433cbf12b7151aab7cab88611ab77f531adb))
+
+
+# v8.0.0-beta.19 (27 September 2022)
+
+### Fix
+* **deps:** Pin graphene-django to v3.0.0b7 ([`3efc320`](https://github.com/projectcaluma/caluma/commit/3efc3209e79d8ea010802e9c11bd0e1b91f0c8b2))
+
+
+# v8.0.0-beta.18 (12 September 2022)
+
+### Feature
+* **analytics:** Provide option labels ([`d1f7a38`](https://github.com/projectcaluma/caluma/commit/d1f7a380caa664e9b24dc6f205f212952a63e63c))
+* **cases:** Add filter to exclude child cases ([`dd58f6c`](https://github.com/projectcaluma/caluma/commit/dd58f6c1d0f8df73b620616d061bc90f73a6a8e8))
+
+
+# v8.0.0-beta.17 (9 September 2022)
+
+### Fix
+* **events:** Don't emit create work item events when updating ([`4f2f491`](https://github.com/projectcaluma/caluma/commit/4f2f4916d62e689b59b805bdfdb6bf12e76d53d7))
+
+### Breaking
+* The `saveWorkItem` mutation doesn't emit `pre_create_work_item` `post_create_work_item` anymore since this is not the expected behaviour.  ([`4f2f491`](https://github.com/projectcaluma/caluma/commit/4f2f4916d62e689b59b805bdfdb6bf12e76d53d7))
+
+
+# v8.0.0-beta.16 (1 September 2022)
+
+### Fix
+* **redo:** Recalculate deadline after updating a redo work item to ready ([`f803fbe`](https://github.com/projectcaluma/caluma/commit/f803fbe9951b09bd677ba3b8c5dda88af258203b))
+* **permissions:** Make sure user permission classes call super ([`6e1945b`](https://github.com/projectcaluma/caluma/commit/6e1945b7a75f15b9ffefcb33173d4202523147af))
+
+
+# v8.0.0-beta.15 (26 August 2022)
+
+### Feature
+* **flow:** Allow flows to not have tasks in next if redoable is given ([`867b796`](https://github.com/projectcaluma/caluma/commit/867b796394c55fda5960d6b889cc594f55594b52))
+* **reopen case:** Allow reopening child cases of ready work items ([`e073cad`](https://github.com/projectcaluma/caluma/commit/e073cad3afb204af18e484f6b59758fdcba09476))
+* **workflow:** Add is_redoable property to work item schema ([`709965d`](https://github.com/projectcaluma/caluma/commit/709965d9822433b58e00d51ec71500fb4865a802))
+* **workflow:** Add search answer filter to work item filters ([`0ceb2c6`](https://github.com/projectcaluma/caluma/commit/0ceb2c6db8405c7eb611cb58bca7881a51e22cdc))
+* **caluma:** Add new work item order key ([`a794211`](https://github.com/projectcaluma/caluma/commit/a794211421846099173a72300309b693888eabe1))
+
+### Fix
+* **redo:** Fix workflow of work items in status redo ([`abbdb92`](https://github.com/projectcaluma/caluma/commit/abbdb924c4d8fa004d4c5eb0f56748218810de49))
+* **analytics:** Handle None and ignore 0 in summary ([`d5c9669`](https://github.com/projectcaluma/caluma/commit/d5c96692c69db4323593563d3cda0298feba38dc))
+
+### Breaking
+* This removes the deprecated properties `userinfo` and `introspection` on the base user class which have been deprecated for a long time.  ([`b4fd9e2`](https://github.com/projectcaluma/caluma/commit/b4fd9e227f5e85c89f800b018e1ca2ae079c434b))
+* This drops the `saveCase` mutation which has been deprecated for a long time.  ([`6cf701d`](https://github.com/projectcaluma/caluma/commit/6cf701d749e34182c6a2e495b3050f3f47bc17b6))
+
+
+# v8.0.0-beta.14 (18 August 2022)
+
+### Fix
+* Exclude not supported questions from answer search
+([`a27681c`](https://github.com/projectcaluma/caluma/commit/a27681ca59079c6783d4498e12f3cfcca17ba53a))
+* Fix multifile migration again
+([`d812956`](https://github.com/projectcaluma/caluma/commit/d812956cffde04f1d10ffc05e674a6942ef19892))
+* Handle files from history that don't exist anymore in migration
+([`21611c3`](https://github.com/projectcaluma/caluma/commit/21611c3636c4a66c67ff2f2593649feca2f6f547))
+
+
+# v8.0.0-beta.13 (15 August 2022)
+
+### Fix
+* **historical-schema:** Fetch the correct historical files
+([`2580e80`](https://github.com/projectcaluma/caluma/commit/2580e80fceb5bdaa2636ffbc30e1f9bf16eac46b))
+* **form:** Migration problem with historicalanswer
+([`a8633b6`](https://github.com/projectcaluma/caluma/commit/a8633b60acc0b3d1ecfc180faf3f4c611f82f293))
+* Multiple fixes for analytics
+([`e78b8d2`](https://github.com/projectcaluma/caluma/commit/e78b8d28a7349c953541c3b4953b8fe7f5476ac6))
+
+
+# v8.0.0-beta.12 (5 August 2022)
+
+### Feature
+* **workflow:** Add ids filter to case
+([`89b70ec`](https://github.com/projectcaluma/caluma/commit/89b70ecf4cc098b8d43d0ddfe87491483f1ab6ae))
+* **form:** Multiple files in file questions
+([`4600ed0`](https://github.com/projectcaluma/caluma/commit/4600ed09bbb3efab6d25308d74384eef8f1a97f1))
+* **core:** Allow input type override
+([`215cdb7`](https://github.com/projectcaluma/caluma/commit/215cdb75f8bff500fcad9f3c58d4593f0b60f4b4))
+* Searchanswers in forms
+([`6a75f17`](https://github.com/projectcaluma/caluma/commit/6a75f17dbc66605a0624fb8b3b3777b30450d513))
+
+### Fix
+* **form:** Fix and test search_answers
+([`371a4f0`](https://github.com/projectcaluma/caluma/commit/371a4f0b019509d06b090908369710aafc2d48b0))
+* **analytics:** Provide more correct supported functions in analytics
+([`2130f34`](https://github.com/projectcaluma/caluma/commit/2130f34b367549cc71eb0977afc25984fc03bab7))
+* **log:** Minio stat errors shouldn't be errors
+([`701bafc`](https://github.com/projectcaluma/caluma/commit/701bafcd1ba0686a06b32c626928eaed0ca6e26b))
+* **workflow:** Remove and fix ordering keys
+([`409e54f`](https://github.com/projectcaluma/caluma/commit/409e54f3719205c07551b038f8de302708165de4))
+* **schema:** Reopen case schema clarification
+([`6153b45`](https://github.com/projectcaluma/caluma/commit/6153b453d92ace28593cb666dc7a399d2a7c9779))
+
+### Breaking
+* This renames the question type constant for file questions, and changes the
+semantics of the answer value for file questions as well: It is now a list of
+dicts instead of a single string. The response type for querying file(s) answers
+now also is a list instead of a single dict.
+([`4600ed0`](https://github.com/winged/caluma/commit/4600ed09bbb3efab6d25308d74384eef8f1a97f1))
+
+
+# v8.0.0-beta.11 (6 July 2022)
+
+### Feature
+* **core:** Allow input type override ([`ec4c899`](https://github.com/projectcaluma/caluma/commit/ec4c8997187452a12e091d3e94c6851e7c235156))
+
+### Fix
+* **form:** Use potentially prefetched answer document set for table rows ([`58e0a7c`](https://github.com/projectcaluma/caluma/commit/58e0a7c16747f8f0ec9a92c90171e898bbbe98e0))
+* **schema:** Reopen case schema clarification ([`a394273`](https://github.com/projectcaluma/caluma/commit/a3942731645dcb94cc64923664be0c3733892d14))
+
+
+# v8.0.0-beta.10 (24 June 2022)
+
+### Fix
+* **document:** Fix label of copied dynamic options ([`00383fc`](https://github.com/projectcaluma/caluma/commit/00383fcb8cbe06bfd53e26067be33ad1bcc975a7))
+
+
 # v8.0.0-beta.9 (24 June 2022)
 
 ### Fix
 * **document:** Copy dynamic options when copying documents ([`67910d9`](https://github.com/projectcaluma/caluma/commit/67910d96b98721be9953920ca23bddc33f4521ea))
 * ReopenCase should disregard WorkItems in status REDO ([`dded3a8`](https://github.com/projectcaluma/caluma/commit/dded3a8b1f54b4efcb4c654966dc2234d9909ddb))
 * **deps:** Update dependencies of dependencies ([`e3a5de3`](https://github.com/projectcaluma/caluma/commit/e3a5de38c3a9b1d1456e9fbee6f108913dc7b6df))
 * **form:** Set questions of searchAnswers as required ([`fb7ad5f`](https://github.com/projectcaluma/caluma/commit/fb7ad5feb120abeaf3ea45670fa5349c86eb8464))
```

### Comparing `caluma-8.0.0b9/LICENSE` & `caluma-9.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b9/README.md` & `caluma-9.0.0/README.md`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b9/caluma/caluma_analytics/README.md` & `caluma-9.0.0/caluma/caluma_analytics/README.md`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b9/caluma/caluma_analytics/conftest.py` & `caluma-9.0.0/caluma/caluma_analytics/conftest.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from caluma.caluma_workflow import models as workflow_models
 
 from . import models
 
 
 @pytest.fixture
-def example_analytics(analytics_table, form_and_document, settings):
+def example_analytics(analytics_table, settings):
     analytics_table.starting_object = "cases"
     analytics_table.save()
 
     settings.META_FIELDS = ["foo"]
 
     analytics_table.fields.create(
         data_source="created_at",
@@ -33,14 +33,19 @@
         alias="statuuuuuus",
     )
     analytics_table.fields.create(
         data_source="document[top_form].top_question",
         function=models.AnalyticsField.FUNCTION_VALUE,
         alias="from_the_doc",
     )
+    analytics_table.fields.create(
+        data_source="document[top_form].form.sub_question",
+        function=models.AnalyticsField.FUNCTION_VALUE,
+        alias="sub_question_sumsumsum",
+    )
     return analytics_table
 
 
 @pytest.fixture
 def analytics_cases(form_and_document, case_factory, set_date, work_item_factory):
     """Create a number of cases with documents to be used in testing.
 
@@ -76,15 +81,14 @@
         _makecase(f"2022-02-{day:02}", status=status)
         for day, status in enumerate(statuses, start=1)
     ]
 
 
 @pytest.fixture
 def example_pivot_table(example_analytics):
-
     status_field = example_analytics.fields.get(alias="statuuuuuus")
 
     status_field.function = models.AnalyticsField.FUNCTION_VALUE
     status_field.alias = "status"
     status_field.save()
 
     created_field = example_analytics.fields.get(alias="created_at")
@@ -92,12 +96,17 @@
     created_field.alias = "last_created"
     created_field.save()
 
     quarter_field = example_analytics.fields.get(alias="quarter")
     quarter_field.function = models.AnalyticsField.FUNCTION_MAX
     quarter_field.save()
 
+    sub_q_field = example_analytics.fields.get(alias="sub_question_sumsumsum")
+    sub_q_field.function = models.AnalyticsField.FUNCTION_SUM
+    sub_q_field.alias = "sub_question_sumsumsum"
+    sub_q_field.save()
+
     example_analytics.fields.all().exclude(
-        pk__in=[status_field.pk, created_field.pk, quarter_field.pk]
+        pk__in=[status_field.pk, created_field.pk, quarter_field.pk, sub_q_field.pk]
     ).delete()
 
     return example_analytics
```

### Comparing `caluma-8.0.0b9/caluma/caluma_analytics/factories.py` & `caluma-9.0.0/caluma/caluma_analytics/factories.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b9/caluma/caluma_analytics/filters.py` & `caluma-9.0.0/caluma/caluma_analytics/filters.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b9/caluma/caluma_analytics/management/commands/run_analytics.py` & `caluma-9.0.0/caluma/caluma_analytics/management/commands/run_analytics.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import hashlib
 import json
 from collections import defaultdict
 
 from django.core.management.base import BaseCommand
 
 from caluma.caluma_analytics.models import AnalyticsTable
 from caluma.caluma_analytics.simple_table import SimpleTable
@@ -78,25 +79,35 @@
                 [{k: str(v) for k, v in rec.items()} for rec in records], indent=4
             )
         )
 
     def show_table(self, records):
         """Output the analytics table as an ASCII table to the console."""
 
+        def _rowkey(val):
+            # rowkey is used so any column names (aliases) incompatible
+            # with format string syntax won't trip up the output code
+            return "row" + hashlib.md5(val.encode("utf-8")).hexdigest()
+
         col_lengths = defaultdict(int)
 
         for rec in records:
-            for key, val in rec.items():
-                new_len = max(col_lengths[key], len(str(val)), len(key))
+            for alias, val in rec.items():
+                key = _rowkey(alias)
+                new_len = max(col_lengths[key], len(str(val)), len(alias))
                 col_lengths[key] = new_len
 
+        # just use the last record to get the labels
+        col_labels = {_rowkey(k): k for k in rec.keys()}
+
         format_string = " ".join(
             [
                 "{" + col + ":<" + str(length + 2) + "}"
                 for col, length in col_lengths.items()
             ]
         )
-        print(format_string.format(**{k: k for k in col_lengths}))
+        print(format_string.format(**col_labels))
         print(format_string.format(**{k: "-" * l for k, l in col_lengths.items()}))
 
         for rec in records:
-            print(format_string.format(**{k: str(v) for k, v in rec.items()}))
+            fdata = {_rowkey(k): str(v) for k, v in rec.items()}
+            print(format_string.format(**fdata))
```

### Comparing `caluma-8.0.0b9/caluma/caluma_analytics/migrations/0001_initial.py` & `caluma-9.0.0/caluma/caluma_analytics/migrations/0001_initial.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import django.db.models.deletion
 import localized_fields.fields.field
 import simple_history.models
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
     dependencies = []
 
     operations = [
         migrations.CreateModel(
             name="AnalyticsTable",
```

### Comparing `caluma-8.0.0b9/caluma/caluma_analytics/migrations/0002_analytics_pivot_table.py` & `caluma-9.0.0/caluma/caluma_analytics/migrations/0002_analytics_pivot_table.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 3.2.12 on 2022-03-24 12:15
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("caluma_analytics", "0001_initial"),
     ]
 
     operations = [
         migrations.RemoveConstraint(
             model_name="analyticsfield",
```

### Comparing `caluma-8.0.0b9/caluma/caluma_analytics/migrations/0003_starting_objects.py` & `caluma-9.0.0/caluma/caluma_analytics/migrations/0003_starting_objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 3.2.12 on 2022-03-31 14:24
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("caluma_analytics", "0002_analytics_pivot_table"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="analyticstable",
```

### Comparing `caluma-8.0.0b9/caluma/caluma_analytics/migrations/0004_simple_history.py` & `caluma-9.0.0/caluma/caluma_analytics/migrations/0004_simple_history.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 3.2.13 on 2022-06-09 11:26
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("caluma_analytics", "0003_starting_objects"),
     ]
 
     operations = [
         migrations.AlterModelOptions(
             name="historicalanalyticsfield",
```

### Comparing `caluma-8.0.0b9/caluma/caluma_analytics/models.py` & `caluma-9.0.0/caluma/caluma_analytics/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,19 +87,21 @@
     filters = ArrayField(models.TextField(), blank=True, null=True, default=list)
 
     function = models.CharField(
         max_length=20, choices=FUNCTION_CHOICES, default=FUNCTION_VALUE
     )
 
     show_output = models.BooleanField(default=True)
+    sort = models.PositiveIntegerField(editable=False, db_index=True, default=0)
 
     def __repr__(self):
         return f"AnalyticsField<{self.table.slug}.{self.alias}>"
 
     class Meta:
+        ordering = ["sort", "-created_at"]
         constraints = [
             UniqueConstraint(
                 name="unique_data_source",
                 fields=["table", "data_source", "function"],
             ),
             UniqueConstraint(
                 name="unique_alias",
```

### Comparing `caluma-8.0.0b9/caluma/caluma_analytics/pivot_table.py` & `caluma-9.0.0/caluma/caluma_analytics/pivot_table.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,49 +1,46 @@
 from __future__ import annotations  # self-referencing annotations
 
+from collections import defaultdict
 from functools import cached_property
 
 from django.db import connection
 from psycopg2.extras import DictCursor
 
-from . import models, simple_table, sql
+from . import simple_table, sql
 
 FUNCTION_PARAMETER_CAST = {
     "sum": "::float",
     "avg": "::float",
 }
 
 
-class PivotTable:
+class PivotTable(simple_table.SQLAliasMixin):
     class _AnonymousInfo:
         """
         Pseudo GraphQL info object.
 
         Used for commandline access, so the commandline version
         can also invoke the visibilities.
         """
 
         context = {}
 
-    def __init__(self, table, info=_AnonymousInfo, is_summary=False):
+    def __init__(self, table, info=_AnonymousInfo):
         self.info = info
 
         self.table = table
         self.last_query = None
         self.last_query_params = None
-        self.base_table = simple_table.SimpleTable(
-            self.table, is_summary=is_summary, info=info
-        )
-        self.is_summary = is_summary
+        self.base_table = simple_table.SimpleTable(self.table, info=info)
+        self._summary = defaultdict(int)
 
     @cached_property
     def _fields(self):
         fields = self.table.fields.all()
-        if self.is_summary:
-            fields = fields.exclude(function=models.AnalyticsField.FUNCTION_VALUE)
 
         return list(fields)
 
     def get_sql_and_params(self):
         """Return a list of records as specified in the given table config."""
 
         group_by = []
@@ -57,57 +54,67 @@
         selects_by_alias = {
             alias: fragment for fragment, alias in aggregate_query.select
         }
 
         new_selects = []
 
         for field in self._fields:
-            key = f"analytics_result_{field.alias}"
+            key = self._sql_alias(field.alias)
 
             # old field might be directly selected in the base query,
-            # in which case we need to alias it's expression. If it's
+            # in which case we need to alias its expression. If it's
             # not directly in the base, it won't be in the top-level selects
             # list, but will be aliased to the known name in a subquery.
             old_field = selects_by_alias.get(key, key)
 
-            new_alias = f"analytics_result_{field.alias}"
+            new_alias = self._sql_alias(field.alias)
 
             if field.function == field.FUNCTION_VALUE:
                 group_by.append(old_field)
                 new_selects.append((old_field, new_alias))
-            else:
+            elif field.function != field.FUNCTION_VALUE:
                 cast = FUNCTION_PARAMETER_CAST.get(field.function, "")
                 new_selects.append((f"{field.function}({old_field}{cast})", new_alias))
 
+        # TODO: instead of replacing selects, use sub-query
         aggregate_query.select = new_selects
         aggregate_query.group_by = group_by
         aggregate_query.select_direct_only = True
 
         sql_query, params, _ = sql.QueryRender(aggregate_query).as_sql(alias=None)
 
         return sql_query, params
 
+    @cached_property
+    def field_ordering(self):
+        return list(self.table.fields.all().values_list("alias", flat=True))
+
     def get_records(self):
+        self._summary = defaultdict(int)
         sql_query, params = self.get_sql_and_params()
 
         with connection.connection.cursor(cursor_factory=DictCursor) as cursor:
             cursor.execute(sql_query, params)
             data = cursor.fetchall()
 
-            return [
-                {
-                    field.alias: field.parse_value(
-                        row[f"analytics_result_{field.alias}"]
-                    )
-                    for field in self.base_table._fields.values()
-                    if field.show_output
-                }
-                for row in data
-            ]
+            result = []
+            for row in data:
+                record = {}
+                for field in self._fields:
+                    field2 = self.base_table._fields[field.alias]
+                    if field.show_output:
+                        value = row[self._sql_alias(field.alias)]
+                        self._update_summary(field, value)
+                        record[field.alias] = field2.parse_value(value)
+                result.append(record)
+
+            return result
+
+    def _update_summary(self, field, value):
+        # value must to eval to True in order to not break on `None` and also ignore `0`
+        if value and field.function in [field.FUNCTION_SUM, field.FUNCTION_COUNT]:
+            self._summary[field.alias] += value
 
     def get_summary(self):
-        summary_self = PivotTable(self.table, self.info, is_summary=True)
-        summary = summary_self.get_records()
-        return summary[0]
-
-    def _sql_alias(self, user_alias):  # pragma: no cover
-        return f"analytics_pivot_{user_alias}"
+        if not self._summary:  # pragma: no cover
+            self.get_records()
+        return self._summary
```

### Comparing `caluma-8.0.0b9/caluma/caluma_analytics/schema.py` & `caluma-9.0.0/caluma/caluma_analytics/schema.py`

 * *Files 15% similar despite different names*

```diff
@@ -74,31 +74,33 @@
     summary = graphene.Field(AnalyticsRow)
 
     @staticmethod
     def resolve_records(table, info, *args, **kwargs):
         rows = [
             AnalyticsRow(
                 edges=[
-                    {"node": {"alias": alias, "value": val}}
-                    for alias, val in row.items()
+                    {"node": {"alias": alias, "value": row[alias]}}
+                    for alias in table.field_ordering
                 ]
             )
             for row in table.get_records()
         ]
         return rows
 
     @staticmethod
     def resolve_summary(table, info, *args, **kwargs):
         summary_row = table.get_summary()
-        return AnalyticsRow(
-            edges=[
-                {"node": {"alias": alias, "value": val}}
-                for alias, val in summary_row.items()
-            ]
-        )
+        if summary_row:
+            return AnalyticsRow(
+                edges=[
+                    {"node": {"alias": alias, "value": summary_row[alias]}}
+                    for alias in table.field_ordering
+                ]
+            )
+        return AnalyticsRow(edges=[])
 
 
 StartingObject = enum_type_from_field(
     "StartingObject",
     models.AnalyticsTable.starting_object,
     serializer_field=serializers.StartingObjectField,
 )
@@ -163,18 +165,14 @@
 
 
 class AnalyticsField(DjangoObjectType):
     meta = generic.GenericScalar()
     filters = graphene.List(String, required=False)
     function = AggregateFunction(required=False)
 
-    @classmethod
-    def get_queryset(cls, queryset, info):
-        return super().get_queryset(queryset, info).order_by("-created_at")
-
     class Meta:
         model = models.AnalyticsField
         interfaces = (relay.Node,)
         connection_class = CountableConnectionBase
         fields = "__all__"
 
 
@@ -200,20 +198,28 @@
 class RemoveAnalyticsField(Mutation):
     class Meta:
         serializer_class = serializers.RemoveAnalyticsFieldSerializer
         lookup_input_kwarg = "id"
         model_operations = ["update"]
 
 
+class ReorderAnalyticsFields(Mutation):
+    class Meta:
+        serializer_class = serializers.ReorderAnalyticsFieldSerializer
+        lookup_input_kwarg = "table"
+        model_operations = ["update"]
+
+
 class Mutation:
     save_analytics_table = SaveAnalyticsTable().Field()
     remove_analytics_table = RemoveAnalyticsTable().Field()
 
     save_analytics_field = SaveAnalyticsField().Field()
     remove_analytics_field = RemoveAnalyticsField().Field()
+    reorder_analytics_fields = ReorderAnalyticsFields().Field()
 
 
 class Query:
     all_analytics_tables = DjangoFilterConnectionField(
         AnalyticsTable,
         filterset_class=CollectionFilterSetFactory(
             filterset_class=filters.AnalyticsTableFilterSet,
```

### Comparing `caluma-8.0.0b9/caluma/caluma_analytics/serializers.py` & `caluma-9.0.0/caluma/caluma_analytics/serializers.py`

 * *Files 18% similar despite different names*

```diff
@@ -116,7 +116,33 @@
         instance.delete()
 
         return instance
 
     class Meta:
         fields = ["id"]
         model = models.AnalyticsField
+
+
+class TableFieldRelatedField(serializers.GlobalIDPrimaryKeyRelatedField):
+    def get_queryset(self):
+        table = self.parent.parent.instance
+        return table.fields.all()
+
+
+class ReorderAnalyticsFieldSerializer(serializers.ModelSerializer):
+    table = serializers.GlobalIDField(source="slug")
+    fields = TableFieldRelatedField(many=True)
+
+    def update(self, instance, validated_data):
+        for sort, analytic_field in enumerate(validated_data["fields"], start=1):
+            models.AnalyticsField.objects.filter(
+                table=instance, pk=analytic_field.pk
+            ).update(sort=sort)
+
+        return instance
+
+    class Meta:
+        model = models.AnalyticsTable
+        fields = [
+            "table",
+            "fields",
+        ]
```

### Comparing `caluma-8.0.0b9/caluma/caluma_analytics/simple_table.py` & `caluma-9.0.0/caluma/caluma_analytics/simple_table.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from __future__ import annotations  # self-referencing annotations
 
 import re
 from copy import deepcopy
 from datetime import datetime
 from decimal import Decimal
 from functools import cached_property, partial
+from hashlib import md5
 from typing import List, Optional
 
 from django.conf import settings
 from django.db import connection
-from django.utils import timezone
+from django.utils import timezone, translation
 from psycopg2.extras import DictCursor
 
 from caluma.caluma_form import models as form_models
 from caluma.caluma_workflow import models as workflow_models
 
 from . import models, sql
 
@@ -202,19 +203,21 @@
             source_path[-1] = self.meta_name
         return source_path
 
     def query_field(self):
         if self.meta_name:
             return sql.JSONExtractorField(
                 self.identifier,
+                self.identifier,
                 parent=self.parent.query_field() if self.parent else None,
                 json_key=self.meta_name,
             )
         return sql.NOOPField(
             self.identifier,
+            self.identifier,
             parent=self.parent.query_field() if self.parent else None,
         )
 
 
 class AttributeField(BaseField):
     """Extractor for regular table attributes.
 
@@ -229,31 +232,48 @@
         )
         self.is_date = is_date
 
     def is_leaf(self):
         return not self.is_date
 
     def is_value(self):
-        return True
+        # meta fields cannot be a value - they *contain* values
+        return self.identifier != "meta"
 
     def supported_functions(self):
+        if not self.is_value:  # pragma: no cover
+            # Non-value fields cannot have functions applied to them.
+            # This mainly applies to "meta" fields in this context
+            return []
+        elif self.identifier == "id" or self.identifier.endswith("_id"):
+            # Identifiers cannot have aggregate functions applied in a
+            # meaningful manner, except counts. Potentially, we *could"
+            # imagine some string functions being useful for slug identifiers,
+            # but we'll keep it simple for now
+            return [
+                models.AnalyticsField.FUNCTION_COUNT.upper(),
+                models.AnalyticsField.FUNCTION_VALUE.upper(),
+            ]
         return [
             models.AnalyticsField.FUNCTION_VALUE.upper(),
             models.AnalyticsField.FUNCTION_MAX.upper(),
             models.AnalyticsField.FUNCTION_MIN.upper(),
+            models.AnalyticsField.FUNCTION_COUNT.upper(),
         ]
 
     def query_field(self):
         if self.is_date and not self.required:
             return sql.NOOPField(
                 self.identifier,
+                self.identifier,
                 parent=self.parent.query_field() if self.parent else None,
             )
         return sql.AttrField(
             self.identifier,
+            self.identifier,
             parent=self.parent.query_field() if self.parent else None,
         )
 
     @cached_property
     def available_children(self):
         if self.is_date:
             # for FormAnswerField, the identifier is the question slug,
@@ -323,14 +343,15 @@
 
     def supported_functions(self):
         return []
 
     def query_field(self):
         return sql.JoinField(
             self.identifier,
+            self.identifier,
             table=self.visibility_source.work_items(),
             outer_ref=("id", "case_id"),
             filters=[f"task_id = '{self.task_slug}'"],
             order_by=self._order_by(),
             parent=self.parent.query_field() if self.parent else None,
         )
 
@@ -365,14 +386,19 @@
                 parent=self,
                 identifier="status",
                 visibility_source=self.visibility_source,
             ),
             "name": AttributeField(
                 parent=self, identifier="name", visibility_source=self.visibility_source
             ),
+            "document_form": FormInfoField(
+                parent=None,
+                identifier="form",
+                visibility_source=self.visibility_source,
+            ),
         }
 
         wi_forms = form_models.Form.objects.filter(
             documents__work_item__isnull=False
         ).distinct()
 
         form_fields = {
@@ -383,44 +409,162 @@
             )
             for form in wi_forms
         }
 
         return {**direct_fields, **form_fields}
 
 
+class CaseField(BaseField):
+    """Field that provides access to a case's data."""
+
+    def __init__(
+        self,
+        parent,
+        identifier,
+        visibility_source,
+        is_family=False,
+    ):
+        super().__init__(
+            parent=parent, identifier=identifier, visibility_source=visibility_source
+        )
+
+        # TODO translate?
+        self.label = "Case family" if is_family else "Case"
+        self.is_family = is_family
+
+    def is_leaf(self):
+        return False
+
+    def is_value(self):
+        return False
+
+    def supported_functions(self):
+        return []
+
+    def query_field(self):
+        outer_ref_left = "case_id"
+        if self.is_family:
+            outer_ref_left = "family_id"
+        return sql.JoinField(
+            self.identifier,
+            self.identifier,
+            table=self.visibility_source.cases(),
+            outer_ref=(outer_ref_left, "id"),
+            parent=self.parent.query_field() if self.parent else None,
+        )
+
+    @cached_property
+    def available_children(self):
+        direct_fields = {
+            "meta": MetaField(
+                parent=self,
+                identifier="meta",
+                label="Meta",
+                visibility_source=self.visibility_source,
+            ),
+            "id": AttributeField(
+                parent=self,
+                identifier="id",
+                is_date=False,
+                visibility_source=self.visibility_source,
+            ),
+            "closed_at": AttributeField(
+                parent=self,
+                identifier="closed_at",
+                is_date=True,
+                visibility_source=self.visibility_source,
+            ),
+            "created_at": AttributeField(
+                parent=self,
+                identifier="created_at",
+                is_date=True,
+                visibility_source=self.visibility_source,
+            ),
+            "status": AttributeField(
+                parent=self,
+                identifier="status",
+                visibility_source=self.visibility_source,
+            ),
+            "document[*]": FormDocumentField(
+                parent=self,
+                identifier="document[*]",
+                visibility_source=self.visibility_source,
+            ),
+        }
+
+        if not self.is_family:
+            direct_fields["family"] = CaseField(
+                parent=self,
+                identifier="family",
+                visibility_source=self.visibility_source,
+                is_family=True,
+            )
+
+        case_forms = form_models.Form.objects.filter(
+            documents__case__isnull=False
+        ).distinct()
+
+        form_fields = {
+            f"document[{form.slug}]": FormDocumentField(
+                identifier=f"document[{form.slug}]",
+                parent=self,
+                visibility_source=self.visibility_source,
+            )
+            for form in case_forms
+        }
+
+        tasks = workflow_models.Task.objects.all()
+
+        workitem_fields = {
+            f"workitem[{task.slug},{selector}]": WorkItemField(
+                identifier=f"workitem[{task.slug},{selector}]",
+                parent=self,
+                visibility_source=self.visibility_source,
+            )
+            for selector in ["first", "last", "firstclosed", "lastclosed"]
+            for task in tasks
+        }
+
+        return {**direct_fields, **form_fields, **workitem_fields}
+
+
 class FormDocumentField(BaseField):
     """Field that provides access to a form's data."""
 
     def __init__(
         self, parent, identifier, visibility_source, subform_level=0, form_slug=None
     ):
         super().__init__(
             parent=parent, identifier=identifier, visibility_source=visibility_source
         )
 
         self.form_slug = form_slug if form_slug else self.path_args()[0]
+        if self.form_slug == "*":
+            self.form_slug = None
 
-        # subform level is used so we can have the "path" as it is presented
+        # subform level is used, so we can have the "path" as it is presented
         # to the user (our `location`) separate from where the corresponding
         # `Answer` is found (remember, answers of questions in subforms are
         # NOT put into sub-documents according to hierarchy, but stored in a
         # single document!)
         self.subform_level = subform_level
 
     def query_field(self):
         # Only for top-level form do we need a Join field.
-        # The "sub-forms"' answers are all on the same document,
+        # The "sub-forms" answers are all on the same document,
         # thus for those we return a NOOP field.
         if self.subform_level == 0:
             return sql.JoinField(
                 self.identifier,
+                self.identifier,
                 table=self.visibility_source.documents(),
                 outer_ref=("document_id", "id"),
-                filters=[f"form_id = '{self.form_slug}'"],
+                filters=[f"form_id = '{self.form_slug}'"] if self.form_slug else [],
                 parent=self.parent.query_field() if self.parent else None,
+                disable_distinct_on=True,
             )
         # else - we just return the field from our "virtual" parent
         return self.parent.query_field()
 
     def is_leaf(self):
         return False
 
@@ -428,17 +572,31 @@
         return False
 
     def supported_functions(self):
         return []
 
     @cached_property
     def available_children(self):
-        form = form_models.Form.objects.get(pk=self.form_slug)
-        questions = form.questions.all().exclude(type=form_models.Question.TYPE_TABLE)
+        if self.form_slug:
+            form = form_models.Form.objects.get(pk=self.form_slug)
+            questions = form.questions.all().exclude(
+                type=form_models.Question.TYPE_TABLE
+            )
+        else:
+            questions = self.visibility_source.questions(as_queryset=True).exclude(
+                type=form_models.Question.TYPE_TABLE
+            )
+
         children = {}
+        if self.subform_level == 0:
+            children["caluma_form"] = FormInfoField(
+                parent=self,
+                identifier="caluma_form",
+                visibility_source=self.visibility_source,
+            )
 
         for question in questions:
             qf = self._question_field(question)
             if qf:
                 children[question.pk] = qf
         return children
 
@@ -450,14 +608,15 @@
         if question.type in (
             question.TYPE_INTEGER,
             question.TYPE_FLOAT,
             question.TYPE_TEXT,
             question.TYPE_TEXTAREA,
             question.TYPE_CHOICE,
             question.TYPE_DYNAMIC_CHOICE,
+            question.TYPE_CALCULATED_FLOAT,
         ):
             return FormAnswerField(
                 parent=self,
                 identifier=question.slug,
                 attr_name="value",
                 subform_level=self.subform_level,
                 visibility_source=self.visibility_source,
@@ -488,28 +647,29 @@
     This is used only for the "Documents" starting object, as here,
     the main table is already the "document".
     """
 
     def query_field(self):
         return sql.NOOPField(
             self.identifier,
+            self.identifier,
             parent=self.parent.query_field() if self.parent else None,
         )
 
 
 class FormAnswerField(AttributeField):
     """Represents access to an answer within a form."""
 
     def __init__(self, parent, identifier, attr_name, subform_level, **kwargs):
         super().__init__(parent=parent, identifier=identifier, **kwargs)
         self.subform_level = subform_level
         self.attr_name = attr_name
+        self._question = form_models.Question.objects.get(pk=self.identifier)
 
     def supported_functions(self):
-        question = form_models.Question.objects.get(pk=self.identifier)
         base_functions = [
             models.AnalyticsField.FUNCTION_VALUE.upper(),
             models.AnalyticsField.FUNCTION_COUNT.upper(),
         ]
         text_functions = [
             models.AnalyticsField.FUNCTION_MAX.upper(),
             models.AnalyticsField.FUNCTION_MIN.upper(),
@@ -523,38 +683,235 @@
         function_support = {
             form_models.Question.TYPE_CHOICE: text_functions,
             form_models.Question.TYPE_TEXT: text_functions,
             form_models.Question.TYPE_TEXTAREA: text_functions,
             form_models.Question.TYPE_DATE: text_functions,
             form_models.Question.TYPE_INTEGER: numeric_functions,
             form_models.Question.TYPE_FLOAT: numeric_functions,
+            form_models.Question.TYPE_CALCULATED_FLOAT: numeric_functions,
         }
 
-        return base_functions + function_support[question.type]
+        return base_functions + function_support[self._question.type]
 
     def query_field(self):
         # Only for top-level form do we need a Join field.
         # The "sub-forms"' answers are all on the same document,
         # thus for those we return a NOOP field.
         answer_join_field = sql.JoinField(
             identifier=self.identifier,
+            extract=self.identifier,
             table=self.visibility_source.answers(),
             # TODO: turn this into SQL parameter
             filters=[f""""question_id" = '{self.identifier}' """],
             outer_ref=("id", "document_id"),
             parent=self.parent.query_field() if self.parent else None,
         )
         value_field = sql.AttrField(
             identifier=self.attr_name,
+            extract=self.attr_name,
             parent=answer_join_field,
             filter_values=self.filters,
             answer_value_mode=(self.attr_name == "value"),
         )
         return value_field
 
+    def is_leaf(self):
+        if self._question.type == form_models.Question.TYPE_CHOICE:
+            return False
+        return super().is_leaf()
+
+    def is_value(self):
+        return (
+            self._question.type == form_models.Question.TYPE_CHOICE
+            or super().is_value()
+        )
+
+    @cached_property
+    def available_children(self):
+        if self._question.type == form_models.Question.TYPE_CHOICE:
+            return {
+                "label": ChoiceLabelField(
+                    parent=self,
+                    identifier="label",
+                    visibility_source=self.visibility_source,
+                )
+            }
+        return super().available_children
+
+
+class FormInfoField(BaseField):
+    """Represent information about a form (Name, slug)."""
+
+    def __init__(self, parent, identifier, *, visibility_source, **kwargs):
+        super().__init__(
+            parent=parent,
+            identifier=identifier,
+            visibility_source=visibility_source,
+            **kwargs,
+        )
+
+    def supported_functions(self):  # pragma: no cover
+        return []
+
+    def query_field(self):
+        return sql.JoinField(
+            identifier=self.identifier,
+            extract=self.identifier,
+            table=self.visibility_source.forms(),
+            filters=[],
+            outer_ref=("form_id", "slug"),
+            parent=self.parent.query_field() if self.parent else None,
+        )
+
+    def is_leaf(self):
+        return False
+
+    def is_value(self):
+        return False
+
+    @cached_property
+    def available_children(self):
+        return {
+            "name": LocalizedAttributeField(
+                parent=self,
+                identifier="name",
+                visibility_source=self.visibility_source,
+            ),
+            "slug": AttributeField(
+                parent=self,
+                identifier="slug",
+                is_date=False,
+                visibility_source=self.visibility_source,
+            ),
+        }
+
+
+class ChoiceLabelField(AttributeField):
+    def __init__(
+        self, parent, identifier, *, visibility_source, language=None, main_field=None
+    ):
+        super().__init__(
+            parent=parent, identifier=identifier, visibility_source=visibility_source
+        )
+        self.language = language
+        self._main_field = main_field
+
+    def is_leaf(self):
+        return bool(self.language)
+
+    def is_value(self):  # pragma: no cover
+        # without language, we return the default language as
+        # per request, so we can still "be" a value
+        return True
+
+    def source_path(self) -> List[str]:
+        """Return the full source path of this field as a list."""
+        fragment = (
+            [self._main_field.identifier, self.identifier]
+            if self._main_field
+            else [self.identifier]
+        )
+        return self.parent.source_path() + fragment if self.parent else fragment
+
+    def query_field(self):
+        # The label is in the choices table, so we need to join
+        # that one.
+        label_join_field = sql.JoinField(
+            identifier=self.identifier,
+            extract=self.identifier,
+            table=self.visibility_source.options(),
+            filters=[],
+            outer_ref=("value #>>'{}'", "slug"),  # noqa:P103
+            parent=self.parent.query_field() if self.parent else None,
+        )
+
+        language = self.language or translation.get_language()
+
+        value_field = sql.HStoreExtractorField(
+            "label",
+            "label",
+            parent=label_join_field,
+            hstore_key=language,
+        )
+
+        return value_field
+
+    @cached_property
+    def available_children(self):
+        if self.language:
+            return {}
+        return {
+            lang: ChoiceLabelField(
+                self.parent,
+                lang,
+                main_field=self,
+                visibility_source=self.visibility_source,
+                language=lang,
+            )
+            for lang, _ in settings.LANGUAGES
+        }
+
+
+class LocalizedAttributeField(AttributeField):
+    def __init__(
+        self, parent, identifier, *, visibility_source, language=None, main_field=None
+    ):
+        super().__init__(
+            parent=parent, identifier=identifier, visibility_source=visibility_source
+        )
+        self.language = language
+        self._main_field = main_field
+
+    def is_leaf(self):
+        return bool(self.language)
+
+    def is_value(self):  # pragma: no cover
+        # without language, we return the default language as
+        # per request, so we can still "be" a value
+        return True
+
+    def source_path(self) -> List[str]:
+        """Return the full source path of this field as a list."""
+        fragment = (
+            [self._main_field.identifier, self.identifier]
+            if self._main_field
+            else [self.identifier]
+        )
+        return self.parent.source_path() + fragment if self.parent else fragment
+
+    def query_field(self):
+        # The label is in the choices table, so we need to join
+        # that one.
+
+        language = self.language or translation.get_language()
+
+        value_field = sql.HStoreExtractorField(
+            "name",
+            "name",
+            parent=self.parent.query_field() if self.parent else None,
+            hstore_key=language,
+        )
+
+        return value_field
+
+    @cached_property
+    def available_children(self):
+        if self.language:
+            return {}
+        return {
+            lang: LocalizedAttributeField(
+                self.parent,
+                lang,
+                main_field=self,
+                visibility_source=self.visibility_source,
+                language=lang,
+            )
+            for lang, _ in settings.LANGUAGES
+        }
+
 
 class DateExtractorField(AttributeField):
     """Specialisation of attribute field: Extract a date part."""
 
     def __init__(self, parent, identifier, visibility_source, date_field, **kwargs):
         super().__init__(
             parent,
@@ -566,28 +923,29 @@
         self.date_field = date_field
 
     def supported_functions(self):
         return self._all_supported_functions()
 
     def query_field(self):
         return sql.DateExprField(
+            self.identifier,
             self.date_field,
             parent=self.parent.query_field() if self.parent else None,
             extract_part=self.identifier,
             filter_values=self.filters,
         )
 
     def parse_value(self, value):
         """Convert extracted date part to integer.
 
         This is necessary because not all supported postgres versions return the
         same datatype which leads to inconsistency. E.g versions < 12 returns a
         float while later versions return a decimal.
         """
-        return int(value)
+        return int(value) if value is not None else None
 
 
 class BaseStartingObject:
     """Base class for starting objects.
 
     Provides interface for listing the fields within the given starting
     object, and also supports Enum generation on the GraphQL side.
@@ -659,15 +1017,14 @@
             fields = self.get_field(prefix).available_children
         else:
             prefix = []
             fields = self.root_fields()
 
         output = {}
         for path, field in fields.items():
-
             output[".".join(prefix + [path])] = field
             for subpath, child in _children_at_depth(field, depth - 1):
                 output[".".join(prefix + [path] + subpath)] = child
         return output
 
     def root_fields(self):  # pragma: no cover
         """Return the root fields for this starting object.
@@ -719,14 +1076,19 @@
                 visibility_source=self.visibility_source,
             ),
             "id": AttributeField(
                 parent=None,
                 identifier="id",
                 visibility_source=self.visibility_source,
             ),
+            "document[*]": FormDocumentField(
+                identifier="document[*]",
+                parent=None,
+                visibility_source=self.visibility_source,
+            ),
         }
 
         case_forms = form_models.Form.objects.filter(
             documents__case__isnull=False
         ).distinct()
 
         form_fields = {
@@ -792,14 +1154,19 @@
                 visibility_source=self.visibility_source,
             ),
             "id": AttributeField(
                 parent=None,
                 identifier="id",
                 visibility_source=self.visibility_source,
             ),
+            "case": CaseField(
+                parent=None,
+                identifier="case",
+                visibility_source=self.visibility_source,
+            ),
         }
 
         workitem_forms = form_models.Form.objects.filter(
             documents__work_item__isnull=False
         ).distinct()
 
         form_fields = {
@@ -830,73 +1197,82 @@
             ),
             "meta": MetaField(
                 parent=None,
                 identifier="meta",
                 label="Meta",
                 visibility_source=self.visibility_source,
             ),
-            "form_id": AttributeField(
-                parent=None,
-                identifier="form_id",
-                is_date=False,
-                visibility_source=self.visibility_source,
-            ),
             "created_at": AttributeField(
                 parent=None,
                 identifier="created_at",
                 is_date=True,
                 visibility_source=self.visibility_source,
             ),
+            "caluma_form": FormInfoField(
+                parent=None,
+                identifier="caluma_form",
+                visibility_source=self.visibility_source,
+            ),
         }
 
         form_fields = {
             f"answers[{form.slug}]": DirectDocumentField(
                 identifier=f"answers[{form.slug}]",
                 parent=None,
                 visibility_source=self.visibility_source,
             )
             for form in form_models.Form.objects.all()
         }
 
         return {**direct_fields, **form_fields}
 
 
-class SimpleTable:
+class SQLAliasMixin:
+    def _sql_alias(self, user_alias):
+        """
+        Compose sql alias.
+
+        Returns f"{prefix}{alias}" by default. If this exceeds 63 bytes (limit by
+        postgresql), it returns f"{prefix}{md5_alias}"
+        """
+        prefix = "analytics_result_"
+        alias = f"{prefix}{user_alias}"
+        if len(alias.encode("utf-8")) > 63:
+            alias = f"{prefix}{md5(user_alias.encode('utf-8')).hexdigest()}"
+        return alias
+
+
+class SimpleTable(SQLAliasMixin):
     class _AnonymousInfo:
         """
         Pseudo GraphQL info object.
 
         Used for commandline access, so the commandline version
         can also invoke the visibilities.
         """
 
         context = {}
 
-    def __init__(self, table, info=_AnonymousInfo, is_summary=False):
+    def __init__(self, table, info=_AnonymousInfo):
         self.info = info
         self.table = table
         self.last_query = None
         self.last_query_params = None
-        self.is_summary = is_summary
 
         self.starting_object = BaseStartingObject.get_object(
             self.table.starting_object,
             self.info,
             disable_visibilities=self.table.disable_visibilities,
         )
 
         self.base_query = sql.Query(from_=self.starting_object.get_query())
 
     @cached_property
     def _fields(self):
         field_spec_qs = self.table.fields.all()
-        if self.is_summary:
-            field_spec_qs = field_spec_qs.exclude(
-                function=models.AnalyticsField.FUNCTION_VALUE
-            )
         # sort fields to join by length. This way, parent fields
         # will be already joined when their children get added, so
         # they will have the right alias.
         table_fields = sorted(field_spec_qs, key=lambda f: len(f.data_source))
 
         fields = {}
         for field_spec in table_fields:
@@ -909,27 +1285,34 @@
             # Filters must always be on the outermost (base) query,
             # as we're using LEFT JOINs to get at related data.
             self.base_query.add_field_filter(
                 self._sql_alias(field_spec.alias), field_spec.filters
             )
         return fields
 
+    @cached_property
+    def field_ordering(self):
+        return list(
+            self.table.fields.all()
+            .filter(show_output=True)
+            .values_list("alias", flat=True)
+        )
+
     def get_sql_and_params(self):
         """Return a list of records as specified in the given table config."""
 
         base_query = self.get_query_object()
 
         sql_query, params, _ = sql.QueryRender(base_query).as_sql(alias=None)
 
         self.last_query = sql_query
         self.last_query_params = params
         return sql_query, params
 
     def get_query_object(self):
-
         fields = self._fields
 
         step_queries = {}
         base_query = deepcopy(self.base_query)
 
         for alias, field in fields.items():
             query = base_query
@@ -946,32 +1329,26 @@
                 else:
                     query = step.annotate(query)
                     step_queries[cache_path] = query
 
         return base_query
 
     def get_records(self):
-
         sql_query, params = self.get_sql_and_params()
 
         with connection.connection.cursor(cursor_factory=DictCursor) as cursor:
             cursor.execute(sql_query, params)
             data = cursor.fetchall()
 
             return [
                 {
-                    field.alias: field.parse_value(
-                        row[f"analytics_result_{field.alias}"]
-                    )
+                    field.alias: field.parse_value(row[self._sql_alias(field.alias)])
                     for field in self._fields.values()
                     if field.show_output
                 }
                 for row in data
             ]
 
     def get_summary(self):
         # simple tables can't do summary, but we must implement
         # it as both table types share the same GQL interface
         return {}  # pragma: no cover
-
-    def _sql_alias(self, user_alias):
-        return f"analytics_result_{user_alias}"
```

### Comparing `caluma-8.0.0b9/caluma/caluma_analytics/sql.py` & `caluma-9.0.0/caluma/caluma_analytics/sql.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,36 @@
 from __future__ import annotations  # self-referencing annotations
 
 import hashlib
+import re
 import textwrap
 from dataclasses import dataclass, field
 from typing import Dict, List, Optional, Tuple, Union
 from uuid import uuid4
 
+import psycopg2.sql
 from django.db import connection
 from django.utils.text import slugify
 
 
 def _make_name(value, name_hint=None):
+    if name_hint:
+        name_hint = re.sub(r"[^a-zA-Z0-9_]", "_", name_hint)
     prefix = name_hint if name_hint else "p"
     length = 5 if name_hint else 12
 
     suffix = hashlib.md5(str(value).encode("utf-8")).hexdigest()
     return f"{prefix}_{suffix[:length]}"
 
 
+def quote_identifier(name):
+    name = name.replace("%", "%%")
+    return psycopg2.sql.Identifier(name).as_string(connection.connection)
+
+
 @dataclass
 class Query:
     """Represent an SQL query (might be a subquery).
 
     Note: The `from` specification might in turn again
     reference another Query object, thus building a subquery
     structure.
@@ -46,14 +55,18 @@
     with_queries: Dict[str, str] = field(
         default_factory=dict
     )  # with_queries are CTEs, used for referencing visibility-filtered tables
 
     is_plain_cte: bool = field(default=False)
     select_direct_only: bool = field(default=False)
 
+    @property
+    def outer_ref_alias(self):
+        return _make_name(self.outer_ref)
+
     def makeparam(self, value, name_hint=None):
         """Return a parameter name for the given value.
 
         The parameter's value is automatically registered and
         can then be used in the generated SQL.
 
         If you pass a name_hint, it is used as a prefix
@@ -104,34 +117,33 @@
         """
         if not filter_values:
             return
 
         filters_sql = ", ".join(
             [self.makeparam(val, f"flt_{alias}") for val in filter_values]
         )
-        self.filters.append(f"{alias} IN ({filters_sql})")
+        self.filters.append(f"{quote_identifier(alias)} IN ({filters_sql})")
 
     @classmethod
     def from_queryset(cls, queryset):
         """Take a Django queryset and represent it as a Query object.
 
         We will use this via CTE (WITH) statement to read data respecting
         the visibility rules as defined in Caluma.
         """
 
         # The queryset may "SELECT" columns (especially from JOINs) that
         # we're not interested in, as we're JOINing our stuff by ourselves.
         # To avoid ambiguity, we select ONLY what's in the main model's
         # field list
-        q = connection.ops.quote_name
         field_list = ",  \n".join(
             [
-                q(queryset.model._meta.db_table)
+                quote_identifier(queryset.model._meta.db_table)
                 + "."
-                + q(field.db_column or field.attname)
+                + quote_identifier(field.db_column or field.attname)
                 for field in queryset.model._meta.concrete_fields
             ]
         )
 
         # Unfortunately, queryset.query.sql_with_params() seems to
         # ignore queryset.only() specification, so we must do it ourselves.
         # Ugly AF, but don't see how else to do it for now...
@@ -140,25 +152,31 @@
 
         wrapped_sql = f"""SELECT {field_list}\nFROM\n      {from_part} -- qs ref\n"""
 
         name = _make_name(value=wrapped_sql, name_hint=queryset.model.__name__.lower())
         self = cls(from_=name, is_plain_cte=True)
 
         # Django does positional parameters, we do named params. Convert them
-        named_params = [self.makeparam(param) for param in params]
+        # In some cases, the SELECT list may contain params, which we don't
+        # use here and thus need to discard
+        discard_placeholders = len(re.findall("(%s)", select))
+        used_params = params[discard_placeholders:]
+
+        named_params = [self.makeparam(param) for param in used_params]
         final_sql = wrapped_sql % tuple(named_params)
 
         self.with_queries[name] = final_sql
 
         return self
 
 
 @dataclass
 class Field:
     identifier: str
+    extract: str
     alias: Optional[str] = field(default=None)
     parent: Optional[Field] = field(default=None)
     filter_values: Optional[List[str]] = field(default=None)
     answer_value_mode: bool = field(default=False)
     _activated_query: Optional[Query] = field(default=None)
 
     def path_from_root(self):
@@ -191,76 +209,95 @@
 
         self._activated_query = query
         query.select.append((self.expr(query), self._alias()))
         return query
 
     def expr(self, query):
         # TODO: should the table alias be prefixed in all field expr()s?
-        alias = query.self_alias()
+        alias = quote_identifier(query.self_alias())
+        extract = quote_identifier(self.extract)
         if self.answer_value_mode:
             # Caluma form answers are in a JSON field named "value", from where
             # we need to extract the actual value, otherwise, for strings, we
             # would get the quoted version back
             extractor_op = "#>>'{}'"  # noqa
-            return f"({alias}.{self.identifier} {extractor_op})"
-        return f"{alias}.{self.identifier}"
+            return f"({alias}.{extract} {extractor_op})"
+        return f"{alias}.{extract}"
 
 
 @dataclass
 class DateExprField(AttrField):
     extract_part: Optional[str] = field(default=None)
 
     def expr(self, query):
-        q_id = connection.ops.quote_name(self.identifier)
-        return f"EXTRACT({self.extract_part} FROM {q_id})"
+        extract = quote_identifier(self.extract)
+        return f"EXTRACT({self.extract_part} FROM {extract})"
 
 
 @dataclass
 class JSONExtractorField(AttrField):
     json_key: Optional[str] = field(default=None)
 
     def expr(self, query):
         key_param = query.makeparam(self.json_key)
-        q_id = connection.ops.quote_name(self.identifier)
-        self_alias = query.self_alias()
+        extract = quote_identifier(self.extract)
+        self_alias = quote_identifier(query.self_alias())
         # Extract text from JSON field, so that it comes from the DB
         # as actual text
         extractor_op = "#>>'{}'"  # noqa
-        return f"""(({self_alias}.{q_id} -> {key_param}) {extractor_op})"""
+        return f"""(({self_alias}.{extract} -> {key_param}) {extractor_op})"""
+
+
+@dataclass
+class HStoreExtractorField(AttrField):
+    hstore_key: Optional[str] = field(default=None)
+
+    def expr(self, query):
+        key_param = query.makeparam(self.hstore_key)
+        extract = quote_identifier(self.extract)
+        self_alias = quote_identifier(query.self_alias())
+        # Extract text from HStore field, so that it comes from the DB
+        # as actual text
+        return f"""({self_alias}.{extract} -> {key_param})"""
 
 
 @dataclass
 class JoinField(Field):
     table: Optional[Union[str, Query]] = field(default=None)
     filters: List[str] = field(default_factory=list)
     order_by: List[str] = field(default_factory=list)
     outer_ref: Optional[Tuple[str, str]] = field(
         default=None
     )  # name_in_outer -> name_in_inner
+    disable_distinct_on: bool = field(default=False)
 
     def annotate(self, query: Query):
         if self._activated_query:  # pragma: no cover (safeguard)
             return self._activated_query
 
         self._activated_query = Query(
             from_=self.table,
             # distinct_on is the inner part of the outer_ref
-            distinct_on=self.outer_ref[1],
+            distinct_on=None if self.disable_distinct_on else self.outer_ref[1],
             filters=self.filters,
             outer_ref=self.outer_ref,
             order_by=self.order_by,
             # limit=1,
         )
 
-        outer_ref, inner_ref = self.outer_ref
+        outer_ref, _ = self.outer_ref
+        quoted_outer_ref_alias = quote_identifier(self._activated_query.outer_ref_alias)
 
         query.joins.append(
             (
                 self._activated_query,
-                f'{query.self_alias()}.{outer_ref} = "{self._activated_query.outer_alias()}".{inner_ref}',
+                (
+                    f"{query.self_alias()}.{outer_ref} = "
+                    f'"{self._activated_query.outer_alias()}".{quoted_outer_ref_alias}'
+                ),
             )
         )
         return self._activated_query
 
 
 class QueryRender:
     """Render a Query structure into actual SQL.
@@ -271,14 +308,15 @@
 
     def __init__(self, query: Query, is_subquery=False, indent: int = 0):
         self._indent = indent
         self.query = query
         self.collected_params = {}
         self.with_queries = {}
         self.is_subquery = is_subquery
+        self.outer_ref_alias = None
 
     def _collect_params(self, query):
         params = query.params.copy()
         if isinstance(query.from_, Query):
             params.update(self._collect_params(query.from_))
         return params
 
@@ -378,34 +416,36 @@
             return f"WHERE {filter_sql}"
         return ""
 
     def _field_list(self):
         # we always need to select everything, even from subqueries
         fields = [
             # First, the direct fields
-            f'''{expr} AS "{alias}"'''
+            f"""{expr} AS {quote_identifier(alias)}"""
             for expr, alias in self.query.select
         ]
         if self.query.outer_ref:
             _, inner = self.query.outer_ref
-            fields.append(f'"{inner}"')
+            quoted_inner = quote_identifier(inner)
+            quoted_alias = quote_identifier(self.query.outer_ref_alias)
+            fields.append(f"{quoted_inner} AS {quoted_alias}")
 
         # The subquery fields are already aliased, so no need
         # to re-alias them
         def _collect(q):
             for _, alias in q.select:
-                yield f'"{alias}"'
+                yield f"{quote_identifier(alias)}"
             for sub_q, _ in q.joins:
                 yield from _collect(sub_q)
 
         # Normally, we take all the "selects" from the inner queries and
-        # pass them further on. However in aggregate queries, this is not
+        # pass them further on. However, in aggregate queries, this is not
         # desired, as any unused field will lead to an SQL error (fields
         # MUST be used in aggregates or group by, which may not be desired).
-        # Thus we allow the query to specify "select direct only", which means
+        # Thus, we allow the query to specify "select direct only", which means
         # we do not pass on any selected fields from inner queries / joins
         # as we usually would.
         if not self.query.select_direct_only:
             for join, _ in self.query.joins:
                 fields.extend(_collect(join))
 
         return ",\n       ".join(fields)
@@ -430,15 +470,14 @@
 
         # Take any CTEs from the subquery and apply them to "us"
         self.with_queries.update(render.with_queries)
 
         return sql, params, alias
 
     def _from_list(self):
-
         from_sql, from_params, from_alias = self._join_source(self.query.from_)
         self.collected_params.update(from_params)
         self.with_queries.update(self.query.with_queries)
 
         sources = [(from_sql, from_alias, "")]
 
         for tbl, cond in self.query.joins:
```

### Comparing `caluma-8.0.0b9/caluma/caluma_analytics/visibility.py` & `caluma-9.0.0/caluma/caluma_analytics/visibility.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,18 +4,21 @@
 from . import sql
 
 
 def qs_method_factory(node_cls, model_cls=None):
     if not model_cls:
         model_cls = node_cls._meta.model
 
-    def method(self):
+    def method(self, as_queryset=False):
         queryset = model_cls.objects.all()
         if not self.is_disabled:
             queryset = node_cls.get_queryset(queryset, self.info)
+
+        if as_queryset:
+            return queryset
         return sql.Query.from_queryset(queryset)
 
     method.__doc__ = f"""
     Return an analytics Query object for {model_cls.__name__}.
 
     The query object contains CTE representing the visibility rules
     as defined in Caluma's settings for {model_cls.__name__}.
@@ -29,7 +32,10 @@
         self.info = info
         self.is_disabled = is_disabled
 
     cases = qs_method_factory(workflow_schema.Case)
     work_items = qs_method_factory(workflow_schema.WorkItem)
     documents = qs_method_factory(form_schema.Document)
     answers = qs_method_factory(form_schema.Answer, form_models.Answer)
+    options = qs_method_factory(form_schema.Option, form_models.Option)
+    forms = qs_method_factory(form_schema.Form, form_models.Form)
+    questions = qs_method_factory(form_schema.Question, form_models.Question)
```

### Comparing `caluma-8.0.0b9/caluma/caluma_core/apps.py` & `caluma-9.0.0/caluma/caluma_core/apps.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b9/caluma/caluma_core/conftest.py` & `caluma-9.0.0/caluma/caluma_core/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -279,14 +279,15 @@
 @pytest.fixture
 def minio_mock_read_error(minio_mock, mocker):
     """Produce exception when downloading file or stat-ing object.
 
     This scenario might occur when there is a internal minio issue or if a
     previous upload isn't successful (which doesn't issue exception).
     """
+
     # raise exception instead of handling request
     def download_side_effect(*args, **kwargs):  # pragma: no cover
         raise requests.exceptions.RequestException("GET request failed")
 
     def stat_side_effect(*args, **kwargs):
         raise Exception("stat_object failed")
 
@@ -312,14 +313,15 @@
 
 @pytest.fixture
 def minio_mock_write_error(minio_mock, mocker):
     """Produce exception when uploading file.
 
     This scenario might occur when there is a internal minio issue.
     """
+
     # raise exception instead of handling request
     def upload_side_effect(*args, **kwargs):
         raise requests.exceptions.RequestException("PUT request failed")
 
     # determine fixed UUID to be used during tests
     uuid = "7c5ad424-e351-4db8-ba37-bbace45d0e0f"
     mocker.patch("uuid.uuid4", return_value=uuid)
@@ -352,12 +354,12 @@
 
 
 @pytest.fixture
 def roll_back_migrations():
     """Roll back database migrations to ensure unapplied migrations exist."""
     # undo applied migrations for app contenttypes
     management.call_command("migrate", "contenttypes", "zero")
-
-    yield
-
-    # re-apply migrations for app contenttypes
-    management.call_command("migrate", "contenttypes")
+    try:
+        yield
+    finally:
+        # re-apply migrations for app contenttypes
+        management.call_command("migrate", "contenttypes")
```

### Comparing `caluma-8.0.0b9/caluma/caluma_core/events.py` & `caluma-9.0.0/caluma/caluma_core/events.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import inspect
 import logging
 from functools import wraps
-from warnings import warn
 
 logger = logging.getLogger(__name__)
 
 
 class SignalHandlingError(RuntimeError):
     def __init__(self, exceptions, *args, **kwargs):
         self.caught_exceptions = exceptions
@@ -13,19 +12,14 @@
         super().__init__(*args, **kwargs)
 
     def __str__(self):
         return ", ".join([str(e) for e in self.caught_exceptions])
 
 
 def on(event, raise_exception=False, *args, **kwargs):
-    deprecation_reason = getattr(event, "_deprecation_reason", None)
-
-    if deprecation_reason:  # pragma: no cover
-        warn(deprecation_reason, DeprecationWarning)
-
     def _decorator(func):
         func._raise_exception = raise_exception
 
         if isinstance(event, (list, tuple)):
             for e in event:
                 e.connect(func, **kwargs)
         else:
```

### Comparing `caluma-8.0.0b9/caluma/caluma_core/filters.py` & `caluma-9.0.0/caluma/caluma_core/filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,15 +152,14 @@
     collection_name = f"{filterset_class.__name__}Collection"
 
     # The field class.
     custom_field_class = type(field_class_name, (CompositeFieldClass,), {})
 
     @convert_form_field.register(custom_field_class)
     def convert_field(field):
-
         registry = get_global_registry()
         converted = registry.get_converted_field(field)
         if converted:
             return converted
 
         _filter_coll = filterset_class()
 
@@ -357,14 +356,24 @@
         label="Only return entries created before the given DateTime (exclusive)",
     )
     created_after = DateTimeFilter(
         field_name="created_at",
         lookup_expr="gte",
         label="Only return entries created at or after the given DateTime (inclusive)",
     )
+    modified_before = DateTimeFilter(
+        field_name="modified_at",
+        lookup_expr="lt",
+        label="Only return entries modified before the given DateTime (exclusive)",
+    )
+    modified_after = DateTimeFilter(
+        field_name="modified_at",
+        lookup_expr="gte",
+        label="Only return entries modified at or after the given DateTime (inclusive)",
+    )
 
 
 class JSONLookupMode(Enum):
     EXACT = "exact"
     STARTSWITH = "startswith"
     CONTAINS = "contains"
     ICONTAINS = "icontains"
```

### Comparing `caluma-8.0.0b9/caluma/caluma_core/forms.py` & `caluma-9.0.0/caluma/caluma_core/forms.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b9/caluma/caluma_core/health_checks.py` & `caluma-9.0.0/caluma/caluma_core/health_checks.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b9/caluma/caluma_core/jexl.py` & `caluma-9.0.0/caluma/caluma_core/jexl.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b9/caluma/caluma_core/management/commands/cleanup_history.py` & `caluma-9.0.0/caluma/caluma_core/management/commands/cleanup_history.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b9/caluma/caluma_core/management/commands/dump_caluma_config.py` & `caluma-9.0.0/caluma/caluma_core/management/commands/dump_caluma_config.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b9/caluma/caluma_core/management/commands/migrate.py` & `caluma-9.0.0/caluma/caluma_core/management/commands/migrate.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b9/caluma/caluma_core/management/commands/migrate_to_prefixed_apps.py` & `caluma-9.0.0/caluma/caluma_core/management/commands/migrate_to_prefixed_apps.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b9/caluma/caluma_core/models.py` & `caluma-9.0.0/caluma/caluma_core/models.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b9/caluma/caluma_core/mutation.py` & `caluma-9.0.0/caluma/caluma_core/mutation.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,15 +115,15 @@
         abstract = True
 
     # will be set in caluma_core.AppConfig.ready hook, see apps.py
     # to avoid recursive import error
     permission_classes = None
 
     @classmethod
-    def __init_subclass_with_meta__(
+    def __init_subclass_with_meta__(  # noqa: C901
         cls,
         lookup_field=None,
         lookup_input_kwarg=None,
         serializer_class=None,
         model_class=None,
         model_operations=None,
         fields=(),
@@ -150,14 +150,25 @@
         if lookup_field is None and model_class:
             lookup_field = model_class._meta.pk.name
         if lookup_input_kwarg is None:
             lookup_input_kwarg = lookup_field
 
         input_fields = fields_for_serializer(serializer, fields, exclude, is_input=True)
 
+        if hasattr(cls, "Input"):
+            # Allow input type override in case the serializer fields cannot
+            # define exactly what we need
+            input_obj = cls.Input()
+            explicit_inputs = [
+                name for name in dir(input_obj) if not name.startswith("_")
+            ]
+            for name in explicit_inputs:
+                input_type = getattr(input_obj, name)
+                input_fields[name] = input_type
+
         if return_field_name is None:
             model_name = model_class.__name__
             return_field_name = model_name[:1].lower() + model_name[1:]
 
         if not return_field_type:
             registry = get_global_registry()
             return_field_type = registry.get_type_for_model(model_class)
@@ -255,15 +266,14 @@
         # also see https://github.com/graphql-python/graphql-core/pull/204
         # potentially split each validation error into on GraphQL error
         serializer.is_valid(raise_exception=True)
         return cls.perform_mutate(serializer, info)
 
     @classmethod
     def perform_mutate(cls, serializer, info):
-
         obj = serializer.save()
         kwargs = {}
         if cls._meta.return_field_name:
             kwargs[cls._meta.return_field_name] = obj
         return cls(**kwargs)
 
     @classmethod
```

### Comparing `caluma-8.0.0b9/caluma/caluma_core/ordering.py` & `caluma-9.0.0/caluma/caluma_core/ordering.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b9/caluma/caluma_core/pagination.py` & `caluma-9.0.0/caluma/caluma_core/pagination.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b9/caluma/caluma_core/permissions.py` & `caluma-9.0.0/caluma/caluma_core/permissions.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b9/caluma/caluma_core/relay.py` & `caluma-9.0.0/caluma/caluma_core/relay.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b9/caluma/caluma_core/serializers.py` & `caluma-9.0.0/caluma/caluma_core/serializers.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b9/caluma/caluma_core/types.py` & `caluma-9.0.0/caluma/caluma_core/types.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b9/caluma/caluma_core/validations.py` & `caluma-9.0.0/caluma/caluma_core/validations.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b9/caluma/caluma_core/views.py` & `caluma-9.0.0/caluma/caluma_core/views.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b9/caluma/caluma_core/visibilities.py` & `caluma-9.0.0/caluma/caluma_core/visibilities.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b9/caluma/caluma_data_source/data_source_handlers.py` & `caluma-9.0.0/caluma/caluma_data_source/data_source_handlers.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,17 +49,17 @@
             if isinstance(ds.info, dict)
             else ds.info,
         )
         for ds in data_source_classes
     ]
 
 
-def get_data_source_data(user, name):
+def get_data_source_data(user, name, question, context):
     data_sources = get_data_sources(dic=True)
     if name not in data_sources:
         raise DataSourceException(f"No data_source found for name: {name}")
 
-    raw_data = data_sources[name]().try_get_data_with_fallback(user)
+    raw_data = data_sources[name]().try_get_data_with_fallback(user, question, context)
     if not is_iterable_and_no_string(raw_data):
         raise DataSourceException(f"Failed to parse data from source: {name}")
 
     return [Data(d) for d in raw_data]
```

### Comparing `caluma-8.0.0b9/caluma/caluma_data_source/data_sources.py` & `caluma-9.0.0/caluma/caluma_data_source/data_sources.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,17 +10,18 @@
     """Basic data source class to be extended by any data source implementation.
 
     The `get_data`-method should return an iterable. This iterable can contain strings,
     ints, floats and also iterables. Those contained iterables can consist of maximally
     two items. The first will be used for the option name, the second one for it's
     value. If only one value is provided, this value will also be used as choice name.
 
-    The `validate_answer_value`-method checks if each value in `self.get_data(user)` equals the value
-    of the parameter `value`. If this is correct the method returns the label as a String
-    and otherwise the method returns `False`.
+    The `validate_answer_value`-method checks if each value in
+    `self.get_data(user, question, context)` equals the value of the parameter
+    `value`. If this is correct the method returns the label as a String and
+    otherwise the method returns `False`.
 
     Examples:
         [['my-option', {"en": "english description", "de": "deutsche Beschreibung"}, ...]
         [['my-option', "my description"], ...]
         ['my-option', ...]
         [['my-option'], ...]
 
@@ -36,32 +37,32 @@
     ... import requests
     ...
     ...
     ... class CustomDataSource(BaseDataSource):
     ...     info = 'User choices from "someapi"'
     ...
     ...     @data_source_cache(timeout=3600)
-    ...     def get_data(self, user):
+    ...     def get_data(self, user, question, context):
     ...         response = requests.get(f"https://someapi/?user={user.username}")
     ...         return [result["value"] for result in response.json()["results"]]
     ```
 
     """
 
     info = None
     default = None
 
     def __init__(self):
         pass
 
-    def get_data(self, user):  # pragma: no cover
+    def get_data(self, user, question, context):  # pragma: no cover
         raise NotImplementedError()
 
-    def validate_answer_value(self, value, document, question, user):
-        for data in self.get_data(user):
+    def validate_answer_value(self, value, document, question, user, context):
+        for data in self.get_data(user, question, context):
             label = data
             if is_iterable_and_no_string(data):
                 label = data[-1]
                 data = data[0]
             if str(data) == value:
                 if not isinstance(label, dict):
                     label = str(label)
@@ -69,17 +70,17 @@
         dynamic_option = DynamicOption.objects.filter(
             document=document, question=question, slug=value
         ).first()
         if dynamic_option:
             return dynamic_option.label
         return False
 
-    def try_get_data_with_fallback(self, user):
+    def try_get_data_with_fallback(self, user, question, context):
         try:
-            new_data = self.get_data(user)
+            new_data = self.get_data(user, question, context)
         except Exception as e:
             logger.exception(
                 f"Executing {type(self).__name__}.get_data() failed:"
                 f"{e}\n Using default data."
             )
             if self.default is None:
                 raise e
```

### Comparing `caluma-8.0.0b9/caluma/caluma_form/api.py` & `caluma-9.0.0/caluma/caluma_form/api.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b9/caluma/caluma_form/domain_logic.py` & `caluma-9.0.0/caluma/caluma_form/domain_logic.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Optional
 
 from django.db import transaction
 from django.db.models import Q
 from rest_framework.exceptions import ValidationError
 
 from caluma.caluma_core.models import BaseModel
+from caluma.caluma_core.relay import extract_global_id
 from caluma.caluma_form import models, validators
 from caluma.caluma_user.models import BaseUser
 from caluma.utils import update_model
 
 
 class BaseLogic:
     @staticmethod
@@ -38,24 +39,78 @@
 class SaveAnswerLogic:
     @classmethod
     def get_new_answer(cls, data, user, answer):
         validated_data = cls.pre_save(
             cls.validate_for_save(data, user, answer=answer, origin=True)
         )
 
+        files = validated_data.pop("files", None)
         if answer is None:
             answer = cls.create(validated_data, user)
         else:
             answer = cls.update(answer, validated_data, user)
 
+        # FILES type needs a bit more work due to the reverse
+        # relation of file -> answer
+        if answer.question.type == models.Question.TYPE_FILES:
+            if files is None:
+                raise ValidationError("Files input must be a list")
+            cls.update_answer_files(answer, files)
+
         return cls.post_save(answer)
 
+    @classmethod
+    def update_answer_files(cls, answer: models.Answer, files: list):
+        """Update the files of a "FILES" answer.
+
+        The files parameter is expected to be a list of dicts, where
+        each entry has a "name" (the file name), and optionally an "id"
+        for the case when the given file already exists.
+        """
+        if not files:
+            files = []
+
+        updated = []
+
+        for file_ in files:
+            file_id = extract_global_id(file_["id"]) if "id" in file_ else None
+            file_name = file_["name"]
+            file_model = (
+                answer.files.filter(pk=file_id).first()
+                if file_id
+                else models.File(answer=answer, name=file_name)
+            )
+            if not file_model:
+                # Client wants to update a file that doesn't exist anymore.
+                # Reject call - this is an inconsistency as either
+                # the file was never created, or was deleted in the mean
+                # time.
+                raise ValidationError(
+                    f"File with id={file_id} for given answer not found"
+                )
+
+            if file_model.name != file_name and file_id:
+                # Renaming existing file
+                file_model.rename(file_name)
+                file_model.save()
+            elif not file_id:
+                # New file
+                file_model.save()
+            updated.append(file_model.pk)
+
+        for file in answer.files.exclude(pk__in=updated):
+            file.delete()
+
     @staticmethod
     def validate_for_save(
-        data: dict, user: BaseUser, answer: models.Answer = None, origin: bool = False
+        data: dict,
+        user: BaseUser,
+        answer: models.Answer = None,
+        origin: bool = False,
+        data_source_context: dict = None,
     ) -> dict:
         question = data["question"]
 
         # Save empty answer by omitting the value property since graphql-core
         # doesn't allow `null` literals yet
         if "value" not in data:
             data["value"] = None
@@ -64,90 +119,86 @@
         if question.type == models.Question.TYPE_TABLE and not data.get("documents"):
             data["documents"] = (
                 models.Document.objects.filter(pk__in=data["value"])
                 if data["value"]
                 else models.Document.objects.none()
             )
             del data["value"]
-        elif question.type == models.Question.TYPE_FILE and not data.get("file"):
-            data["file"] = data["value"]
+        elif question.type == models.Question.TYPE_FILES and not data.get("files"):
+            data["files"] = data["value"]
             del data["value"]
         elif question.type == models.Question.TYPE_DATE and not data.get("date"):
             data["date"] = data["value"]
             del data["value"]
 
         validators.AnswerValidator().validate(
-            **data, user=user, instance=answer, origin=origin
+            **data,
+            user=user,
+            instance=answer,
+            origin=origin,
+            data_source_context=data_source_context,
         )
 
         return data
 
     @staticmethod
     def pre_save(validated_data: dict) -> dict:
         # TODO emit events
         return validated_data
 
     @staticmethod
     def post_save(answer: models.Answer) -> models.Answer:
         # TODO emit events
         return answer
 
-    @staticmethod
+    @classmethod
     @transaction.atomic
-    def create(validated_data: dict, user: Optional[BaseUser] = None) -> models.Answer:
-        if validated_data["question"].type == models.Question.TYPE_FILE:
-            validated_data = __class__.set_file(validated_data)
-
+    def create(
+        cls, validated_data: dict, user: Optional[BaseUser] = None
+    ) -> models.Answer:
         if validated_data["question"].type == models.Question.TYPE_TABLE:
             documents = validated_data.pop("documents")
 
+        files = validated_data.pop("files", None)
         answer = BaseLogic.create(models.Answer, validated_data, user)
 
+        if validated_data["question"].type == models.Question.TYPE_FILES:
+            cls.update_answer_files(answer, files)
+
         if answer.question.type == models.Question.TYPE_TABLE:
             answer.create_answer_documents(documents)
 
         return answer
 
-    @staticmethod
+    @classmethod
     @transaction.atomic
-    def update(answer, validated_data, user: Optional[BaseUser] = None):
+    def update(cls, answer, validated_data, user: Optional[BaseUser] = None):
         if answer.question.type == models.Question.TYPE_TABLE:
             documents = validated_data.pop("documents")
             answer.unlink_unused_rows(docs_to_keep=documents)
 
-        if (
-            answer.question.type == models.Question.TYPE_FILE
-            and answer.file.name is not validated_data["file"]
-        ):
-            answer.file.delete()
-            validated_data = __class__.set_file(validated_data)
+        if answer.question.type == models.Question.TYPE_FILES:
+            cls.update_answer_files(answer, validated_data.pop("files", None))
 
         BaseLogic.update(answer, validated_data, user)
 
         if answer.question.type == models.Question.TYPE_TABLE:
             answer.create_answer_documents(documents)
 
         answer.refresh_from_db()
         return answer
 
-    @staticmethod
-    def set_file(validated_data):
-        file_name = validated_data.get("file")
-        file = models.File.objects.create(name=file_name)
-        validated_data["file"] = file
-        return validated_data
-
 
 class SaveDefaultAnswerLogic(SaveAnswerLogic):
     @staticmethod
     def validate_for_save(
         data: dict, user: BaseUser, answer: models.Answer = None, origin: bool = False
     ) -> dict:
         if data["question"].type in [
-            models.Question.TYPE_FILE,
+            models.Question.TYPE_FILES,
             models.Question.TYPE_STATIC,
             models.Question.TYPE_DYNAMIC_CHOICE,
             models.Question.TYPE_DYNAMIC_MULTIPLE_CHOICE,
             models.Question.TYPE_CALCULATED_FLOAT,
             models.Question.TYPE_ACTION_BUTTON,
         ]:
             raise ValidationError(
```

### Comparing `caluma-8.0.0b9/caluma/caluma_form/factories.py` & `caluma-9.0.0/caluma/caluma_form/factories.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,18 @@
 import faker
-from factory import Faker, LazyAttribute, Maybe, SubFactory, lazy_attribute
+from django.db.models.signals import post_save
+from factory import (
+    Faker,
+    LazyAttribute,
+    Maybe,
+    SubFactory,
+    django,
+    lazy_attribute,
+    post_generation,
+)
 
 from ..caluma_core.factories import DjangoModelFactory
 from . import models
 
 AUTO_QUESTION_TYPES = [
     t
     for t in models.Question.TYPE_CHOICES
@@ -137,21 +146,14 @@
     family = None
     meta = {}
 
     class Meta:
         model = models.Document
 
 
-class FileFactory(DjangoModelFactory):
-    name = Faker("file_name")
-
-    class Meta:
-        model = models.File
-
-
 class AnswerFactory(DjangoModelFactory):
     question = SubFactory(QuestionFactory)
     document = SubFactory(DocumentFactory)
     meta = {}
 
     @lazy_attribute
     def value(self):
@@ -162,34 +164,52 @@
             return [faker.Faker().name(), faker.Faker().name()]
         elif self.question.type == models.Question.TYPE_FLOAT:
             return faker.Faker().pyfloat()
         elif self.question.type == models.Question.TYPE_INTEGER:
             return faker.Faker().pyint()
         elif self.question.type not in [
             models.Question.TYPE_TABLE,
-            models.Question.TYPE_FILE,
+            models.Question.TYPE_FILES,
             models.Question.TYPE_DATE,
         ]:
             return faker.Faker().name()
 
         return None
 
-    file = Maybe(
-        "is_file", yes_declaration=SubFactory(FileFactory), no_declaration=None
-    )
     date = Maybe("is_date", yes_declaration=Faker("date"), no_declaration=None)
 
+    @post_generation
+    @django.mute_signals(post_save)
+    def files(self, create, extracted, **kwargs):
+        if not create:  # pragma: no cover
+            return
+        if self.question.type == models.Question.TYPE_FILES:
+            if extracted is not None:
+                self.files.set(extracted)
+            else:
+                num_files = kwargs.pop("count", 1)
+                self.files.set(
+                    FileFactory.create_batch(num_files, **kwargs, answer=self)
+                )
+
     class Meta:
         model = models.Answer
 
     class Params:
-        is_file = LazyAttribute(lambda a: a.question.type == models.Question.TYPE_FILE)
         is_date = LazyAttribute(lambda a: a.question.type == models.Question.TYPE_DATE)
 
 
+class FileFactory(DjangoModelFactory):
+    name = Faker("file_name")
+    answer = SubFactory(AnswerFactory)
+
+    class Meta:
+        model = models.File
+
+
 class AnswerDocumentFactory(DjangoModelFactory):
     answer = SubFactory(AnswerFactory)
     document = SubFactory(DocumentFactory)
     sort = 0
 
     class Meta:
         model = models.AnswerDocument
```

### Comparing `caluma-8.0.0b9/caluma/caluma_form/filters.py` & `caluma-9.0.0/caluma/caluma_form/filters.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import shlex
 from functools import reduce
 
 import graphene
 from django.core import exceptions
 from django.db import ProgrammingError
 from django.db.models import Q
 from django.forms import BooleanField
@@ -15,16 +16,18 @@
 from ..caluma_core.filters import (
     CompositeFieldClass,
     GlobalIDFilter,
     GlobalIDMultipleChoiceFilter,
     MetaFilterSet,
     SearchFilter,
 )
+from ..caluma_core.forms import GlobalIDFormField
 from ..caluma_core.ordering import AttributeOrderingFactory, MetaFieldOrdering
-from ..caluma_form.models import Answer, DynamicOption, Question
+from ..caluma_core.relay import extract_global_id
+from ..caluma_form.models import Answer, DynamicOption, Form, Question
 from ..caluma_form.ordering import AnswerValueOrdering
 from . import models, validators
 
 
 class FormFilterSet(MetaFilterSet):
     search = SearchFilter(fields=("slug", "name", "description"))
     slugs = MultipleChoiceFilter(field_name="slug")
@@ -77,31 +80,14 @@
     )
 
     class Meta:
         model = models.Question
         fields = ("meta", "attribute")
 
 
-class QuestionFilterSet(MetaFilterSet):
-    exclude_forms = GlobalIDMultipleChoiceFilter(field_name="forms", exclude=True)
-    search = SearchFilter(fields=("slug", "label"))
-    slugs = MultipleChoiceFilter(field_name="slug")
-
-    class Meta:
-        model = models.Question
-        fields = (
-            "label",
-            "is_required",
-            "is_hidden",
-            "is_archived",
-            "sub_form",
-            "row_form",
-        )
-
-
 class QuestionOrderSet(FilterSet):
     meta = MetaFieldOrdering()
     attribute = AttributeOrderingFactory(
         models.Question,
         fields=[
             "created_at",
             "modified_at",
@@ -293,17 +279,26 @@
 class SearchLookupMode(Enum):
     STARTSWITH = "startswith"
     CONTAINS = "icontains"
     TEXT = "search"
 
 
 class SearchAnswersFilterType(InputObjectType):
-    """Lookup type to search in answers."""
+    """
+    Lookup type to search in answers.
 
-    questions = List(graphene.ID, required=True)
+    You may pass in a list of question slugs and/or a list of form slugs to define
+    which answers to search. If you pass in one or more forms, answers to the
+    questions in that form will be searched. If you pass in one or more question
+    slug, the corresponding answers are searched. If you pass both, a superset
+    of both is searched (ie. they do not limit each other).
+    """
+
+    questions = List(graphene.ID)
+    forms = List(graphene.ID)
     value = graphene.types.generic.GenericScalar(required=True)
     lookup = SearchLookupMode(required=False)
 
 
 class SearchAnswersFilterField(CompositeFieldClass):
     pass
 
@@ -323,33 +318,75 @@
         Question.TYPE_FLOAT: "value",
     }
 
     def __init__(self, *args, **kwargs):
         self.document_id = kwargs.pop("document_id")
         super().__init__(*args, **kwargs)
 
+    @staticmethod
+    def _split(value):
+        lex = shlex.shlex(value, posix=True)
+        lex.whitespace_split = True
+        lex.commenters = ""
+        lex.quotes = '"'
+        return [i.strip() for i in lex if i.strip()]
+
+    def get_search_terms(self, value):
+        value = value.replace("\x00", "")  # strip null characters
+        try:
+            return self._split(value)
+        except ValueError as e:
+            if e.args[0] == "No closing quotation":
+                return self._split(f'{value}"')
+
     def filter(self, qs, value):
         if value in EMPTY_VALUES:  # pragma: no cover
             return qs
 
         assert isinstance(value, list)
 
         for val in value:
             if val in EMPTY_VALUES:  # pragma: no cover
                 continue
             qs = self._apply_filter(qs, val)
         return qs
 
-    def _apply_filter(self, qs, value):
+    def _get_questions(self, value):
+        raw_questions = value.get("questions")
+        raw_forms = value.get("forms")
+        questions = Question.objects.none()
 
-        questions = self._validate_and_get_questions(value["questions"])
+        if not raw_questions and not raw_forms:
+            raise exceptions.ValidationError(
+                '"forms" and/or "questions" parameter must be set'
+            )
 
-        for word in value["value"].split():
+        if raw_questions:
+            questions = self._validate_and_get_questions(raw_questions)
+
+        if raw_forms:
+            forms = self._validate_and_get_forms(raw_forms)
+            form_questions = Form.get_all_questions(forms)
+            # Combine querysets: All questions of the given forms, as well as the
+            # explicitly-requested questions.
+            questions = questions | form_questions.filter(
+                type__in=self.FIELD_MAP.keys()
+            )
+
+        return questions
+
+    def _apply_filter(self, qs, value):
+        questions = self._get_questions(value)
+
+        for word in self.get_search_terms(value["value"]):
             answers_with_word = self._answers_with_word(
-                questions, word, value.get("lookup", SearchLookupMode.CONTAINS.value)
+                questions,
+                word,
+                value.get("lookup", SearchLookupMode.CONTAINS.value),
+                value.get("forms"),
             )
             qs = qs.filter(
                 **{
                     f"{self.document_id}__in": answers_with_word.values(
                         "document__family"
                     )
                 }
@@ -400,34 +437,56 @@
             return Q(value=False) & Q(value=True)
 
         filt = "value__contains" if is_multiple else "value"
         return reduce(
             lambda a, b: a | b, [Q(**{filt: slug}) for slug in matching_options]
         )
 
-    def _answers_with_word(self, questions, word, lookup):
+    def _answers_with_word(self, questions, word, lookup, form_slugs):
+        if not questions:
+            return Answer.objects.none()
+
         exprs = [
             self._word_lookup_for_question(question, word, lookup)
-            for q_slug, question in questions.items()
+            for question in questions
         ]
 
         # join expressions with OR
         answer_qs = Answer.objects.filter(reduce(lambda a, b: a | b, exprs))
+
+        # add form filter if given,
+        # otherwise it would return all answers of the question filter ignoring the form filter
+        if form_slugs not in EMPTY_VALUES:
+            answer_qs = answer_qs.filter(document__form__pk__in=form_slugs)
+
         return answer_qs
 
-    def _validate_and_get_questions(self, questions):
-        res = {}
-        for q_slug in questions:
+    def _validate_and_get_questions(self, question_slugs):
+        res = []
+        for q_slug in question_slugs:
             question = Question.objects.get(pk=q_slug)
             if question.type not in self.FIELD_MAP:
                 raise exceptions.ValidationError(
                     f"Questions of type {question.type} cannot be used in searchAnswers"
                 )
-            res[q_slug] = question
-        return res
+            res.append(question)
+        return Question.objects.filter(pk__in=res)
+
+    @staticmethod
+    def _validate_and_get_forms(form_slugs):
+        forms = Form.objects.filter(slug__in=form_slugs)
+        not_found = [
+            x for x in form_slugs if x not in forms.values_list("slug", flat=True)
+        ]
+        if not_found:
+            not_found_string = ", ".join(not_found)
+            raise exceptions.ValidationError(
+                f"Following forms could not be found: {not_found_string}"
+            )
+        return form_slugs
 
     @staticmethod
     @convert_form_field.register(SearchAnswersFilterField)
     def convert_meta_value_field(field):
         registry = get_global_registry()
         converted = registry.get_converted_field(field)
         if converted:
@@ -445,15 +504,15 @@
     id = GlobalIDFilter()
     search = SearchFilter(
         fields=(
             "form__slug",
             "form__name",
             "form__description",
             "answers__value",
-            "answers__file__name",
+            "answers__files__name",
         )
     )
     root_document = GlobalIDFilter(field_name="family")
     forms = GlobalIDMultipleChoiceFilter(field_name="form")
 
     has_answer = HasAnswerFilter(document_id="pk")
     search_answers = SearchAnswersFilter(document_id="pk")
@@ -487,14 +546,48 @@
 
         # assuming qs can only ever be in the context of a single document
         document = qs.first().document.family
         validator = validators.DocumentValidator()
         return qs.filter(question__slug__in=validator.visible_questions(document))
 
 
+class VisibleQuestionFilter(Filter):
+    field_class = GlobalIDFormField
+
+    def filter(self, qs, value):
+        if value in EMPTY_VALUES or not qs.exists():  # pragma: no cover
+            return qs
+
+        document_id = extract_global_id(value)
+
+        # assuming qs can only ever be in the context of a single document
+        document = models.Document.objects.get(pk=document_id)
+        validator = validators.DocumentValidator()
+        return qs.filter(slug__in=validator.visible_questions(document))
+
+
+class QuestionFilterSet(MetaFilterSet):
+    exclude_forms = GlobalIDMultipleChoiceFilter(field_name="forms", exclude=True)
+    search = SearchFilter(fields=("slug", "label"))
+    slugs = MultipleChoiceFilter(field_name="slug")
+
+    visible_in_document = VisibleQuestionFilter()
+
+    class Meta:
+        model = models.Question
+        fields = (
+            "label",
+            "is_required",
+            "is_hidden",
+            "is_archived",
+            "sub_form",
+            "row_form",
+        )
+
+
 class AnswerFilterSet(MetaFilterSet):
     search = SearchFilter(fields=("value", "file__name"))
     questions = GlobalIDMultipleChoiceFilter(field_name="question")
 
     visible_in_context = VisibleAnswerFilter()
 
     class Meta:
```

### Comparing `caluma-8.0.0b9/caluma/caluma_form/format_validators.py` & `caluma-9.0.0/caluma/caluma_form/format_validators.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b9/caluma/caluma_form/historical_schema.py` & `caluma-9.0.0/caluma/caluma_form/historical_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from ..caluma_core.relay import extract_global_id
 from ..caluma_core.types import ConnectionField, CountableConnectionBase
 from . import models
 from .schema import (
     Answer,
     DateAnswer,
-    FileAnswer,
+    FilesAnswer,
     FloatAnswer,
     FormDjangoObjectType,
     IntegerAnswer,
     ListAnswer,
     StringAnswer,
     TableAnswer,
 )
@@ -51,57 +51,57 @@
     class Meta:
         node = HistoricalAnswer
 
 
 class HistoricalIntegerAnswer(IntegerAnswer):
     class Meta:
         model = models.Answer.history.model
-        exclude = ("document", "file", "date")
+        exclude = ("document", "date")
         use_connection = False
         interfaces = (HistoricalAnswer, graphene.Node)
 
 
 class HistoricalFloatAnswer(FloatAnswer):
     class Meta:
         model = models.Answer.history.model
-        exclude = ("document", "file", "date")
+        exclude = ("document", "date")
         use_connection = False
         interfaces = (HistoricalAnswer, graphene.Node)
 
 
 class HistoricalDateAnswer(DateAnswer):
     class Meta:
         model = models.Answer.history.model
-        exclude = ("document", "file")
+        exclude = ("document",)
         use_connection = False
         interfaces = (HistoricalAnswer, graphene.Node)
 
 
 class HistoricalStringAnswer(StringAnswer):
     class Meta:
         model = models.Answer.history.model
-        exclude = ("document", "file", "date")
+        exclude = ("document", "date")
         use_connection = False
         interfaces = (HistoricalAnswer, graphene.Node)
 
 
 class HistoricalListAnswer(ListAnswer):
     class Meta:
         model = models.Answer.history.model
-        exclude = ("document", "file", "date")
+        exclude = ("document", "date")
         use_connection = False
         interfaces = (HistoricalAnswer, graphene.Node)
 
 
 class HistoricalFile(ObjectType):
     name = graphene.String(required=True)
     download_url = graphene.String()
     metadata = generic.GenericScalar()
     historical_answer = graphene.Field(
-        "caluma.caluma_form.historical_schema.HistoricalFileAnswer"
+        "caluma.caluma_form.historical_schema.HistoricalFilesAnswer"
     )
     history_date = graphene.types.datetime.DateTime(required=True)
     history_user_id = graphene.String()
     history_type = graphene.String()
 
     @classmethod
     def resolve_download_url(cls, instance, info):
@@ -112,26 +112,26 @@
         return client.download_url(f"{instance.pk}_{instance.name}")
 
     class Meta:
         model = models.File.history.model
         interfaces = (relay.Node,)
 
 
-class HistoricalFileAnswer(FileAnswer):
-    value = graphene.Field(
+class HistoricalFilesAnswer(FilesAnswer):
+    value = graphene.List(
         HistoricalFile,
         required=False,
         as_of=graphene.types.datetime.DateTime(required=True),
     )
 
     def resolve_value(self, info, as_of, **args):
         # we need to use the HistoricalFile of the correct revision
-        return models.File.history.filter(
-            id=self.file_id, history_date__lte=as_of
-        ).first()
+        return historical_qs_as_of(models.File.history, as_of, pk_attr="id").filter(
+            answer_id=self.id
+        )
 
     class Meta:
         model = models.Answer.history.model
         exclude = ("document", "date")
         use_connection = False
         interfaces = (HistoricalAnswer, graphene.Node)
 
@@ -192,15 +192,15 @@
         # a language feature.
         # Luckily django model instances are hashable, so we're able to make use of
         # this.
         return list(dict.fromkeys(documents))
 
     class Meta:
         model = models.Answer.history.model
-        exclude = ("file", "date")
+        exclude = ("date",)
         use_connection = False
         interfaces = (HistoricalAnswer, graphene.Node)
 
 
 def document_as_of(info, document_global_id, timestamp):
     document_id = extract_global_id(document_global_id)
     document_qs = HistoricalDocument.get_queryset(models.Document.history.all(), info)
@@ -226,12 +226,12 @@
     models.Question.TYPE_INTEGER: HistoricalIntegerAnswer,
     models.Question.TYPE_FLOAT: HistoricalFloatAnswer,
     models.Question.TYPE_DATE: HistoricalDateAnswer,
     models.Question.TYPE_CHOICE: HistoricalStringAnswer,
     models.Question.TYPE_TEXTAREA: HistoricalStringAnswer,
     models.Question.TYPE_TEXT: HistoricalStringAnswer,
     models.Question.TYPE_TABLE: HistoricalTableAnswer,
-    models.Question.TYPE_FILE: HistoricalFileAnswer,
+    models.Question.TYPE_FILES: HistoricalFilesAnswer,
     models.Question.TYPE_DYNAMIC_CHOICE: HistoricalStringAnswer,
     models.Question.TYPE_DYNAMIC_MULTIPLE_CHOICE: HistoricalListAnswer,
     models.Question.TYPE_CALCULATED_FLOAT: HistoricalFloatAnswer,
 }
```

### Comparing `caluma-8.0.0b9/caluma/caluma_form/jexl.py` & `caluma-9.0.0/caluma/caluma_form/jexl.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,14 @@
             yield f"{transform.subject.value} is not a valid question slug."
 
         yield from super().visit_Transform(transform)
 
 
 class QuestionJexl(JEXL):
     def __init__(self, validation_context=None, **kwargs):
-
         if validation_context:
             if "jexl_cache" not in validation_context:
                 validation_context["jexl_cache"] = defaultdict(dict)
             self._cache = validation_context["jexl_cache"]
         else:
             self._cache = defaultdict(dict)
```

### Comparing `caluma-8.0.0b9/caluma/caluma_form/management/commands/copy_form.py` & `caluma-9.0.0/caluma/caluma_form/management/commands/copy_form.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b9/caluma/caluma_form/management/commands/create_bucket.py` & `caluma-9.0.0/caluma/caluma_form/management/commands/create_bucket.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b9/caluma/caluma_form/migrations/0001_initial.py` & `caluma-9.0.0/caluma/caluma_form/migrations/0001_initial.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 import django.db.models.deletion
 import localized_fields.fields.field
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
     dependencies = []
 
     operations = [
         migrations.CreateModel(
             name="Answer",
```

### Comparing `caluma-8.0.0b9/caluma/caluma_form/migrations/0002_auto_20181221_1517.py` & `caluma-9.0.0/caluma/caluma_form/migrations/0002_auto_20181221_1517.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # Generated by Django 1.11.17 on 2018-12-21 15:17
 from __future__ import unicode_literals
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("caluma_form", "0001_initial")]
 
     operations = [
         migrations.AlterField(
             model_name="answer",
             name="created_by_group",
             field=models.CharField(
```

### Comparing `caluma-8.0.0b9/caluma/caluma_form/migrations/0003_auto_20190130_0920.py` & `caluma-9.0.0/caluma/caluma_form/migrations/0003_auto_20190130_0920.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import uuid
 
 import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("caluma_form", "0002_auto_20181221_1517")]
 
     operations = [
         migrations.CreateModel(
             name="AnswerDocument",
             fields=[
                 ("created_at", models.DateTimeField(auto_now_add=True)),
```

### Comparing `caluma-8.0.0b9/caluma/caluma_form/migrations/0004_auto_20190207_1405.py` & `caluma-9.0.0/caluma/caluma_form/migrations/0004_auto_20190207_1405.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from __future__ import unicode_literals
 
 import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("caluma_form", "0003_auto_20190130_0920")]
 
     operations = [
         migrations.AddField(
             model_name="form",
             name="source",
             field=models.ForeignKey(
```

### Comparing `caluma-8.0.0b9/caluma/caluma_form/migrations/0005_auto_20190208_1016.py` & `caluma-9.0.0/caluma/caluma_form/migrations/0005_auto_20190208_1016.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # Generated by Django 1.11.18 on 2019-02-08 10:16
 from __future__ import unicode_literals
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("caluma_form", "0004_auto_20190207_1405")]
 
     operations = [
         migrations.AlterField(
             model_name="question",
             name="type",
             field=models.CharField(
```

### Comparing `caluma-8.0.0b9/caluma/caluma_form/migrations/0006_choice_type_conversion.py` & `caluma-9.0.0/caluma/caluma_form/migrations/0006_choice_type_conversion.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,11 +14,10 @@
 def reverse_func(apps, schema_editor):
     Question = apps.get_model("caluma_form", "Question")
     Question.objects.filter(type="multiple_choice").update(type="checkbox")
     Question.objects.filter(type="choice").update(type="radio")
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("caluma_form", "0005_auto_20190208_1016")]
 
     operations = [migrations.RunPython(forwards_func, reverse_func)]
```

### Comparing `caluma-8.0.0b9/caluma/caluma_form/migrations/0007_auto_20190208_1232.py` & `caluma-9.0.0/caluma/caluma_form/migrations/0007_auto_20190208_1232.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # Generated by Django 1.11.18 on 2019-02-08 12:32
 from __future__ import unicode_literals
 
 from django.db import migrations
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("caluma_form", "0006_choice_type_conversion")]
 
     operations = [
         migrations.AlterModelOptions(
             name="answerdocument", options={"ordering": ["-sort"]}
         ),
         migrations.AlterModelOptions(
```

### Comparing `caluma-8.0.0b9/caluma/caluma_form/migrations/0008_auto_20190319_1720.py` & `caluma-9.0.0/caluma/caluma_form/migrations/0008_auto_20190319_1720.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from __future__ import unicode_literals
 
 import django.core.serializers.json
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("caluma_form", "0007_auto_20190208_1232")]
 
     operations = [
         migrations.AlterField(
             model_name="answer",
             name="value",
             field=models.JSONField(
```

### Comparing `caluma-8.0.0b9/caluma/caluma_form/migrations/0009_auto_20190321_1722.py` & `caluma-9.0.0/caluma/caluma_form/migrations/0009_auto_20190321_1722.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from __future__ import unicode_literals
 
 import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("caluma_form", "0008_auto_20190319_1720")]
 
     operations = [
         migrations.AddField(
             model_name="answer",
             name="value_document",
             field=models.ForeignKey(
```

### Comparing `caluma-8.0.0b9/caluma/caluma_form/migrations/0010_auto_20190404_0652.py` & `caluma-9.0.0/caluma/caluma_form/migrations/0010_auto_20190404_0652.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import uuid
 
 import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("caluma_form", "0009_auto_20190321_1722")]
 
     operations = [
         migrations.CreateModel(
             name="File",
             fields=[
                 ("created_at", models.DateTimeField(auto_now_add=True)),
```

### Comparing `caluma-8.0.0b9/caluma/caluma_form/migrations/0011_auto_20190411_0607.py` & `caluma-9.0.0/caluma/caluma_form/migrations/0011_auto_20190411_0607.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # Generated by Django 1.11.20 on 2019-04-11 06:07
 from __future__ import unicode_literals
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("caluma_form", "0010_auto_20190404_0652")]
 
     operations = [
         migrations.AddField(
             model_name="answer",
             name="date",
             field=models.DateField(blank=True, null=True),
```

### Comparing `caluma-8.0.0b9/caluma/caluma_form/migrations/0012_auto_20190416_1835.py` & `caluma-9.0.0/caluma/caluma_form/migrations/0012_auto_20190416_1835.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from __future__ import unicode_literals
 
 import localized_fields.fields.field
 from django.db import migrations
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("caluma_form", "0011_auto_20190411_0607")]
 
     operations = [
         migrations.AddField(
             model_name="question",
             name="info_text",
             field=localized_fields.fields.field.LocalizedField(
```

### Comparing `caluma-8.0.0b9/caluma/caluma_form/migrations/0013_auto_20190418_0733.py` & `caluma-9.0.0/caluma/caluma_form/migrations/0013_auto_20190418_0733.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # Generated by Django 1.11.20 on 2019-04-18 07:33
 from __future__ import unicode_literals
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("caluma_form", "0012_auto_20190416_1835")]
 
     operations = [
         migrations.AddField(
             model_name="question",
             name="data_source",
             field=models.CharField(blank=True, max_length=255, null=True),
```

### Comparing `caluma-8.0.0b9/caluma/caluma_form/migrations/0014_auto_20190429_0910.py` & `caluma-9.0.0/caluma/caluma_form/migrations/0014_auto_20190429_0910.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from __future__ import unicode_literals
 
 import localized_fields.fields.text_field
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("caluma_form", "0013_auto_20190418_0733")]
 
     operations = [
         migrations.AddField(
             model_name="question",
             name="static_content",
             field=localized_fields.fields.text_field.LocalizedTextField(
```

### Comparing `caluma-8.0.0b9/caluma/caluma_form/migrations/0015_question_format_validators.py` & `caluma-9.0.0/caluma/caluma_form/migrations/0015_question_format_validators.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from __future__ import unicode_literals
 
 import django.contrib.postgres.fields
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("caluma_form", "0014_auto_20190429_0910")]
 
     operations = [
         migrations.AddField(
             model_name="question",
             name="format_validators",
             field=django.contrib.postgres.fields.ArrayField(
```

### Comparing `caluma-8.0.0b9/caluma/caluma_form/migrations/0016_auto_20190510_0843.py` & `caluma-9.0.0/caluma/caluma_form/migrations/0016_auto_20190510_0843.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # Generated by Django 1.11.20 on 2019-05-10 08:43
 from __future__ import unicode_literals
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("caluma_form", "0015_question_format_validators")]
 
     operations = [
         migrations.AlterField(
             model_name="questionoption",
             name="id",
             field=models.CharField(
```

### Comparing `caluma-8.0.0b9/caluma/caluma_form/migrations/0017_auto_20190619_1320.py` & `caluma-9.0.0/caluma/caluma_form/migrations/0017_auto_20190619_1320.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # Generated by Django 1.11.20 on 2019-06-19 13:20
 from __future__ import unicode_literals
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("caluma_form", "0016_auto_20190510_0843")]
 
     operations = [
         migrations.AddIndex(
             model_name="answer",
             index=models.Index(fields=["value"], name="form_answer_value_70b2d0_idx"),
         ),
```

### Comparing `caluma-8.0.0b9/caluma/caluma_form/migrations/0018_remove_answer_value_document_data_migration.py` & `caluma-9.0.0/caluma/caluma_form/migrations/0018_remove_answer_value_document_data_migration.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,14 @@
     logger.warning(
         "Reverting '0018_remove_answer_value_document_data_migration'"
         "doesn't nest the answer structure."
     )
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("caluma_form", "0017_auto_20190619_1320")]
 
     operations = [
         migrations.RunPython(
             attach_form_sub_answers_to_main_document,
             undo_attach_form_sub_answers_to_main_document,
         )
```

### Comparing `caluma-8.0.0b9/caluma/caluma_form/migrations/0020_historicalanswer_historicalanswerdocument_historicaldocument_historicalfile_historicalform_historica.py` & `caluma-9.0.0/caluma/caluma_form/migrations/0020_historicalanswer_historicalanswerdocument_historicaldocument_historicalfile_historicalform_historica.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 import localized_fields.fields.field
 import localized_fields.fields.text_field
 import simple_history.models
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("caluma_form", "0019_remove_answer_value_document")]
 
     operations = [
         migrations.CreateModel(
             name="HistoricalAnswer",
             fields=[
                 ("created_at", models.DateTimeField(blank=True, editable=False)),
```

### Comparing `caluma-8.0.0b9/caluma/caluma_form/migrations/0021_auto_20190708_0905.py` & `caluma-9.0.0/caluma/caluma_form/migrations/0021_auto_20190708_0905.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated by Django 2.2.3 on 2019-07-08 09:05
 
 import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         (
             "caluma_form",
             "0020_historicalanswer_historicalanswerdocument_historicaldocument_historicalfile_historicalform_historica",
         )
     ]
```

### Comparing `caluma-8.0.0b9/caluma/caluma_form/migrations/0022_add_gin_index_to_jsonfields.py` & `caluma-9.0.0/caluma/caluma_form/migrations/0022_add_gin_index_to_jsonfields.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated by Django 2.2.3 on 2019-07-29 09:08
 
 import django.contrib.postgres.indexes
 from django.db import migrations
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("caluma_form", "0021_auto_20190708_0905")]
 
     operations = [
         migrations.RemoveIndex(
             model_name="answer", name="form_answer_value_70b2d0_idx"
         ),
         migrations.AddIndex(
```

### Comparing `caluma-8.0.0b9/caluma/caluma_form/migrations/0024_auto_20190919_1244.py` & `caluma-9.0.0/caluma/caluma_form/migrations/0024_auto_20190919_1244.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
     for fq in FormQuestion.objects.all():
         FormQuestion.objects.filter(form=fq.form, question=fq.question).delete()
         fq.pk = f"{fq.form_id}.{fq.question_id}"
         fq.save()
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("caluma_form", "0023_auto_20190729_1448")]
 
     operations = [
         migrations.AlterField(
             model_name="formquestion",
             name="id",
             field=models.CharField(
```

### Comparing `caluma-8.0.0b9/caluma/caluma_form/migrations/0025_dynamicoption_historicaldynamicoption.py` & `caluma-9.0.0/caluma/caluma_form/migrations/0025_dynamicoption_historicaldynamicoption.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import django.db.models.deletion
 import localized_fields.fields.field
 import simple_history.models
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("caluma_form", "0024_auto_20190919_1244")]
 
     operations = [
         migrations.CreateModel(
             name="HistoricalDynamicOption",
             fields=[
                 ("created_at", models.DateTimeField(blank=True, editable=False)),
```

### Comparing `caluma-8.0.0b9/caluma/caluma_form/migrations/0026_auto_20191031_0834.py` & `caluma-9.0.0/caluma/caluma_form/migrations/0026_auto_20191031_0834.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 2.2.6 on 2019-10-31 08:34
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("caluma_form", "0025_dynamicoption_historicaldynamicoption")]
 
     operations = [
         migrations.RemoveField(model_name="dynamicoption", name="value"),
         migrations.RemoveField(model_name="historicaldynamicoption", name="value"),
         migrations.AddField(
             model_name="dynamicoption",
```

### Comparing `caluma-8.0.0b9/caluma/caluma_form/migrations/0027_auto_20200113_0727.py` & `caluma-9.0.0/caluma/caluma_form/migrations/0027_auto_20200113_0727.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated by Django 2.2.8 on 2020-01-13 07:27
 
 import django.contrib.postgres.indexes
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("caluma_form", "0026_auto_20191031_0834")]
 
     operations = [
         migrations.RemoveIndex(model_name="answer", name="form_answer_date_6485f0_idx"),
         migrations.RemoveIndex(model_name="answer", name="form_answer_meta_98edaa_gin"),
         migrations.RemoveIndex(
             model_name="document", name="form_docume_meta_333f0b_gin"
```

### Comparing `caluma-8.0.0b9/caluma/caluma_form/migrations/0028_auto_20200210_0929.py` & `caluma-9.0.0/caluma/caluma_form/migrations/0028_auto_20200210_0929.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 2.2.8 on 2020-02-10 09:29
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("caluma_form", "0027_auto_20200113_0727")]
 
     operations = [
         migrations.AlterField(
             model_name="answer",
             name="created_at",
             field=models.DateTimeField(auto_now_add=True, db_index=True),
```

### Comparing `caluma-8.0.0b9/caluma/caluma_form/migrations/0029_dynamic_option_unique_together.py` & `caluma-9.0.0/caluma/caluma_form/migrations/0029_dynamic_option_unique_together.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,14 @@
         )
 
         historical_to_delete.delete()
         to_delete.delete()
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("caluma_form", "0028_auto_20200210_0929")]
 
     operations = [
         migrations.RunPython(remove_duplicates, migrations.RunPython.noop),
         migrations.AlterUniqueTogether(
             name="dynamicoption", unique_together={("slug", "document", "question")}
         ),
```

### Comparing `caluma-8.0.0b9/caluma/caluma_form/migrations/0030_auto_20200219_1359.py` & `caluma-9.0.0/caluma/caluma_form/migrations/0030_auto_20200219_1359.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 2.2.10 on 2020-02-19 13:59
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("caluma_form", "0029_dynamic_option_unique_together")]
 
     operations = [
         migrations.AlterField(
             model_name="form",
             name="slug",
             field=models.SlugField(max_length=150, primary_key=True, serialize=False),
```

### Comparing `caluma-8.0.0b9/caluma/caluma_form/migrations/0031_auto_20200220_0910.py` & `caluma-9.0.0/caluma/caluma_form/migrations/0031_auto_20200220_0910.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,14 @@
             f"Document pk={doc.pk} (form={doc.form_id}) missing it's family={doc.family}. Resetting to itself"
         )
         doc.family = doc.pk
         doc.save()
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("caluma_form", "0030_auto_20200219_1359")]
 
     operations = [
         migrations.RunPython(
             cleanup_invalid_family_pointers, migrations.RunPython.noop
         ),
         migrations.AlterField(
```

### Comparing `caluma-8.0.0b9/caluma/caluma_form/migrations/0032_auto_20200220_1311.py` & `caluma-9.0.0/caluma/caluma_form/migrations/0032_auto_20200220_1311.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated by Django 2.2.10 on 2020-02-20 13:11
 
 import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("caluma_form", "0031_auto_20200220_0910")]
 
     operations = [
         migrations.AddField(
             model_name="document",
             name="source",
             field=models.ForeignKey(
```

### Comparing `caluma-8.0.0b9/caluma/caluma_form/migrations/0033_slugfield_length.py` & `caluma-9.0.0/caluma/caluma_form/migrations/0033_slugfield_length.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 2.2.10 on 2020-02-26 09:12
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("caluma_form", "0032_auto_20200220_1311")]
 
     operations = [
         migrations.AlterField(
             model_name="form",
             name="slug",
             field=models.SlugField(max_length=127, primary_key=True, serialize=False),
```

### Comparing `caluma-8.0.0b9/caluma/caluma_form/migrations/0034_fix_fk_lengths.py` & `caluma-9.0.0/caluma/caluma_form/migrations/0034_fix_fk_lengths.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,18 @@
 
 from django.db import migrations
 
 from caluma.utils import fix_foreign_key_types
 
 
 def fix_fk_types_migration(apps, schema_editor):
-
     fix_foreign_key_types(apps, schema_editor.connection)
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("caluma_form", "0033_slugfield_length"),
         ("caluma_workflow", "0019_slugfield_length"),
     ]
 
     operations = [
         migrations.RunPython(fix_fk_types_migration, migrations.RunPython.noop)
```

### Comparing `caluma-8.0.0b9/caluma/caluma_form/migrations/0035_historicalanswer_history_question_type.py` & `caluma-9.0.0/caluma/caluma_form/migrations/0035_historicalanswer_history_question_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
     SET history_question_type = q.type
     FROM caluma_form_question q
     WHERE ha.history_question_type IS NULL AND q.slug = ha.question_id;
 """
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("caluma_form", "0034_fix_fk_lengths")]
 
     operations = [
         migrations.AddField(
             model_name="historicalanswer",
             name="history_question_type",
             field=models.CharField(default=None, max_length=23, null=True),
```

### Comparing `caluma-8.0.0b9/caluma/caluma_form/migrations/0036_default_answers.py` & `caluma-9.0.0/caluma/caluma_form/migrations/0036_default_answers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated by Django 2.2.16 on 2020-11-09 06:23
 
 import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("caluma_form", "0035_historicalanswer_history_question_type")]
 
     operations = [
         migrations.AddField(
             model_name="historicalquestion",
             name="default_answer",
             field=models.ForeignKey(
```

### Comparing `caluma-8.0.0b9/caluma/caluma_form/migrations/0037_default_answer_one2one.py` & `caluma-9.0.0/caluma/caluma_form/migrations/0037_default_answer_one2one.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated by Django 2.2.17 on 2020-11-23 14:28
 
 import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("caluma_form", "0036_default_answers")]
 
     operations = [
         migrations.AlterField(
             model_name="question",
             name="default_answer",
             field=models.OneToOneField(
```

### Comparing `caluma-8.0.0b9/caluma/caluma_form/migrations/0038_auto_20201224_0920.py` & `caluma-9.0.0/caluma/caluma_form/migrations/0038_auto_20201224_0920.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated by Django 2.2.17 on 2020-12-24 09:20
 
 import django.contrib.postgres.fields
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("caluma_form", "0037_default_answer_one2one")]
 
     operations = [
         migrations.AddField(
             model_name="historicalquestion",
             name="calc_dependents",
             field=django.contrib.postgres.fields.ArrayField(
```

### Comparing `caluma-8.0.0b9/caluma/caluma_form/migrations/0040_add_modified_by_user_group.py` & `caluma-9.0.0/caluma/caluma_form/migrations/0040_add_modified_by_user_group.py`

 * *Files identical despite different names*

```diff
@@ -21,15 +21,14 @@
         Model.objects.update(
             modified_by_user=F("created_by_user"),
             modified_by_group=F("created_by_group"),
         )
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("caluma_form", "0039_merge_20210114_0956"),
     ]
 
     operations = [
         migrations.AddField(
             model_name="answer",
```

### Comparing `caluma-8.0.0b9/caluma/caluma_form/migrations/0041_action_button_question.py` & `caluma-9.0.0/caluma/caluma_form/migrations/0041_action_button_question.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 2.2.22 on 2021-11-03 08:52
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("caluma_form", "0040_add_modified_by_user_group"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="historicalquestion",
```

### Comparing `caluma-8.0.0b9/caluma/caluma_form/migrations/0042_auto_20220110_1051.py` & `caluma-9.0.0/caluma/caluma_form/migrations/0042_auto_20220110_1051.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated by Django 2.2.24 on 2022-01-10 10:51
 
 from django.db import migrations
 import localized_fields.fields.field
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("caluma_form", "0041_action_button_question"),
     ]
 
     operations = [
         migrations.AddField(
             model_name="historicalquestion",
```

### Comparing `caluma-8.0.0b9/caluma/caluma_form/migrations/0043_alter_historicalanswer_history_question_type.py` & `caluma-9.0.0/caluma/caluma_form/migrations/0043_alter_historicalanswer_history_question_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 3.2.11 on 2022-01-19 09:17
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("caluma_form", "0042_auto_20220110_1051"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="historicalanswer",
```

### Comparing `caluma-8.0.0b9/caluma/caluma_form/migrations/0044_migrate_format_validators.py` & `caluma-9.0.0/caluma/caluma_form/migrations/0044_migrate_format_validators.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b9/caluma/caluma_form/migrations/0045_simple_history.py` & `caluma-9.0.0/caluma/caluma_form/migrations/0045_simple_history.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 3.2.13 on 2022-06-09 11:26
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("caluma_form", "0044_migrate_format_validators"),
     ]
 
     operations = [
         migrations.AlterModelOptions(
             name="historicalanswer",
```

### Comparing `caluma-8.0.0b9/caluma/caluma_form/models.py` & `caluma-9.0.0/caluma/caluma_form/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,49 @@
         blank=True,
         null=True,
         help_text="Reference this form has been copied from",
         related_name="+",
         on_delete=models.SET_NULL,
     )
 
+    @classmethod
+    def _get_all_raw_forms(cls, forms: list):
+        return cls.objects.raw(
+            """
+            WITH RECURSIVE
+                forms(slug) AS (
+                    SELECT slug
+                    FROM caluma_form_form
+                    WHERE slug = ANY (%s)
+                    UNION ALL
+                    SELECT
+                        all_subforms.subform_id AS slug
+                    FROM forms JOIN all_subforms ON (all_subforms.form_id = forms.slug )
+                ),
+                all_subforms(form_id, subform_id) AS (
+                    SELECT
+                        caluma_form_formquestion.form_id,
+                        COALESCE(caluma_form_question.row_form_id, caluma_form_question.sub_form_id) AS subform_id
+                    FROM caluma_form_formquestion
+                    JOIN caluma_form_question ON (caluma_form_formquestion.question_id = caluma_form_question.slug)
+                    WHERE caluma_form_question.type IN ('form', 'table')
+                )
+            SELECT * FROM forms;
+        """,
+            [forms],
+        )
+
+    @classmethod
+    def get_all_forms(cls, forms: list):  # pragma: no cover
+        return Form.objects.filter(pk__in=cls._get_all_raw_forms(forms))
+
+    @classmethod
+    def get_all_questions(cls, forms: list):
+        return Question.objects.filter(forms__in=cls._get_all_raw_forms(forms))
+
     class Meta:
         indexes = [GinIndex(fields=["meta"])]
 
 
 class FormQuestion(core_models.NaturalKeyModel):
     form = models.ForeignKey("Form", on_delete=models.CASCADE)
     question = models.ForeignKey("Question", on_delete=models.CASCADE)
@@ -54,15 +89,15 @@
     TYPE_FLOAT = "float"
     TYPE_DATE = "date"
     TYPE_CHOICE = "choice"
     TYPE_TEXTAREA = "textarea"
     TYPE_TEXT = "text"
     TYPE_TABLE = "table"
     TYPE_FORM = "form"
-    TYPE_FILE = "file"
+    TYPE_FILES = "files"
     TYPE_DYNAMIC_CHOICE = "dynamic_choice"
     TYPE_DYNAMIC_MULTIPLE_CHOICE = "dynamic_multiple_choice"
     TYPE_STATIC = "static"
     TYPE_CALCULATED_FLOAT = "calculated_float"
     TYPE_ACTION_BUTTON = "action_button"
 
     TYPE_CHOICES = (
@@ -71,15 +106,15 @@
         TYPE_FLOAT,
         TYPE_DATE,
         TYPE_CHOICE,
         TYPE_TEXTAREA,
         TYPE_TEXT,
         TYPE_TABLE,
         TYPE_FORM,
-        TYPE_FILE,
+        TYPE_FILES,
         TYPE_DYNAMIC_CHOICE,
         TYPE_DYNAMIC_MULTIPLE_CHOICE,
         TYPE_STATIC,
         TYPE_CALCULATED_FLOAT,
         TYPE_ACTION_BUTTON,
     )
     TYPE_CHOICES_TUPLE = [(type_choice, type_choice) for type_choice in TYPE_CHOICES]
@@ -402,30 +437,29 @@
         null=True,
         blank=True,
     )
     documents = models.ManyToManyField(
         Document, through="AnswerDocument", related_name="+"
     )
     date = models.DateField(null=True, blank=True)
-    file = models.OneToOneField(
-        "File", on_delete=models.SET_NULL, null=True, blank=True
-    )
 
     # override history to add extra fields on historical model
     history = HistoricalRecords(
         inherit=True,
         history_user_id_field=models.CharField(null=True, max_length=150),
         history_user_setter=core_models._history_user_setter,
         history_user_getter=core_models._history_user_getter,
         bases=[QuestionTypeHistoricalModel],
     )
 
     def delete(self, *args, **kwargs):
-        if self.file:
-            self.file.delete()
+        # Files need to be deleted in sequence (not via on_delete)
+        # so the deletion code on the storage is properly triggered
+        for file in self.files.all():
+            file.delete()
         super().delete(args, kwargs)
 
     def create_answer_documents(self, documents):
         family = getattr(self.document, "family", None)
         document_ids = [document.pk for document in documents]
 
         for sort, document_id in enumerate(reversed(document_ids), start=1):
@@ -461,31 +495,31 @@
                 "created_by_user": user.username if user else None,
                 "created_by_group": user.group if user else None,
                 "modified_by_user": user.username if user else None,
                 "modified_by_group": user.group if user else None,
             },
         )
 
-        if self.question.type == Question.TYPE_FILE:
-            new_answer.file = self.file.copy()
-            new_answer.save()
+        if self.question.type == Question.TYPE_FILES:
+            for file in self.files.all():
+                file.copy(to_answer=new_answer)
 
         if self.question.type in [
             Question.TYPE_DYNAMIC_CHOICE,
             Question.TYPE_DYNAMIC_MULTIPLE_CHOICE,
         ]:
             for dynamic_option in DynamicOption.objects.filter(
                 document=self.document, question=self.question
             ):
                 DynamicOption.objects.update_or_create(
                     document=to_document,
                     question=dynamic_option.question,
                     slug=dynamic_option.slug,
                     defaults={
-                        "label": dynamic_option.slug,
+                        "label": dynamic_option.label,
                         "created_by_user": user.username if user else None,
                         "created_by_group": user.group if user else None,
                     },
                 )
 
         # TableAnswer: copy AnswerDocument too
         for answer_doc in AnswerDocument.objects.filter(answer=self):
@@ -567,31 +601,43 @@
 
     return wrapper
 
 
 class File(core_models.UUIDModel):
     name = models.CharField(max_length=255)
 
+    answer = models.ForeignKey(
+        Answer, on_delete=models.CASCADE, related_name="files", null=True, default=None
+    )
+
     @_ignore_missing_file
     def _move_blob(self):
         # move the file on update
         # this makes sure it stays available when querying the history
         old_file = self.history.first()
+        if not old_file:  # pragma: no cover
+            # No history - cannot move object to preserve history.
+            return
         new_name = f"{old_file.pk}_{old_file.name}"
         client.move_object(self.object_name, new_name)
 
     @_ignore_missing_file
     def _copy(self, new_object_name):
         client.copy_object(self.object_name, new_object_name)
 
-    def copy(self):
-        copy = File.objects.create(name=self.name)
+    def copy(self, to_answer):
+        copy = File.objects.create(name=self.name, answer=to_answer or self.answer)
         self._copy(copy.object_name)
         return copy
 
+    def rename(self, new_name):
+        from_object_name = self.object_name
+        self.name = new_name
+        client.move_object(from_object_name, self.object_name)
+
     def delete(self, *args, **kwargs):
         self._move_blob()
         super().delete(*args, **kwargs)
 
     def save(self, *args, **kwargs):
         if self.created_at:
             self._move_blob()
```

### Comparing `caluma-8.0.0b9/caluma/caluma_form/ordering.py` & `caluma-9.0.0/caluma/caluma_form/ordering.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         QUESTION_TYPE_TO_FIELD = {
             Question.TYPE_INTEGER: "value",
             Question.TYPE_FLOAT: "value",
             Question.TYPE_DATE: "date",
             Question.TYPE_CHOICE: "value",
             Question.TYPE_TEXTAREA: "value",
             Question.TYPE_TEXT: "value",
-            Question.TYPE_FILE: "file__name",
+            Question.TYPE_FILES: "files__name",
             Question.TYPE_DYNAMIC_CHOICE: "value",
         }
 
         try:
             value_field = QUESTION_TYPE_TO_FIELD[question.type]
         except KeyError:  # pragma: no cover
             raise exceptions.ValidationError(
```

### Comparing `caluma-8.0.0b9/caluma/caluma_form/schema.py` & `caluma-9.0.0/caluma/caluma_form/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -324,20 +324,25 @@
             "calc_dependents",
         )
         use_connection = False
         interfaces = (Question, graphene.Node)
 
 
 class DynamicQuestion(graphene.Interface):
-    options = ConnectionField(DataSourceDataConnection)
+    options = ConnectionField(
+        DataSourceDataConnection,
+        context=graphene.JSONString(
+            description="JSON object passed as context to the data source"
+        ),
+    )
     data_source = graphene.String(required=True)
     hint_text = graphene.String()
 
-    def resolve_options(self, info, *args, **kwargs):
-        return get_data_source_data(info.context.user, self.data_source)
+    def resolve_options(self, info, context=None, *args, **kwargs):
+        return get_data_source_data(info.context.user, self.data_source, self, context)
 
 
 class DynamicChoiceQuestion(QuestionQuerysetMixin, FormDjangoObjectType):
     hint_text = graphene.String()
 
     class Meta:
         model = models.Question
@@ -491,15 +496,15 @@
             "calc_expression",
             "calc_dependents",
         )
         use_connection = False
         interfaces = (Question, graphene.Node)
 
 
-class FileQuestion(QuestionQuerysetMixin, FormDjangoObjectType):
+class FilesQuestion(QuestionQuerysetMixin, FormDjangoObjectType):
     hint_text = graphene.String()
 
     class Meta:
         model = models.Question
         exclude = (
             "type",
             "configuration",
@@ -731,15 +736,15 @@
 
 class SaveFormQuestion(SaveQuestion):
     class Meta:
         serializer_class = serializers.SaveFormQuestionSerializer
         return_field_type = Question
 
 
-class SaveFileQuestion(SaveQuestion):
+class SaveFilesQuestion(SaveQuestion):
     class Meta:
         serializer_class = serializers.SaveFileQuestionSerializer
         return_field_type = Question
 
 
 class SaveStaticQuestion(SaveQuestion):
     class Meta:
@@ -795,38 +800,38 @@
 
 
 class IntegerAnswer(AnswerQuerysetMixin, FormDjangoObjectType):
     value = graphene.Int()
 
     class Meta:
         model = models.Answer
-        exclude = ("document", "documents", "file", "date")
+        exclude = ("document", "documents", "files", "date")
         use_connection = False
         interfaces = (Answer, graphene.Node)
 
 
 class FloatAnswer(AnswerQuerysetMixin, FormDjangoObjectType):
     value = graphene.Float()
 
     class Meta:
         model = models.Answer
-        exclude = ("document", "documents", "file", "date")
+        exclude = ("document", "documents", "files", "date")
         use_connection = False
         interfaces = (Answer, graphene.Node)
 
 
 class DateAnswer(AnswerQuerysetMixin, FormDjangoObjectType):
     value = graphene.types.datetime.Date()
 
     def resolve_value(self, info, **args):
         return self.date
 
     class Meta:
         model = models.Answer
-        exclude = ("document", "documents", "file")
+        exclude = ("document", "documents", "files")
         use_connection = False
         interfaces = (Answer, graphene.Node)
 
 
 class SelectedOption(ObjectType):
     label = graphene.String(required=True)
     slug = graphene.String(required=True)
@@ -843,26 +848,26 @@
 
     def resolve_selected_option(self, info, **args):
         selected_options = self.selected_options
         return selected_options[0] if selected_options else None
 
     class Meta:
         model = models.Answer
-        exclude = ("document", "documents", "file", "date")
+        exclude = ("document", "documents", "files", "date")
         use_connection = False
         interfaces = (Answer, graphene.Node)
 
 
 class ListAnswer(AnswerQuerysetMixin, FormDjangoObjectType):
     value = graphene.List(graphene.String)
     selected_options = ConnectionField(SelectedOptionConnection)
 
     class Meta:
         model = models.Answer
-        exclude = ("document", "documents", "file", "date")
+        exclude = ("document", "documents", "files", "date")
         use_connection = False
         interfaces = (Answer, graphene.Node)
 
 
 class AnswerConnection(CountableConnectionBase):
     class Meta:
         node = Answer
@@ -892,41 +897,40 @@
     value = graphene.List(Document)
 
     def resolve_value(self, info, **args):
         return self.documents.order_by("-answerdocument__sort")
 
     class Meta:
         model = models.Answer
-        exclude = ("documents", "file", "date")
+        exclude = ("documents", "files", "date")
         use_connection = False
         interfaces = (Answer, graphene.Node)
 
 
 class File(FormDjangoObjectType):
     name = graphene.String(required=True)
     upload_url = graphene.String()
     download_url = graphene.String()
     metadata = generic.GenericScalar()
-    answer = graphene.Field("caluma.caluma_form.schema.FileAnswer")
 
     class Meta:
         model = models.File
         interfaces = (relay.Node,)
         fields = "__all__"
 
 
-class FileAnswer(AnswerQuerysetMixin, FormDjangoObjectType):
-    value = graphene.Field(File, required=True)
+class FilesAnswer(AnswerQuerysetMixin, FormDjangoObjectType):
+    value = graphene.List(File, required=True)
 
     def resolve_value(self, info, **args):
-        return self.file
+        return self.files.all()
 
     class Meta:
         model = models.Answer
-        exclude = ("document", "documents", "date")
+        exclude = ("document", "documents", "date", "files")
         use_connection = False
         interfaces = (Answer, graphene.Node)
 
 
 class SaveDocument(Mutation):
     class Input:
         id = graphene.String()
@@ -988,17 +992,25 @@
 
 class SaveDocumentTableAnswer(SaveDocumentAnswer):
     class Meta:
         serializer_class = serializers.SaveDocumentTableAnswerSerializer
         return_field_type = Answer
 
 
-class SaveDocumentFileAnswer(SaveDocumentAnswer):
+class SaveFile(graphene.InputObjectType):
+    id = graphene.String()
+    name = graphene.String()
+
+
+class SaveDocumentFilesAnswer(SaveDocumentAnswer):
+    class Input:
+        value = graphene.List(SaveFile, required=False)
+
     class Meta:
-        serializer_class = serializers.SaveDocumentFileAnswerSerializer
+        serializer_class = serializers.SaveDocumentFilesAnswerSerializer
         return_field_type = Answer
 
 
 class SaveDefaultAnswer(Mutation):
     @classmethod
     def get_object(cls, root, info, queryset, **input):
         question_id = extract_global_id(input["question"])
@@ -1083,28 +1095,28 @@
     save_multiple_choice_question = SaveMultipleChoiceQuestion().Field()
     save_dynamic_choice_question = SaveDynamicChoiceQuestion().Field()
     save_dynamic_multiple_choice_question = SaveDynamicMultipleChoiceQuestion().Field()
     save_float_question = SaveFloatQuestion().Field()
     save_integer_question = SaveIntegerQuestion().Field()
     save_table_question = SaveTableQuestion().Field()
     save_form_question = SaveFormQuestion().Field()
-    save_file_question = SaveFileQuestion().Field()
+    save_files_question = SaveFilesQuestion().Field()
     save_static_question = SaveStaticQuestion().Field()
     save_calculated_float_question = SaveCalculatedFloatQuestion().Field()
     save_action_button_question = SaveActionButtonQuestion().Field()
 
     copy_document = CopyDocument().Field()
     save_document = SaveDocument().Field()
     save_document_string_answer = SaveDocumentStringAnswer().Field()
     save_document_integer_answer = SaveDocumentIntegerAnswer().Field()
     save_document_float_answer = SaveDocumentFloatAnswer().Field()
     save_document_date_answer = SaveDocumentDateAnswer().Field()
     save_document_list_answer = SaveDocumentListAnswer().Field()
     save_document_table_answer = SaveDocumentTableAnswer().Field()
-    save_document_file_answer = SaveDocumentFileAnswer().Field()
+    save_document_files_answer = SaveDocumentFilesAnswer().Field()
 
     save_default_string_answer = SaveDefaultStringAnswer().Field()
     save_default_integer_answer = SaveDefaultIntegerAnswer().Field()
     save_default_float_answer = SaveDefaultFloatAnswer().Field()
     save_default_date_answer = SaveDefaultDateAnswer().Field()
     save_default_list_answer = SaveDefaultListAnswer().Field()
     save_default_table_answer = SaveDefaultTableAnswer().Field()
@@ -1128,22 +1140,21 @@
 
 
 class DocumentValidityConnection(CountableConnectionBase):
     class Meta:
         node = ValidationResult
 
 
-def validate_document(info, document_global_id):
-
+def validate_document(info, document_global_id, **kwargs):
     document_id = extract_global_id(document_global_id)
 
     document_qs = Document.get_queryset(models.Document.objects.all(), info)
 
     document = get_object_or_404(document_qs, pk=document_id)
-    result = get_document_validity(document, info)
+    result = get_document_validity(document, info.context.user, **kwargs)
 
     errors = result.pop("errors")
     result = ValidationResult(
         **result, errors=[ValidationEntry(**err) for err in errors]
     )
 
     return [result]
@@ -1177,34 +1188,36 @@
         filterset_class=CollectionFilterSetFactory(
             filterset_class=filters.DynamicOptionFilterSet,
             orderset_class=filters.DynamicOptionOrderSet,
         ),
     )
 
     document_validity = ConnectionField(
-        DocumentValidityConnection, id=graphene.ID(required=True)
+        DocumentValidityConnection,
+        id=graphene.ID(required=True),
+        data_source_context=graphene.JSONString(),
     )
 
     def resolve_all_format_validators(self, info, **kwargs):
         return get_format_validators()
 
     def resolve_document_validity(self, info, id, **kwargs):
-        return validate_document(info, id)
+        return validate_document(info, id, **kwargs)
 
 
 QUESTION_ANSWER_TYPES = {
     models.Question.TYPE_MULTIPLE_CHOICE: ListAnswer,
     models.Question.TYPE_INTEGER: IntegerAnswer,
     models.Question.TYPE_FLOAT: FloatAnswer,
     models.Question.TYPE_DATE: DateAnswer,
     models.Question.TYPE_CHOICE: StringAnswer,
     models.Question.TYPE_TEXTAREA: StringAnswer,
     models.Question.TYPE_TEXT: StringAnswer,
     models.Question.TYPE_TABLE: TableAnswer,
-    models.Question.TYPE_FILE: FileAnswer,
+    models.Question.TYPE_FILES: FilesAnswer,
     models.Question.TYPE_DYNAMIC_CHOICE: StringAnswer,
     models.Question.TYPE_DYNAMIC_MULTIPLE_CHOICE: ListAnswer,
     models.Question.TYPE_CALCULATED_FLOAT: FloatAnswer,
 }
 
 QUESTION_OBJECT_TYPES = {
     models.Question.TYPE_TEXT: TextQuestion,
@@ -1214,12 +1227,12 @@
     models.Question.TYPE_MULTIPLE_CHOICE: MultipleChoiceQuestion,
     models.Question.TYPE_DYNAMIC_CHOICE: DynamicChoiceQuestion,
     models.Question.TYPE_DYNAMIC_MULTIPLE_CHOICE: DynamicMultipleChoiceQuestion,
     models.Question.TYPE_TEXTAREA: TextareaQuestion,
     models.Question.TYPE_DATE: DateQuestion,
     models.Question.TYPE_TABLE: TableQuestion,
     models.Question.TYPE_FORM: FormQuestion,
-    models.Question.TYPE_FILE: FileQuestion,
+    models.Question.TYPE_FILES: FilesQuestion,
     models.Question.TYPE_STATIC: StaticQuestion,
     models.Question.TYPE_CALCULATED_FLOAT: CalculatedFloatQuestion,
     models.Question.TYPE_ACTION_BUTTON: ActionButtonQuestion,
 }
```

### Comparing `caluma-8.0.0b9/caluma/caluma_form/serializers.py` & `caluma-9.0.0/caluma/caluma_form/serializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from rest_framework import exceptions
 from rest_framework.serializers import (
     BooleanField,
     CharField,
     DateField,
     FloatField,
     IntegerField,
+    JSONField,
     ListField,
     PrimaryKeyRelatedField,
 )
 
 from ..caluma_core import serializers
 from . import domain_logic, models, validators
 from .jexl import QuestionJexl
@@ -419,15 +420,15 @@
 
     class Meta(SaveQuestionSerializer.Meta):
         fields = SaveQuestionSerializer.Meta.fields + ["sub_form"]
 
 
 class SaveFileQuestionSerializer(SaveQuestionSerializer):
     def validate(self, data):
-        data["type"] = models.Question.TYPE_FILE
+        data["type"] = models.Question.TYPE_FILES
         return super().validate(data)
 
     class Meta(SaveQuestionSerializer.Meta):
         fields = SaveQuestionSerializer.Meta.fields + ["hint_text"]
 
 
 class SaveStaticQuestionSerializer(SaveQuestionSerializer):
@@ -520,17 +521,29 @@
             "form",
             "meta",
         ]
         extra_kwargs = {"id": {"read_only": False, "required": False}}
 
 
 class SaveAnswerSerializer(serializers.ModelSerializer):
+    data_source_context = JSONField(
+        encoder=None,
+        required=False,
+        allow_null=True,
+        write_only=True,
+        help_text="JSON object passed as context to the data source of dynamic questions",
+    )
+
     def validate(self, data):
         data = domain_logic.SaveAnswerLogic.validate_for_save(
-            data, self.context["request"].user, self.instance, True
+            data,
+            self.context["request"].user,
+            self.instance,
+            True,
+            data.pop("data_source_context", None),
         )
         return super().validate(data)
 
     @transaction.atomic
     def create(self, validated_data):
         return domain_logic.SaveAnswerLogic.create(
             validated_data, user=self.context["request"].user
@@ -538,15 +551,22 @@
 
     @transaction.atomic
     def update(self, instance, validated_data):
         return domain_logic.SaveAnswerLogic.update(instance, validated_data)
 
     class Meta:
         model = models.Answer
-        fields = ["question", "document", "meta", "value"]
+        fields = [
+            "question",
+            "document",
+            "meta",
+            "value",
+            "question",
+            "data_source_context",
+        ]
 
 
 class SaveDocumentStringAnswerSerializer(SaveAnswerSerializer):
     value = CharField(trim_whitespace=False, allow_blank=True, required=False)
 
     class Meta(SaveAnswerSerializer.Meta):
         pass
@@ -589,22 +609,23 @@
         help_text="List of document IDs representing the rows in the table.",
     )
 
     class Meta(SaveAnswerSerializer.Meta):
         pass
 
 
-class SaveDocumentFileAnswerSerializer(SaveAnswerSerializer):
-    value = CharField(write_only=True, source="file", required=False)
-    value_id = PrimaryKeyRelatedField(read_only=True, source="file", required=False)
+class SaveDocumentFilesAnswerSerializer(SaveAnswerSerializer):
+    value = ListField(
+        source="files",
+        required=False,
+        help_text="List of files for this answer",
+    )
 
     class Meta(SaveAnswerSerializer.Meta):
-        fields = SaveAnswerSerializer.Meta.fields + [
-            "value_id",
-        ]
+        fields = SaveAnswerSerializer.Meta.fields
 
 
 class RemoveAnswerSerializer(serializers.ModelSerializer):
     answer = PrimaryKeyRelatedField(
         queryset=models.Answer.objects.filter(document__isnull=False)
     )
```

### Comparing `caluma-8.0.0b9/caluma/caluma_form/signals.py` & `caluma-9.0.0/caluma/caluma_form/signals.py`

 * *Files 5% similar despite different names*

```diff
@@ -115,15 +115,14 @@
 # mutated whenever a calculated question is created, updated or deleted.
 
 
 @receiver(pre_save, sender=models.Question)
 @disable_raw
 @filter_events(lambda instance: instance.type == models.Question.TYPE_CALCULATED_FLOAT)
 def save_calc_dependents(sender, instance, **kwargs):
-
     original = models.Question.objects.filter(pk=instance.pk).first()
     if not original:
         _update_calc_dependents(
             instance.slug, old_expr="false", new_expr=instance.calc_expression
         )
 
     elif original.calc_expression != instance.calc_expression:
@@ -148,15 +147,14 @@
 # related model is performed.
 
 
 @receiver(post_save, sender=models.Question)
 @disable_raw
 @filter_events(lambda instance: instance.type == models.Question.TYPE_CALCULATED_FLOAT)
 def update_calc_from_question(sender, instance, created, update_fields, **kwargs):
-
     # TODO optimize: only update answers if calc_expression is updated
     # needs to happen during save() or __init__()
 
     for document in models.Document.objects.filter(form__questions=instance):
         _update_or_create_calc_answer(instance, document)
 
 
@@ -183,20 +181,20 @@
         pk__in=instance.question.calc_dependents
     ):
         _update_or_create_calc_answer(question, instance.document)
 
 
 @receiver(post_save, sender=models.Document)
 @disable_raw
-@filter_events(lambda created: created)
+# We're only interested in table row forms
+@filter_events(lambda instance, created: instance.pk != instance.family_id or created)
 def update_calc_from_document(sender, instance, created, **kwargs):
-
-    for question in instance.form.questions.filter(
-        type=models.Question.TYPE_CALCULATED_FLOAT
-    ):
+    for question in models.Form.get_all_questions(
+        [(instance.family or instance).form_id]
+    ).filter(type=models.Question.TYPE_CALCULATED_FLOAT):
         _update_or_create_calc_answer(question, instance)
 
 
 @receiver(m2m_changed, sender=models.AnswerDocument)
 def update_calc_from_answerdocument(sender, instance, **kwargs):
     dependents = instance.document.form.questions.exclude(
         calc_dependents=[]
```

### Comparing `caluma-8.0.0b9/caluma/caluma_form/storage_clients.py` & `caluma-9.0.0/caluma/caluma_form/storage_clients.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
             return fn(self, *args, **kwargs)
         except S3Error as exc:
             if (
                 exc.code == "NoSuchBucket"
                 and settings.MINIO_STORAGE_AUTO_CREATE_MEDIA_BUCKET
             ):
                 log.warning(
-                    b"Minio bucket '{self.bucket}' missing, trying to create it"
+                    f"Minio bucket '{self.bucket}' missing, trying to create it"
                 )
                 self.client.make_bucket(self.bucket)
                 return fn(self, *args, **kwargs)
             raise
 
     return wrapper
 
@@ -77,15 +77,15 @@
 
         :param object_name: str
         :return: stat response if successful, otherwise None
         """
         try:
             return self.client.stat_object(self.bucket, object_name)
         except S3Error as exc:
-            log.error(f"Minio error, cannot stat object: {exc.code}")
+            log.warning(f"Minio error, cannot stat object '{object_name}': {exc.code}")
             return None
 
     @_retry_on_missing_bucket
     def download_url(self, object_name):
         return self.client.presigned_get_object(
             self.bucket,
             object_name,
```

### Comparing `caluma-8.0.0b9/caluma/caluma_form/structure.py` & `caluma-9.0.0/caluma/caluma_form/structure.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Hierarchical representation of a document / form."""
 import weakref
 from functools import singledispatch
 from typing import List, Optional
 
-from .models import AnswerDocument, Question
+from .models import Question
 
 
 def object_local_memoise(method):
     def new_method(self, *args, **kwargs):
         if not hasattr(self, "_memoise"):
             self._memoise = {}
 
@@ -87,16 +87,16 @@
 
         elif self.question.type == Question.TYPE_TABLE:  # pragma: no cover
             return [
                 {cell.question.slug: cell.value() for cell in row.children()}
                 for row in self.children()
             ]
 
-        elif self.question.type == Question.TYPE_FILE:
-            return self.answer.file
+        elif self.question.type == Question.TYPE_FILES:
+            return [f.name for f in self.answer.files.all()]
 
         elif self.question.type == Question.TYPE_DATE:
             return self.answer.date
 
         elif self.question.type in (
             Question.TYPE_MULTIPLE_CHOICE,
             Question.TYPE_DYNAMIC_MULTIPLE_CHOICE,
@@ -112,15 +112,20 @@
 
 class RowField(Field):
     @object_local_memoise
     def children(self):
         if not self.answer:
             return []  # pragma: no cover
 
-        rows = AnswerDocument.objects.filter(answer=self.answer).order_by("sort")
+        # We're sorting in python-space here to reuse the already-executed query
+        # for the answerdocument_set. Sorting in DB would re-issue the query
+        rows = sorted(
+            self.answer.answerdocument_set.all(),
+            key=lambda answer_document: answer_document.sort,
+        )
         return [
             FieldSet(
                 ans_doc.document,
                 self.question.row_form,
                 question=self.question,
                 parent=self.parent(),
             )
```

### Comparing `caluma-8.0.0b9/caluma/caluma_form/validators.py` & `caluma-9.0.0/caluma/caluma_form/validators.py`

 * *Files 3% similar despite different names*

```diff
@@ -103,48 +103,54 @@
             raise CustomValidationError(
                 f"Invalid options [{', '.join(invalid_options)}]. "
                 f"Should be one of the options [{', '.join(options)}]",
                 slugs=[question.slug],
             )
 
     def _validate_question_dynamic_choice(
-        self, question, value, document, user, **kwargs
+        self, question, value, document, user, data_source_context, **kwargs
     ):
         if not isinstance(value, str):
             raise CustomValidationError(
                 f'Invalid value "{value}". Must be of type str.', slugs=[question.slug]
             )
 
-        self._validate_dynamic_option(question, document, value, user)
+        self._validate_dynamic_option(
+            question, document, value, user, data_source_context
+        )
         self._remove_unused_dynamic_options(question, document, [value])
 
     def _validate_question_dynamic_multiple_choice(
-        self, question, value, document, user, **kwargs
+        self, question, value, document, user, data_source_context, **kwargs
     ):
         if not isinstance(value, list):
             raise CustomValidationError(
                 f'Invalid value: "{value}". Must be of type list', slugs=[question.slug]
             )
 
         for v in value:
             if not isinstance(v, str):
                 raise CustomValidationError(
                     f'Invalid value: "{v}". Must be of type string',
                     slugs=[question.slug],
                 )
-            self._validate_dynamic_option(question, document, v, user)
+            self._validate_dynamic_option(
+                question, document, v, user, data_source_context
+            )
 
         self._remove_unused_dynamic_options(question, document, value)
 
-    def _validate_dynamic_option(self, question, document, option, user):
+    def _validate_dynamic_option(
+        self, question, document, option, user, data_source_context
+    ):
         data_source = get_data_sources(dic=True)[question.data_source]
         data_source_object = data_source()
 
         valid_label = data_source_object.validate_answer_value(
-            option, document, question, user
+            option, document, question, user, data_source_context
         )
         if valid_label is False:
             raise CustomValidationError(
                 f'Invalid value "{option}". Not a valid option.', slugs=[question.slug]
             )
 
         DynamicOption.objects.get_or_create(
@@ -178,34 +184,37 @@
 
         for row_doc in value:
             if row_doc.form_id != question.row_form_id:
                 raise exceptions.ValidationError(
                     f"Document {row_doc.pk} is not of form type {question.row_form.pk}."
                 )
 
-    def _validate_question_file(self, question, value, **kwargs):
-        pass
+    def _validate_question_files(self, question, value, **kwargs):
+        if not isinstance(value, list) and value is not None:  # pragma: no cover
+            # should already have been rejected by schema / gql level
+            raise exceptions.ValidationError("Input files must be a list")
 
     def _validate_question_calculated_float(self, question, value, **kwargs):
         pass
 
     def validate(
         self,
         *,
         question,
         document,
         user,
         validation_context=None,
         instance=None,
         origin=False,
+        data_source_context=None,
         **kwargs,
     ):
         # Check all possible fields for value
         value = None
-        for i in ["documents", "file", "date", "value"]:
+        for i in ["documents", "files", "date", "value"]:
             value = kwargs.get(i, value)
             if value:
                 break
 
         # empty values are allowed
         # required check will be done in DocumentValidator
         if value in EMPTY_VALUES:
@@ -216,23 +225,31 @@
             question,
             value,
             document=document,
             user=user,
             validation_context=validation_context,
             instance=instance,
             origin=origin,
+            data_source_context=data_source_context,
         )
 
         format_validators = get_format_validators(dic=True)
         for validator_slug in question.format_validators:
             format_validators[validator_slug]().validate(value, document)
 
 
 class DocumentValidator:
-    def validate(self, document, user, validation_context=None, **kwargs):
+    def validate(
+        self,
+        document,
+        user,
+        validation_context=None,
+        data_source_context=None,
+        **kwargs,
+    ):
         if not validation_context:
             validation_context = self._validation_context(document)
 
         self._validate_required(validation_context)
 
         for answer in document.answers.filter(
             question_id__in=validation_context["visible_questions"]
@@ -241,14 +258,15 @@
             validator.validate(
                 document=document,
                 question=answer.question,
                 value=answer.value,
                 documents=answer.documents.all(),
                 user=user,
                 validation_context=validation_context,
+                data_source_context=data_source_context,
             )
 
     def _validation_context(self, document):
         # we need to build the context in two steps (for now), as
         # `self.visible_questions()` already needs a context to evaluate
         # `is_hidden` expressions
         intermediate_context = {
@@ -441,20 +459,20 @@
         elif data["type"] == models.Question.TYPE_CALCULATED_FLOAT:
             self._validate_calc_expression(data)
 
         if "dataSource" in data:
             self._validate_data_source(data["dataSource"])
 
 
-def get_document_validity(document, user):
+def get_document_validity(document, user, **kwargs):
     validator = DocumentValidator()
     is_valid = True
     errors = []
 
     try:
-        validator.validate(document, user)
+        validator.validate(document, user, **kwargs)
     except CustomValidationError as exc:
         is_valid = False
         detail = str(exc.detail[0])
         errors = [{"slug": slug, "error_msg": detail} for slug in exc.slugs]
 
     return {"id": document.id, "is_valid": is_valid, "errors": errors}
```

### Comparing `caluma-8.0.0b9/caluma/caluma_logging/management/commands/cleanup_access_log.py` & `caluma-9.0.0/caluma/caluma_logging/management/commands/cleanup_access_log.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b9/caluma/caluma_logging/middleware.py` & `caluma-9.0.0/caluma/caluma_logging/middleware.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b9/caluma/caluma_logging/migrations/0001_initial.py` & `caluma-9.0.0/caluma/caluma_logging/migrations/0001_initial.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 2.2.16 on 2020-09-18 15:59
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
     dependencies = []
 
     operations = [
         migrations.CreateModel(
             name="AccessLog",
```

### Comparing `caluma-8.0.0b9/caluma/caluma_logging/models.py` & `caluma-9.0.0/caluma/caluma_logging/models.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b9/caluma/caluma_user/views.py` & `caluma-9.0.0/caluma/caluma_user/views.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import base64
 import functools
 import hashlib
 
 import requests
 from django.conf import settings
 from django.core.cache import cache
 from django.core.exceptions import ImproperlyConfigured
@@ -47,33 +46,14 @@
             settings.OIDC_USERINFO_ENDPOINT,
             verify=settings.OIDC_VERIFY_SSL,
             headers={"Authorization": f"Bearer {smart_str(token)}"},
         )
         response.raise_for_status()
         return response.json()
 
-    def get_introspection(self, token):
-        basic = base64.b64encode(
-            f"{settings.OIDC_INTROSPECT_CLIENT_ID}:{settings.OIDC_INTROSPECT_CLIENT_SECRET}".encode(
-                "utf-8"
-            )
-        ).decode()
-        headers = {
-            "Authorization": f"Basic {basic}",
-            "Content-Type": "application/x-www-form-urlencoded",
-        }
-        response = requests.post(
-            settings.OIDC_INTROSPECT_ENDPOINT,
-            verify=settings.OIDC_VERIFY_SSL,
-            headers=headers,
-            data={"token": token},
-        )
-        response.raise_for_status()
-        return response.json()
-
     def _oidc_user(self, *args, **kwargs):
         factory = import_string(settings.CALUMA_OIDC_USER_FACTORY)
         return factory(*args, **kwargs)
 
     def get_user(self, request):
         token = self.get_bearer_token(request)
 
@@ -82,49 +62,30 @@
 
         if not settings.OIDC_USERINFO_ENDPOINT:
             raise ImproperlyConfigured(
                 'Token was provided, but "OIDC_USERINFO_ENDPOINT" is not set.'
             )
 
         userinfo_method = functools.partial(self.get_userinfo, token=token)
-        # token might be too long for key so we use hash sum instead.
+        # token might be too long for key, so we use hash sum instead.
         hashsum_token = hashlib.sha256(force_bytes(token)).hexdigest()
 
         try:
-            userinfo = cache.get_or_set(
+            claims = cache.get_or_set(
                 f"authentication.userinfo.{hashsum_token}",
                 userinfo_method,
                 timeout=settings.OIDC_BEARER_TOKEN_REVALIDATION_TIME,
             )
-            return self._oidc_user(token=token, userinfo=userinfo)
         except requests.HTTPError as e:
-            try:
-                if (
-                    e.response.status_code in [401, 403]
-                    and settings.OIDC_INTROSPECT_ENDPOINT
-                ):
-                    introspect_method = functools.partial(
-                        self.get_introspection, token=token
-                    )
-                    introspection = cache.get_or_set(
-                        f"authentication.introspect.{hashsum_token}",
-                        introspect_method,
-                        timeout=settings.OIDC_BEARER_TOKEN_REVALIDATION_TIME,
-                    )
-                    if "client_id" not in introspection:
-                        response = HttpResponse(status=401)
-                        raise HttpError(response)
-                    return self._oidc_user(token=token, introspection=introspection)
-                else:
-                    raise e
-            except requests.HTTPError as internal_exception:
-                # convert request error to django http error
-                response = HttpResponse()
-                response.status_code = internal_exception.response.status_code
-                raise HttpError(response, message=str(internal_exception))
+            # convert request error to django http error
+            response = HttpResponse()
+            response.status_code = e.response.status_code
+            raise HttpError(response, message=str(e))
+
+        return self._oidc_user(token=token, claims=claims)
 
     def dispatch(self, request, *args, **kwargs):
         try:
             request.user = self.get_user(request)
             return super().dispatch(request, *args, **kwargs)
         except HttpError as e:
             response = e.response
```

### Comparing `caluma-8.0.0b9/caluma/caluma_user/visibilities.py` & `caluma-9.0.0/caluma/caluma_user/visibilities.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b9/caluma/caluma_workflow/api.py` & `caluma-9.0.0/caluma/caluma_workflow/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,17 @@
     >>> complete_work_item(
     ...     work_item=models.WorkItem.first(),
     ...     user=AnonymousUser()
     ... )
     <WorkItem: WorkItem object (some-uuid)>
     ```
     """
-    domain_logic.CompleteWorkItemLogic.validate_for_complete(work_item, user)
+    domain_logic.CompleteWorkItemLogic.validate_for_complete(
+        work_item, user, context=context
+    )
     validated_data = domain_logic.CompleteWorkItemLogic.pre_complete(
         work_item, {}, user, context
     )
 
     update_model(work_item, validated_data)
 
     domain_logic.CompleteWorkItemLogic.post_complete(work_item, user, context)
```

### Comparing `caluma-8.0.0b9/caluma/caluma_workflow/apps.py` & `caluma-9.0.0/caluma/caluma_workflow/apps.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b9/caluma/caluma_workflow/domain_logic.py` & `caluma-9.0.0/caluma/caluma_workflow/domain_logic.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,22 +109,24 @@
             status__in=(
                 models.WorkItem.STATUS_COMPLETED,
                 models.WorkItem.STATUS_SKIPPED,
             ),
         ).exists()
 
     @staticmethod
-    def validate_for_complete(work_item, user):
+    def validate_for_complete(work_item, user, context=None):
         validators.WorkItemValidator().validate(
             status=work_item.status,
             child_case=work_item.child_case,
             task=work_item.task,
             case=work_item.case,
             document=work_item.document,
             user=user,
+            validation_context=context.get("validation_context") if context else None,
+            data_source_context=context.get("data_source_context") if context else None,
         )
 
     @staticmethod
     def pre_complete(
         work_item,
         validated_data,
         user,
@@ -177,15 +179,19 @@
             all_siblings_complete = all(
                 CompleteWorkItemLogic._can_continue(work_item, task)
                 for task in sibling_tasks
             )
 
             if all_siblings_complete:
                 created_work_items = utils.create_work_items(
-                    next_tasks, case, user, work_item, context
+                    next_tasks,
+                    case,
+                    user,
+                    work_item,
+                    context,
                 )
 
                 for created_work_item in created_work_items:  # pragma: no cover
                     send_event(
                         events.post_create_work_item,
                         sender=sender,
                         work_item=created_work_item,
@@ -375,16 +381,21 @@
     def validate_for_reopen(case, work_items):
         if case.status not in [
             models.Case.STATUS_COMPLETED,
             models.Case.STATUS_CANCELED,
         ]:
             raise ValidationError("Only completed and canceled cases can be reopened.")
 
-        if not case.family == case:
-            raise ValidationError("Child cases can not be reopened.")
+        if (
+            case.family != case
+            and case.parent_work_item.status != models.WorkItem.STATUS_READY
+        ):
+            raise ValidationError(
+                "Only child cases of ready work items can be reopened."
+            )
 
         for work_item in work_items:
             if work_item.succeeding_work_items.exclude(
                 status=models.WorkItem.STATUS_REDO
             ).exists():
                 raise ValidationError(
                     "Only work items at the end of a branch can be reopened."
@@ -608,21 +619,26 @@
         that task's workitem (redoable).
         We allow redoing a work item if at least one ready work item allows "our" task
         to be re-done.
         """
         if work_item.status == models.WorkItem.STATUS_READY:
             raise ValidationError("Ready work items can't be redone.")
 
+        if not cls.is_work_item_redoable(work_item):
+            raise ValidationError("Workflow doesn't allow to redo this work item.")
+
+    @classmethod
+    def is_work_item_redoable(cls, work_item):
         for wi in cls._find_ready_in_work_item_tree(
             work_item, allowed_states=[models.WorkItem.STATUS_READY]
         ):
             if work_item.task in wi.get_redoable():
-                return
+                return True
 
-        raise ValidationError("Workflow doesn't allow to redo this work item.")
+        return False
 
     @classmethod
     def set_succeeding_work_item_status_redo(cls, work_item):
         for wi in cls._find_ready_in_work_item_tree(work_item):
             wi.status = models.WorkItem.STATUS_REDO
             wi.save()
```

### Comparing `caluma-8.0.0b9/caluma/caluma_workflow/dynamic_groups.py` & `caluma-9.0.0/caluma/caluma_workflow/dynamic_groups.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b9/caluma/caluma_workflow/dynamic_tasks.py` & `caluma-9.0.0/caluma/caluma_workflow/dynamic_tasks.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b9/caluma/caluma_workflow/events.py` & `caluma-9.0.0/caluma/caluma_workflow/events.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,9 +9,8 @@
     "case": ["create", "complete", "cancel", "suspend", "resume", "reopen"],
 }
 
 # create "pre|post"_"create|complete|..."_"work_item|case" events in all given combinations
 for obj, actions in MODEL_ACTIONS.items():
     for action in actions:
         for prefix in ["pre", "post"]:
-
             setattr(module, f"{prefix}_{action}_{obj}", Signal())
```

### Comparing `caluma-8.0.0b9/caluma/caluma_workflow/factories.py` & `caluma-9.0.0/caluma/caluma_workflow/factories.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b9/caluma/caluma_workflow/filters.py` & `caluma-9.0.0/caluma/caluma_workflow/filters.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 import graphene
-from django_filters.rest_framework import BooleanFilter, MultipleChoiceFilter
+from django_filters.rest_framework import (
+    BooleanFilter,
+    DateTimeFilter,
+    MultipleChoiceFilter,
+)
 
 from ..caluma_core.filters import (
     BaseFilterSet,
     CharFilter,
     GlobalIDFilter,
+    GlobalIDMultipleChoiceFilter,
     JSONValueFilter,
     MetaFilterSet,
     SearchFilter,
     StringListFilter,
     generate_list_filter_class,
 )
 from ..caluma_core.ordering import AttributeOrderingFactory, MetaFieldOrdering
@@ -82,44 +87,48 @@
     class Meta:
         model = models.Flow
         fields = ("meta", "attribute")
 
 
 class CaseFilterSet(MetaFilterSet):
     id = GlobalIDFilter()
+    id.deprecation_reason = "Use ids filter instead"
+    ids = GlobalIDMultipleChoiceFilter(field_name="pk")
 
     document_form = CharFilter(field_name="document__form_id")
     document_forms = MultipleChoiceFilter(field_name="document__form_id")
     has_answer = HasAnswerFilter(document_id="document__pk")
     work_item_document_has_answer = HasAnswerFilter(
         document_id="work_items__document__pk"
     )
     root_case = GlobalIDFilter(field_name="family")
     search_answers = SearchAnswersFilter(document_id="document__pk")
     status = case_status_filter(lookup_expr="in")
+    exclude_child_cases = BooleanFilter(method="filter_exclude_child_cases")
+
+    def filter_exclude_child_cases(self, queryset, name, value):
+        if not value:
+            return queryset
+
+        return queryset.filter(parent_work_item__isnull=True)
 
     class Meta:
         model = models.Case
         fields = ("workflow",)
 
 
 class CaseOrderSet(BaseFilterSet):
     meta = MetaFieldOrdering()
     attribute = AttributeOrderingFactory(
         models.Case,
         fields=[
             "created_at",
             "modified_at",
-            "allow_all_forms",
-            "description",
-            "is_archived",
-            "is_published",
-            "name",
             "status",
-            "slug",
+            "document__form__name",
         ],
     )
     document_answer = AnswerValueOrdering(document_via="document")
 
     class Meta:
         model = models.Case
         fields = ("meta", "attribute", "document_answer")
@@ -136,20 +145,18 @@
 class TaskOrderSet(BaseFilterSet):
     meta = MetaFieldOrdering()
     attribute = AttributeOrderingFactory(
         models.Task,
         fields=[
             "created_at",
             "modified_at",
-            "allow_all_forms",
             "lead_time",
             "type",
             "description",
             "is_archived",
-            "is_published",
             "name",
             "slug",
         ],
     )
 
     class Meta:
         model = models.Task
@@ -160,16 +167,29 @@
     id = GlobalIDFilter()
     addressed_groups = StringListFilter(lookup_expr="overlap")
     controlling_groups = StringListFilter(lookup_expr="overlap")
     assigned_users = StringListFilter(lookup_expr="overlap")
 
     document_has_answer = HasAnswerFilter(document_id="document__pk")
     case_document_has_answer = HasAnswerFilter(document_id="case__document__pk")
+    case_document_forms = MultipleChoiceFilter(field_name="case__document__form_id")
     case_meta_value = JSONValueFilter(field_name="case__meta")
     root_case_meta_value = JSONValueFilter(field_name="case__family__meta")
+    case_search_answers = SearchAnswersFilter(document_id="case__document__pk")
+
+    deadline_before = DateTimeFilter(
+        field_name="deadline",
+        lookup_expr="lt",
+        label="Only return work items whose deadline is set to before the given datetime",
+    )
+    deadline_after = DateTimeFilter(
+        field_name="deadline",
+        lookup_expr="gte",
+        label="Only return work items whose deadline is set to after the given datetime",
+    )
 
     tasks = MultipleChoiceFilter(field_name="task_id")
 
     has_deadline = BooleanFilter(
         field_name="deadline", lookup_expr="isnull", exclude=True
     )
     case_family = GlobalIDFilter(field_name="case__family")
@@ -196,22 +216,20 @@
     case_meta = MetaFieldOrdering(field_name="case__meta")
     attribute = AttributeOrderingFactory(
         models.WorkItem,
         fields=[
             "created_at",
             "modified_at",
             "closed_at",
-            "allow_all_forms",
             "description",
-            "is_archived",
-            "is_published",
             "name",
             "deadline",
             "status",
             "slug",
+            "case__document__form__name",
         ],
     )
     document_answer = AnswerValueOrdering(document_via="document")
     case_document_answer = AnswerValueOrdering(document_via="case__document")
 
     class Meta:
         model = models.WorkItem
```

### Comparing `caluma-8.0.0b9/caluma/caluma_workflow/jexl.py` & `caluma-9.0.0/caluma/caluma_workflow/jexl.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0001_initial.py` & `caluma-9.0.0/caluma/caluma_workflow/migrations/0001_initial.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 import django.db.models.deletion
 import localized_fields.fields.field
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
     dependencies = [("caluma_form", "0001_initial")]
 
     operations = [
         migrations.CreateModel(
             name="Case",
```

### Comparing `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0002_auto_20181213_1334.py` & `caluma-9.0.0/caluma/caluma_workflow/migrations/0002_auto_20181213_1334.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from __future__ import unicode_literals
 
 import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("caluma_workflow", "0001_initial")]
 
     operations = [
         migrations.AlterField(
             model_name="case",
             name="document",
             field=models.OneToOneField(
```

### Comparing `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0003_auto_20181217_1051.py` & `caluma-9.0.0/caluma/caluma_workflow/migrations/0003_auto_20181217_1051.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # Generated by Django 1.11.17 on 2018-12-17 10:51
 from __future__ import unicode_literals
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("caluma_workflow", "0002_auto_20181213_1334")]
 
     operations = [
         migrations.AlterField(
             model_name="task",
             name="type",
             field=models.CharField(
```

### Comparing `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0004_auto_20181218_1352.py` & `caluma-9.0.0/caluma/caluma_workflow/migrations/0004_auto_20181218_1352.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from __future__ import unicode_literals
 
 import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("caluma_form", "0001_initial"),
         ("caluma_workflow", "0003_auto_20181217_1051"),
     ]
 
     operations = [
         migrations.AddField(
```

### Comparing `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0005_auto_20181228_1243.py` & `caluma-9.0.0/caluma/caluma_workflow/migrations/0005_auto_20181228_1243.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import django.contrib.postgres.fields
 import django.contrib.postgres.indexes
 import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("caluma_workflow", "0004_auto_20181218_1352")]
 
     operations = [
         migrations.AddField(
             model_name="task",
             name="address_groups",
             field=models.TextField(blank=True, null=True),
```

### Comparing `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0006_auto_20190121_1440.py` & `caluma-9.0.0/caluma/caluma_workflow/migrations/0006_auto_20190121_1440.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from __future__ import unicode_literals
 
 import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("caluma_workflow", "0005_auto_20181228_1243")]
 
     operations = [
         migrations.AlterField(
             model_name="task",
             name="address_groups",
             field=models.TextField(
```

### Comparing `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0007_auto_20190206_0854.py` & `caluma-9.0.0/caluma/caluma_workflow/migrations/0010_auto_20190213_1050.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,26 @@
 # -*- coding: utf-8 -*-
-# Generated by Django 1.11.18 on 2019-02-06 08:54
+# Generated by Django 1.11.20 on 2019-02-13 10:50
 from __future__ import unicode_literals
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
-    dependencies = [
-        ("caluma_form", "0003_auto_20190130_0920"),
-        ("caluma_workflow", "0006_auto_20190121_1440"),
-    ]
+    dependencies = [("caluma_workflow", "0009_auto_20190213_0939")]
 
     operations = [
-        migrations.RemoveField(model_name="workflow", name="form"),
         migrations.AddField(
-            model_name="workflow",
-            name="allow_all_forms",
-            field=models.BooleanField(
-                default=False, help_text="Allow workflow to be started with any form"
+            model_name="task",
+            name="lead_time",
+            field=models.PositiveIntegerField(
+                blank=True,
+                help_text="Time in seconds task may take to be processed.",
+                null=True,
             ),
         ),
         migrations.AddField(
-            model_name="workflow",
-            name="allow_forms",
-            field=models.ManyToManyField(
-                blank=True,
-                help_text="List of forms which are allowed to start workflow with",
-                related_name="workflows",
-                to="caluma_form.Form",
-            ),
+            model_name="workitem",
+            name="deadline",
+            field=models.DateTimeField(blank=True, null=True),
         ),
     ]
```

### Comparing `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0008_auto_20190208_1302.py` & `caluma-9.0.0/caluma/caluma_workflow/migrations/0008_auto_20190208_1302.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # Generated by Django 1.11.18 on 2019-02-08 13:02
 from __future__ import unicode_literals
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("caluma_workflow", "0007_auto_20190206_0854")]
 
     operations = [
         migrations.RemoveField(model_name="workflow", name="start"),
         migrations.AddField(
             model_name="workflow",
             name="start_tasks",
```

### Comparing `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0009_auto_20190213_0939.py` & `caluma-9.0.0/caluma/caluma_workflow/migrations/0009_auto_20190213_0939.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # Generated by Django 1.11.18 on 2019-02-13 09:39
 from __future__ import unicode_literals
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("caluma_workflow", "0008_auto_20190208_1302")]
 
     operations = [
         migrations.AddField(
             model_name="case",
             name="closed_at",
             field=models.DateTimeField(
```

### Comparing `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0010_auto_20190213_1050.py` & `caluma-9.0.0/caluma/caluma_form/migrations/0023_auto_20190729_1448.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,20 @@
-# -*- coding: utf-8 -*-
-# Generated by Django 1.11.20 on 2019-02-13 10:50
-from __future__ import unicode_literals
+# Generated by Django 2.2.3 on 2019-07-29 14:48
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
-    dependencies = [("caluma_workflow", "0009_auto_20190213_0939")]
+    dependencies = [("caluma_form", "0022_add_gin_index_to_jsonfields")]
 
     operations = [
         migrations.AddField(
-            model_name="task",
-            name="lead_time",
-            field=models.PositiveIntegerField(
-                blank=True,
-                help_text="Time in seconds task may take to be processed.",
-                null=True,
-            ),
+            model_name="historicaloption",
+            name="is_archived",
+            field=models.BooleanField(default=False),
         ),
         migrations.AddField(
-            model_name="workitem",
-            name="deadline",
-            field=models.DateTimeField(blank=True, null=True),
+            model_name="option",
+            name="is_archived",
+            field=models.BooleanField(default=False),
         ),
     ]
```

### Comparing `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0011_auto_20190220_1303.py` & `caluma-9.0.0/caluma/caluma_workflow/migrations/0011_auto_20190220_1303.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # Generated by Django 1.11.20 on 2019-02-20 13:03
 from __future__ import unicode_literals
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("caluma_workflow", "0010_auto_20190213_1050")]
 
     operations = [
         migrations.AddField(
             model_name="task",
             name="is_multiple_instance",
             field=models.BooleanField(
```

### Comparing `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0012_historicalcase_historicalflow_historicaltask_historicaltaskflow_historicalworkflow_historicalworkite.py` & `caluma-9.0.0/caluma/caluma_workflow/migrations/0012_historicalcase_historicalflow_historicaltask_historicaltaskflow_historicalworkflow_historicalworkite.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 import django.db.models.deletion
 import localized_fields.fields.field
 import simple_history.models
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         (
             "caluma_form",
             "0020_historicalanswer_historicalanswerdocument_historicaldocument_historicalfile_historicalform_historica",
         ),
         ("caluma_workflow", "0011_auto_20190220_1303"),
     ]
```

### Comparing `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0013_auto_20190718_1235.py` & `caluma-9.0.0/caluma/caluma_workflow/migrations/0013_auto_20190718_1235.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from django.db import migrations
 
 import caluma.caluma_core.models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         (
             "caluma_workflow",
             "0012_historicalcase_historicalflow_historicaltask_historicaltaskflow_historicalworkflow_historicalworkite",
         )
     ]
```

### Comparing `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0014_add_gin_index_to_jsonfields.py` & `caluma-9.0.0/caluma/caluma_workflow/migrations/0014_add_gin_index_to_jsonfields.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated by Django 2.2.3 on 2019-07-29 09:08
 
 import django.contrib.postgres.indexes
 from django.db import migrations
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("caluma_workflow", "0013_auto_20190718_1235")]
 
     operations = [
         migrations.AddIndex(
             model_name="case",
             index=django.contrib.postgres.indexes.GinIndex(
                 fields=["meta"], name="workflow_ca_meta_08775a_gin"
```

### Comparing `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0015_add_work_item_skipped.py` & `caluma-9.0.0/caluma/caluma_workflow/migrations/0015_add_work_item_skipped.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from django.db import migrations
 
 import caluma.caluma_core.models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("caluma_workflow", "0014_add_gin_index_to_jsonfields")]
 
     operations = [
         migrations.AlterField(
             model_name="historicalworkitem",
             name="status",
             field=caluma.caluma_core.models.ChoicesCharField(
```

### Comparing `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0016_auto_20200113_0727.py` & `caluma-9.0.0/caluma/caluma_workflow/migrations/0016_auto_20200113_0727.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated by Django 2.2.8 on 2020-01-13 07:27
 
 import django.contrib.postgres.indexes
 from django.db import migrations
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("caluma_workflow", "0015_add_work_item_skipped")]
 
     operations = [
         migrations.RemoveIndex(model_name="case", name="workflow_ca_meta_08775a_gin"),
         migrations.RemoveIndex(model_name="task", name="workflow_ta_meta_6864a4_gin"),
         migrations.RemoveIndex(
             model_name="workflow", name="workflow_wo_meta_2ac517_gin"
```

### Comparing `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0017_auto_20200210_0929.py` & `caluma-9.0.0/caluma/caluma_workflow/migrations/0017_auto_20200210_0929.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 2.2.8 on 2020-02-10 09:29
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("caluma_workflow", "0016_auto_20200113_0727")]
 
     operations = [
         migrations.AlterField(
             model_name="case",
             name="created_at",
             field=models.DateTimeField(auto_now_add=True, db_index=True),
```

### Comparing `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0018_auto_20200219_1359.py` & `caluma-9.0.0/caluma/caluma_workflow/migrations/0018_auto_20200219_1359.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 2.2.10 on 2020-02-19 13:59
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("caluma_workflow", "0017_auto_20200210_0929")]
 
     operations = [
         migrations.AlterField(
             model_name="historicaltask",
             name="slug",
             field=models.SlugField(max_length=150),
```

### Comparing `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0019_slugfield_length.py` & `caluma-9.0.0/caluma/caluma_workflow/migrations/0019_slugfield_length.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 2.2.10 on 2020-02-26 09:12
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("caluma_workflow", "0018_auto_20200219_1359")]
 
     operations = [
         migrations.AlterField(
             model_name="historicaltask",
             name="slug",
             field=models.SlugField(max_length=127),
```

### Comparing `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0020_case_families.py` & `caluma-9.0.0/caluma/caluma_workflow/migrations/0020_case_families.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
     for case in orphan_cases:
         family = case
 
         # Navigate up the hierarchy, but avoid hanging
         # if we have a loop in the data structure
         try:
-
             while (
                 hasattr(family, "parent_work_item")
                 and family.parent_work_item.case != family
             ):
                 family = family.parent_work_item.case
         except models.DoesNotExist:
             # Some times, hasattr() succeeds, but accessing the
@@ -50,15 +49,14 @@
 
     HistoricalCase.objects.using(db_alias).bulk_update(
         orphan_historical_cases, ["family"]
     )
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("caluma_workflow", "0019_slugfield_length")]
 
     operations = [
         migrations.AddField(
             model_name="case",
             name="family",
             field=models.ForeignKey(
```

### Comparing `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0021_work_item_controlling_groups.py` & `caluma-9.0.0/caluma/caluma_workflow/migrations/0021_work_item_controlling_groups.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated by Django 2.2.10 on 2020-03-13 09:23
 
 import django.contrib.postgres.fields
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("caluma_workflow", "0020_case_families")]
 
     operations = [
         migrations.AddField(
             model_name="historicaltask",
             name="control_groups",
             field=models.TextField(
```

### Comparing `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0022_workitem_name_description.py` & `caluma-9.0.0/caluma/caluma_workflow/migrations/0022_workitem_name_description.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,14 @@
         ):
             historical_work_item.name = work_item.name
             historical_work_item.description = work_item.description
             historical_work_item.save()
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("caluma_workflow", "0021_work_item_controlling_groups")]
 
     operations = [
         migrations.AddField(
             model_name="historicalworkitem",
             name="description",
             field=localized_fields.fields.field.LocalizedField(
```

### Comparing `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0023_auto_20200730_1135.py` & `caluma-9.0.0/caluma/caluma_workflow/migrations/0023_auto_20200730_1135.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated by Django 2.2.14 on 2020-07-30 11:35
 
 import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("caluma_workflow", "0022_workitem_name_description")]
 
     operations = [
         migrations.AddField(
             model_name="historicalworkitem",
             name="previous_work_item",
             field=models.ForeignKey(
```

### Comparing `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0024_auto_20200901_1026.py` & `caluma-9.0.0/caluma/caluma_workflow/migrations/0024_auto_20200901_1026.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from django.db import migrations
 
 import caluma.caluma_core.models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("caluma_workflow", "0023_auto_20200730_1135")]
 
     operations = [
         migrations.AlterField(
             model_name="case",
             name="status",
             field=caluma.caluma_core.models.ChoicesCharField(
```

### Comparing `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0025_auto_20200901_1415.py` & `caluma-9.0.0/caluma/caluma_workflow/migrations/0025_auto_20200901_1415.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from django.db import migrations
 
 import caluma.caluma_core.models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("caluma_workflow", "0024_auto_20200901_1026")]
 
     operations = [
         migrations.AlterField(
             model_name="historicalworkitem",
             name="status",
             field=caluma.caluma_core.models.ChoicesCharField(
```

### Comparing `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0026_auto_20200901_1435.py` & `caluma-9.0.0/caluma/caluma_workflow/migrations/0026_auto_20200901_1435.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from django.db import migrations
 
 import caluma.caluma_core.models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("caluma_workflow", "0025_auto_20200901_1415")]
 
     operations = [
         migrations.AlterField(
             model_name="case",
             name="status",
             field=caluma.caluma_core.models.ChoicesCharField(
```

### Comparing `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0027_add_modified_by_user_group.py` & `caluma-9.0.0/caluma/caluma_workflow/migrations/0027_add_modified_by_user_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
         Model.objects.update(
             modified_by_user=F("created_by_user"),
             modified_by_group=F("created_by_group"),
         )
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("caluma_workflow", "0026_auto_20200901_1435"),
     ]
 
     operations = [
         migrations.AddField(
             model_name="case",
```

### Comparing `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0028_redoable_field.py` & `caluma-9.0.0/caluma/caluma_workflow/migrations/0028_redoable_field.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import django.db.models.deletion
 from django.db import migrations, models
 
 import caluma.caluma_core.models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("caluma_workflow", "0027_add_modified_by_user_group"),
     ]
 
     operations = [
         migrations.AddField(
             model_name="historicaltaskflow",
```

### Comparing `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0029_task_continue_async.py` & `caluma-9.0.0/caluma/caluma_workflow/migrations/0029_task_continue_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 3.2.12 on 2022-03-09 11:50
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("caluma_workflow", "0028_redoable_field"),
     ]
 
     operations = [
         migrations.AddField(
             model_name="historicaltask",
```

### Comparing `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0030_remove_choices_char_field.py` & `caluma-9.0.0/caluma/caluma_workflow/migrations/0030_remove_choices_char_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 3.2.13 on 2022-04-27 09:04
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("caluma_workflow", "0029_task_continue_async"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="case",
```

### Comparing `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0031_simple_history.py` & `caluma-9.0.0/caluma/caluma_workflow/migrations/0031_simple_history.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 3.2.13 on 2022-06-09 11:26
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("caluma_workflow", "0030_remove_choices_char_field"),
     ]
 
     operations = [
         migrations.AlterModelOptions(
             name="historicalcase",
```

### Comparing `caluma-8.0.0b9/caluma/caluma_workflow/models.py` & `caluma-9.0.0/caluma/caluma_workflow/models.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b9/caluma/caluma_workflow/schema.py` & `caluma-9.0.0/caluma/caluma_workflow/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from ..caluma_core.mutation import Mutation, UserDefinedPrimaryKeyMixin
 from ..caluma_core.types import (
     CountableConnectionBase,
     DjangoObjectType,
     Node,
     enum_type_from_field,
 )
+from ..caluma_workflow.domain_logic import RedoWorkItemLogic
 from . import filters, jexl, models, serializers
 
 
 class FlowJexl(graphene.String):
     """Flow jexl represents a jexl expression returning task slugs.
 
     Following transforms can be used:
@@ -190,14 +191,27 @@
 class WorkItem(DjangoObjectType):
     task = graphene.Field(Task, required=True)
     meta = generic.GenericScalar()
     assigned_users = graphene.List(graphene.String, required=True)
     controlling_groups = graphene.List(graphene.String, required=True)
     addressed_groups = graphene.List(graphene.String, required=True)
     status = WorkItemStatus(required=True)
+    is_redoable = graphene.Boolean(
+        description=(
+            "This property potentially performs poorly if used in a large set"
+            "of entries, as the evaluation of the redoable jexl configuration"
+            "cannot be performed on the database level. Please use carefully."
+        )
+    )
+
+    def resolve_is_redoable(self, *args, **kwargs):
+        return (
+            self.status != models.WorkItem.STATUS_READY
+            and RedoWorkItemLogic.is_work_item_redoable(self)
+        )
 
     class Meta:
         model = models.WorkItem
         interfaces = (relay.Node,)
         connection_class = CountableConnectionBase
         fields = "__all__"
 
@@ -221,17 +235,17 @@
     status = CaseStatus(required=True)
 
     def resolve_family_work_items(self, info, **args):
         return models.WorkItem.objects.filter(case__family=self.family)
 
     class Meta:
         model = models.Case
-        exclude = ("family",)
         interfaces = (relay.Node,)
         connection_class = CountableConnectionBase
+        fields = "__all__"
 
 
 class SaveWorkflow(UserDefinedPrimaryKeyMixin, Mutation):
     class Meta:
         serializer_class = serializers.SaveWorkflowSerializer
 
 
@@ -276,20 +290,14 @@
 
 class SaveCompleteTaskFormTask(SaveTask):
     class Meta:
         serializer_class = serializers.SaveCompleteTaskFormTaskSerializer
         return_field_type = Task
 
 
-class StartCase(Mutation):
-    class Meta:
-        serializer_class = serializers.CaseSerializer
-        model_operations = ["create"]
-
-
 class SaveCase(Mutation):
     class Input:
         id = graphene.String()
 
     class Meta:
         serializer_class = serializers.SaveCaseSerializer
         model_operations = ["create", "update"]
@@ -311,15 +319,15 @@
     class Meta:
         serializer_class = serializers.ResumeCaseSerializer
         model_operations = ["update"]
 
 
 class ReopenCase(Mutation):
     class Input:
-        id = graphene.ID()
+        id = graphene.ID(required=True)
         work_items = graphene.List(
             graphene.ID,
             required=True,
             description="List of work item ids to be readied when the case is reopened",
         )
 
     class Meta:
@@ -381,23 +389,20 @@
     add_workflow_flow = AddWorkflowFlow().Field()
     remove_flow = RemoveFlow().Field()
 
     save_simple_task = SaveSimpleTask().Field()
     save_complete_workflow_form_task = SaveCompleteWorkflowFormTask().Field()
     save_complete_task_form_task = SaveCompleteTaskFormTask().Field()
 
-    start_case = StartCase().Field()
-
-    start_case.deprecation_reason = "Use SaveCase mutation instead"
-
     save_case = SaveCase().Field()
     cancel_case = CancelCase().Field()
     suspend_case = SuspendCase().Field()
     resume_case = ResumeCase().Field()
     reopen_case = ReopenCase().Field()
+
     complete_work_item = CompleteWorkItem().Field()
     skip_work_item = SkipWorkItem().Field()
     cancel_work_item = CancelWorkItem().Field()
     suspend_work_item = SuspendWorkItem().Field()
     resume_work_item = ResumeWorkItem().Field()
     redo_work_item = RedoWorkItem().Field()
     save_work_item = SaveWorkItem().Field()
```

### Comparing `caluma-8.0.0b9/caluma/caluma_workflow/serializers.py` & `caluma-9.0.0/caluma/caluma_workflow/serializers.py`

 * *Files 6% similar despite different names*

```diff
@@ -70,26 +70,30 @@
     workflow = serializers.GlobalIDField(source="slug")
     tasks = serializers.GlobalIDPrimaryKeyRelatedField(
         queryset=models.Task.objects, many=True
     )
     next = FlowJexlField(required=True)
     redoable = FlowJexlField(required=False, write_only=True)
 
-    def validate_next(self, value):
-        jexl = FlowJexl()
-        tasks = set(jexl.extract_tasks(value))
+    def has_tasks_in_jexl(self, expression):
+        if not expression:
+            return False
 
-        if not tasks:
+        return len(set(FlowJexl().extract_tasks(expression))) > 0
+
+    def validate(self, data):
+        next_has_tasks = self.has_tasks_in_jexl(data.get("next"))
+        redoable_has_tasks = self.has_tasks_in_jexl(data.get("redoable"))
+
+        if not next_has_tasks and not redoable_has_tasks:
             raise exceptions.ValidationError(
-                f"jexl `{value}` does not contain any tasks as return value"
+                "Either `next` or `redoable` must contain tasks"
             )
-        return value
 
-    def validate_redoable(self, value):
-        return self.validate_next(value)
+        return super().validate(data)
 
     @transaction.atomic
     def update(self, instance, validated_data):
         user = self.context["request"].user
         tasks = validated_data["tasks"]
         redoable = validated_data.get("redoable")
         models.Flow.objects.filter(
@@ -189,15 +193,15 @@
         data["type"] = models.Task.TYPE_COMPLETE_TASK_FORM
         return super().validate(data)
 
     class Meta(SaveTaskSerializer.Meta):
         fields = SaveTaskSerializer.Meta.fields + ["form"]
 
 
-class CaseSerializer(SendEventSerializerMixin, ContextModelSerializer):
+class SaveCaseSerializer(ContextModelSerializer):
     workflow = serializers.GlobalIDPrimaryKeyRelatedField(
         queryset=models.Workflow.objects.prefetch_related("start_tasks")
     )
     parent_work_item = serializers.GlobalIDPrimaryKeyRelatedField(
         queryset=models.WorkItem.objects, required=False
     )
     form = serializers.GlobalIDPrimaryKeyRelatedField(
@@ -222,42 +226,19 @@
 
         return domain_logic.StartCaseLogic.post_start(
             case, user, validated_data.get("parent_work_item"), self.context_data
         )
 
     class Meta:
         model = models.Case
-        fields = ["workflow", "meta", "parent_work_item", "form", "context"]
-
-
-class SaveCaseSerializer(CaseSerializer):
-    @transaction.atomic
-    def create(self, validated_data):
-        self.send_event(
-            events.pre_create_case, case=None, validated_data=validated_data
-        )
-        instance = super().create(validated_data)
-        self.send_event(events.post_create_case, case=instance)
-        return instance
-
-    @transaction.atomic
-    def update(self, instance, validated_data):
-        self.send_event(
-            events.pre_create_case, case=instance, validated_data=validated_data
-        )
-        instance = super().update(instance, validated_data)
-        self.send_event(events.post_create_case, case=instance)
-        return instance
-
-    class Meta(CaseSerializer.Meta):
         fields = ["id", "workflow", "meta", "parent_work_item", "form", "context"]
         extra_kwargs = {"id": {"read_only": False, "required": False}}
 
 
-class CancelCaseSerializer(SendEventSerializerMixin, ContextModelSerializer):
+class CancelCaseSerializer(ContextModelSerializer):
     id = serializers.GlobalIDField()
 
     class Meta:
         model = models.Case
         fields = ["id", "context"]
 
     def validate(self, data):
@@ -280,15 +261,15 @@
         )
 
         domain_logic.CancelCaseLogic.post_cancel(case, user, self.context_data)
 
         return case
 
 
-class SuspendCaseSerializer(SendEventSerializerMixin, ContextModelSerializer):
+class SuspendCaseSerializer(ContextModelSerializer):
     id = serializers.GlobalIDField()
 
     class Meta:
         model = models.Case
         fields = ["id", "context"]
 
     def validate(self, data):
@@ -311,15 +292,15 @@
         )
 
         domain_logic.SuspendCaseLogic.post_suspend(case, user, self.context_data)
 
         return case
 
 
-class ResumeCaseSerializer(SendEventSerializerMixin, ContextModelSerializer):
+class ResumeCaseSerializer(ContextModelSerializer):
     id = serializers.GlobalIDField()
 
     class Meta:
         model = models.Case
         fields = ["id", "context"]
 
     def validate(self, data):
@@ -342,15 +323,15 @@
         )
 
         domain_logic.ResumeCaseLogic.post_resume(case, user, self.context_data)
 
         return case
 
 
-class ReopenCaseSerializer(SendEventSerializerMixin, ContextModelSerializer):
+class ReopenCaseSerializer(ContextModelSerializer):
     id = serializers.GlobalIDField()
     work_items = ListField(child=serializers.GlobalIDField(), required=True)
 
     class Meta:
         model = models.Case
         fields = ["id", "work_items", "context"]
 
@@ -378,15 +359,15 @@
 
 class CompleteWorkItemSerializer(ContextModelSerializer):
     id = serializers.GlobalIDField()
 
     def validate(self, data):
         try:
             domain_logic.CompleteWorkItemLogic.validate_for_complete(
-                self.instance, self.context["request"].user
+                self.instance, self.context["request"].user, context=data.get("context")
             )
         except ValidationError as e:
             raise exceptions.ValidationError(str(e))
 
         return super().validate(data)
 
     @transaction.atomic
@@ -467,40 +448,29 @@
         return work_item
 
     class Meta:
         model = models.WorkItem
         fields = ["id", "context"]
 
 
-class SaveWorkItemSerializer(SendEventSerializerMixin, ContextModelSerializer):
+class SaveWorkItemSerializer(ContextModelSerializer):
     work_item = serializers.GlobalIDField(source="id")
     name = CharField(
         required=False,
         allow_blank=True,
         allow_null=True,
         help_text=models.WorkItem._meta.get_field("name").help_text,
     )
     description = CharField(
         required=False,
         allow_blank=True,
         allow_null=True,
         help_text=models.WorkItem._meta.get_field("description").help_text,
     )
 
-    @transaction.atomic
-    def update(self, instance, validated_data):
-        self.send_event(
-            events.pre_create_work_item,
-            work_item=instance,
-            validated_data=validated_data,
-        )
-        instance = super().update(instance, validated_data)
-        self.send_event(events.post_create_work_item, work_item=instance)
-        return instance
-
     class Meta:
         model = models.WorkItem
         fields = [
             "work_item",
             "name",
             "description",
             "assigned_users",
```

### Comparing `caluma-8.0.0b9/caluma/caluma_workflow/utils.py` & `caluma-9.0.0/caluma/caluma_workflow/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -102,14 +102,32 @@
                         models.WorkItem.STATUS_SUSPENDED,
                     ],
                 ).exists()
             ):
                 # work item already exists, do not create a new one
                 continue
 
+            work_items_to_redo = models.WorkItem.objects.filter(
+                addressed_groups=groups,
+                controlling_groups=controlling_groups,
+                task_id=task.pk,
+                case=case,
+                status=models.WorkItem.STATUS_REDO,
+            )
+
+            if work_items_to_redo.exists():
+                for work_item in work_items_to_redo:
+                    work_item.deadline = task.calculate_deadline()
+                    work_item.modified_by_user = user.username
+                    work_item.modified_by_group = user.username
+                    work_item.status = models.WorkItem.STATUS_READY
+                    work_item.save()
+                    work_items.append(work_item)
+                continue
+
             work_items.append(
                 models.WorkItem.objects.create(
                     addressed_groups=groups,
                     controlling_groups=controlling_groups,
                     task_id=task.pk,
                     deadline=task.calculate_deadline(),
                     document=Document.objects.create_document_for_task(task, user),
```

### Comparing `caluma-8.0.0b9/caluma/caluma_workflow/visibilities.py` & `caluma-9.0.0/caluma/caluma_workflow/visibilities.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b9/caluma/conftest.py` & `caluma-9.0.0/caluma/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import contextlib
 import datetime
 import functools
 import inspect
 import sys
+from collections import defaultdict
 
 import pytest
 import urllib3
 from django.apps import apps
 from django.core.cache import cache
+from django.db import connection
+from django.db.migrations.executor import MigrationExecutor
 from factory import Faker
 from factory.base import FactoryMetaClass
 from graphene import ResolveInfo
 from minio import Minio
 from minio.datatypes import Object as MinioStatObject
 from pytest_factoryboy import register
 from pytest_factoryboy.fixture import Box
@@ -341,15 +344,15 @@
             )
             fallback_factory(
                 form_question_factory, form=form, question=questions["form"]
             )
             questions["sub_question"] = fallback_factory(
                 question_factory,
                 slug="sub_question",
-                type="text",
+                type="integer",
                 is_required="true",
                 is_hidden="false",
             )
             fallback_factory(
                 form_question_factory, form=sub_form, question=questions["sub_question"]
             )
 
@@ -407,7 +410,32 @@
     def make_context(date):
         old_now = datetime.datetime.now()
         freezer.move_to(date)
         yield
         freezer.move_to(old_now)
 
     return make_context
+
+
+@pytest.fixture
+def post_migrate_to_current_state(transactional_db):
+    """
+    Apply all current migrations after test has run.
+
+    In migration-tests, the `transactional_db` fixture seems to fail to apply the
+    newest migrations for all apps, leading to flaky tests. This fixture makes sure,
+    that all apps are migrated to their most current state.
+    """
+    try:
+        yield
+    finally:
+        executor = MigrationExecutor(connection)
+        migrations_dict = defaultdict(list)
+        for app, migration in executor.loader.disk_migrations.keys():
+            migrations_dict[app].append(migration)
+
+        migrations_list = [
+            (app, max(migrations)) for app, migrations in migrations_dict.items()
+        ]
+        executor.loader.build_graph()
+        executor.migrate(migrations_list)
+        executor.loader.build_graph()
```

### Comparing `caluma-8.0.0b9/caluma/schema.py` & `caluma-9.0.0/caluma/schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,23 +44,23 @@
     form_schema.DynamicMultipleChoiceQuestion,
     form_schema.TextareaQuestion,
     form_schema.FloatQuestion,
     form_schema.IntegerQuestion,
     form_schema.DateQuestion,
     form_schema.TableQuestion,
     form_schema.FormQuestion,
-    form_schema.FileQuestion,
+    form_schema.FilesQuestion,
     form_schema.StaticQuestion,
     form_schema.StringAnswer,
     form_schema.ListAnswer,
     form_schema.IntegerAnswer,
     form_schema.FloatAnswer,
     form_schema.DateAnswer,
     form_schema.TableAnswer,
-    form_schema.FileAnswer,
+    form_schema.FilesAnswer,
     form_schema.CalculatedFloatQuestion,
     form_schema.ActionButtonQuestion,
     workflow_schema.SimpleTask,
     workflow_schema.CompleteWorkflowFormTask,
     workflow_schema.CompleteTaskFormTask,
     analytics_schema.AnalyticsTable,
     analytics_schema.AnalyticsField,
@@ -69,15 +69,15 @@
 historical_types = [
     form_historical_schema.HistoricalStringAnswer,
     form_historical_schema.HistoricalListAnswer,
     form_historical_schema.HistoricalIntegerAnswer,
     form_historical_schema.HistoricalFloatAnswer,
     form_historical_schema.HistoricalDateAnswer,
     form_historical_schema.HistoricalTableAnswer,
-    form_historical_schema.HistoricalFileAnswer,
+    form_historical_schema.HistoricalFilesAnswer,
 ]
 
 if settings.ENABLE_HISTORICAL_API:
     types += historical_types
     query_inherit_from.append(form_historical_schema.Query)
```

### Comparing `caluma-8.0.0b9/caluma/settings/caluma.py` & `caluma-9.0.0/caluma/settings/caluma.py`

 * *Files 10% similar despite different names*

```diff
@@ -54,22 +54,21 @@
 
 # OpenID connect
 
 OIDC_USERINFO_ENDPOINT = env.str("OIDC_USERINFO_ENDPOINT", default=None)
 OIDC_VERIFY_SSL = env.bool("OIDC_VERIFY_SSL", default=True)
 OIDC_GROUPS_CLAIM = env.str("OIDC_GROUPS_CLAIM", default="caluma_groups")
 OIDC_USERNAME_CLAIM = env.str("OIDC_USERNAME_CLAIM", default="sub")
+# Claim to use for the "client" claim. Should normally be left to the default value
+OIDC_CLIENT_CLAIM = env.str("OIDC_CLIENT_CLAIM", default="client_id")
+
 OIDC_BEARER_TOKEN_REVALIDATION_TIME = env.int(
     "OIDC_BEARER_TOKEN_REVALIDATION_TIME", default=0
 )
 
-OIDC_INTROSPECT_ENDPOINT = env.str("OIDC_INTROSPECT_ENDPOINT", default=None)
-OIDC_INTROSPECT_CLIENT_ID = env.str("OIDC_INTROSPECT_CLIENT_ID", default=None)
-OIDC_INTROSPECT_CLIENT_SECRET = env.str("OIDC_INTROSPECT_CLIENT_SECRET", default=None)
-
 CALUMA_OIDC_USER_FACTORY = env.str(
     "CALUMA_OIDC_USER_FACTORY", default="caluma.caluma_user.models.OIDCUser"
 )
 
 
 # Extensions
```

### Comparing `caluma-8.0.0b9/caluma/settings/django.py` & `caluma-9.0.0/caluma/settings/django.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,22 @@
     "caluma.caluma_workflow.apps.DefaultConfig",
     "caluma.caluma_data_source.apps.DefaultConfig",
     "caluma.caluma_logging.apps.DefaultConfig",
     "watchman",
 ]
 
 if DEBUG:
-    INSTALLED_APPS.append("django_extensions")
+    try:
+        __import__("django_extensions")
+        INSTALLED_APPS.append("django_extensions")
+    except ImportError:  # pragma: no cover
+        # Nothing bad, just won't have django-extensions
+        # niceties installed (Most likely Caluma was built)
+        # without dev dependencies
+        pass
 
 MIDDLEWARE = [
     "django.middleware.security.SecurityMiddleware",
     "corsheaders.middleware.CorsMiddleware",
     "django.middleware.common.CommonMiddleware",
     "django.middleware.locale.LocaleMiddleware",
     "simple_history.middleware.HistoryRequestMiddleware",
```

### Comparing `caluma-8.0.0b9/caluma/utils.py` & `caluma-9.0.0/caluma/utils.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b9/pyproject.toml` & `caluma-9.0.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "caluma"
-version = "8.0.0-beta.9"
+version = "9.0.0"
 description = "Caluma Service providing GraphQL API"
 homepage = "https://caluma.io"
 repository = "https://github.com/projectcaluma/caluma"
 documentation = "https://caluma.gitbook.io/"
 authors = ["Caluma <info@caluma.io>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
@@ -16,67 +16,70 @@
 ]
 include = ["CHANGELOG.md"]
 exclude = [
     "caluma/**/tests",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.8.1"
 dateparser = "^1.1.0"
-Django = "^3.2.12"
+Django = "^3.2.19"
 django-cors-headers = "^3.11.0"
-django-environ = "^0.9.0"
-django-extensions = "^3.1.5"
-django-filter = "^22.1"
+django-environ = "^0.10.0"
+django-filter = "^23.1"
 django-localized-fields = "^6.6"
 django-postgres-extra = "^2.0.4"
 django-watchman = "^1.2.0"
 djangorestframework = "^3.13.1"
 django-simple-history = "^3.0.0"
-graphene-django = "^3.0.0b7"
+graphene-django = "3.0.0b7"
 graphql-relay = "^3.1.5"
 idna = "^3.3"
 minio = "^7.1.4"
 psycopg2-binary = "^2.9.3"
 pyjexl = "^0.3.0"
 python-memcached = "^1.59"
 requests = "^2.27.1"
 urllib3 = "^1.26.8"
 uWSGI = "^2.0.20"
 graphql-core = "~3.1.7"
 
-[tool.poetry.dev-dependencies]
-black = "22.3.0"
+[tool.poetry.group.dev.dependencies]
+# Dev dependencies are always pinned to an exact version (No caret or tilde
+# matching) to ensure everyone uses the same version of the tools, especially
+# linters & formatters
+black = "23.3.0"
+django-extensions = "3.2.1"
 factory-boy = "3.2.1"
-Faker = "13.14.0"
-flake8 = "4.0.1"
-flake8-bugbear = "22.6.22"
+Faker = "18.7.0"
+flake8 = "6.0.0"
+flake8-bugbear = "23.5.9"
 flake8-debugger = "4.1.2"
-flake8-docstrings = "1.6.0"
-flake8-isort = "4.1.1"
+flake8-docstrings = "1.7.0"
+flake8-isort = "6.0.0"
 flake8-string-format = "0.3.0"
 flake8-tuple = "0.4.1"
-gitlint = "0.17.0"
-isort = "5.10.1"
+gitlint = "0.19.1"
+isort = "5.12.0"
 pdbpp = "0.10.3"
-pre-commit = "2.19.0"
-pydocstyle = "6.1.1"
-pytest = "7.1.2"
-pytest-cov = "3.0.0"
+pre-commit = "3.3.1"
+pydocstyle = "6.3.0"
+pytest = "7.3.1"
+pytest-cov = "4.0.0"
 pytest-django = "4.5.2"
-pytest-env = "0.6.2"
-pytest-factoryboy = "2.5.0"
+pytest-env = "0.8.1"
+pytest-factoryboy = "2.5.1"
 pytest-freezegun = "0.4.2"
-pytest-mock = "3.7.0"
+pytest-mock = "3.10.0"
 pytest-randomly = "3.12.0"
-pytest-xdist = "2.5.0"
-python-semantic-release = "7.29.2"
-requests-mock = "1.9.3"
-reuse = "1.0.0"
-syrupy = "2.3.0"
+pytest-xdist = "3.2.1"
+python-semantic-release = "7.33.3"
+requests-mock = "1.10.0"
+reuse = "1.1.2"
+syrupy = "4.0.2"
 
 [tool.isort]
 skip = [
   "migrations",
   "snapshots",
 ]
 known_first_party = ["caluma"]
@@ -89,27 +92,29 @@
 
 [tool.pytest.ini_options]
 addopts = "-n auto --reuse-db --randomly-seed=1521188766 --randomly-dont-reorganize"
 DJANGO_SETTINGS_MODULE = "caluma.settings.django"
 env = [
     "META_FIELDS=test-key,foobar",
     "OIDC_USERINFO_ENDPOINT=mock://caluma.io/openid/userinfo",
-    "OIDC_INTROSPECT_ENDPOINT=mock://caluma.io/openid/introspect",
     "OIDC_BEARER_TOKEN_REVALIDATION_TIME=60",
     "LANGUAGES=en,de,fr",
     "ENABLE_HISTORICAL_API=true",
     "ENABLE_ACCESS_LOG=true",
     "ENABLE_HEALTHZ_ENDPOINT=true",
 ]
 filterwarnings = [
     "error::DeprecationWarning",
     "error::PendingDeprecationWarning",
     "ignore:The 'arrayconnection' module is deprecated:DeprecationWarning", # deprecation in graphene
     "ignore:distutils Version classes are deprecated:DeprecationWarning", # deprecation in pytest-freezegun
+    "ignore:'django_extensions' defines default_app_config:PendingDeprecationWarning", # deprecation in django_extensions
     "ignore::requests.packages.urllib3.exceptions.InsecureRequestWarning", # MinIO tests do "insecure" requests - that's ok
+    "ignore:invalid escape sequence",
+    "ignore:pkg_resources is deprecated as an API:DeprecationWarning", # deprecation in django-simple-history
 ]
 
 [tool.coverage.run]
 source = ["."]
 
 [tool.coverage.report]
 fail_under = 100
```

### Comparing `caluma-8.0.0b9/PKG-INFO` & `caluma-9.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
 Name: caluma
-Version: 8.0.0b9
+Version: 9.0.0
 Summary: Caluma Service providing GraphQL API
 Home-page: https://caluma.io
 License: GPL-3.0-or-later
 Author: Caluma
 Author-email: info@caluma.io
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: Django (>=3.2.12,<4.0.0)
+Requires-Dist: Django (>=3.2.19,<4.0.0)
 Requires-Dist: dateparser (>=1.1.0,<2.0.0)
 Requires-Dist: django-cors-headers (>=3.11.0,<4.0.0)
-Requires-Dist: django-environ (>=0.9.0,<0.10.0)
-Requires-Dist: django-extensions (>=3.1.5,<4.0.0)
-Requires-Dist: django-filter (>=22.1,<23.0)
+Requires-Dist: django-environ (>=0.10.0,<0.11.0)
+Requires-Dist: django-filter (>=23.1,<24.0)
 Requires-Dist: django-localized-fields (>=6.6,<7.0)
 Requires-Dist: django-postgres-extra (>=2.0.4,<3.0.0)
 Requires-Dist: django-simple-history (>=3.0.0,<4.0.0)
 Requires-Dist: django-watchman (>=1.2.0,<2.0.0)
 Requires-Dist: djangorestframework (>=3.13.1,<4.0.0)
-Requires-Dist: graphene-django (>=3.0.0b7,<4.0.0)
+Requires-Dist: graphene-django (==3.0.0b7)
 Requires-Dist: graphql-core (>=3.1.7,<3.2.0)
 Requires-Dist: graphql-relay (>=3.1.5,<4.0.0)
 Requires-Dist: idna (>=3.3,<4.0)
 Requires-Dist: minio (>=7.1.4,<8.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.3,<3.0.0)
 Requires-Dist: pyjexl (>=0.3.0,<0.4.0)
 Requires-Dist: python-memcached (>=1.59,<2.0)
```

