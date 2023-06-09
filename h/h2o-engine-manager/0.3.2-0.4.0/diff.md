# Comparing `tmp/h2o_engine_manager-0.3.2.tar.gz` & `tmp/h2o_engine_manager-0.4.0.tar.gz`

## Comparing `h2o_engine_manager-0.3.2.tar` & `h2o_engine_manager-0.4.0.tar`

### file list

```diff
@@ -1,265 +1,272 @@
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/Makefile
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/requirements.txt
--rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/docs/templates/config.mako
--rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/docs/templates/text.mako
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/local/ambassador_host.yaml
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/local/example.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/.openapi-generator-ignore
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/__init__.py
--rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/login.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/__init__.py
--rw-r--r--   0        0        0     5086 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/connection_config.py
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/exception.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/h2o_cli_config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/convert/__init__.py
--rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/convert/duration_convertor.py
--rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/convert/quantity_convertor.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/dai_engine/__init__.py
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/dai_engine/client_info.py
--rw-r--r--   0        0        0    20406 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/dai_engine/dai_engine.py
--rw-r--r--   0        0        0    19525 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/dai_engine/dai_engine_client.py
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/dai_engine/dai_engine_page.py
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/dai_engine/dai_engine_state.py
--rw-r--r--   0        0        0     9330 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/dai_engine/expression.py
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/dai_engine/token_api_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/dai_engine_constraint/__init__.py
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/dai_engine_constraint/client.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/dai_engine_constraint/token_api_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/dai_version/__init__.py
--rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/dai_version/client.py
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/dai_version/dai_version.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/dai_version/mapper.py
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/dai_version/page.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/dai_version/token_api_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/engine/__init__.py
--rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/engine/client.py
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/engine/engine.py
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/engine/mapper.py
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/engine/page.py
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/engine/state.py
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/engine/token_api_client.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/engine/type.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/h2o_engine/__init__.py
--rw-r--r--   0        0        0    17952 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/h2o_engine/client.py
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/h2o_engine/client_info.py
--rw-r--r--   0        0        0    11551 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/h2o_engine/h2o_engine.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/h2o_engine/page.py
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/h2o_engine/state.py
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/h2o_engine/token_api_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/h2o_engine_constraint/__init__.py
--rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/h2o_engine_constraint/client.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/h2o_engine_constraint/token_api_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/h2o_version/__init__.py
--rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/h2o_version/client.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/h2o_version/h2o_version.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/h2o_version/mapper.py
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/h2o_version/page.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/h2o_version/token_api_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/__init__.py
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/__init__.py
--rw-r--r--   0        0        0    39546 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/api_client.py
--rw-r--r--   0        0        0    16369 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/configuration.py
--rw-r--r--   0        0        0     5157 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/exceptions.py
--rw-r--r--   0        0        0    82609 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model_utils.py
--rw-r--r--   0        0        0    14403 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/rest.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/api/__init__.py
--rw-r--r--   0        0        0     6750 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/api/dai_engine_constraint_set_service_api.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/apis/__init__.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/__init__.py
--rw-r--r--   0        0        0    14231 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/protobuf_any.py
--rw-r--r--   0        0        0    12185 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/rpc_status.py
--rw-r--r--   0        0        0    12365 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/v1_constraint_duration.py
--rw-r--r--   0        0        0    12362 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/v1_constraint_numeric.py
--rw-r--r--   0        0        0    13685 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/v1_dai_engine_constraint_set.py
--rw-r--r--   0        0        0    12067 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/v1_get_dai_engine_constraint_set_response.py
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/models/__init__.py
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/__init__.py
--rw-r--r--   0        0        0    39350 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/api_client.py
--rw-r--r--   0        0        0    16324 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/configuration.py
--rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/exceptions.py
--rw-r--r--   0        0        0    82579 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/model_utils.py
--rw-r--r--   0        0        0    14373 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/rest.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/api/__init__.py
--rw-r--r--   0        0        0    67367 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/api/dai_engine_service_api.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/apis/__init__.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/model/__init__.py
--rw-r--r--   0        0        0    12791 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/model/api_http_body.py
--rw-r--r--   0        0        0    20707 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_resource.py
--rw-r--r--   0        0        0    11715 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_service_migrate_creator_request.py
--rw-r--r--   0        0        0    11758 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_service_pause_dai_engine_request.py
--rw-r--r--   0        0        0    11761 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_service_resume_dai_engine_request.py
--rw-r--r--   0        0        0    11879 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_service_upgrade_version_request.py
--rw-r--r--   0        0        0    14186 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/model/protobuf_any.py
--rw-r--r--   0        0        0    12125 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/model/rpc_status.py
--rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/model/v1_create_dai_engine_response.py
--rw-r--r--   0        0        0    20949 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine.py
--rw-r--r--   0        0        0    11821 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine_service_download_logs_response.py
--rw-r--r--   0        0        0    11856 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine_service_migrate_creator_response.py
--rw-r--r--   0        0        0    11856 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine_service_upgrade_version_response.py
--rw-r--r--   0        0        0    14589 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine_state.py
--rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/model/v1_delete_dai_engine_response.py
--rw-r--r--   0        0        0    11802 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/model/v1_get_dai_engine_response.py
--rw-r--r--   0        0        0    12669 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/model/v1_list_dai_engines_response.py
--rw-r--r--   0        0        0    11808 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/model/v1_pause_dai_engine_response.py
--rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/model/v1_resume_dai_engine_response.py
--rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/model/v1_update_dai_engine_response.py
--rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/models/__init__.py
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_version_service/__init__.py
--rw-r--r--   0        0        0    39360 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_version_service/api_client.py
--rw-r--r--   0        0        0    16327 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_version_service/configuration.py
--rw-r--r--   0        0        0     5143 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_version_service/exceptions.py
--rw-r--r--   0        0        0    82581 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_version_service/model_utils.py
--rw-r--r--   0        0        0    14375 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_version_service/rest.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_version_service/api/__init__.py
--rw-r--r--   0        0        0     8609 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_version_service/api/dai_version_service_api.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_version_service/apis/__init__.py
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_version_service/model/__init__.py
--rw-r--r--   0        0        0    14189 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_version_service/model/protobuf_any.py
--rw-r--r--   0        0        0    12129 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_version_service/model/rpc_status.py
--rw-r--r--   0        0        0    13076 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_version_service/model/v1_dai_version.py
--rw-r--r--   0        0        0    12692 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_version_service/model/v1_list_dai_versions_response.py
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_version_service/models/__init__.py
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/engine_service/__init__.py
--rw-r--r--   0        0        0    39287 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/engine_service/api_client.py
--rw-r--r--   0        0        0    16312 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/engine_service/configuration.py
--rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/engine_service/exceptions.py
--rw-r--r--   0        0        0    82571 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/engine_service/model_utils.py
--rw-r--r--   0        0        0    14365 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/engine_service/rest.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/engine_service/api/__init__.py
--rw-r--r--   0        0        0    11137 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/engine_service/api/engine_service_api.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/engine_service/apis/__init__.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/engine_service/model/__init__.py
--rw-r--r--   0        0        0    14174 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/engine_service/model/protobuf_any.py
--rw-r--r--   0        0        0    12109 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/engine_service/model/rpc_status.py
--rw-r--r--   0        0        0    18744 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/engine_service/model/v1_engine.py
--rw-r--r--   0        0        0    14456 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/engine_service/model/v1_engine_state.py
--rw-r--r--   0        0        0    12642 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/engine_service/model/v1_engine_type.py
--rw-r--r--   0        0        0    12591 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/engine_service/model/v1_list_engines_response.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/engine_service/models/__init__.py
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/__init__.py
--rw-r--r--   0        0        0    39550 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/api_client.py
--rw-r--r--   0        0        0    16369 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/configuration.py
--rw-r--r--   0        0        0     5157 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/exceptions.py
--rw-r--r--   0        0        0    82609 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model_utils.py
--rw-r--r--   0        0        0    14403 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/rest.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/api/__init__.py
--rw-r--r--   0        0        0     6756 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/api/h2_o_engine_constraint_set_service_api.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/apis/__init__.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/__init__.py
--rw-r--r--   0        0        0    14231 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/protobuf_any.py
--rw-r--r--   0        0        0    12185 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/rpc_status.py
--rw-r--r--   0        0        0    12365 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/v1_constraint_duration.py
--rw-r--r--   0        0        0    12362 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/v1_constraint_numeric.py
--rw-r--r--   0        0        0    12068 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/v1_get_h2_o_engine_constraint_set_response.py
--rw-r--r--   0        0        0    13415 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/v1_h2_o_engine_constraint_set.py
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/models/__init__.py
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_service/__init__.py
--rw-r--r--   0        0        0    39354 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_service/api_client.py
--rw-r--r--   0        0        0    16324 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_service/configuration.py
--rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_service/exceptions.py
--rw-r--r--   0        0        0    82579 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_service/model_utils.py
--rw-r--r--   0        0        0    14373 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_service/rest.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_service/api/__init__.py
--rw-r--r--   0        0        0    35542 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_service/api/h2_o_engine_service_api.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_service/apis/__init__.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_service/model/__init__.py
--rw-r--r--   0        0        0    12791 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_service/model/api_http_body.py
--rw-r--r--   0        0        0    14186 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_service/model/protobuf_any.py
--rw-r--r--   0        0        0    12125 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_service/model/rpc_status.py
--rw-r--r--   0        0        0    11812 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_create_h2_o_engine_response.py
--rw-r--r--   0        0        0    11812 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_delete_h2_o_engine_response.py
--rw-r--r--   0        0        0    11803 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_get_h2_o_engine_response.py
--rw-r--r--   0        0        0    19101 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_h2_o_engine.py
--rw-r--r--   0        0        0    11821 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_h2_o_engine_service_download_logs_response.py
--rw-r--r--   0        0        0    14501 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_h2_o_engine_state.py
--rw-r--r--   0        0        0    12670 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_list_h2_o_engines_response.py
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_service/models/__init__.py
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_version_service/__init__.py
--rw-r--r--   0        0        0    39364 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_version_service/api_client.py
--rw-r--r--   0        0        0    16327 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_version_service/configuration.py
--rw-r--r--   0        0        0     5143 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_version_service/exceptions.py
--rw-r--r--   0        0        0    82581 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_version_service/model_utils.py
--rw-r--r--   0        0        0    14375 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_version_service/rest.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_version_service/api/__init__.py
--rw-r--r--   0        0        0     8617 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_version_service/api/h2_o_version_service_api.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_version_service/apis/__init__.py
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_version_service/model/__init__.py
--rw-r--r--   0        0        0    14189 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_version_service/model/protobuf_any.py
--rw-r--r--   0        0        0    12129 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_version_service/model/rpc_status.py
--rw-r--r--   0        0        0    13036 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_version_service/model/v1_h2_o_version.py
--rw-r--r--   0        0        0    12693 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_version_service/model/v1_list_h2_o_versions_response.py
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_version_service/models/__init__.py
--rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/conftest.py
--rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/setup.py
--rw-r--r--   0        0        0     4855 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/test_admission_webhook.py
--rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/api/dai/create_dai_request.py
--rw-r--r--   0        0        0     5786 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/api/dai/test_create.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/api/dai/test_delete.py
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/api/dai/test_get.py
--rw-r--r--   0        0        0     5144 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/api/dai/test_list.py
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/api/dai/test_list_versions.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/api/dai/test_upgrade_available.py
--rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/api/dai_engine_constraint/test_get_dai_engine_constraint.py
--rw-r--r--   0        0        0     6149 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/api/engine/test_list_engines.py
--rw-r--r--   0        0        0     3952 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/api/h2o/test_create_h2o_engine.py
--rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/api/h2o/test_delete_h2o_engine.py
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/api/h2o/test_get_h2o_engine.py
--rw-r--r--   0        0        0     3521 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/api/h2o/test_list_h2o_engines.py
--rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/api/h2o/test_list_h2o_versions.py
--rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/api/h2o_engine_constraint/test_get_h2o_engine_constraint.py
--rw-r--r--   0        0        0     4938 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/e2e/dai/test_connect.py
--rw-r--r--   0        0        0    11667 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/e2e/dai/test_dai_pod_template_spec.py
--rw-r--r--   0        0        0     8695 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/e2e/dai/test_dai_resume.py
--rw-r--r--   0        0        0     5007 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/e2e/dai/test_lifecycle.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/e2e/dai/test_login_discovery.py
--rw-r--r--   0        0        0     2286 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/e2e/dai/test_migrate_creator.py
--rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/e2e/dai/test_migration.py
--rw-r--r--   0        0        0     7241 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/e2e/dai/test_update.py
--rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/e2e/dai/test_upgrade_version.py
--rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/e2e/h2o/test_h2o_engine_lifecycle.py
--rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/e2e/h2o/test_h2o_logs.py
--rw-r--r--   0        0        0     5080 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/e2e/h2o/test_h2o_pod_template_spec.py
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/test_data/dai_setups/dai-connect.yaml
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/test_data/dai_setups/dai-lifecycle.yaml
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/test_data/dai_setups/dai-mocked-server-logs.yaml
--rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/test_data/dai_setups/dai-setup.yaml
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/test_data/dai_setups/existing-dai-engine-constraint-set.yaml
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/test_data/dai_setups/list-generic-engines.yaml
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/test_data/dai_setups/system.default.yaml
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/test_data/dai_versions/1_10_4.yaml
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/test_data/dai_versions/1_10_5.yaml
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/test_data/dai_versions/1_10_5_do_not_use_me.yaml
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/test_data/dai_versions/1_10_6.yaml
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/test_data/dai_versions/1_10_6_1.yaml
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/test_data/dai_versions/1_10_6_1_aplha.yaml
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/test_data/h2o_setups/existing-h2o-engine-constraint-set.yaml
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/test_data/h2o_setups/h2o-setup.yaml
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/test_data/h2o_setups/list-generic-engines.yaml
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/test_data/h2o_setups/system.default.yaml
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/test_data/h2o_versions/0_0_0_0.yaml
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/test_data/h2o_versions/3_36_1_5.yaml
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/test_data/h2o_versions/3_38_0_1.yaml
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/test_data/h2o_versions/3_38_0_2.yaml
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/test_data/invalid_dai_setups/invalid-cpu-constraint.yaml
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/test_data/invalid_dai_setups/invalid-gpu-constraint.yaml
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/test_data/invalid_dai_setups/invalid-max-idle-duration-constraint.yaml
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/test_data/invalid_dai_versions/alias_and_version_conflict.yaml
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/test_data/invalid_dai_versions/invalid_version_format.yaml
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/test_data/invalid_dai_versions/repeated_alias.yaml
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/test_data/invalid_dai_versions/unsupported_version.yaml
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/test_data/sw_pods_creation/no_labels.yaml
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/integration/test_data/sw_pods_creation/unwanted_label.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/unit/__init__.py
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/unit/test_dai_engine.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/unit/test_duration_convertor.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/unit/test_engine_state.py
--rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/unit/test_filter.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/unit/test_h2o_cli_config.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/unit/test_quantity_convertor.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/unit/dai_version/__init__.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/unit/dai_version/test_mapper.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/tests/unit/test_data/h2o-cli-config.toml
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/.gitignore
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/README.md
--rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 h2o_engine_manager-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/Makefile
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/requirements.txt
+-rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/docs/templates/config.mako
+-rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/docs/templates/text.mako
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/local/ambassador_host.yaml
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/local/example.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/.openapi-generator-ignore
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/__init__.py
+-rw-r--r--   0        0        0     5086 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/connection_config.py
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/exception.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_cli_config.py
+-rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/login.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/convert/__init__.py
+-rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/convert/duration_convertor.py
+-rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/convert/quantity_convertor.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_engine/__init__.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_engine/client_info.py
+-rw-r--r--   0        0        0    21286 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_engine/dai_engine.py
+-rw-r--r--   0        0        0    19872 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_engine/dai_engine_client.py
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_engine/dai_engine_page.py
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_engine/dai_engine_state.py
+-rw-r--r--   0        0        0     9330 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_engine/expression.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_engine/token_api_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_engine_constraint/__init__.py
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_engine_constraint/client.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_engine_constraint/token_api_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_version/__init__.py
+-rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_version/client.py
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_version/dai_version.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_version/mapper.py
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_version/page.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_version/token_api_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/engine/__init__.py
+-rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/engine/client.py
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/engine/engine.py
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/engine/mapper.py
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/engine/page.py
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/engine/state.py
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/engine/token_api_client.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/engine/type.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/engine_id/__init__.py
+-rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/engine_id/generator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_engine/__init__.py
+-rw-r--r--   0        0        0    18472 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_engine/client.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_engine/client_info.py
+-rw-r--r--   0        0        0    12575 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_engine/h2o_engine.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_engine/page.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_engine/state.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_engine/token_api_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_engine_constraint/__init__.py
+-rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_engine_constraint/client.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_engine_constraint/token_api_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_version/__init__.py
+-rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_version/client.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_version/h2o_version.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_version/mapper.py
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_version/page.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_version/token_api_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/__init__.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/__init__.py
+-rw-r--r--   0        0        0    39546 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/api_client.py
+-rw-r--r--   0        0        0    16369 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/configuration.py
+-rw-r--r--   0        0        0     5157 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/exceptions.py
+-rw-r--r--   0        0        0    82609 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model_utils.py
+-rw-r--r--   0        0        0    14403 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/rest.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/api/__init__.py
+-rw-r--r--   0        0        0     6750 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/api/dai_engine_constraint_set_service_api.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/apis/__init__.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/__init__.py
+-rw-r--r--   0        0        0    14231 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/protobuf_any.py
+-rw-r--r--   0        0        0    12185 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/rpc_status.py
+-rw-r--r--   0        0        0    12365 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/v1_constraint_duration.py
+-rw-r--r--   0        0        0    12362 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/v1_constraint_numeric.py
+-rw-r--r--   0        0        0    13685 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/v1_dai_engine_constraint_set.py
+-rw-r--r--   0        0        0    12067 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/v1_get_dai_engine_constraint_set_response.py
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/models/__init__.py
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/__init__.py
+-rw-r--r--   0        0        0    39350 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/api_client.py
+-rw-r--r--   0        0        0    16324 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/configuration.py
+-rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/exceptions.py
+-rw-r--r--   0        0        0    82579 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model_utils.py
+-rw-r--r--   0        0        0    14373 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/rest.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/api/__init__.py
+-rw-r--r--   0        0        0    65707 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/api/dai_engine_service_api.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/apis/__init__.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/__init__.py
+-rw-r--r--   0        0        0    12791 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/api_http_body.py
+-rw-r--r--   0        0        0    21561 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_resource.py
+-rw-r--r--   0        0        0    11715 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_service_migrate_creator_request.py
+-rw-r--r--   0        0        0    11758 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_service_pause_dai_engine_request.py
+-rw-r--r--   0        0        0    11761 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_service_resume_dai_engine_request.py
+-rw-r--r--   0        0        0    11879 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_service_upgrade_version_request.py
+-rw-r--r--   0        0        0    14186 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/protobuf_any.py
+-rw-r--r--   0        0        0    12125 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/rpc_status.py
+-rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_create_dai_engine_response.py
+-rw-r--r--   0        0        0    21803 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine.py
+-rw-r--r--   0        0        0    11821 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine_service_download_logs_response.py
+-rw-r--r--   0        0        0    11856 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine_service_migrate_creator_response.py
+-rw-r--r--   0        0        0    11856 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine_service_upgrade_version_response.py
+-rw-r--r--   0        0        0    14589 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine_state.py
+-rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_delete_dai_engine_response.py
+-rw-r--r--   0        0        0    11802 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_get_dai_engine_response.py
+-rw-r--r--   0        0        0    12669 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_list_dai_engines_response.py
+-rw-r--r--   0        0        0    11808 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_pause_dai_engine_response.py
+-rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_resume_dai_engine_response.py
+-rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_update_dai_engine_response.py
+-rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/models/__init__.py
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_version_service/__init__.py
+-rw-r--r--   0        0        0    39360 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_version_service/api_client.py
+-rw-r--r--   0        0        0    16327 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_version_service/configuration.py
+-rw-r--r--   0        0        0     5143 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_version_service/exceptions.py
+-rw-r--r--   0        0        0    82581 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_version_service/model_utils.py
+-rw-r--r--   0        0        0    14375 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_version_service/rest.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_version_service/api/__init__.py
+-rw-r--r--   0        0        0     7911 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_version_service/api/dai_version_service_api.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_version_service/apis/__init__.py
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_version_service/model/__init__.py
+-rw-r--r--   0        0        0    14189 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_version_service/model/protobuf_any.py
+-rw-r--r--   0        0        0    12129 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_version_service/model/rpc_status.py
+-rw-r--r--   0        0        0    13076 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_version_service/model/v1_dai_version.py
+-rw-r--r--   0        0        0    12692 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_version_service/model/v1_list_dai_versions_response.py
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_version_service/models/__init__.py
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/__init__.py
+-rw-r--r--   0        0        0    39287 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/api_client.py
+-rw-r--r--   0        0        0    16312 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/configuration.py
+-rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/exceptions.py
+-rw-r--r--   0        0        0    82571 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/model_utils.py
+-rw-r--r--   0        0        0    14365 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/rest.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/api/__init__.py
+-rw-r--r--   0        0        0     9434 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/api/engine_service_api.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/apis/__init__.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/model/__init__.py
+-rw-r--r--   0        0        0    14174 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/model/protobuf_any.py
+-rw-r--r--   0        0        0    12109 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/model/rpc_status.py
+-rw-r--r--   0        0        0    20396 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/model/v1_engine.py
+-rw-r--r--   0        0        0    14456 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/model/v1_engine_state.py
+-rw-r--r--   0        0        0    12642 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/model/v1_engine_type.py
+-rw-r--r--   0        0        0    12591 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/model/v1_list_engines_response.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/models/__init__.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/__init__.py
+-rw-r--r--   0        0        0    39550 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/api_client.py
+-rw-r--r--   0        0        0    16369 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/configuration.py
+-rw-r--r--   0        0        0     5157 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/exceptions.py
+-rw-r--r--   0        0        0    82609 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model_utils.py
+-rw-r--r--   0        0        0    14403 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/rest.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/api/__init__.py
+-rw-r--r--   0        0        0     6756 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/api/h2_o_engine_constraint_set_service_api.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/apis/__init__.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/__init__.py
+-rw-r--r--   0        0        0    14231 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/protobuf_any.py
+-rw-r--r--   0        0        0    12185 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/rpc_status.py
+-rw-r--r--   0        0        0    12365 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/v1_constraint_duration.py
+-rw-r--r--   0        0        0    12362 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/v1_constraint_numeric.py
+-rw-r--r--   0        0        0    12068 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/v1_get_h2_o_engine_constraint_set_response.py
+-rw-r--r--   0        0        0    13670 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/v1_h2_o_engine_constraint_set.py
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/models/__init__.py
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/__init__.py
+-rw-r--r--   0        0        0    39354 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/api_client.py
+-rw-r--r--   0        0        0    16324 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/configuration.py
+-rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/exceptions.py
+-rw-r--r--   0        0        0    82579 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/model_utils.py
+-rw-r--r--   0        0        0    14373 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/rest.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/api/__init__.py
+-rw-r--r--   0        0        0    34374 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/api/h2_o_engine_service_api.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/apis/__init__.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/model/__init__.py
+-rw-r--r--   0        0        0    12791 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/model/api_http_body.py
+-rw-r--r--   0        0        0    14186 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/model/protobuf_any.py
+-rw-r--r--   0        0        0    12125 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/model/rpc_status.py
+-rw-r--r--   0        0        0    11812 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_create_h2_o_engine_response.py
+-rw-r--r--   0        0        0    11812 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_delete_h2_o_engine_response.py
+-rw-r--r--   0        0        0    11803 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_get_h2_o_engine_response.py
+-rw-r--r--   0        0        0    20349 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_h2_o_engine.py
+-rw-r--r--   0        0        0    11821 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_h2_o_engine_service_download_logs_response.py
+-rw-r--r--   0        0        0    14501 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_h2_o_engine_state.py
+-rw-r--r--   0        0        0    12670 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_list_h2_o_engines_response.py
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/models/__init__.py
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_version_service/__init__.py
+-rw-r--r--   0        0        0    39364 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_version_service/api_client.py
+-rw-r--r--   0        0        0    16327 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_version_service/configuration.py
+-rw-r--r--   0        0        0     5143 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_version_service/exceptions.py
+-rw-r--r--   0        0        0    82581 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_version_service/model_utils.py
+-rw-r--r--   0        0        0    14375 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_version_service/rest.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_version_service/api/__init__.py
+-rw-r--r--   0        0        0     7919 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_version_service/api/h2_o_version_service_api.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_version_service/apis/__init__.py
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_version_service/model/__init__.py
+-rw-r--r--   0        0        0    14189 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_version_service/model/protobuf_any.py
+-rw-r--r--   0        0        0    12129 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_version_service/model/rpc_status.py
+-rw-r--r--   0        0        0    13036 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_version_service/model/v1_h2_o_version.py
+-rw-r--r--   0        0        0    12693 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_version_service/model/v1_list_h2_o_versions_response.py
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_version_service/models/__init__.py
+-rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/conftest.py
+-rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/setup.py
+-rw-r--r--   0        0        0     4855 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_admission_webhook.py
+-rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/api/dai/create_dai_request.py
+-rw-r--r--   0        0        0     6752 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/api/dai/test_create.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/api/dai/test_delete.py
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/api/dai/test_get.py
+-rw-r--r--   0        0        0     5171 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/api/dai/test_list.py
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/api/dai/test_list_versions.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/api/dai/test_upgrade_available.py
+-rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/api/dai_engine_constraint/test_get_dai_engine_constraint.py
+-rw-r--r--   0        0        0     6219 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/api/engine/test_list_engines.py
+-rw-r--r--   0        0        0     4993 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/api/h2o/test_create_h2o_engine.py
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/api/h2o/test_delete_h2o_engine.py
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/api/h2o/test_get_h2o_engine.py
+-rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/api/h2o/test_list_h2o_engines.py
+-rw-r--r--   0        0        0     2931 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/api/h2o/test_list_h2o_versions.py
+-rw-r--r--   0        0        0     2957 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/api/h2o_engine_constraint/test_get_h2o_engine_constraint.py
+-rw-r--r--   0        0        0     4938 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/e2e/dai/test_connect.py
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/e2e/dai/test_current_idle_running_duration.py
+-rw-r--r--   0        0        0    11667 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/e2e/dai/test_dai_pod_template_spec.py
+-rw-r--r--   0        0        0     8695 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/e2e/dai/test_dai_resume.py
+-rw-r--r--   0        0        0     5092 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/e2e/dai/test_lifecycle.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/e2e/dai/test_login_discovery.py
+-rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/e2e/dai/test_migrate_creator.py
+-rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/e2e/dai/test_migration.py
+-rw-r--r--   0        0        0     7152 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/e2e/dai/test_update.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/e2e/dai/test_upgrade_version.py
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/e2e/h2o/test_h2o_current_idle_running_duration.py
+-rw-r--r--   0        0        0     2111 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/e2e/h2o/test_h2o_engine_lifecycle.py
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/e2e/h2o/test_h2o_logs.py
+-rw-r--r--   0        0        0     5102 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/e2e/h2o/test_h2o_pod_template_spec.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/dai_setups/dai-connect.yaml
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/dai_setups/dai-lifecycle.yaml
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/dai_setups/dai-mocked-server-logs.yaml
+-rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/dai_setups/dai-setup.yaml
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/dai_setups/existing-dai-engine-constraint-set.yaml
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/dai_setups/list-generic-engines.yaml
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/dai_setups/system.default.yaml
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/dai_versions/1_10_4.yaml
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/dai_versions/1_10_5.yaml
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/dai_versions/1_10_5_do_not_use_me.yaml
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/dai_versions/1_10_5_mock.yaml
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/dai_versions/1_10_6.yaml
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/dai_versions/1_10_6_1.yaml
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/dai_versions/1_10_6_1_aplha.yaml
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/h2o_setups/existing-h2o-engine-constraint-set.yaml
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/h2o_setups/h2o-setup.yaml
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/h2o_setups/list-generic-engines.yaml
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/h2o_setups/system.default.yaml
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/h2o_versions/0_0_0_0.yaml
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/h2o_versions/0_0_0_0_latest.yaml
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/h2o_versions/3_36_1_5.yaml
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/h2o_versions/3_38_0_4.yaml
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/h2o_versions/3_40_0_4.yaml
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/invalid_dai_setups/invalid-cpu-constraint.yaml
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/invalid_dai_setups/invalid-gpu-constraint.yaml
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/invalid_dai_setups/invalid-max-idle-duration-constraint.yaml
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/invalid_dai_versions/alias_and_version_conflict.yaml
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/invalid_dai_versions/invalid_version_format.yaml
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/invalid_dai_versions/repeated_alias.yaml
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/invalid_dai_versions/unsupported_version.yaml
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/sw_pods_creation/no_labels.yaml
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/sw_pods_creation/unwanted_label.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/unit/__init__.py
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/unit/test_dai_engine.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/unit/test_duration_convertor.py
+-rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/unit/test_engine_id_generator.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/unit/test_engine_state.py
+-rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/unit/test_filter.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/unit/test_h2o_cli_config.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/unit/test_quantity_convertor.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/unit/dai_version/__init__.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/unit/dai_version/test_mapper.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/unit/test_data/h2o-cli-config.toml
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/README.md
+-rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/PKG-INFO
```

### Comparing `h2o_engine_manager-0.3.2/requirements.txt` & `h2o_engine_manager-0.4.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/docs/templates/config.mako` & `h2o_engine_manager-0.4.0/docs/templates/config.mako`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/docs/templates/text.mako` & `h2o_engine_manager-0.4.0/docs/templates/text.mako`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/local/example.py` & `h2o_engine_manager-0.4.0/local/example.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/login.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/login.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/connection_config.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/connection_config.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/exception.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/exception.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/h2o_cli_config.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_cli_config.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/convert/duration_convertor.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/convert/duration_convertor.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import re
+from typing import Optional
 
 suffix_values = {"d": 86400, "h": 3600, "m": 60, "s": 1}
 
 
 def duration_to_seconds(duration: str) -> str:
     """
     Converts duration specified in seconds, minutes, hours or days into a durating specified in seconds.
@@ -39,37 +40,44 @@
 
     if suffix:
         multiplier = suffix_values.get(suffix)
 
     return f"{num * multiplier}s"
 
 
+def none_seconds_to_duration(seconds: Optional[str]) -> Optional[str]:
+    if not seconds:
+        return None
+    return seconds_to_duration(seconds)
+
+
 def seconds_to_duration(seconds: str) -> str:
     """
     Converts seconds into a human-readable duration string. The highest possible duration unit will be
     applied.
 
     Args:
-        seconds: number of seconds followed with a `s` suffix.
+        seconds: number of seconds followed with a `s` suffix. Decimal values will be rounded down.
 
     Returns:
         string representing duration in highest possible unit available (up to `d` representing days).
 
     Examples:
         "1s" -> "1s"
+        "1.9s" -> "1s"
         "60s" -> "1m"
         "61s" -> "61s"
         "3600s" -> "1h"
         "3601s" -> "3601s"
     """
-    duration_regex = re.compile("^[0-9]+s$")
+    duration_regex = re.compile("^[0-9]+[.]?[0-9]*s$")
     if duration_regex.match(seconds) is None:
         raise ValueError(f"invalid duration format: {seconds}")
 
-    num = int(seconds.rstrip("s"))
+    num = int(float(seconds.rstrip("s")))
 
     for suffix in suffix_values.keys():
         multiplier = suffix_values.get(suffix)
 
         if num % multiplier == 0:
             return f"{int(num / multiplier)}{suffix}"
```

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/convert/quantity_convertor.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/convert/quantity_convertor.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/dai_engine/client_info.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_engine/client_info.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/dai_engine/dai_engine.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_engine/dai_engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,14 +66,16 @@
         resume_time: datetime = None,
         login_url: str = "",
         api_url: str = "",
         reconciling: bool = False,
         uid: str = "",
         upgrade_available: bool = False,
         client_info: ClientInfo = None,
+        current_running_duration: str = None,
+        current_idle_duration: str = None,
     ) -> None:
         self.version = version
         self.cpu = cpu
         self.gpu = gpu
         self.memory_bytes = memory_bytes
         self.storage_bytes = storage_bytes
         self.config = config
@@ -99,14 +101,16 @@
         self.workspace_id = ""
         self.engine_id = ""
         if name:
             self.workspace_id = self.name.split("/")[1]
             self.engine_id = self.name.split("/")[3]
 
         self.client_info = client_info
+        self.current_running_duration = current_running_duration
+        self.current_idle_duration = current_idle_duration
 
     def __repr__(self) -> str:
         return pprint.pformat(self.__dict__)
 
     def resume(self):
         """Resumes the engine and updates its data from the server response."""
         exc = None
@@ -456,22 +460,32 @@
         if self.max_idle_duration is not None:
             mid = duration_convertor.duration_to_seconds(self.max_idle_duration)
 
         mrd = None
         if self.max_running_duration is not None:
             mrd = duration_convertor.duration_to_seconds(self.max_running_duration)
 
+        cid = None
+        if self.current_idle_duration is not None:
+            cid = duration_convertor.duration_to_seconds(self.current_idle_duration)
+
+        crd = None
+        if self.current_running_duration is not None:
+            crd = duration_convertor.duration_to_seconds(self.current_running_duration)
+
         return V1DAIEngine._from_openapi_data(
             version=self.version,
             cpu=self.cpu,
             gpu=self.gpu,
             memory_bytes=mb,
             storage_bytes=sb,
             max_idle_duration=mid,
             max_running_duration=mrd,
+            current_idle_duration=cid,
+            current_running_duration=crd,
             display_name=self.display_name,
             name=self.name,
             state=self.state.to_api_object(),
             config=self.config,
             creator=self.creator,
             creator_display_name=self.creator_display_name,
             create_time=self.create_time,
@@ -553,8 +567,14 @@
         resume_time=api_engine.resume_time,
         login_url=api_engine.login_url,
         api_url=api_engine.api_url,
         reconciling=api_engine.reconciling,
         uid=api_engine.uid,
         upgrade_available=api_engine.upgrade_available,
         client_info=client_info,
+        current_idle_duration=duration_convertor.none_seconds_to_duration(
+            api_engine.current_idle_duration
+        ),
+        current_running_duration=duration_convertor.none_seconds_to_duration(
+            api_engine.current_running_duration
+        ),
     )
```

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/dai_engine/dai_engine_client.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_engine/dai_engine_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from h2o_engine_manager.clients.dai_engine.dai_engine import DAIEngine
 from h2o_engine_manager.clients.dai_engine.dai_engine import from_dai_engine_api_object
 from h2o_engine_manager.clients.dai_engine.dai_engine_page import DAIEnginesPage
 from h2o_engine_manager.clients.dai_engine.token_api_client import TokenApiClient
 from h2o_engine_manager.clients.dai_version.client import DAIVersionClient
 from h2o_engine_manager.clients.dai_version.dai_version import DAIVersion
 from h2o_engine_manager.clients.dai_version.page import DAIVersionsPage
+from h2o_engine_manager.clients.engine_id.generator import generate_engine_id
 from h2o_engine_manager.clients.exception import ApiException
 from h2o_engine_manager.gen.dai_engine_service import (
     ApiException as DAIEngineApiException,
 )
 from h2o_engine_manager.gen.dai_engine_service.api.dai_engine_service_api import (
     DAIEngineServiceApi,
 )
@@ -58,15 +59,15 @@
         Args:
             default_workspace_id (str): The workspace resource id to be used in subsequent requests.
         """
         self.default_workspace_id = default_workspace_id
 
     def create_engine(
         self,
-        engine_id: str,
+        engine_id: str = None,
         version: str = None,
         cpu: int = None,
         gpu: int = None,
         memory_bytes: str = None,
         storage_bytes: str = None,
         max_idle_duration: str = None,
         max_running_duration: str = None,
@@ -75,15 +76,16 @@
         config: Dict[str, str] = {},
         annotations: Dict[str, str] = {},
         validate_only: bool = False,
     ) -> DAIEngine:
         """Creates Driverless AI engine and initiates launch. Immediately returned engine had just begun launching.
 
         Args:
-            engine_id (str): The ID to use for the Driverless AI engine, which will become the final component of the engine's resource name.
+            engine_id (str, optional): The ID to use for the Driverless AI engine, which will become the final component of the engine's resource name.
+            If left unspecified, the client will generate a random value.
                 This value must:
 
                 - contain 1-63 characters
                 - contain only lowercase alphanumeric characters or hyphen ('-')
                 - start with an alphabetic character
                 - end with an alphanumeric character
             version (str, optional): Driverless AI version identifier. For example: "1.10.1" or "latest".
@@ -137,14 +139,17 @@
             )
 
         if max_running_duration is not None:
             max_running_duration = duration_convertor.duration_to_seconds(
                 max_running_duration
             )
 
+        if engine_id is None:
+            engine_id = generate_engine_id(display_name=display_name, workspace_id=workspace_id, engine_type="dai", engine_getter=self.get_engine)
+
         api_engine = APIEngine(
             version=version,
             cpu=cpu,
             gpu=gpu,
             memory_bytes=memory_bytes,
             storage_bytes=storage_bytes,
             config=config,
```

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/dai_engine/dai_engine_page.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_engine/dai_engine_page.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/dai_engine/dai_engine_state.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_engine/dai_engine_state.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/dai_engine/expression.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_engine/expression.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/dai_engine/token_api_client.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_engine/token_api_client.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/dai_engine_constraint/client.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_engine_constraint/client.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/dai_engine_constraint/token_api_client.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_engine_constraint/token_api_client.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/dai_version/client.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_version/client.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/dai_version/mapper.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_version/mapper.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/dai_version/page.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_version/page.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/dai_version/token_api_client.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_version/token_api_client.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/engine/client.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/engine/client.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/engine/engine.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/engine/engine.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/engine/mapper.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/engine/mapper.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/engine/page.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/engine/page.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/engine/state.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/engine/state.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/engine/token_api_client.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/engine/token_api_client.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/h2o_engine/client.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_engine/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Dict
 from typing import List
 
 from h2o_engine_manager.clients.connection_config import ConnectionConfig
 from h2o_engine_manager.clients.convert import duration_convertor
 from h2o_engine_manager.clients.convert import quantity_convertor
+from h2o_engine_manager.clients.engine_id.generator import generate_engine_id
 from h2o_engine_manager.clients.exception import ApiException
 from h2o_engine_manager.clients.h2o_engine.client_info import ClientInfo
 from h2o_engine_manager.clients.h2o_engine.h2o_engine import H2OEngine
 from h2o_engine_manager.clients.h2o_engine.h2o_engine import build_api_engine_name
 from h2o_engine_manager.clients.h2o_engine.h2o_engine import from_h2o_engine_api_object
 from h2o_engine_manager.clients.h2o_engine.page import H2OEnginesPage
 from h2o_engine_manager.clients.h2o_engine.token_api_client import TokenApiClient
@@ -49,43 +50,46 @@
             url=connection_config.aiem_url,
             token_provider=connection_config.token_provider,
             api_instance=api_instance,
         )
 
     def create_engine(
         self,
+        version: str,
         engine_id: str = None,
-        version: str = None,
+        node_count: int = None,
         cpu: int = None,
         gpu: int = None,
         memory_bytes: str = None,
         max_idle_duration: str = None,
         max_running_duration: str = None,
         workspace_id: str = "",
         display_name: str = "",
         annotations: Dict[str, str] = {},
         validate_only: bool = False,
     ) -> H2OEngine:
         """Creates H2O engine and initiates launch.
 
         Args:
-            engine_id (str): The ID to use for the H2O engine, which will become the final component of the engine's resource name.
+            version (str): Version identifier. For example "3.38.0.1".
+            engine_id (str, optional): The ID to use for the H2O engine, which will become the final component of the engine's resource name.
+                If left unspecified, the client will generate a random value.
                 This value must:
 
                 - contain 1-63 characters
                 - contain only lowercase alphanumeric characters or hyphen ('-')
                 - start with an alphabetic character
                 - end with an alphanumeric character
-            version (str, optional): Version identifier. For example "3.38.0.1".
+            node_count (int, optional): Number of nodes of the H2O cluster.
                 If not specified, a default value will be set by server.
-            cpu (int, optional): The amount of [CPU units](https://kubernetes.io/docs/concepts/configuration/manage-resources-containers/#meaning-of-cpu) allocated for the engine.
+            cpu (int, optional): The amount of [CPU units](https://kubernetes.io/docs/concepts/configuration/manage-resources-containers/#meaning-of-cpu) per node allocated for the engine.
                 If not specified, a default value will be set by server.
-            gpu (int, optional): Number of nvidia.com/gpu Kubernetes resource units.
+            gpu (int, optional): Number of nvidia.com/gpu Kubernetes resource units per node.
                 If not specified, a default value will be set by server.
-            memory_bytes (str, optional): Quantity of bytes. Example `8G`, `16Gi`.
+            memory_bytes (str, optional): The amount of memory per node. Quantity of bytes. Example `8G`, `16Gi`.
                 If not specified, a default value will be set by server.
                 Detailed syntax:
 
                 - [quantity] = [number][suffix]
                 - [suffix] = [binarySI] | [decimalSI]
                 - [binarySI] = Ki | Mi | Gi | Ti | Pi
                 - [decimalSI] = k | M | G | T | P
@@ -120,16 +124,21 @@
             )
 
         if max_running_duration is not None:
             max_running_duration = duration_convertor.duration_to_seconds(
                 max_running_duration
             )
 
+        if engine_id is None:
+            engine_id = generate_engine_id(display_name=display_name, workspace_id=workspace_id, engine_type="h2o", engine_getter=self.get_engine)
+
+
         api_engine = V1H2OEngine(
             version=version,
+            node_count=node_count,
             cpu=cpu,
             gpu=gpu,
             memory_bytes=memory_bytes,
             annotations=annotations,
             max_idle_duration=max_idle_duration,
             max_running_duration=max_running_duration,
             display_name=display_name,
```

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/h2o_engine/client_info.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_engine/client_info.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/h2o_engine/h2o_engine.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_engine/h2o_engine.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     port: int
 
 
 class H2OEngine:
     def __init__(
         self,
         version: str,
+        node_count: int,
         cpu: int,
         gpu: int,
         memory_bytes: str,
         annotations: Dict[str, str],
         max_idle_duration: str,
         max_running_duration: str,
         display_name: str,
@@ -52,16 +53,19 @@
         update_time: datetime = None,
         delete_time: datetime = None,
         login_url: str = "",
         api_url: str = "",
         reconciling: bool = False,
         uid: str = "",
         client_info: ClientInfo = None,
+        current_running_duration: str = None,
+        current_idle_duration: str = None,
     ) -> None:
         self.version = version
+        self.node_count = node_count
         self.cpu = cpu
         self.gpu = gpu
         self.memory_bytes = memory_bytes
         self.annotations = annotations
         self.max_idle_duration = max_idle_duration
         self.max_running_duration = max_running_duration
         self.display_name = display_name
@@ -81,14 +85,16 @@
         self.workspace_id = ""
         self.engine_id = ""
         if name:
             self.workspace_id = self.name.split("/")[1]
             self.engine_id = self.name.split("/")[3]
 
         self.client_info = client_info
+        self.current_running_duration = current_running_duration
+        self.current_idle_duration = current_idle_duration
 
     def __repr__(self) -> str:
         return pprint.pformat(self.__dict__)
 
     def delete(self, allow_missing: bool = False, validate_only: bool = False):
         """Initiates deletion of the engine from its workspace.
            Once the engine is deleted, any further action with the engine will result in an error.
@@ -139,21 +145,32 @@
         if self.max_idle_duration is not None:
             mid = duration_convertor.duration_to_seconds(self.max_idle_duration)
 
         mrd = None
         if self.max_running_duration is not None:
             mrd = duration_convertor.duration_to_seconds(self.max_running_duration)
 
+        cid = None
+        if self.current_idle_duration is not None:
+            cid = duration_convertor.duration_to_seconds(self.current_idle_duration)
+
+        crd = None
+        if self.current_running_duration is not None:
+            crd = duration_convertor.duration_to_seconds(self.current_running_duration)
+
         return V1H2OEngine._from_openapi_data(
             version=self.version,
+            node_count=self.node_count,
             cpu=self.cpu,
             gpu=self.gpu,
             memory_bytes=mb,
             max_idle_duration=mid,
             max_running_duration=mrd,
+            current_idle_duration=cid,
+            current_running_duration=crd,
             display_name=self.display_name,
             name=self.name,
             state=self.state.to_api_object(),
             creator=self.creator,
             creator_display_name=self.creator_display_name,
             create_time=self.create_time,
             update_time=self.update_time,
@@ -305,14 +322,15 @@
 
 
 def from_h2o_engine_api_object(
     client_info: ClientInfo, api_engine: V1H2OEngine
 ) -> H2OEngine:
     return H2OEngine(
         version=api_engine.version,
+        node_count=api_engine.node_count,
         cpu=api_engine.cpu,
         gpu=api_engine.gpu,
         memory_bytes=quantity_convertor.number_str_to_quantity(api_engine.memory_bytes),
         annotations=api_engine.annotations,
         max_idle_duration=duration_convertor.seconds_to_duration(
             api_engine.max_idle_duration
         ),
@@ -328,14 +346,20 @@
         update_time=api_engine.update_time,
         delete_time=api_engine.delete_time,
         login_url=api_engine.login_url,
         api_url=api_engine.api_url,
         reconciling=api_engine.reconciling,
         uid=api_engine.uid,
         client_info=client_info,
+        current_idle_duration=duration_convertor.none_seconds_to_duration(
+            api_engine.current_idle_duration
+        ),
+        current_running_duration=duration_convertor.none_seconds_to_duration(
+            api_engine.current_running_duration
+        ),
     )
 
 
 def build_api_engine_name(workspace_id: str, engine_id: str) -> str:
     """Function builds full OpenAPI resource name of an engine.
     Args:
         workspace_id (str): ID of the workspace.
```

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/h2o_engine/page.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_engine/page.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/h2o_engine/state.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_engine/state.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/h2o_engine/token_api_client.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_engine/token_api_client.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/h2o_engine_constraint/client.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_engine_constraint/client.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/h2o_engine_constraint/token_api_client.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_engine_constraint/token_api_client.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/h2o_version/client.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_version/client.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/h2o_version/mapper.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_version/mapper.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/h2o_version/page.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_version/page.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/clients/h2o_version/token_api_client.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_version/token_api_client.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/__init__.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: version not set
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "0.3.2"
+__version__ = "0.4.0"
 
 # import ApiClient
 from h2o_engine_manager.gen.dai_engine_constraint_set_service.api_client import ApiClient
 
 # import Configuration
 from h2o_engine_manager.gen.dai_engine_constraint_set_service.configuration import Configuration
```

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/api_client.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.3.2/python'
+        self.user_agent = 'OpenAPI-Generator/0.4.0/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/configuration.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -376,15 +376,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: version not set\n"\
-               "SDK Package Version: 0.3.2".\
+               "SDK Package Version: 0.4.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/exceptions.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/exceptions.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model_utils.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model_utils.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/rest.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/rest.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/api/dai_engine_constraint_set_service_api.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/api/dai_engine_constraint_set_service_api.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/apis/__init__.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/protobuf_any.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/protobuf_any.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/rpc_status.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/rpc_status.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/v1_constraint_duration.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/v1_constraint_duration.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/v1_constraint_numeric.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/v1_constraint_numeric.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/v1_dai_engine_constraint_set.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/v1_dai_engine_constraint_set.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/v1_get_dai_engine_constraint_set_response.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/v1_get_dai_engine_constraint_set_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/models/__init__.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/models/__init__.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/__init__.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: version not set
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "0.3.2"
+__version__ = "0.4.0"
 
 # import ApiClient
 from h2o_engine_manager.gen.dai_engine_service.api_client import ApiClient
 
 # import Configuration
 from h2o_engine_manager.gen.dai_engine_service.configuration import Configuration
```

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/api_client.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.3.2/python'
+        self.user_agent = 'OpenAPI-Generator/0.4.0/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/configuration.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -376,15 +376,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: version not set\n"\
-               "SDK Package Version: 0.3.2".\
+               "SDK Package Version: 0.4.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/exceptions.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/exceptions.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/model_utils.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model_utils.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/rest.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/rest.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/api/dai_engine_service_api.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/api/dai_engine_service_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1077,15 +1077,15 @@
         Args:
             parent (str): Workspace resource name. Format: workspaces/{workspace}
 
         Keyword Args:
             page_size (int): Maximum number of DAIEngines to return in a response. If unspecified (or set to 0), at most 50 DAIEngines will be returned. The maximum value is 1000; values above 1000 will be coerced to 1000.. [optional]
             page_token (str): Leave unset to receive the initial page. To list any subsequent pages use the value of 'next_page_token' returned from the ListDAIEnginesResponse.. [optional]
             order_by (str): Used to specify the sorting order.  When unset, DAIEngines are ordered by their time of creation in descending order. This is equivalent to \"create_time desc\".  When specified, the value must be a comma separated list of supported fields. The supported fields are: - name - version - cpu - gpu - memory_bytes - storage_bytes - creator - create_time - update_time - delete_time - resume_time - display_name - max_idle_duration - max_running_duration - uid  The default sorting order is ascending. For example: \"name\" and \"name asc\" are equivalent values.  To specify descending order for a field, append a \" desc\" suffix. For example: \"name desc\".  Redundant space characters are insignificant. For example these values are all equal: - \"  name, cpu     desc\" - \"name, cpu desc\" - \"name   , cpu desc   \"  Undefined (empty) time is interpreted as a zero time (0s since epoch, i.e. 1970-01-01T00:00:00Z).  Undefined (empty) duration is interpreted as a zero duration (0 seconds).. [optional]
-            filter (str): Used to filter DAIEngines.  When unset, no filtering is applied.  When specified, the filter string must follow this formatting rules: filter expression: [term] AND [term] AND [term] ... term: [filter_field] [operator] [value] filter_field: (name|version|state|cpu|gpu|memory_bytes|storage_bytes|creator|create_time|update_time|delete_time|resume_time|reconciling|uid|display_name|max_idle_duration|max_running_duration) operator: (=|!=|<=|<|>=|>) value: ([text]|[string]) text: free-form set of characters without whitespace (WS) or . (DOT) within it. (e.g. `28`, `abc`, `@5_6_7$`) string: a quoted string. Text may contain whitespace (WS) or . (DOT) within it. (e.g. `\"28\"`, `\"abc\"`, `\"@5_6_7$\"`, `\"   foo .  \"`)  Filter expression is case sensitive. Additional constraints: - You MUST use separator `<space>AND<space>` between terms. - String value MUST NOT contain `<space>AND<space>`.  Each field may support only some operators: - string fields (name, creator, uid) support: =, !=, <=, <, >=, > - number fields (cpu, gpu, memory_bytes, storage_bytes) support: =, !=, <=, <, >=, > - bool fields (reconciling) support: =, != - enum fields (state) support: =, != - time fields (create_time) support: =, !=, <=, <, >=, > - version fields (version) support: =, !=, <=, <, >=, >  Each field may expect values in a specified format: - string fields expect: text or string. For example `foo`, `\"f oo\"`. For example `f oo` is invalid. - number fields expect: numbers (can be wrapped in parentheses). For example: `28`, `-100`, `56.8`, `\"666\"` - integer number fields expect: integers. For example: `cpu = 10.5` is invalid. - bool fields expect: `true` or `false` literals. For example: `reconciling = true` is valid. `reconciling = 1` or `reconciling = TRUE` is invalid. - enum fields expect: enum's string representation. For example `state = STATE_RUNNING` is valid. `state = RUNNING` or `state = state_running` is invalid. - time fields expect: RFC-3339 formatted string. UTC offsets are supported. For example `2012-04-21T11:30:00-04:00` is valid. `2012-04-21` is invalid. - version fields expect: version identifier. Aliases are also accepted. For example: `1.10.1` or `latest`   If version identifier is NOT an alias and is not in semver format, then it may not be accepted. For example: `abc` is invalid value, if no version has alias 'abc'.  Valid filter expression examples: - `state = STATE_RUNNING AND cpu <= 5 AND gpu != 0 AND create_time > 2012-04-21T11:30:00-04:00` - `state=STATE_RUNNING AND cpu<=5` (there may be no whitespace between term parts: `[filter_field][operator][value]`)  Invalid filter expression examples: - `state = STATE_RUNNING    AND    cpu <= 5` (invalid separator between terms) - `state = STATE_RUNNING OR cpu <= 5` (unsupported logical operator) - `(state = STATE_RUNNING) AND (cpu <= 5)` (unsupported parentheses). [optional]
+            filter (str): Used to filter DAIEngines. When unset, no filtering is applied.  Filtering implements specification https://google.aip.dev/160.  Supported filter fields: - name - dai_engine_id - version (supporting version semantic comparison and version aliases) - state - cpu - gpu - memory_bytes - storage_bytes - creator - creator_display_name - create_time - update_time - delete_time - resume_time - reconciling - uid - display_name - max_idle_duration - max_running_duration - current_idle_duration - current_running_duration  Examples: - `cpu > 5` - `gpu < 3` - `cpu >= 5 AND gpu <= 3` - `cpu != 5 OR gpu == 3` - `NOT (cpu > 5 OR gpu < 3)` - `-(cpu > 5 OR gpu < 3)` - `NOT (cpu > 5 OR (gpu < 3))` - `(cpu > 5 OR gpu < 3) AND memory_bytes != 1000` - `(cpu > 5 OR gpu < 3) AND (NOT ((((memory_bytes = 1000)))))` - `state = STATE_RUNNING AND create_time > \"2012-04-21T11:30:00-04:00\"` - `max_running_duration > \"1s\" AND max_running_duration != \"5s\"` - `version > \"latest\" AND version >= \"1.10.3\"` - `reconciling = true OR reconciling = false` (supporting bool literals) - `dai_engine_id = \"*e*\" OR display_name = \"*e*\"` (supporting prefix/suffix wildcard `*` for string fields equality comparison). [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
```

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/apis/__init__.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/model/api_http_body.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/api_http_body.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_resource.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,14 +105,16 @@
             'gpu': (int, none_type,),  # noqa: E501
             'memory_bytes': (str, none_type,),  # noqa: E501
             'storage_bytes': (str, none_type,),  # noqa: E501
             'config': ({str: (str,)},),  # noqa: E501
             'max_idle_duration': (str, none_type,),  # noqa: E501
             'max_running_duration': (str, none_type,),  # noqa: E501
             'upgrade_available': (bool,),  # noqa: E501
+            'current_idle_duration': (str, none_type,),  # noqa: E501
+            'current_running_duration': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -135,28 +137,32 @@
         'gpu': 'gpu',  # noqa: E501
         'memory_bytes': 'memoryBytes',  # noqa: E501
         'storage_bytes': 'storageBytes',  # noqa: E501
         'config': 'config',  # noqa: E501
         'max_idle_duration': 'maxIdleDuration',  # noqa: E501
         'max_running_duration': 'maxRunningDuration',  # noqa: E501
         'upgrade_available': 'upgradeAvailable',  # noqa: E501
+        'current_idle_duration': 'currentIdleDuration',  # noqa: E501
+        'current_running_duration': 'currentRunningDuration',  # noqa: E501
     }
 
     read_only_vars = {
         'uid',  # noqa: E501
         'creator',  # noqa: E501
         'creator_display_name',  # noqa: E501
         'reconciling',  # noqa: E501
         'create_time',  # noqa: E501
         'delete_time',  # noqa: E501
         'update_time',  # noqa: E501
         'resume_time',  # noqa: E501
         'api_url',  # noqa: E501
         'login_url',  # noqa: E501
         'upgrade_available',  # noqa: E501
+        'current_idle_duration',  # noqa: E501
+        'current_running_duration',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
@@ -211,14 +217,16 @@
             gpu (int, none_type): The amount of GPU units requested by this DAIEngine.. [optional]  # noqa: E501
             memory_bytes (str, none_type): The amount of memory in bytes requested by this DAIEngine.. [optional]  # noqa: E501
             storage_bytes (str, none_type): The amount of storage requested by this DAIEngine.. [optional]  # noqa: E501
             config ({str: (str,)}): Additional Driverless AI configuration.  Temporary: Some config keys are reserved and their value cannot be changed. Attempting to set or override a reserved key will have no effect, no error will be raised. Entries with reserved keys will not be available in this field (they are hidden).. [optional]  # noqa: E501
             max_idle_duration (str, none_type): [optional]  # noqa: E501
             max_running_duration (str, none_type): Maximum time the DAIEngine can be running. When exceeded, the DAIEngine will pause.. [optional]  # noqa: E501
             upgrade_available (bool): Indicates, whether the used version can be upgraded to a later one.. [optional]  # noqa: E501
+            current_idle_duration (str, none_type): Current time the DAIEngine is idle.. [optional]  # noqa: E501
+            current_running_duration (str, none_type): Current time the DAIEngine is running.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -318,14 +326,16 @@
             gpu (int, none_type): The amount of GPU units requested by this DAIEngine.. [optional]  # noqa: E501
             memory_bytes (str, none_type): The amount of memory in bytes requested by this DAIEngine.. [optional]  # noqa: E501
             storage_bytes (str, none_type): The amount of storage requested by this DAIEngine.. [optional]  # noqa: E501
             config ({str: (str,)}): Additional Driverless AI configuration.  Temporary: Some config keys are reserved and their value cannot be changed. Attempting to set or override a reserved key will have no effect, no error will be raised. Entries with reserved keys will not be available in this field (they are hidden).. [optional]  # noqa: E501
             max_idle_duration (str, none_type): [optional]  # noqa: E501
             max_running_duration (str, none_type): Maximum time the DAIEngine can be running. When exceeded, the DAIEngine will pause.. [optional]  # noqa: E501
             upgrade_available (bool): Indicates, whether the used version can be upgraded to a later one.. [optional]  # noqa: E501
+            current_idle_duration (str, none_type): Current time the DAIEngine is idle.. [optional]  # noqa: E501
+            current_running_duration (str, none_type): Current time the DAIEngine is running.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_service_migrate_creator_request.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_service_migrate_creator_request.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_service_pause_dai_engine_request.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_service_pause_dai_engine_request.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_service_resume_dai_engine_request.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_service_resume_dai_engine_request.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_service_upgrade_version_request.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_service_upgrade_version_request.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/model/protobuf_any.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/protobuf_any.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/model/rpc_status.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/rpc_status.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/model/v1_create_dai_engine_response.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_create_dai_engine_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_h2_o_engine.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 """
-    ai/h2o/engine/v1/dai_engine_service.proto
+    ai/h2o/engine/v1/h2o_engine_service.proto
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: version not set
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from h2o_engine_manager.gen.dai_engine_service.model_utils import (  # noqa: F401
+from h2o_engine_manager.gen.h2o_engine_service.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from h2o_engine_manager.gen.dai_engine_service.exceptions import ApiAttributeError
+from h2o_engine_manager.gen.h2o_engine_service.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from h2o_engine_manager.gen.dai_engine_service.model.v1_dai_engine_state import V1DAIEngineState
-    globals()['V1DAIEngineState'] = V1DAIEngineState
+    from h2o_engine_manager.gen.h2o_engine_service.model.v1_h2_o_engine_state import V1H2OEngineState
+    globals()['V1H2OEngineState'] = V1H2OEngineState
 
 
-class V1DAIEngine(ModelNormal):
+class V1H2OEngine(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -83,91 +83,92 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
+            'version': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
             'uid': (str,),  # noqa: E501
             'creator': (str,),  # noqa: E501
             'creator_display_name': (str,),  # noqa: E501
-            'state': (V1DAIEngineState,),  # noqa: E501
+            'state': (V1H2OEngineState,),  # noqa: E501
             'reconciling': (bool,),  # noqa: E501
             'create_time': (datetime,),  # noqa: E501
             'delete_time': (datetime, none_type,),  # noqa: E501
             'update_time': (datetime, none_type,),  # noqa: E501
-            'resume_time': (datetime, none_type,),  # noqa: E501
             'api_url': (str,),  # noqa: E501
             'login_url': (str,),  # noqa: E501
             'annotations': ({str: (str,)},),  # noqa: E501
             'display_name': (str,),  # noqa: E501
-            'version': (str, none_type,),  # noqa: E501
             'cpu': (int, none_type,),  # noqa: E501
             'gpu': (int, none_type,),  # noqa: E501
             'memory_bytes': (str, none_type,),  # noqa: E501
-            'storage_bytes': (str, none_type,),  # noqa: E501
-            'config': ({str: (str,)},),  # noqa: E501
             'max_idle_duration': (str, none_type,),  # noqa: E501
             'max_running_duration': (str, none_type,),  # noqa: E501
-            'upgrade_available': (bool,),  # noqa: E501
+            'current_idle_duration': (str, none_type,),  # noqa: E501
+            'current_running_duration': (str, none_type,),  # noqa: E501
+            'node_count': (int, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
+        'version': 'version',  # noqa: E501
         'name': 'name',  # noqa: E501
         'uid': 'uid',  # noqa: E501
         'creator': 'creator',  # noqa: E501
         'creator_display_name': 'creatorDisplayName',  # noqa: E501
         'state': 'state',  # noqa: E501
         'reconciling': 'reconciling',  # noqa: E501
         'create_time': 'createTime',  # noqa: E501
         'delete_time': 'deleteTime',  # noqa: E501
         'update_time': 'updateTime',  # noqa: E501
-        'resume_time': 'resumeTime',  # noqa: E501
         'api_url': 'apiUrl',  # noqa: E501
         'login_url': 'loginUrl',  # noqa: E501
         'annotations': 'annotations',  # noqa: E501
         'display_name': 'displayName',  # noqa: E501
-        'version': 'version',  # noqa: E501
         'cpu': 'cpu',  # noqa: E501
         'gpu': 'gpu',  # noqa: E501
         'memory_bytes': 'memoryBytes',  # noqa: E501
-        'storage_bytes': 'storageBytes',  # noqa: E501
-        'config': 'config',  # noqa: E501
         'max_idle_duration': 'maxIdleDuration',  # noqa: E501
         'max_running_duration': 'maxRunningDuration',  # noqa: E501
-        'upgrade_available': 'upgradeAvailable',  # noqa: E501
+        'current_idle_duration': 'currentIdleDuration',  # noqa: E501
+        'current_running_duration': 'currentRunningDuration',  # noqa: E501
+        'node_count': 'nodeCount',  # noqa: E501
     }
 
     read_only_vars = {
         'name',  # noqa: E501
         'uid',  # noqa: E501
         'creator',  # noqa: E501
         'creator_display_name',  # noqa: E501
         'reconciling',  # noqa: E501
         'create_time',  # noqa: E501
         'delete_time',  # noqa: E501
         'update_time',  # noqa: E501
-        'resume_time',  # noqa: E501
         'api_url',  # noqa: E501
         'login_url',  # noqa: E501
-        'upgrade_available',  # noqa: E501
+        'current_idle_duration',  # noqa: E501
+        'current_running_duration',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """V1DAIEngine - a model defined in OpenAPI
+    def _from_openapi_data(cls, version, *args, **kwargs):  # noqa: E501
+        """V1H2OEngine - a model defined in OpenAPI
+
+        Args:
+            version (str): H2OEngine version identifier. Version must be specified during engine creation but cannot be changed later. For example: \"3.38.0.1\" or \"latest\".
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -192,37 +193,35 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str): DAIEngine resource name.. [optional]  # noqa: E501
+            name (str): H2OEngine resource name.. [optional]  # noqa: E501
             uid (str): Globally unique identifier of the resource.. [optional]  # noqa: E501
-            creator (str): Name of an entity that created the DAIEngine.. [optional]  # noqa: E501
+            creator (str): Name of na entity that created the H2OEngine.. [optional]  # noqa: E501
             creator_display_name (str): Human-readable name of creator.. [optional]  # noqa: E501
-            state (V1DAIEngineState): [optional]  # noqa: E501
-            reconciling (bool): Indicates whether changes to the resource are in progress. If true, current state of the DAIEngine does not match the intended state.. [optional]  # noqa: E501
-            create_time (datetime): Time when the DAIEngine creation was requested.. [optional]  # noqa: E501
-            delete_time (datetime, none_type): Time when the DAIEngine was deleted.. [optional]  # noqa: E501
-            update_time (datetime, none_type): Time when the DAIEngine was last updated.. [optional]  # noqa: E501
-            resume_time (datetime, none_type): Time when the DAIEngine was last resumed (or started for the first time).. [optional]  # noqa: E501
+            state (V1H2OEngineState): [optional]  # noqa: E501
+            reconciling (bool): Indicates whether changes to the resource are in progress. If true, current state of the H2OEngine does not match the intended state.. [optional]  # noqa: E501
+            create_time (datetime): Time when the H2OEngine creation was requested.. [optional]  # noqa: E501
+            delete_time (datetime, none_type): Time when the H2OEngine was deleted.. [optional]  # noqa: E501
+            update_time (datetime, none_type): Time when the H2OEngine was last updated.. [optional]  # noqa: E501
             api_url (str): The URL address to access the engine API.. [optional]  # noqa: E501
             login_url (str): The URL address to initiate login flow.. [optional]  # noqa: E501
-            annotations ({str: (str,)}): Additional arbitrary metadata associated with the DAIEngine.  Annotations are key/value pairs. The key must: - be 63 characters or less - begin and end with an alphanumeric character ([a-z0-9A-Z]) - with dashes (-), underscores (_), dots (.), and alphanumerics between - regex used for validation is: ^[A-Za-z0-9]([-A-Za-z0-9_.]{0,61}[A-Za-z0-9])?$. [optional]  # noqa: E501
-            display_name (str): Human-readable name of the DAIEngine. Must contain at most 63 characters. Does not have to be unique.. [optional]  # noqa: E501
-            version (str, none_type): Driverless AI version identifier. Version may be specified during engine creation but cannot be changed later. For example: \"1.10.1\" or \"latest\".. [optional]  # noqa: E501
-            cpu (int, none_type): The amount of CPU units requested by this DAIEngine.. [optional]  # noqa: E501
-            gpu (int, none_type): The amount of GPU units requested by this DAIEngine.. [optional]  # noqa: E501
-            memory_bytes (str, none_type): The amount of memory in bytes requested by this DAIEngine.. [optional]  # noqa: E501
-            storage_bytes (str, none_type): The amount of storage requested by this DAIEngine.. [optional]  # noqa: E501
-            config ({str: (str,)}): Additional Driverless AI configuration.  Temporary: Some config keys are reserved and their value cannot be changed. Attempting to set or override a reserved key will have no effect, no error will be raised. Entries with reserved keys will not be available in this field (they are hidden).. [optional]  # noqa: E501
-            max_idle_duration (str, none_type): [optional]  # noqa: E501
-            max_running_duration (str, none_type): Maximum time the DAIEngine can be running. When exceeded, the DAIEngine will pause.. [optional]  # noqa: E501
-            upgrade_available (bool): Indicates, whether the used version can be upgraded to a later one.. [optional]  # noqa: E501
+            annotations ({str: (str,)}): Additional arbitrary metadata associated with the H2OEngine.  Annotations are key/value pairs. The key must: - be 63 characters or less - begin and end with an alphanumeric character ([a-z0-9A-Z]) - with dashes (-), underscores (_), dots (.), and alphanumerics between - regex used for validation is: ^[A-Za-z0-9]([-A-Za-z0-9_.]{0,61}[A-Za-z0-9])?$. [optional]  # noqa: E501
+            display_name (str): Human-readable name of the H2OEngine. Must contain at most 63 characters. Does not have to be unique.. [optional]  # noqa: E501
+            cpu (int, none_type): The amount of CPU units per node requested by this H2OEngine.. [optional]  # noqa: E501
+            gpu (int, none_type): The amount of GPU units per node requested by this H2OEngine.. [optional]  # noqa: E501
+            memory_bytes (str, none_type): The amount of memory in bytes per node requested by this H2OEngine.. [optional]  # noqa: E501
+            max_idle_duration (str, none_type): Maximum time an H2OEngine can be idle. When exceeded, the H2OEngine will pause.. [optional]  # noqa: E501
+            max_running_duration (str, none_type): Maximum time an H2OEngine can be running. When exceeded, the H2OEngine will pause.. [optional]  # noqa: E501
+            current_idle_duration (str, none_type): Current time the H2OEngine is idle.. [optional]  # noqa: E501
+            current_running_duration (str, none_type): Current time the H2OEngine is running.. [optional]  # noqa: E501
+            node_count (int, none_type): The number of nodes requested by this H2OEngine.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -246,14 +245,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.version = version
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -266,16 +266,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """V1DAIEngine - a model defined in OpenAPI
+    def __init__(self, version, *args, **kwargs):  # noqa: E501
+        """V1H2OEngine - a model defined in OpenAPI
+
+        Args:
+            version (str): H2OEngine version identifier. Version must be specified during engine creation but cannot be changed later. For example: \"3.38.0.1\" or \"latest\".
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -300,37 +303,35 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str): DAIEngine resource name.. [optional]  # noqa: E501
+            name (str): H2OEngine resource name.. [optional]  # noqa: E501
             uid (str): Globally unique identifier of the resource.. [optional]  # noqa: E501
-            creator (str): Name of an entity that created the DAIEngine.. [optional]  # noqa: E501
+            creator (str): Name of na entity that created the H2OEngine.. [optional]  # noqa: E501
             creator_display_name (str): Human-readable name of creator.. [optional]  # noqa: E501
-            state (V1DAIEngineState): [optional]  # noqa: E501
-            reconciling (bool): Indicates whether changes to the resource are in progress. If true, current state of the DAIEngine does not match the intended state.. [optional]  # noqa: E501
-            create_time (datetime): Time when the DAIEngine creation was requested.. [optional]  # noqa: E501
-            delete_time (datetime, none_type): Time when the DAIEngine was deleted.. [optional]  # noqa: E501
-            update_time (datetime, none_type): Time when the DAIEngine was last updated.. [optional]  # noqa: E501
-            resume_time (datetime, none_type): Time when the DAIEngine was last resumed (or started for the first time).. [optional]  # noqa: E501
+            state (V1H2OEngineState): [optional]  # noqa: E501
+            reconciling (bool): Indicates whether changes to the resource are in progress. If true, current state of the H2OEngine does not match the intended state.. [optional]  # noqa: E501
+            create_time (datetime): Time when the H2OEngine creation was requested.. [optional]  # noqa: E501
+            delete_time (datetime, none_type): Time when the H2OEngine was deleted.. [optional]  # noqa: E501
+            update_time (datetime, none_type): Time when the H2OEngine was last updated.. [optional]  # noqa: E501
             api_url (str): The URL address to access the engine API.. [optional]  # noqa: E501
             login_url (str): The URL address to initiate login flow.. [optional]  # noqa: E501
-            annotations ({str: (str,)}): Additional arbitrary metadata associated with the DAIEngine.  Annotations are key/value pairs. The key must: - be 63 characters or less - begin and end with an alphanumeric character ([a-z0-9A-Z]) - with dashes (-), underscores (_), dots (.), and alphanumerics between - regex used for validation is: ^[A-Za-z0-9]([-A-Za-z0-9_.]{0,61}[A-Za-z0-9])?$. [optional]  # noqa: E501
-            display_name (str): Human-readable name of the DAIEngine. Must contain at most 63 characters. Does not have to be unique.. [optional]  # noqa: E501
-            version (str, none_type): Driverless AI version identifier. Version may be specified during engine creation but cannot be changed later. For example: \"1.10.1\" or \"latest\".. [optional]  # noqa: E501
-            cpu (int, none_type): The amount of CPU units requested by this DAIEngine.. [optional]  # noqa: E501
-            gpu (int, none_type): The amount of GPU units requested by this DAIEngine.. [optional]  # noqa: E501
-            memory_bytes (str, none_type): The amount of memory in bytes requested by this DAIEngine.. [optional]  # noqa: E501
-            storage_bytes (str, none_type): The amount of storage requested by this DAIEngine.. [optional]  # noqa: E501
-            config ({str: (str,)}): Additional Driverless AI configuration.  Temporary: Some config keys are reserved and their value cannot be changed. Attempting to set or override a reserved key will have no effect, no error will be raised. Entries with reserved keys will not be available in this field (they are hidden).. [optional]  # noqa: E501
-            max_idle_duration (str, none_type): [optional]  # noqa: E501
-            max_running_duration (str, none_type): Maximum time the DAIEngine can be running. When exceeded, the DAIEngine will pause.. [optional]  # noqa: E501
-            upgrade_available (bool): Indicates, whether the used version can be upgraded to a later one.. [optional]  # noqa: E501
+            annotations ({str: (str,)}): Additional arbitrary metadata associated with the H2OEngine.  Annotations are key/value pairs. The key must: - be 63 characters or less - begin and end with an alphanumeric character ([a-z0-9A-Z]) - with dashes (-), underscores (_), dots (.), and alphanumerics between - regex used for validation is: ^[A-Za-z0-9]([-A-Za-z0-9_.]{0,61}[A-Za-z0-9])?$. [optional]  # noqa: E501
+            display_name (str): Human-readable name of the H2OEngine. Must contain at most 63 characters. Does not have to be unique.. [optional]  # noqa: E501
+            cpu (int, none_type): The amount of CPU units per node requested by this H2OEngine.. [optional]  # noqa: E501
+            gpu (int, none_type): The amount of GPU units per node requested by this H2OEngine.. [optional]  # noqa: E501
+            memory_bytes (str, none_type): The amount of memory in bytes per node requested by this H2OEngine.. [optional]  # noqa: E501
+            max_idle_duration (str, none_type): Maximum time an H2OEngine can be idle. When exceeded, the H2OEngine will pause.. [optional]  # noqa: E501
+            max_running_duration (str, none_type): Maximum time an H2OEngine can be running. When exceeded, the H2OEngine will pause.. [optional]  # noqa: E501
+            current_idle_duration (str, none_type): Current time the H2OEngine is idle.. [optional]  # noqa: E501
+            current_running_duration (str, none_type): Current time the H2OEngine is running.. [optional]  # noqa: E501
+            node_count (int, none_type): The number of nodes requested by this H2OEngine.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -352,14 +353,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.version = version
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine_service_download_logs_response.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine_service_download_logs_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine_service_migrate_creator_response.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine_service_migrate_creator_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine_service_upgrade_version_response.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine_service_upgrade_version_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine_state.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine_state.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/model/v1_delete_dai_engine_response.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_delete_dai_engine_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/model/v1_get_dai_engine_response.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_get_dai_engine_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/model/v1_list_dai_engines_response.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_list_dai_engines_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/model/v1_pause_dai_engine_response.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_pause_dai_engine_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/model/v1_resume_dai_engine_response.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_resume_dai_engine_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/model/v1_update_dai_engine_response.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_update_dai_engine_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_engine_service/models/__init__.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/models/__init__.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_version_service/__init__.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_version_service/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: version not set
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "0.3.2"
+__version__ = "0.4.0"
 
 # import ApiClient
 from h2o_engine_manager.gen.dai_version_service.api_client import ApiClient
 
 # import Configuration
 from h2o_engine_manager.gen.dai_version_service.configuration import Configuration
```

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_version_service/api_client.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_version_service/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.3.2/python'
+        self.user_agent = 'OpenAPI-Generator/0.4.0/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_version_service/configuration.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_version_service/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -376,15 +376,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: version not set\n"\
-               "SDK Package Version: 0.3.2".\
+               "SDK Package Version: 0.4.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_version_service/exceptions.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_version_service/exceptions.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_version_service/model_utils.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_version_service/model_utils.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_version_service/rest.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_version_service/rest.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_version_service/api/dai_version_service_api.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_version_service/api/dai_version_service_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -112,15 +112,15 @@
         >>> result = thread.get()
 
 
         Keyword Args:
             page_size (int): Maximum number of DAIVersions to return in a response. If unspecified (or set to 0), at most 50 DAIVersions will be returned. The maximum value is 1000; values above 1000 will be coerced to 1000.. [optional]
             page_token (str): Leave unset to receive the initial page. To list any subsequent pages use the value of 'next_page_token' returned from the ListDAIVersionsResponse.. [optional]
             order_by (str): Used to specify the sorting order.  When unset, DAIVersions are ordered by their version name in descending order. This is equivalent to \"version desc\".  When specified, the value must be a comma separated list of supported fields. The supported fields are: - version  The default sorting order is ascending. For example: \"version\" and \"version asc\" are equivalent values.  To specify descending order for a field, append a \" desc\" suffix. For example: \"version desc\".  Redundant space characters are insignificant.. [optional]
-            filter (str): Used to filter DAIEngines.  When unset, no filtering is applied.  When specified, the filter string must follow these formatting rules:  filter expression: [term] AND [term] AND [term] ... term: [filter_field] [operator] [value] filter_field: (version) operator: (=|!=|<=|<|>=|>) value: ([text]|[string])  Filter expression is case sensitive. Additional constraints: - You MUST use separator `<space>AND<space>` between terms. - String value MUST NOT contain `<space>AND<space>`.  Each field may support only some operators: - version fields (version) support: =, !=, <=, <, >=, >  Each field may expect values in a specified format: - version fields expect: version identifier. Aliases are also accepted. For example: `1.10.1` or `latest`.   If version identifier is NOT an alias and is not in semver format, then it may not be accepted. For example: `abc` is invalid value, if no version has alias 'abc'.  Valid filter expression examples: - `version >= 1.10.1 AND version != latest`. [optional]
+            filter (str): Used to filter DAIVersions. When unset, no filtering is applied.  Filtering implements specification https://google.aip.dev/160.  Supported filter fields: - version (supporting version semantic comparison and version aliases)  Examples: - `version > \"latest\" AND version >= \"1.10.3\"`. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
```

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_version_service/apis/__init__.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_version_service/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_version_service/model/protobuf_any.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_version_service/model/protobuf_any.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_version_service/model/rpc_status.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_version_service/model/rpc_status.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_version_service/model/v1_dai_version.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_version_service/model/v1_dai_version.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_version_service/model/v1_list_dai_versions_response.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_version_service/model/v1_list_dai_versions_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/dai_version_service/models/__init__.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_version_service/models/__init__.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/engine_service/__init__.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: version not set
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "0.3.2"
+__version__ = "0.4.0"
 
 # import ApiClient
 from h2o_engine_manager.gen.engine_service.api_client import ApiClient
 
 # import Configuration
 from h2o_engine_manager.gen.engine_service.configuration import Configuration
```

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/engine_service/api_client.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.3.2/python'
+        self.user_agent = 'OpenAPI-Generator/0.4.0/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/engine_service/configuration.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -376,15 +376,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: version not set\n"\
-               "SDK Package Version: 0.3.2".\
+               "SDK Package Version: 0.4.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/engine_service/exceptions.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/exceptions.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/engine_service/model_utils.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/model_utils.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/engine_service/rest.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/rest.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/engine_service/apis/__init__.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/engine_service/model/protobuf_any.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/model/protobuf_any.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/engine_service/model/rpc_status.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/model/rpc_status.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/engine_service/model/v1_engine.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/model/v1_engine.py`

 * *Files 15% similar despite different names*

```diff
@@ -105,14 +105,18 @@
             'display_name': (str,),  # noqa: E501
             'version': (str,),  # noqa: E501
             'cpu': (int,),  # noqa: E501
             'gpu': (int,),  # noqa: E501
             'memory_bytes': (str,),  # noqa: E501
             'storage_bytes': (str,),  # noqa: E501
             'upgrade_available': (bool,),  # noqa: E501
+            'max_idle_duration': (str, none_type,),  # noqa: E501
+            'max_running_duration': (str, none_type,),  # noqa: E501
+            'current_idle_duration': (str, none_type,),  # noqa: E501
+            'current_running_duration': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -133,14 +137,18 @@
         'display_name': 'displayName',  # noqa: E501
         'version': 'version',  # noqa: E501
         'cpu': 'cpu',  # noqa: E501
         'gpu': 'gpu',  # noqa: E501
         'memory_bytes': 'memoryBytes',  # noqa: E501
         'storage_bytes': 'storageBytes',  # noqa: E501
         'upgrade_available': 'upgradeAvailable',  # noqa: E501
+        'max_idle_duration': 'maxIdleDuration',  # noqa: E501
+        'max_running_duration': 'maxRunningDuration',  # noqa: E501
+        'current_idle_duration': 'currentIdleDuration',  # noqa: E501
+        'current_running_duration': 'currentRunningDuration',  # noqa: E501
     }
 
     read_only_vars = {
         'name',  # noqa: E501
         'uid',  # noqa: E501
         'creator',  # noqa: E501
         'creator_display_name',  # noqa: E501
@@ -154,14 +162,18 @@
         'display_name',  # noqa: E501
         'version',  # noqa: E501
         'cpu',  # noqa: E501
         'gpu',  # noqa: E501
         'memory_bytes',  # noqa: E501
         'storage_bytes',  # noqa: E501
         'upgrade_available',  # noqa: E501
+        'max_idle_duration',  # noqa: E501
+        'max_running_duration',  # noqa: E501
+        'current_idle_duration',  # noqa: E501
+        'current_running_duration',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
@@ -214,14 +226,18 @@
             display_name (str): Human-readable name of the Engine. Contains at most 63 characters and is not unique.. [optional]  # noqa: E501
             version (str): Engine version identifier. For example: \"1.10.1\" or \"latest\".. [optional]  # noqa: E501
             cpu (int): The amount of CPU units in total requested by this Engine.. [optional]  # noqa: E501
             gpu (int): The amount of GPU units in total requested by this Engine.. [optional]  # noqa: E501
             memory_bytes (str): The amount of memory in bytes requested by this Engine.. [optional]  # noqa: E501
             storage_bytes (str): The amount of storage in bytes requested by this Engine.. [optional]  # noqa: E501
             upgrade_available (bool): Indicates, whether the used version can be upgraded to a later one.. [optional]  # noqa: E501
+            max_idle_duration (str, none_type): Maximum time the engine can be idle.. [optional]  # noqa: E501
+            max_running_duration (str, none_type): Maximum time the engine can be running.. [optional]  # noqa: E501
+            current_idle_duration (str, none_type): Current time the engine is idle.. [optional]  # noqa: E501
+            current_running_duration (str, none_type): Current time the engine is running.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -319,14 +335,18 @@
             display_name (str): Human-readable name of the Engine. Contains at most 63 characters and is not unique.. [optional]  # noqa: E501
             version (str): Engine version identifier. For example: \"1.10.1\" or \"latest\".. [optional]  # noqa: E501
             cpu (int): The amount of CPU units in total requested by this Engine.. [optional]  # noqa: E501
             gpu (int): The amount of GPU units in total requested by this Engine.. [optional]  # noqa: E501
             memory_bytes (str): The amount of memory in bytes requested by this Engine.. [optional]  # noqa: E501
             storage_bytes (str): The amount of storage in bytes requested by this Engine.. [optional]  # noqa: E501
             upgrade_available (bool): Indicates, whether the used version can be upgraded to a later one.. [optional]  # noqa: E501
+            max_idle_duration (str, none_type): Maximum time the engine can be idle.. [optional]  # noqa: E501
+            max_running_duration (str, none_type): Maximum time the engine can be running.. [optional]  # noqa: E501
+            current_idle_duration (str, none_type): Current time the engine is idle.. [optional]  # noqa: E501
+            current_running_duration (str, none_type): Current time the engine is running.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/engine_service/model/v1_engine_state.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/model/v1_engine_state.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/engine_service/model/v1_engine_type.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/model/v1_engine_type.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/engine_service/model/v1_list_engines_response.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/model/v1_list_engines_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/engine_service/models/__init__.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/models/__init__.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/__init__.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: version not set
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "0.3.2"
+__version__ = "0.4.0"
 
 # import ApiClient
 from h2o_engine_manager.gen.h2o_engine_constraint_set_service.api_client import ApiClient
 
 # import Configuration
 from h2o_engine_manager.gen.h2o_engine_constraint_set_service.configuration import Configuration
```

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/api_client.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.3.2/python'
+        self.user_agent = 'OpenAPI-Generator/0.4.0/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/configuration.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -376,15 +376,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: version not set\n"\
-               "SDK Package Version: 0.3.2".\
+               "SDK Package Version: 0.4.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/exceptions.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/exceptions.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model_utils.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model_utils.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/rest.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/rest.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/api/h2_o_engine_constraint_set_service_api.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/api/h2_o_engine_constraint_set_service_api.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/apis/__init__.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/protobuf_any.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/protobuf_any.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/rpc_status.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/rpc_status.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/v1_constraint_duration.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/v1_constraint_duration.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/v1_constraint_numeric.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/v1_constraint_numeric.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/v1_get_h2_o_engine_constraint_set_response.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/v1_get_h2_o_engine_constraint_set_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/v1_h2_o_engine_constraint_set.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/v1_h2_o_engine_constraint_set.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,28 +91,30 @@
         return {
             'name': (str,),  # noqa: E501
             'cpu': (V1ConstraintNumeric,),  # noqa: E501
             'gpu': (V1ConstraintNumeric,),  # noqa: E501
             'memory_bytes': (V1ConstraintNumeric,),  # noqa: E501
             'max_idle_duration': (V1ConstraintDuration,),  # noqa: E501
             'max_running_duration': (V1ConstraintDuration,),  # noqa: E501
+            'node_count': (V1ConstraintNumeric,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'name': 'name',  # noqa: E501
         'cpu': 'cpu',  # noqa: E501
         'gpu': 'gpu',  # noqa: E501
         'memory_bytes': 'memoryBytes',  # noqa: E501
         'max_idle_duration': 'maxIdleDuration',  # noqa: E501
         'max_running_duration': 'maxRunningDuration',  # noqa: E501
+        'node_count': 'nodeCount',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
@@ -154,14 +156,15 @@
                                 _visited_composed_classes = (Animal,)
             name (str): H2OEngineConstraintSet resource name.. [optional]  # noqa: E501
             cpu (V1ConstraintNumeric): [optional]  # noqa: E501
             gpu (V1ConstraintNumeric): [optional]  # noqa: E501
             memory_bytes (V1ConstraintNumeric): [optional]  # noqa: E501
             max_idle_duration (V1ConstraintDuration): [optional]  # noqa: E501
             max_running_duration (V1ConstraintDuration): [optional]  # noqa: E501
+            node_count (V1ConstraintNumeric): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -245,14 +248,15 @@
                                 _visited_composed_classes = (Animal,)
             name (str): H2OEngineConstraintSet resource name.. [optional]  # noqa: E501
             cpu (V1ConstraintNumeric): [optional]  # noqa: E501
             gpu (V1ConstraintNumeric): [optional]  # noqa: E501
             memory_bytes (V1ConstraintNumeric): [optional]  # noqa: E501
             max_idle_duration (V1ConstraintDuration): [optional]  # noqa: E501
             max_running_duration (V1ConstraintDuration): [optional]  # noqa: E501
+            node_count (V1ConstraintNumeric): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/models/__init__.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/models/__init__.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_service/__init__.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: version not set
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "0.3.2"
+__version__ = "0.4.0"
 
 # import ApiClient
 from h2o_engine_manager.gen.h2o_engine_service.api_client import ApiClient
 
 # import Configuration
 from h2o_engine_manager.gen.h2o_engine_service.configuration import Configuration
```

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_service/api_client.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.3.2/python'
+        self.user_agent = 'OpenAPI-Generator/0.4.0/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_service/configuration.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -376,15 +376,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: version not set\n"\
-               "SDK Package Version: 0.3.2".\
+               "SDK Package Version: 0.4.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_service/exceptions.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/exceptions.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_service/model_utils.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/model_utils.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_service/rest.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/rest.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_service/api/h2_o_engine_service_api.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/api/h2_o_engine_service_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -735,16 +735,16 @@
 
         Args:
             parent (str): Workspace resource name. Format: workspaces/{workspace}
 
         Keyword Args:
             page_size (int): Maximum number of H2OEngines to return in a response. If unspecified (or set to 0), at most 50 H2OEngines will be returned. The maximum value is 1000; values above 1000 will be coerced to 1000.. [optional]
             page_token (str): Leave unset to receive the initial page. To list any subsequent pages use the value of 'next_page_token' returned from the ListH2OEnginesResponse.. [optional]
-            order_by (str): Used to specify the sorting order.  When unset, H2OEngines are ordered by their time of creation in descending order. This is equivalent to \"create_time desc\".  When specified, the value must be a comma separated list of supported fields. The supported fields are: TODO: Fill out  The default sorting order is ascending. For example: \"name\" and \"name asc\" are equivalent values.  To specify descending order for a field, append a \" desc\" suffix. For example: \"name desc\".  Redundant space characters are insignificant. For example these values are all equal: - \"  name, cpu     desc\" - \"name, cpu desc\" - \"name   , cpu desc   \"  Undefined (empty) time is interpreted as a zero time (0s since epoch, i.e. 1970-01-01T00:00:00Z).  Undefined (empty) duration is interpreted as a zero duration (0 seconds).. [optional]
-            filter (str): Used to filter H2OEngines.  When unset, no filtering is applied.  When specified, the filter string must follow this formatting rules: filter expression: [term] AND [term] AND [term] ... term: [filter_field] [operator] [value] filter_field: (name|version|state|cpu|gpu|memory_bytes|creator|create_time|update_time|delete_time|reconciling|uid|display_name|max_idle_duration|max_running_duration) operator: (=|!=|<=|<|>=|>) value: ([text]|[string]) text: free-form set of characters without whitespace (WS) or . (DOT) within it. (e.g. `28`, `abc`, `@5_6_7$`) string: a quoted string. Text may contain whitespace (WS) or . (DOT) within it. (e.g. `\"28\"`, `\"abc\"`, `\"@5_6_7$\"`, `\"   foo .  \"`)  Filter expression is case sensitive. Additional constraints: - You MUST use separator `<space>AND<space>` between terms. - String value MUST NOT contain `<space>AND<space>`.  Each field may support only some operators: - string fields (name, version, creator, uid) support: =, !=, <=, <, >=, > - number fields (cpu, gpu, memory_bytes, storage_bytes) support: =, !=, <=, <, >=, > - bool fields (reconciling) support: =, != - enum fields (state) support: =, != - time fields (create_time) support: =, !=, <=, <, >=, >  Each field may expect values in a specified format: - string fields expect: text or string. For example `foo`, `\"f oo\"`. For example `f oo` is invalid. - number fields expect: numbers (can be wrapped in parentheses). For example: `28`, `-100`, `56.8`, `\"666\"` - integer number fields expect: integers. For example: `cpu = 10.5` is invalid. - bool fields expect: `true` or `false` literals. For example: `reconciling = true` is valid. `reconciling = 1` or `reconciling = TRUE` is invalid. - enum fields expect: enum's string representation. For example `state = STATE_RUNNING` is valid. `state = RUNNING` or `state = state_running` is invalid. - time fields expect: RFC-3339 formatted string. UTC offsets are supported. For example `2012-04-21T11:30:00-04:00` is valid. `2012-04-21` is invalid.  Valid filter expression examples: - `state = STATE_RUNNING AND cpu <= 5 AND gpu != 0 AND create_time > 2012-04-21T11:30:00-04:00` - `state=STATE_RUNNING AND cpu<=5` (there may be no whitespace between term parts: `[filter_field][operator][value]`)  Invalid filter expression examples: - `state = STATE_RUNNING    AND    cpu <= 5` (invalid separator between terms) - `state = STATE_RUNNING OR cpu <= 5` (unsupported logical operator) - `(state = STATE_RUNNING) AND (cpu <= 5)` (unsupported parentheses). [optional]
+            order_by (str): Used to specify the sorting order.  When unset, H2OEngines are ordered by their time of creation in descending order. This is equivalent to \"create_time desc\".  When specified, the value must be a comma separated list of supported fields. The supported fields are:  - name  - version  - cpu  - gpu  - memoryBytes  - creator  - createTime  - updateTime  - deleteTime  - displayName  - maxIdleDuration  - maxRunningDuration  - uid  - nodeCount  The default sorting order is ascending. For example: \"name\" and \"name asc\" are equivalent values.  To specify descending order for a field, append a \" desc\" suffix. For example: \"name desc\".  Redundant space characters are insignificant. For example these values are all equal: - \"  name, cpu     desc\" - \"name, cpu desc\" - \"name   , cpu desc   \"  Undefined (empty) time is interpreted as a zero time (0s since epoch, i.e. 1970-01-01T00:00:00Z).  Undefined (empty) duration is interpreted as a zero duration (0 seconds).. [optional]
+            filter (str): Used to filter H2OEngines. When unset, no filtering is applied.  Filtering implements specification https://google.aip.dev/160.  Supported filter fields: - name - h2o_engine_id - version (supporting version semantic comparison and version aliases) - state - cpu - gpu - memory_bytes - creator - creator_display_name - create_time - update_time - delete_time - reconciling - uid - display_name - max_idle_duration - max_running_duration - current_idle_duration - current_running_duration - node_count  Examples: - `cpu > 5` - `gpu < 3` - `cpu >= 5 AND gpu <= 3` - `cpu != 5 OR gpu == 3` - `NOT (cpu > 5 OR gpu < 3)` - `-(cpu > 5 OR gpu < 3)` - `NOT (cpu > 5 OR (gpu < 3))` - `(cpu > 5 OR gpu < 3) AND memory_bytes != 1000` - `(cpu > 5 OR gpu < 3) AND (NOT ((((memory_bytes = 1000)))))` - `state = STATE_RUNNING AND create_time > \"2012-04-21T11:30:00-04:00\"` - `max_running_duration > \"1s\" AND max_running_duration != \"5s\"` - `version < \"latest\" AND version >= \"3.38.0.1\"` - `reconciling = true OR reconciling = false` (supporting bool literals) - `h2o_engine_id = \"*e*\" OR display_name = \"*e*\"` (supporting prefix/suffix wildcard `*` for string fields equality comparison). [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
```

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_service/apis/__init__.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_service/model/api_http_body.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/model/api_http_body.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_service/model/protobuf_any.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/model/protobuf_any.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_service/model/rpc_status.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/model/rpc_status.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_create_h2_o_engine_response.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_create_h2_o_engine_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_delete_h2_o_engine_response.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_delete_h2_o_engine_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_get_h2_o_engine_response.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_get_h2_o_engine_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_h2_o_engine_service_download_logs_response.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_h2_o_engine_service_download_logs_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_h2_o_engine_state.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_h2_o_engine_state.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_list_h2_o_engines_response.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_list_h2_o_engines_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_engine_service/models/__init__.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/models/__init__.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_version_service/__init__.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_version_service/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: version not set
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "0.3.2"
+__version__ = "0.4.0"
 
 # import ApiClient
 from h2o_engine_manager.gen.h2o_version_service.api_client import ApiClient
 
 # import Configuration
 from h2o_engine_manager.gen.h2o_version_service.configuration import Configuration
```

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_version_service/api_client.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_version_service/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.3.2/python'
+        self.user_agent = 'OpenAPI-Generator/0.4.0/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_version_service/configuration.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_version_service/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -376,15 +376,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: version not set\n"\
-               "SDK Package Version: 0.3.2".\
+               "SDK Package Version: 0.4.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_version_service/exceptions.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_version_service/exceptions.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_version_service/model_utils.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_version_service/model_utils.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_version_service/rest.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_version_service/rest.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_version_service/api/h2_o_version_service_api.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_version_service/api/h2_o_version_service_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -112,15 +112,15 @@
         >>> result = thread.get()
 
 
         Keyword Args:
             page_size (int): Maximum number of H2OVersions to return in a response. If unspecified (or set to 0), at most 50 H2OVersions will be returned. The maximum value is 1000; values above 1000 will be coerced to 1000.. [optional]
             page_token (str): Leave unset to receive the initial page. To list any subsequent pages use the value of 'next_page_token' returned from the ListH2OVersionsResponse.. [optional]
             order_by (str): Used to specify the sorting order.  When unset, H2OVersions are ordered by their version name in descending order. This is equivalent to \"version desc\".  When specified, the value must be a comma separated list of supported fields. The supported fields are: - version  The default sorting order is ascending. For example: \"version\" and \"version asc\" are equivalent values.  To specify descending order for a field, append a \" desc\" suffix. For example: \"version desc\".  Redundant space characters are insignificant.. [optional]
-            filter (str): Used to filter H2OEngines.  When unset, no filtering is applied.  When specified, the filter string must follow these formatting rules:  filter expression: [term] AND [term] AND [term] ... term: [filter_field] [operator] [value] filter_field: (version) operator: (=|!=|<=|<|>=|>) value: ([text]|[string])  Filter expression is case sensitive. Additional constraints: - You MUST use separator `<space>AND<space>` between terms. - String value MUST NOT contain `<space>AND<space>`.  Each field may support only some operators: - version fields (version) support: =, !=, <=, <, >=, >  Each field may expect values in a specified format: - version fields expect: version identifier. Aliases are also accepted. For example: `1.10.1` or `latest`.   If version identifier is NOT an alias and is not in semver format, then it may not be accepted. For example: `abc` is invalid value, if no version has alias 'abc'.  Valid filter expression examples: - `version >= 3.38.0.1 AND version != latest`. [optional]
+            filter (str): Used to filter H2OVersions. When unset, no filtering is applied.  Filtering implements specification https://google.aip.dev/160.  Supported filter fields: - version (supporting version semantic comparison and version aliases)  Examples: - `version > \"latest\" AND version >= \"3.38.0.1\"`. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
```

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_version_service/apis/__init__.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_version_service/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_version_service/model/protobuf_any.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_version_service/model/protobuf_any.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_version_service/model/rpc_status.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_version_service/model/rpc_status.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_version_service/model/v1_h2_o_version.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_version_service/model/v1_h2_o_version.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_version_service/model/v1_list_h2_o_versions_response.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_version_service/model/v1_list_h2_o_versions_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/src/h2o_engine_manager/gen/h2o_version_service/models/__init__.py` & `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_version_service/models/__init__.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/tests/integration/conftest.py` & `h2o_engine_manager-0.4.0/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/tests/integration/setup.py` & `h2o_engine_manager-0.4.0/tests/integration/setup.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/tests/integration/test_admission_webhook.py` & `h2o_engine_manager-0.4.0/tests/integration/test_admission_webhook.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/tests/integration/api/dai/create_dai_request.py` & `h2o_engine_manager-0.4.0/tests/integration/api/dai/create_dai_request.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/tests/integration/api/dai/test_create.py` & `h2o_engine_manager-0.4.0/tests/integration/api/dai/test_create.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import http
 import os
+import time
 
 import pytest
 
 from h2o_engine_manager.clients.dai_engine.dai_engine_state import DAIEngineState
 from h2o_engine_manager.clients.exception import ApiException
 from tests.integration.api.dai.create_dai_request import *
+from tests.integration.conftest import CACHE_SYNC_SECONDS
 
 
 def incorrect_workspace_id(req: CreateDAIEngineRequest) -> CreateDAIEngineRequest:
     req.workspace_id = "no space in id allowed"
     return req
 
 
@@ -49,35 +51,40 @@
 
 
 def incorrect_version(req: CreateDAIEngineRequest) -> CreateDAIEngineRequest:
     req.version = "non-existing-version"
     return req
 
 
+def incorrect_config(req: CreateDAIEngineRequest) -> CreateDAIEngineRequest:
+    req.config = {"base_url": "whatever"}
+    return req
+
+
 def test_create_dai(dai_client):
     # When
     engine = dai_client.create_engine(
         workspace_id="create-dai",
         engine_id="engine1",
-        version="1.10.5",
+        version="1.10.5-mock",
         cpu=1,
         gpu=0,
         memory_bytes="1Gi",
         storage_bytes="1Gi",
         max_idle_duration="2h",
         max_running_duration="12h",
         display_name="Proboscis monkey",
-        config={"key1": "val1", "auth_openid_client_id": "youShallNotPass"},
+        config={"key1": "val1"},
     )
 
     # Then
     assert engine.name == "workspaces/create-dai/daiEngines/engine1"
     assert engine.state == DAIEngineState.STATE_STARTING
     assert engine.reconciling is True
-    assert engine.version == "1.10.5"
+    assert engine.version == "1.10.5-mock"
     assert engine.cpu == 1
     assert engine.gpu == 0
     assert engine.max_idle_duration == "2h"
     assert engine.max_running_duration == "12h"
     assert engine.display_name == "Proboscis monkey"
     assert engine.annotations == {}
     assert engine.config == {"key1": "val1"}
@@ -103,27 +110,28 @@
     # When
     req = CreateDAIEngineRequest(
         workspace_id="create-dai-version-alias", version="alias-foo"
     )
     eng = create_dai_from_request(dai_client, req)
 
     # Then
-    assert eng.version == "1.10.5"
+    assert eng.version == "1.10.5-mock"
 
 
 @pytest.mark.parametrize(
     "modify_func",
     [
         incorrect_workspace_id,
         incorrect_engine_id,
         cpu_below_min,
         gpu_below_min,
         memory_below_min,
         incorrect_display_name,
         incorrect_version,
+        incorrect_config,
     ],
 )
 def test_create_dai_server_validation(dai_client, modify_func):
     # When
     req = modify_func(CreateDAIEngineRequest(workspace_id="create-dai-validation"))
 
     # Then
@@ -183,7 +191,22 @@
     )
     assert e.cpu == 1
     assert e.gpu == 0
     assert e.memory_bytes == "1Gi"
     assert e.storage_bytes == "1Gi"
     assert e.max_idle_duration == "4h"
     assert e.max_running_duration == "4h"
+
+
+def test_create_engine_id_generator(dai_client):
+    # Engine ID should be uniquely generated if not provided
+    no_param_1 = dai_client.create_engine(workspace_id="create-dai-generate-engine-id")
+    time.sleep(CACHE_SYNC_SECONDS)
+    no_param_2 = dai_client.create_engine(workspace_id="create-dai-generate-engine-id")
+    assert no_param_1.name != no_param_2.name
+
+    # Engine ID should be uniquely generated from display name
+    display_name_1 = dai_client.create_engine(workspace_id="create-dai-generate-engine-id", display_name="Smoker@2023")
+    time.sleep(CACHE_SYNC_SECONDS)
+    display_name_2 = dai_client.create_engine(workspace_id="create-dai-generate-engine-id", display_name="Smoker@2023")
+    assert display_name_1.name != display_name_2.name
+
```

### Comparing `h2o_engine_manager-0.3.2/tests/integration/api/dai/test_delete.py` & `h2o_engine_manager-0.4.0/tests/integration/api/dai/test_delete.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/tests/integration/api/dai/test_get.py` & `h2o_engine_manager-0.4.0/tests/integration/api/dai/test_get.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/tests/integration/api/dai/test_list.py` & `h2o_engine_manager-0.4.0/tests/integration/api/dai/test_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 def create_engines(dai_client, workspace_id):
     req1 = CreateDAIEngineRequest(
         workspace_id=workspace_id, engine_id="engine1", cpu=1, gpu=3, version="latest"
     )
     req2 = CreateDAIEngineRequest(
-        workspace_id=workspace_id, engine_id="engine2", cpu=2, gpu=2, version="1.10.5"
+        workspace_id=workspace_id, engine_id="engine2", cpu=2, gpu=2, version="1.10.5-mock"
     )
     req3 = CreateDAIEngineRequest(
         workspace_id=workspace_id, engine_id="engine3", cpu=2, gpu=1, version="1.10.6"
     )
     create_dai_from_request(dai_client, req1)
     create_dai_from_request(dai_client, req2)
     create_dai_from_request(dai_client, req3)
@@ -124,23 +124,23 @@
     assert len(engines) == 2
     check_ordered_filtered(engines=engines)
 
     # Test version sorting & filtering.
     engines = dai_client.list_all_engines(
         workspace_id=workspace_id,
         order_by="version asc",
-        filter="version < latest AND version >= 1.10.5",
+        filter="version < \"latest\" AND version >= \"1.10.5-mock\"",
     )
     assert len(engines) == 2
-    assert engines[0].version == "1.10.5"
+    assert engines[0].version == "1.10.5-mock"
     assert engines[1].version == "1.10.6"
 
     # Test version sorting & filtering.
     engines = dai_client.list_all_engines(
-        workspace_id=workspace_id, filter="version = latest"
+        workspace_id=workspace_id, filter="version = \"latest\""
     )
     assert len(engines) == 1
     assert engines[0].version == "1.10.6.1"
 
     # Test order by UID.
     page = dai_client.list_engines(workspace_id=workspace_id, order_by="uid desc")
```

### Comparing `h2o_engine_manager-0.3.2/tests/integration/api/dai/test_list_versions.py` & `h2o_engine_manager-0.4.0/tests/integration/api/dai/test_list_versions.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 
 def test_list_all_dai_version(dai_client):
     # Arrange - DAIVersion CRDs are already present in the cluster.
     expected = [
         DAIVersion(version="1.10.6.1", aliases=["latest"], annotations={}),
         DAIVersion(version="1.10.6.1-alpha", aliases=[], annotations={}),
         DAIVersion(version="1.10.6", aliases=[], annotations={}),
-        DAIVersion(version="1.10.5", aliases=["mock", "alias-foo"], annotations={}),
+        DAIVersion(version="1.10.5", aliases=[], annotations={}),
+        DAIVersion(version="1.10.5-mock", aliases=["mock", "alias-foo"], annotations={}),
         DAIVersion(version="1.10.5-do-not-use-me", aliases=[], annotations={}),
         DAIVersion(version="1.10.4", aliases=[], annotations={"foo": "foo"}),
     ]
 
     # When
     dai_versions = dai_client.list_all_versions()
 
@@ -28,26 +29,26 @@
 def test_paging_dai_versions(dai_client):
     # Arrange - DAIVersion CRDs are already present in the cluster.
 
     # When - list first page.
     first_page = dai_client.list_versions(page_size=1)
 
     # Then
-    assert first_page.total_size == 6
+    assert first_page.total_size == 7
     assert len(first_page.dai_versions) == 1
     assert first_page.next_page_token != ""
 
     # When - list second (last) page.
     second_page = dai_client.list_versions(
-        page_size=5, page_token=first_page.next_page_token
+        page_size=6, page_token=first_page.next_page_token
     )
 
     # Then
-    assert second_page.total_size == 6
-    assert len(second_page.dai_versions) == 5
+    assert second_page.total_size == 7
+    assert len(second_page.dai_versions) == 6
     assert second_page.next_page_token == ""
     assert first_page.dai_versions[0].version != second_page.dai_versions[0].version
 
 
 def test_incorrect_page_token(dai_client):
     with pytest.raises(ApiException) as exc:
         dai_client.list_versions(page_token="non-existing-token")
@@ -62,20 +63,20 @@
 
 
 def test_page_size(dai_client):
     # When - request page size greater than total number of items.
     page = dai_client.list_versions(page_size=10000)
 
     # Then
-    assert page.total_size == 6
+    assert page.total_size == 7
 
 
 def test_filter(dai_client):
     # When supported filter expression (alias values are supported).
-    vs = dai_client.list_versions(filter="version < latest AND version > 1.10.6")
+    vs = dai_client.list_versions(filter="version < \"latest\" AND version > \"1.10.6\"")
 
     # Then only one DAIVersion conforms to the filter expression
     assert vs.total_size == 1
     assert vs.next_page_token == ""
     assert len(vs.dai_versions) == 1
     assert vs.dai_versions[0].version == "1.10.6.1-alpha"
```

### Comparing `h2o_engine_manager-0.3.2/tests/integration/api/dai/test_upgrade_available.py` & `h2o_engine_manager-0.4.0/tests/integration/api/dai/test_upgrade_available.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/tests/integration/api/dai_engine_constraint/test_get_dai_engine_constraint.py` & `h2o_engine_manager-0.4.0/tests/integration/api/dai_engine_constraint/test_get_dai_engine_constraint.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/tests/integration/api/engine/test_list_engines.py` & `h2o_engine_manager-0.4.0/tests/integration/api/engine/test_list_engines.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,34 +44,37 @@
     for req in requests:
         create_dai_from_request(dai_client, req)
 
     h2o_engine_client.create_engine(
         workspace_id=workspace_id,
         engine_id="engine1",
         version="3.36.1.5",
+        node_count=1,
         cpu=2,
         gpu=0,
         memory_bytes="1Mi",
         max_idle_duration="2h",
         max_running_duration="12h",
     )
     h2o_engine_client.create_engine(
         workspace_id=workspace_id,
         engine_id="engine2",
-        version="3.38.0.1",
+        version="3.38.0.4",
+        node_count=1,
         cpu=2,
         gpu=0,
         memory_bytes="1Ki",
         max_idle_duration="2h",
         max_running_duration="12h",
     )
     h2o_engine_client.create_engine(
         workspace_id=workspace_id,
         engine_id="engine3",
-        version="3.38.0.2",
+        version="3.40.0.3",
+        node_count=1,
         cpu=3,
         gpu=1,
         memory_bytes="1Mi",
         max_idle_duration="2h",
         max_running_duration="12h",
     )
 
@@ -134,18 +137,18 @@
         page.engines[0].name == f"workspaces/{workspace_id}/daiEngines/engine2"
     )  # highest cpu (4)
     assert (
         page.engines[1].name == f"workspaces/{workspace_id}/h2oEngines/engine3"
     )  # second-highest cpu (3)
     assert (
         page.engines[2].name == f"workspaces/{workspace_id}/h2oEngines/engine2"
-    )  # highest version (3.38.0.1)
+    )  # highest version (3.40.0.3)
     assert (
         page.engines[3].name == f"workspaces/{workspace_id}/h2oEngines/engine1"
-    )  # second-highest version (3.36.1.5)
+    )  # second-highest version (3.38.0.4)
     assert (
         page.engines[4].name == f"workspaces/{workspace_id}/daiEngines/engine1"
     )  # highest memory_bytes (1Mi)
     assert page.engines[5].name == f"workspaces/{workspace_id}/daiEngines/engine3"
 
     # When filter non-existing
     page = engine_client.list_engines(
@@ -155,15 +158,15 @@
 
     # Then
     assert len(page.engines) == 0
     assert page.total_size == 0
     assert page.next_page_token == ""
 
     # When filter
-    expr = "type = TYPE_DRIVERLESS_AI AND version < 1.10.5 AND memory_bytes > 1024"
+    expr = "type = TYPE_DRIVERLESS_AI AND version < \"1.10.5\" AND memory_bytes > 1024"
     page = engine_client.list_engines(workspace_id=workspace_id, filter_expr=expr)
 
     # Then
     assert len(page.engines) == 1
     assert page.total_size == 1
     assert page.next_page_token == ""
     assert page.engines[0].name == f"workspaces/{workspace_id}/daiEngines/engine1"
```

### Comparing `h2o_engine_manager-0.3.2/tests/integration/api/h2o/test_create_h2o_engine.py` & `h2o_engine_manager-0.4.0/tests/integration/api/h2o/test_create_h2o_engine.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 import http
 import json
 import os
+import time
 
 import pytest
 
 from h2o_engine_manager.clients.exception import ApiException
 from h2o_engine_manager.clients.h2o_engine.state import H2OEngineState
+from tests.integration.conftest import CACHE_SYNC_SECONDS
 
 
 def test_create(h2o_engine_client):
     # When
     engine = h2o_engine_client.create_engine(
         workspace_id="create-h2o-engine",
         engine_id="engine1",
         version="latest",
+        node_count=2,
         cpu=1,
         gpu=0,
         memory_bytes="2Gi",
         max_idle_duration="2h",
         max_running_duration="12h",
         display_name="Proboscis monkey",
         annotations={"foo": "bar"},
     )
 
     # Then
     assert engine.name == "workspaces/create-h2o-engine/h2oEngines/engine1"
     assert engine.state == H2OEngineState.STATE_STARTING
     assert engine.reconciling is True
-    assert engine.version == "3.38.0.2"
+    assert engine.version == "0.0.0.0-latest"
+    assert engine.node_count == 2
     assert engine.cpu == 1
     assert engine.gpu == 0
     assert engine.max_idle_duration == "2h"
     assert engine.max_running_duration == "12h"
     assert engine.display_name == "Proboscis monkey"
     assert engine.annotations == {"foo": "bar"}
     assert engine.create_time is not None
@@ -55,27 +59,28 @@
     engine = h2o_engine_client.create_engine(
         workspace_id="create-h2o-engine",
         engine_id="engine-default-values",
         version="latest",
     )
 
     # Then default values are filled from workspace constraints (see system.default H2OSetup)
+    assert engine.node_count == 1
     assert engine.cpu == 1
     assert engine.gpu == 0
     assert engine.max_idle_duration == "1h"
     assert engine.max_running_duration == "4h"
     assert engine.memory_bytes == "4Gi"
 
     # Other fields are set according to API
     assert (
         engine.name == "workspaces/create-h2o-engine/h2oEngines/engine-default-values"
     )
     assert engine.state == H2OEngineState.STATE_STARTING
     assert engine.reconciling is True
-    assert engine.version == "3.38.0.2"
+    assert engine.version == "0.0.0.0-latest"
     assert engine.display_name == ""
     assert engine.annotations == {}
     assert engine.create_time is not None
     assert engine.delete_time is None
     external_hostname = os.getenv("MANAGER_EXTERNAL_HOSTNAME")
     assert (
         engine.api_url
@@ -105,7 +110,21 @@
         h2o_engine_client.create_engine(
             workspace_id="create-h2o-engine-validation-unavailable-version",
             engine_id="engine1",
             version="foo",
         )
     assert exc.value.status == http.HTTPStatus.BAD_REQUEST
     assert 'version "foo" is unavailable' == json.loads(exc.value.body)["message"]
+
+
+def test_create_engine_id_generator(h2o_engine_client):
+    # Engine ID should be uniquely generated if not provided
+    no_param_1 = h2o_engine_client.create_engine(workspace_id="create-h2o-generate-engine-id", version="latest")
+    time.sleep(CACHE_SYNC_SECONDS)
+    no_param_2 = h2o_engine_client.create_engine(workspace_id="create-h2o-generate-engine-id", version="latest")
+    assert no_param_1.name != no_param_2.name
+
+    # Engine ID should be uniquely generated from display name
+    display_name_1 = h2o_engine_client.create_engine(workspace_id="create-h2o-generate-engine-id", display_name="Smoker@2023", version="latest")
+    time.sleep(CACHE_SYNC_SECONDS)
+    display_name_2 = h2o_engine_client.create_engine(workspace_id="create-h2o-generate-engine-id", display_name="Smoker@2023", version="latest")
+    assert display_name_1.name != display_name_2.name
```

### Comparing `h2o_engine_manager-0.3.2/tests/integration/api/h2o/test_delete_h2o_engine.py` & `h2o_engine_manager-0.4.0/tests/integration/api/h2o/test_delete_h2o_engine.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 def test_delete_validate_only(h2o_engine_client):
     workspace_id = "delete-h2o-validate"
     engine_id = "e1"
 
     e = h2o_engine_client.create_engine(
         workspace_id=workspace_id,
         engine_id=engine_id,
-        version="3.38.0.2",
+        version="3.40.0.3",
+        node_count=1,
         cpu=1,
         gpu=0,
         max_idle_duration="5h",
         max_running_duration="10h",
     )
 
     e.delete(validate_only=True)
@@ -34,15 +35,16 @@
 def test_delete(h2o_engine_client):
     workspace_id = "delete-h2o"
     engine_id = "e1"
 
     e = h2o_engine_client.create_engine(
         workspace_id=workspace_id,
         engine_id=engine_id,
-        version="3.38.0.2",
+        version="3.40.0.3",
+        node_count=1,
         cpu=1,
         gpu=0,
         max_idle_duration="5h",
         max_running_duration="10h",
     )
 
     e.delete()
```

### Comparing `h2o_engine_manager-0.3.2/tests/integration/api/h2o/test_get_h2o_engine.py` & `h2o_engine_manager-0.4.0/tests/integration/api/h2o/test_get_h2o_engine.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     engine_id = "engine1"
 
     # Given
     h2o_engine_client.create_engine(
         workspace_id=workspace_id,
         engine_id=engine_id,
         version="latest",
+        node_count=1,
         cpu=1,
         gpu=0,
         memory_bytes="2Gi",
         max_idle_duration="2h",
         max_running_duration="12h",
         display_name="Proboscis monkey",
         annotations={"foo": "bar"},
@@ -28,15 +29,16 @@
     # When
     e = h2o_engine_client.get_engine(workspace_id=workspace_id, engine_id=engine_id)
 
     # Then
     assert e.name == f"workspaces/{workspace_id}/h2oEngines/{engine_id}"
     assert e.state == H2OEngineState.STATE_STARTING
     assert e.reconciling is True
-    assert e.version == "3.38.0.2"
+    assert e.version == "0.0.0.0-latest"
+    assert e.node_count == 1
     assert e.cpu == 1
     assert e.gpu == 0
     assert e.max_idle_duration == "2h"
     assert e.max_running_duration == "12h"
     assert e.display_name == "Proboscis monkey"
     assert e.annotations == {"foo": "bar"}
     assert e.create_time is not None
```

### Comparing `h2o_engine_manager-0.3.2/tests/integration/api/h2o/test_list_h2o_engines.py` & `h2o_engine_manager-0.4.0/tests/integration/api/h2o/test_list_h2o_engines.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,39 +5,42 @@
 from tests.integration.conftest import CACHE_SYNC_SECONDS
 
 
 def create_engines(h2o_engine_client, workspace_id):
     h2o_engine_client.create_engine(
         workspace_id=workspace_id,
         engine_id="e1",
-        version="3.38.0.2",
+        version="3.40.0.3",
+        node_count=1,
         cpu=1,
         gpu=0,
         memory_bytes="2Gi",
         display_name="my engine 1",
         max_idle_duration="5h",
         max_running_duration="10h",
     )
 
     h2o_engine_client.create_engine(
         workspace_id=workspace_id,
         engine_id="e2",
         version="3.36.1.5",
+        node_count=1,
         cpu=2,
         gpu=0,
         memory_bytes="2Gi",
         display_name="my engine 2",
         max_idle_duration="5h",
         max_running_duration="10h",
     )
 
     h2o_engine_client.create_engine(
         workspace_id=workspace_id,
         engine_id="e3",
-        version="3.38.0.1",
+        version="3.38.0.4",
+        node_count=1,
         cpu=3,
         gpu=0,
         memory_bytes="2Gi",
         display_name="my engine 3",
         max_idle_duration="5h",
         max_running_duration="10h",
     )
@@ -93,18 +96,18 @@
     assert len(page.engines) == 2
     assert page.next_page_token == ""
     assert page.total_size == 2
     check_ordered_filtered(engines=page.engines)
 
     # List all with order and filter (+ testing version alias filtering).
     engines = h2o_engine_client.list_all_engines(
-        workspace_id=workspace_id, order_by="version desc", filter="version < latest"
+        workspace_id=workspace_id, order_by="version desc", filter="version < \"smoker\""
     )
     assert len(engines) == 2
-    assert engines[0].version == "3.38.0.1"
+    assert engines[0].version == "3.38.0.4"
     assert engines[1].version == "3.36.1.5"
 
 
 def check_ordered_filtered(engines: List[H2OEngine]):
     # Hardcoded values based on filter/orderBy params in tests.
     for i in range(0, len(engines) - 1):
         assert engines[i].cpu >= 2
```

### Comparing `h2o_engine_manager-0.3.2/tests/integration/api/h2o/test_list_h2o_versions.py` & `h2o_engine_manager-0.4.0/tests/integration/api/h2o/test_list_h2o_versions.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 
 from h2o_engine_manager.clients.exception import ApiException
 from h2o_engine_manager.clients.h2o_version.h2o_version import H2OVersion
 
 
 def test_list_all_h2o_version(h2o_engine_client):
     expected = [
-        H2OVersion(version="3.38.0.2", aliases=["latest"], annotations={}),
-        H2OVersion(version="3.38.0.1", aliases=[], annotations={}),
+        H2OVersion(version="3.40.0.3", aliases=["smoker"], annotations={}),
+        H2OVersion(version="3.38.0.4", aliases=[], annotations={}),
         H2OVersion(version="3.36.1.5", aliases=[], annotations={"bar": "baz"}),
         H2OVersion(version="0.0.0.0", aliases=["mock"], annotations={}),
+        H2OVersion(version="0.0.0.0-latest", aliases=["latest"], annotations={}),
     ]
 
     # When
     h2o_versions = h2o_engine_client.list_all_versions()
 
     # Then
     for i in range(0, len(expected)):
@@ -23,26 +24,26 @@
 
 
 def test_paging_h2o_versions(h2o_engine_client):
     # When - list first page.
     first_page = h2o_engine_client.list_versions(page_size=1)
 
     # Then
-    assert first_page.total_size == 4
+    assert first_page.total_size == 5
     assert len(first_page.h2o_versions) == 1
     assert first_page.next_page_token != ""
 
     # When - list second (last) page.
     second_page = h2o_engine_client.list_versions(
         page_size=5, page_token=first_page.next_page_token
     )
 
     # Then
-    assert second_page.total_size == 4
-    assert len(second_page.h2o_versions) == 3
+    assert second_page.total_size == 5
+    assert len(second_page.h2o_versions) == 4
     assert second_page.next_page_token == ""
     assert first_page.h2o_versions[0].version != second_page.h2o_versions[0].version
 
 
 def test_incorrect_page_token(h2o_engine_client):
     with pytest.raises(ApiException) as exc:
         h2o_engine_client.list_versions(page_token="non-existing-token")
@@ -57,28 +58,28 @@
 
 
 def test_page_size(h2o_engine_client):
     # When - request page size greater than total number of items.
     page = h2o_engine_client.list_versions(page_size=10000)
 
     # Then
-    assert page.total_size == 4
+    assert page.total_size == 5
 
 
 def test_filter(h2o_engine_client):
     # When supported filter expression (alias values are supported).
     vs = h2o_engine_client.list_versions(
-        filter="version < latest AND version >= 3.38.0.0"
+        filter="version < \"smoker\" AND version >= \"3.38.0.0\""
     )
 
     # Then only one H2OVersion conforms to the filter expression
     assert vs.total_size == 1
     assert vs.next_page_token == ""
     assert len(vs.h2o_versions) == 1
-    assert vs.h2o_versions[0].version == "3.38.0.1"
+    assert vs.h2o_versions[0].version == "3.38.0.4"
 
 
 def test_invalid_filter_expr(h2o_engine_client):
     with pytest.raises(ApiException) as exc:
         # alias field is not supported for filtering
         h2o_engine_client.list_versions(filter="alias = latest")
     assert exc.value.status == http.HTTPStatus.BAD_REQUEST
```

### Comparing `h2o_engine_manager-0.3.2/tests/integration/api/h2o_engine_constraint/test_get_h2o_engine_constraint.py` & `h2o_engine_manager-0.4.0/tests/integration/api/h2o_engine_constraint/test_get_h2o_engine_constraint.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 
     # When getting h2oEngineConstraintSet from workspace without DriverlessAISetup
     constraint_set = h2o_engine_constraint_set_client.get_constraint_set(
         workspace_id="definitely-not-existing-workspace-h2o-engine-constraint-set"
     )
 
     # Then h2oEngineConstraintSet should be equal to default (system.default H2OSetup)
+    assert constraint_set.node_count.min == "1"
+    assert constraint_set.node_count.max is None
+    assert constraint_set.node_count.default == "1"
+
     assert constraint_set.cpu.min == "1"
     assert constraint_set.cpu.max is None
     assert constraint_set.cpu.default == "1"
 
     assert constraint_set.gpu.min == "0"
     assert constraint_set.gpu.max is None
     assert constraint_set.gpu.default == "0"
@@ -37,14 +41,18 @@
 
     # When getting h2oEngineConstraintSet from workspace without H2OSetup
     constraint_set = h2o_engine_constraint_set_client.get_constraint_set(
         workspace_id="existing-h2o-engine-constraint-set"
     )
 
     # Then h2oEngineConstraintSet should be equal to existing-h2o-engine-constraint-set
+    assert constraint_set.node_count.min == "1"
+    assert constraint_set.node_count.max == "10"
+    assert constraint_set.node_count.default == "3"
+
     assert constraint_set.cpu.min == "2"
     assert constraint_set.cpu.max == "4"
     assert constraint_set.cpu.default == "2"
 
     assert constraint_set.gpu.min == "1"
     assert constraint_set.gpu.max is None
     assert constraint_set.gpu.default == "1"
```

### Comparing `h2o_engine_manager-0.3.2/tests/integration/e2e/dai/test_connect.py` & `h2o_engine_manager-0.4.0/tests/integration/e2e/dai/test_connect.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/tests/integration/e2e/dai/test_dai_pod_template_spec.py` & `h2o_engine_manager-0.4.0/tests/integration/e2e/dai/test_dai_pod_template_spec.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/tests/integration/e2e/dai/test_dai_resume.py` & `h2o_engine_manager-0.4.0/tests/integration/e2e/dai/test_dai_resume.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/tests/integration/e2e/dai/test_lifecycle.py` & `h2o_engine_manager-0.4.0/tests/integration/e2e/dai/test_lifecycle.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,27 +28,28 @@
 
     # Test Create
     engine = dai_client.create_engine(
         workspace_id=workspace_id,
         engine_id=engine_id,
         version=want_version,
         cpu=1,
-        gpu=0,
+        gpu=1,
         memory_bytes="8Gi",
         storage_bytes="16Gi",
         max_idle_duration="15m",
         max_running_duration="2d",
         display_name="My engine 1",
         config={"max_runtime_minutes": "120", "feature_engineering_effort": "5"},
     )
     deleted = False
 
     try:
         assert engine.name == f"workspaces/{workspace_id}/daiEngines/{engine_id}"
         assert engine.state.name == DAIEngineState.STATE_STARTING.name
+        assert engine.gpu == 1
 
         # Test Pause during STARTING.
         engine.pause()
         assert engine.state.name == DAIEngineState.STATE_PAUSING.name
 
         # Test Pause noop. Engine can be already paused (current state is updated even for noop).
         engine.pause()
@@ -107,16 +108,18 @@
 
         # Test Wait for PAUSED
         engine.wait()
         assert engine.state.name == DAIEngineState.STATE_PAUSED.name
 
         # Test Update
         engine.cpu = 2
+        engine.gpu = 0
         engine.update()
         assert engine.cpu == 2
+        assert engine.gpu == 0
 
         # Test Resume
         engine.resume()
         assert engine.state.name == DAIEngineState.STATE_STARTING.name
 
         # Test waiting with timeout. Expecting that engine reaches RUNNING state
         # in more than 2 seconds.
```

### Comparing `h2o_engine_manager-0.3.2/tests/integration/e2e/dai/test_login_discovery.py` & `h2o_engine_manager-0.4.0/tests/integration/e2e/dai/test_login_discovery.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/tests/integration/e2e/dai/test_migrate_creator.py` & `h2o_engine_manager-0.4.0/tests/integration/e2e/dai/test_migrate_creator.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 from tests.integration.api.dai.create_dai_request import CreateDAIEngineRequest
 from tests.integration.api.dai.create_dai_request import create_dai_from_request
 from tests.integration.conftest import CACHE_SYNC_SECONDS
 
 
 # Migrate creator test must be performed in tests
 # that run also operator because the engine needs to be connected to.
-@pytest.mark.timeout(180)
-@pytest.mark.skip(reason="waiting for the 1.10.5 official release")
+@pytest.mark.timeout(600)
 def test_migrate_creator(dai_client, dai_admin_client):
     workspace_id = "set-creator"
     engine_id = "e1"
     aiem_test_admin_user = (
         "fd138058-c564-4bed-a7b9-e63a5eb6348d"  # taken from the platform token
     )
     req = CreateDAIEngineRequest(
         workspace_id=workspace_id,
         engine_id=engine_id,
         memory_bytes="8Gi",
         storage_bytes="8Gi",
+        version="1.10.5"
     )
     # Create an engine as the aiem-test-user user
     eng = create_dai_from_request(dai_client, req)
     time.sleep(CACHE_SYNC_SECONDS)
     try:
         # Get the engine as an admin user
         eng_admin = dai_admin_client.get_engine(
```

### Comparing `h2o_engine_manager-0.3.2/tests/integration/e2e/dai/test_migration.py` & `h2o_engine_manager-0.4.0/tests/integration/e2e/dai/test_migration.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     os.environ["UPGRADE_VERSION"] = "1.10.4"
     os.environ["ISSUER_URL"] = os.getenv("PLATFORM_OIDC_URL")
     os.environ["CLIENT_ID"] = os.getenv("PLATFORM_OIDC_CLIENT_ID")
 
     migration_finished = False
 
     # Migrated engines will have these IDs.
-    migrated_engines_id = ["mig1-19", "mig2-20", "mig3-21", "renamed-22"]
+    migrated_engines_id = ["mig1-19", "mig2-20", "mig3-21", "renamed-22", "non-dai-data-25"]
 
     try:
         # Call the script.
         subprocess.check_call(["hatch", "run", "test:python", "../migrator/migrate_steam.py"])
         migration_finished = True
 
         # Test that all engines were migrated.
@@ -43,14 +43,21 @@
         engine.resume()
         engine.wait()
         dai = engine.connect()
 
         # Experiment was trained on the Steam-launched instance, it should migrate and be found on the AIEM-resumed engine.
         assert dai.experiments.get("c27ee8de-e595-11ed-a4ca-be06d0bbe0b9").name == "ginofove"
 
+        # Verify also second instance that was created with non-dai uid/gid.
+        engine = dai_client.get_engine(workspace_id="default", engine_id="non-dai-data-25")
+        engine.resume()
+        engine.wait()
+        dai = engine.connect()
+        assert dai.experiments.get("3064f046-efeb-11ed-b0de-1e2c8af3eb07").name == "bemurati"
+
     finally:
         allow_missing = False
         if not migration_finished:
             # If the migration failed, then we cannot know whether the engines were created.
             allow_missing = True
 
         for engine_id in migrated_engines_id:
```

### Comparing `h2o_engine_manager-0.3.2/tests/integration/e2e/dai/test_update.py` & `h2o_engine_manager-0.4.0/tests/integration/e2e/dai/test_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,16 +140,14 @@
         assert engine.state.name == DAIEngineState.STATE_PAUSED.name
 
         assert engine.config == {"key1": "val1", "key2": "val2"}
 
         engine.config = {
             "key1": "newVal1",
             "key3": "val3",
-            "authentication_method": "Darwin?",
-            "base_url": "Wot is mista?",
         }
         engine.update(update_mask="config")
 
         assert engine.config == {"key1": "newVal1", "key3": "val3"}
 
         # Extra white-box testing using k8s client to check that baseConfig in CRD object is not
         # affected by this update action (we cannot verify directly via AIEM API as its hidden).
```

### Comparing `h2o_engine_manager-0.3.2/tests/integration/e2e/dai/test_upgrade_version.py` & `h2o_engine_manager-0.4.0/tests/integration/e2e/dai/test_upgrade_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         workspace_id=workspace_id, engine_id=engine_id, version="1.10.4"
     )
     eng = create_dai_from_request(dai_client, req)
     try:
         # Only stopped engine can be upgraded.
         assert eng.state != DAIEngineState.STATE_PAUSED
         with pytest.raises(ApiException) as exc:
-            eng.upgrade_version(new_version="1.10.5")
+            eng.upgrade_version(new_version="1.10.5-mock")
         assert exc.value.status == http.HTTPStatus.BAD_REQUEST
 
         eng.pause()
         eng.wait()
 
         # Only available version can be used for upgrade.
         with pytest.raises(ApiException) as exc:
@@ -35,16 +35,16 @@
         assert exc.value.status == http.HTTPStatus.BAD_REQUEST
 
         # Can upgrade only to newer version.
         with pytest.raises(ApiException) as exc:
             eng.upgrade_version(new_version="1.10.4")
         assert exc.value.status == http.HTTPStatus.BAD_REQUEST
 
-        eng.upgrade_version(new_version="1.10.5")
-        assert eng.version == "1.10.5"
+        eng.upgrade_version(new_version="1.10.5-mock")
+        assert eng.version == "1.10.5-mock"
         # Upgrading version is also a form of update -> update_time should be set.
         ut = eng.update_time
         assert ut is not None
 
         # update_time precision is one second,
         # need to wait at least one second for correct later comparison
         time.sleep(1)
```

### Comparing `h2o_engine_manager-0.3.2/tests/integration/e2e/h2o/test_h2o_engine_lifecycle.py` & `h2o_engine_manager-0.4.0/tests/integration/e2e/h2o/test_h2o_engine_lifecycle.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import h2o
 import pytest
+from h2o.estimators import H2OXGBoostEstimator
 
 from h2o_engine_manager.clients.h2o_engine.state import H2OEngineState
 
 
 @pytest.mark.timeout(900)
 def test_lifecycle(h2o_engine_client):
     workspace_id = "test-h2o-lifecycle"
@@ -19,14 +20,15 @@
     )
     assert len(result) > 0
 
     e = h2o_engine_client.create_engine(
         workspace_id=workspace_id,
         engine_id=engine_id,
         version="latest",
+        node_count=3,
         cpu=1,
         gpu=0,
         memory_bytes="2Gi",
         max_idle_duration="2h",
         max_running_duration="12h",
         display_name="Karlito",
         annotations={"Lela": "Lulu"},
@@ -37,14 +39,20 @@
         assert e.state.name == H2OEngineState.STATE_STARTING.name
 
         e.wait()
         assert e.state.name == H2OEngineState.STATE_RUNNING.name
 
         h2o.connect(config=e.get_connection_config())
 
+        df = h2o.import_file(path="https://s3.amazonaws.com/h2o-public-test-data/smalldata/gbm_test/ecology_model.csv")
+
+        df["Angaus"] = df["Angaus"].asfactor()
+        model = H2OXGBoostEstimator()
+        model.train(x=list(range(2, df.ncol)), y="Angaus", training_frame=df)
+
         e2 = h2o_engine_client.get_engine(
             engine_id=engine_id, workspace_id=workspace_id
         )
         assert e.name == e2.name
 
         engs = h2o_engine_client.list_all_engines(workspace_id=workspace_id)
         assert len(engs) == 1
```

### Comparing `h2o_engine_manager-0.3.2/tests/integration/e2e/h2o/test_h2o_logs.py` & `h2o_engine_manager-0.4.0/tests/integration/e2e/h2o/test_h2o_logs.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     workspace_id = "test-logs"
     engine_id = "felix"
 
     e = h2o_engine_client.create_engine(
         workspace_id=workspace_id,
         engine_id=engine_id,
         version="mock",
+        node_count=1,
         cpu=1,
         gpu=0,
         memory_bytes="2Gi",
         max_idle_duration="2h",
         max_running_duration="12h",
     )
```

### Comparing `h2o_engine_manager-0.3.2/tests/integration/e2e/h2o/test_h2o_pod_template_spec.py` & `h2o_engine_manager-0.4.0/tests/integration/e2e/h2o/test_h2o_pod_template_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,14 +90,15 @@
     want_version = "mock"
 
     # Create H2OEngine (which internally creates H2O k8s object).
     return h2o_engine_client.create_engine(
         workspace_id=workspace_id,
         engine_id=engine_id,
         version=want_version,
+        node_count=1,
         cpu=1,
         gpu=gpu,
         memory_bytes="1Gi",
         max_idle_duration="15m",
         max_running_duration="2d",
         display_name="My engine 1",
     )
```

### Comparing `h2o_engine_manager-0.3.2/tests/integration/test_data/dai_setups/dai-connect.yaml` & `h2o_engine_manager-0.4.0/tests/integration/test_data/dai_setups/dai-connect.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -5,19 +5,14 @@
   # (this additional setup is applied on all DAIEngines that are in 'dai-connect' workspace)
   name: dai-connect
 spec:
   podTemplateSpec:
     spec:
       containers:
         - name: driverless-ai
-      tolerations:
-        - key: "dedicated"
-          operator: "Equal"
-          value: "steam"
-          effect: "NoSchedule"
   cpuConstraint:
     min: 1
     default: 1
   gpuConstraint:
     min: 0
     default: 0
   memoryBytesConstraint:
@@ -27,8 +22,13 @@
     min: 1
     default: 1
   maxIdleDurationConstraint:
     min: "0s"
     default: "2h"
   maxRunningDurationConstraint:
     min: "0s"
-    default: "2h"
+    default: "2h"
+  gpuTolerations:
+    - key: "dedicated"
+      operator: "Equal"
+      value: "gpu"
+      effect: "NoSchedule"
```

### Comparing `h2o_engine_manager-0.3.2/tests/integration/test_data/dai_setups/dai-lifecycle.yaml` & `h2o_engine_manager-0.4.0/tests/integration/test_data/dai_setups/dai-lifecycle.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -5,19 +5,14 @@
   # (this additional setup is applied on all DAIEngines that are in 'dai-lifecycle' workspace)
   name: dai-lifecycle
 spec:
   podTemplateSpec:
     spec:
       containers:
         - name: driverless-ai
-      tolerations:
-        - key: "dedicated"
-          operator: "Equal"
-          value: "steam"
-          effect: "NoSchedule"
   cpuConstraint:
     min: 1
     default: 1
   gpuConstraint:
     min: 0
     default: 0
   memoryBytesConstraint:
@@ -27,8 +22,13 @@
     min: 1
     default: 1
   maxIdleDurationConstraint:
     min: "0s"
     default: "2h"
   maxRunningDurationConstraint:
     min: "0s"
-    default: "2h"
+    default: "2h"
+  gpuTolerations:
+    - key: "dedicated"
+      operator: "Equal"
+      value: "gpu"
+      effect: "NoSchedule"
```

### Comparing `h2o_engine_manager-0.3.2/tests/integration/test_data/dai_setups/dai-mocked-server-logs.yaml` & `h2o_engine_manager-0.4.0/tests/integration/test_data/dai_setups/dai-mocked-server-logs.yaml`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/tests/integration/test_data/dai_setups/dai-setup.yaml` & `h2o_engine_manager-0.4.0/tests/integration/test_data/dai_setups/dai-setup.yaml`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/tests/integration/test_data/dai_setups/existing-dai-engine-constraint-set.yaml` & `h2o_engine_manager-0.4.0/tests/integration/test_data/dai_setups/existing-dai-engine-constraint-set.yaml`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/tests/integration/test_data/dai_setups/system.default.yaml` & `h2o_engine_manager-0.4.0/tests/integration/test_data/dai_setups/system.default.yaml`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/tests/integration/test_data/h2o_setups/existing-h2o-engine-constraint-set.yaml` & `h2o_engine_manager-0.4.0/tests/integration/test_data/h2o_setups/existing-h2o-engine-constraint-set.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 apiVersion: engine.h2o.ai/v1alpha1
 kind: H2OSetup
 metadata:
   # Name of this object corresponds to the workspaceID of H2OEngine resource.
   # (this additional setup is applied on all H2OEngines that are in 'existing-h2o-engine-constraint-set' workspace)
   name: existing-h2o-engine-constraint-set
 spec:
+  nodeCountConstraint:
+    min: 1
+    max: 10
+    default: 3
   cpuConstraint:
     min: 2
     max: 4
     default: 2
   gpuConstraint:
     min: 1
     default: 1
```

### Comparing `h2o_engine_manager-0.3.2/tests/integration/test_data/h2o_setups/h2o-setup.yaml` & `h2o_engine_manager-0.4.0/tests/integration/test_data/h2o_setups/h2o-setup.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 apiVersion: engine.h2o.ai/v1alpha1
 kind: H2OSetup
 metadata:
   # Name of this object corresponds to the workspaceID of H2OEngine resource.
   # (this additional setup is applied on all H2OEngines that are in 'h2o-setup' workspace)
   name: h2o-setup
 spec:
+  nodeCountConstraint:
+    min: 1
+    default: 1
   cpuConstraint:
     min: 1
     default: 1
   gpuConstraint:
     min: 0
     default: 0
   memoryBytesConstraint:
```

### Comparing `h2o_engine_manager-0.3.2/tests/integration/test_data/h2o_setups/system.default.yaml` & `h2o_engine_manager-0.4.0/tests/integration/test_data/h2o_setups/system.default.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,17 @@
   # "system.default" is a reserved placeholder for a "default" H2OSetup that is used as a fallback
   # H2OSetup for H2OEngines that are in workspace that do not have their "own" H2OSetup.
   # Note: there cannot exist a workspace with workspace_id="system.default" (dot '.' is not an allowed character),
   # hence, there cannot be a collision of a "default" H2OSetup with H2OSetup from "system.default"
   # workspace (such workspace cannot exist).
   name: system.default
 spec:
+  nodeCountConstraint:
+    min: 1
+    default: 1
   cpuConstraint:
     min: 1
     default: 1
   gpuConstraint:
     min: 0
     default: 0
   memoryBytesConstraint:
```

### Comparing `h2o_engine_manager-0.3.2/tests/unit/test_dai_engine.py` & `h2o_engine_manager-0.4.0/tests/unit/test_dai_engine.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/tests/unit/test_duration_convertor.py` & `h2o_engine_manager-0.4.0/tests/unit/test_duration_convertor.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,11 +14,11 @@
     [("1s", "1s"), ("1m", "60s"), ("12h", "43200s"), ("2d", "172800s")],
 )
 def test_duration_to_seconds(duration, expected):
     assert duration_to_seconds(duration) == expected
 
 
 @pytest.mark.parametrize(
-    "seconds,expected", [("1s", "1s"), ("60s", "1m"), ("61s", "61s"), ("43200s", "12h")]
+    "seconds,expected", [("1s", "1s"), ("2.99s", "2s"), ("60s", "1m"), ("61s", "61s"), ("43200s", "12h")]
 )
-def test_seconds_to_duratiob(seconds, expected):
+def test_seconds_to_duration(seconds, expected):
     assert seconds_to_duration(seconds) == expected
```

### Comparing `h2o_engine_manager-0.3.2/tests/unit/test_engine_state.py` & `h2o_engine_manager-0.4.0/tests/unit/test_engine_state.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/tests/unit/test_filter.py` & `h2o_engine_manager-0.4.0/tests/unit/test_filter.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/tests/unit/test_quantity_convertor.py` & `h2o_engine_manager-0.4.0/tests/unit/test_quantity_convertor.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/tests/unit/dai_version/test_mapper.py` & `h2o_engine_manager-0.4.0/tests/unit/dai_version/test_mapper.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/README.md` & `h2o_engine_manager-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/pyproject.toml` & `h2o_engine_manager-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.3.2/PKG-INFO` & `h2o_engine_manager-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h2o-engine-manager
-Version: 0.3.2
+Version: 0.4.0
 Summary: H2O Engine Manager python client
 Project-URL: Documentation, https://github.com/h2oai/ai-engine-manager#readme
 Project-URL: Issues, https://github.com/h2oai/ai-engine-manager/issues
 Project-URL: Source, https://github.com/h2oai/ai-engine-manager/py/h2o-engine-manager
 Author-email: Jan Sykora <jan.sykora@h2o.ai>, Tomas Pastorek <tomas.pastorek@h2o.ai>, Ondrej Bilek <ondrej.bilek@h2o.ai>
 Requires-Python: >=3.7
 Requires-Dist: certifi>=2022.12.7
```

