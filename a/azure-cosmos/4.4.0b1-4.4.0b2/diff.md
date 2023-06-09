# Comparing `tmp/azure-cosmos-4.4.0b1.zip` & `tmp/azure-cosmos-4.4.0b2.zip`

## zipinfo {}

```diff
@@ -1,176 +1,177 @@
-Zip file size: 448571 bytes, number of entries: 174
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-11 18:16 azure-cosmos-4.4.0b1/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-11 18:16 azure-cosmos-4.4.0b1/samples/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-11 18:16 azure-cosmos-4.4.0b1/azure/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-11 18:16 azure-cosmos-4.4.0b1/test/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-11 18:16 azure-cosmos-4.4.0b1/azure_cosmos.egg-info/
--rw-rw-r--  2.0 unx      149 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/MANIFEST.in
--rw-rw-r--  2.0 unx       99 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/pyproject.toml
--rw-rw-r--  2.0 unx     1073 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/LICENSE
--rw-rw-r--  2.0 unx     2429 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/setup.py
--rw-rw-r--  2.0 unx    53931 b- defN 23-Apr-11 18:16 azure-cosmos-4.4.0b1/PKG-INFO
--rw-rw-r--  2.0 unx    33721 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/README.md
--rw-rw-r--  2.0 unx      147 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/Contributing.md
--rw-rw-r--  2.0 unx       38 b- defN 23-Apr-11 18:16 azure-cosmos-4.4.0b1/setup.cfg
--rw-rw-r--  2.0 unx    19213 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/CHANGELOG.md
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-11 18:16 azure-cosmos-4.4.0b1/samples/MultiMasterOperations/
--rw-rw-r--  2.0 unx    11921 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/samples/document_management_async.py
--rw-rw-r--  2.0 unx     3794 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/samples/change_feed_management.py
--rw-rw-r--  2.0 unx    11297 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/samples/container_management.py
--rw-rw-r--  2.0 unx     4292 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/samples/database_management.py
--rw-rw-r--  2.0 unx     6438 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/samples/examples.py
--rw-rw-r--  2.0 unx     6419 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/samples/database_management_async.py
--rw-rw-r--  2.0 unx    30428 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/samples/index_management_async.py
--rw-rw-r--  2.0 unx     4484 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/samples/access_cosmos_with_aad.py
--rw-rw-r--  2.0 unx     8388 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/samples/examples_async.py
--rw-rw-r--  2.0 unx    10642 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/samples/access_cosmos_with_resource_token_async.py
--rw-rw-r--  2.0 unx    10519 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/samples/document_management.py
--rw-rw-r--  2.0 unx      820 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/samples/config.py
--rw-rw-r--  2.0 unx     9407 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/samples/access_cosmos_with_resource_token.py
--rw-rw-r--  2.0 unx     3367 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/samples/README.md
--rw-rw-r--  2.0 unx     2571 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/samples/client_user_configs_async.py
--rw-rw-r--  2.0 unx    30131 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/samples/index_management.py
--rw-rw-r--  2.0 unx     4258 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/samples/change_feed_management_async.py
--rw-rw-r--  2.0 unx    13997 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/samples/container_management_async.py
--rw-rw-r--  2.0 unx     5234 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/samples/access_cosmos_with_aad_async.py
--rw-rw-r--  2.0 unx     2538 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/samples/client_user_configs.py
--rw-rw-r--  2.0 unx      402 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/samples/MultiMasterOperations/Configurations.py
--rw-rw-r--  2.0 unx      318 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/samples/MultiMasterOperations/Program.py
--rw-rw-r--  2.0 unx     2843 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/samples/MultiMasterOperations/Worker.py
--rw-rw-r--  2.0 unx    35093 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/samples/MultiMasterOperations/ConflictWorker.py
--rw-rw-r--  2.0 unx     4083 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/samples/MultiMasterOperations/MultiMasterScenario.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-11 18:16 azure-cosmos-4.4.0b1/azure/cosmos/
--rw-rw-r--  2.0 unx       81 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-11 18:16 azure-cosmos-4.4.0b1/azure/cosmos/_execution_context/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-11 18:16 azure-cosmos-4.4.0b1/azure/cosmos/_routing/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-11 18:16 azure-cosmos-4.4.0b1/azure/cosmos/aio/
--rw-rw-r--  2.0 unx    97103 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/_cosmos_client_connection.py
--rw-rw-r--  2.0 unx     7198 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/_auth_policy.py
--rw-rw-r--  2.0 unx     2430 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/_retry_options.py
--rw-rw-r--  2.0 unx    29333 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/_base.py
--rw-rw-r--  2.0 unx    12763 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/user.py
--rw-rw-r--  2.0 unx     5771 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/_session_retry_policy.py
--rw-rw-r--  2.0 unx     2603 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/offer.py
--rw-rw-r--  2.0 unx     2992 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/_resource_throttle_retry_policy.py
--rw-rw-r--  2.0 unx     2861 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/partition_key.py
--rw-rw-r--  2.0 unx    14926 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/http_constants.py
--rw-rw-r--  2.0 unx     3274 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/_default_retry_policy.py
--rw-rw-r--  2.0 unx     1990 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/_utils.py
--rw-rw-r--  2.0 unx     7918 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/_synchronized_request.py
--rw-rw-r--  2.0 unx     1142 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/_version.py
--rw-rw-r--  2.0 unx    39514 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/database.py
--rw-rw-r--  2.0 unx     1753 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/_constants.py
--rw-rw-r--  2.0 unx     2200 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/__init__.py
--rw-rw-r--  2.0 unx    19609 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/scripts.py
--rw-rw-r--  2.0 unx     4798 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/_range_partition_resolver.py
--rw-rw-r--  2.0 unx    14934 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/_location_cache.py
--rw-rw-r--  2.0 unx    44338 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/container.py
--rw-rw-r--  2.0 unx     9656 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/_session.py
--rw-rw-r--  2.0 unx    24294 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/cosmos_client.py
--rw-rw-r--  2.0 unx     3427 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/exceptions.py
--rw-rw-r--  2.0 unx     4685 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/_endpoint_discovery_retry_policy.py
--rw-rw-r--  2.0 unx     2593 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/_partition.py
--rw-rw-r--  2.0 unx    15277 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/documents.py
--rw-rw-r--  2.0 unx     3478 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/_cosmos_http_logging_policy.py
--rw-rw-r--  2.0 unx     6575 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/_vector_session_token.py
--rw-rw-r--  2.0 unx     2302 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/_gone_retry_policy.py
--rw-rw-r--  2.0 unx     1696 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/_runtime_constants.py
--rw-rw-r--  2.0 unx     1509 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/errors.py
--rw-rw-r--  2.0 unx     2258 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/_request_object.py
--rw-rw-r--  2.0 unx     2806 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/_range.py
--rw-rw-r--  2.0 unx     3996 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/_query_iterable.py
--rw-rw-r--  2.0 unx     1848 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/permission.py
--rw-rw-r--  2.0 unx        0 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/py.typed
--rw-rw-r--  2.0 unx     2720 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/diagnostics.py
--rw-rw-r--  2.0 unx     6007 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/auth.py
--rw-rw-r--  2.0 unx    10529 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/_retry_utility.py
--rw-rw-r--  2.0 unx     7801 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/_global_endpoint_manager.py
--rw-rw-r--  2.0 unx     4548 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/_timeout_failover_retry_policy.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-11 18:16 azure-cosmos-4.4.0b1/azure/cosmos/_execution_context/aio/
--rw-rw-r--  2.0 unx     9096 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/_execution_context/execution_dispatcher.py
--rw-rw-r--  2.0 unx     6113 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/_execution_context/base_execution_context.py
--rw-rw-r--  2.0 unx     1121 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/_execution_context/__init__.py
--rw-rw-r--  2.0 unx     9259 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/_execution_context/document_producer.py
--rw-rw-r--  2.0 unx     8091 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/_execution_context/multi_execution_aggregator.py
--rw-rw-r--  2.0 unx     7627 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/_execution_context/endpoint_component.py
--rw-rw-r--  2.0 unx     3295 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/_execution_context/aggregators.py
--rw-rw-r--  2.0 unx     4697 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/_execution_context/query_execution_info.py
--rw-rw-r--  2.0 unx     8955 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/_execution_context/aio/execution_dispatcher.py
--rw-rw-r--  2.0 unx     6197 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/_execution_context/aio/base_execution_context.py
--rw-rw-r--  2.0 unx     1121 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/_execution_context/aio/__init__.py
--rw-rw-r--  2.0 unx     3220 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/_execution_context/aio/_queue_async_helper.py
--rw-rw-r--  2.0 unx     9210 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/_execution_context/aio/document_producer.py
--rw-rw-r--  2.0 unx     8507 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/_execution_context/aio/multi_execution_aggregator.py
--rw-rw-r--  2.0 unx     7472 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/_execution_context/aio/endpoint_component.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-11 18:16 azure-cosmos-4.4.0b1/azure/cosmos/_routing/aio/
--rw-rw-r--  2.0 unx     7528 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/_routing/collection_routing_map.py
--rw-rw-r--  2.0 unx     1121 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/_routing/__init__.py
--rw-rw-r--  2.0 unx     7964 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/_routing/routing_map_provider.py
--rw-rw-r--  2.0 unx     4520 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/_routing/routing_range.py
--rw-rw-r--  2.0 unx     1121 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/_routing/aio/__init__.py
--rw-rw-r--  2.0 unx     8085 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/_routing/aio/routing_map_provider.py
--rw-rw-r--  2.0 unx     7761 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/aio/_global_endpoint_manager_async.py
--rw-rw-r--  2.0 unx    22102 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/aio/_scripts.py
--rw-rw-r--  2.0 unx     9962 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/aio/_retry_utility_async.py
--rw-rw-r--  2.0 unx    20787 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/aio/_cosmos_client.py
--rw-rw-r--  2.0 unx     1417 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/aio/__init__.py
--rw-rw-r--  2.0 unx    43104 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/aio/_container.py
--rw-rw-r--  2.0 unx     8185 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/aio/_auth_policy_async.py
--rw-rw-r--  2.0 unx     7239 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/aio/_asynchronous_request.py
--rw-rw-r--  2.0 unx    95722 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/aio/_cosmos_client_connection_async.py
--rw-rw-r--  2.0 unx    39434 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/aio/_database.py
--rw-rw-r--  2.0 unx    14320 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/aio/_user.py
--rw-rw-r--  2.0 unx     4215 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/azure/cosmos/aio/_query_iterable_async.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-11 18:16 azure-cosmos-4.4.0b1/test/routing/
--rw-rw-r--  2.0 unx     3985 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/test/test_session_token_unit.py
--rw-rw-r--  2.0 unx     4494 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/test/test_partition_split_query.py
--rw-rw-r--  2.0 unx     7167 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/test/test_auto_scale.py
--rw-rw-r--  2.0 unx     2673 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/test/test_correlated_activity_id.py
--rw-rw-r--  2.0 unx     7087 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/test/test_aad.py
--rw-rw-r--  2.0 unx    22619 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/test/test_orderby.py
--rw-rw-r--  2.0 unx     6967 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/test/test_user_configs.py
--rw-rw-r--  2.0 unx    13679 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/test/test_analytical_ttl.py
--rw-rw-r--  2.0 unx     5354 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/test/test_session.py
--rw-rw-r--  2.0 unx     3879 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/test/test_headers.py
--rw-rw-r--  2.0 unx     8567 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/test/test_streaming_failover.py
--rw-rw-r--  2.0 unx     2382 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/test/test_media.py
--rw-rw-r--  2.0 unx    41041 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/test/test_query.py
--rw-rw-r--  2.0 unx     4317 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/test/test_partition_key.py
--rw-rw-r--  2.0 unx     4003 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/test/test_routing_map.py
--rw-rw-r--  2.0 unx    14793 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/test/test_ttl.py
--rw-rw-r--  2.0 unx    12416 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/test/test_multi_orderby.py
--rw-rw-r--  2.0 unx     2960 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/test/test_encoding.py
--rw-rw-r--  2.0 unx     7579 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/test/test_auto_scale_async.py
--rw-rw-r--  2.0 unx   126060 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/test/test_crud_async.py
--rw-rw-r--  2.0 unx     5014 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/test/test_multimaster.py
--rw-rw-r--  2.0 unx     1338 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/test/cleanup.py
--rw-rw-r--  2.0 unx     2335 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/test/test_client_user_agent.py
--rw-rw-r--  2.0 unx     9864 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/test/test_aggregate.py
--rw-rw-r--  2.0 unx     6491 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/test/test_cosmos_http_logging_policy.py
--rw-rw-r--  2.0 unx     3861 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/test/test_session_container.py
--rw-rw-r--  2.0 unx    15048 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/test/test_retry_policy.py
--rw-rw-r--  2.0 unx    13949 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/test/test_analytical_ttl_async.py
--rw-rw-r--  2.0 unx     4541 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/test/test_backwards_compatibility.py
--rw-rw-r--  2.0 unx     4384 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/test/test_env.py
--rw-rw-r--  2.0 unx     2120 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/test/test_utils.py
--rw-rw-r--  2.0 unx    24366 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/test/test_location_cache.py
--rw-rw-r--  2.0 unx     9224 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/test/test_query_execution_context.py
--rw-rw-r--  2.0 unx     8455 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/test/test_config.py
--rw-rw-r--  2.0 unx     1508 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/test/conftest.py
--rw-rw-r--  2.0 unx     9482 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/test/test_globaldb_mock.py
--rw-rw-r--  2.0 unx      465 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/test/test_base_unit.py
--rw-rw-r--  2.0 unx     1357 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/test/test_diagnostics.py
--rw-rw-r--  2.0 unx     4204 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/test/test_proxy.py
--rw-rw-r--  2.0 unx     4762 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/test/test_integrated_cache.py
--rw-rw-r--  2.0 unx   120857 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/test/test_crud.py
--rw-rw-r--  2.0 unx    26150 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/test/test_globaldb.py
--rw-rw-r--  2.0 unx    10381 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/test/routing/test_routing_map_provider.py
--rw-rw-r--  2.0 unx    10369 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/test/routing/test_collection_routing_map.py
--rw-rw-r--  2.0 unx     1103 b- defN 23-Apr-11 18:14 azure-cosmos-4.4.0b1/test/routing/__init__.py
--rw-rw-r--  2.0 unx        1 b- defN 23-Apr-11 18:16 azure-cosmos-4.4.0b1/azure_cosmos.egg-info/dependency_links.txt
--rw-rw-r--  2.0 unx       26 b- defN 23-Apr-11 18:16 azure-cosmos-4.4.0b1/azure_cosmos.egg-info/requires.txt
--rw-rw-r--  2.0 unx    53931 b- defN 23-Apr-11 18:16 azure-cosmos-4.4.0b1/azure_cosmos.egg-info/PKG-INFO
--rw-rw-r--  2.0 unx     5229 b- defN 23-Apr-11 18:16 azure-cosmos-4.4.0b1/azure_cosmos.egg-info/SOURCES.txt
--rw-rw-r--  2.0 unx        1 b- defN 23-Apr-11 18:16 azure-cosmos-4.4.0b1/azure_cosmos.egg-info/not-zip-safe
--rw-rw-r--  2.0 unx        6 b- defN 23-Apr-11 18:16 azure-cosmos-4.4.0b1/azure_cosmos.egg-info/top_level.txt
-174 files, 1833432 bytes uncompressed, 417381 bytes compressed:  77.2%
+Zip file size: 452043 bytes, number of entries: 175
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 15:33 azure-cosmos-4.4.0b2/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 15:33 azure-cosmos-4.4.0b2/samples/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 15:33 azure-cosmos-4.4.0b2/azure/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 15:33 azure-cosmos-4.4.0b2/azure_cosmos.egg-info/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 15:33 azure-cosmos-4.4.0b2/test/
+-rw-rw-r--  2.0 unx     1073 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/LICENSE
+-rw-rw-r--  2.0 unx      147 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/Contributing.md
+-rw-rw-r--  2.0 unx     2416 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/setup.py
+-rw-rw-r--  2.0 unx    19741 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/CHANGELOG.md
+-rw-rw-r--  2.0 unx    34526 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/README.md
+-rw-rw-r--  2.0 unx       38 b- defN 23-May-22 15:33 azure-cosmos-4.4.0b2/setup.cfg
+-rw-rw-r--  2.0 unx    55251 b- defN 23-May-22 15:33 azure-cosmos-4.4.0b2/PKG-INFO
+-rw-rw-r--  2.0 unx       99 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/pyproject.toml
+-rw-rw-r--  2.0 unx      149 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/MANIFEST.in
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 15:33 azure-cosmos-4.4.0b2/samples/MultiMasterOperations/
+-rw-rw-r--  2.0 unx     8376 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/samples/examples_async.py
+-rw-rw-r--  2.0 unx     6419 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/samples/database_management_async.py
+-rw-rw-r--  2.0 unx     5234 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/samples/access_cosmos_with_aad_async.py
+-rw-rw-r--  2.0 unx    13997 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/samples/container_management_async.py
+-rw-rw-r--  2.0 unx     2538 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/samples/client_user_configs.py
+-rw-rw-r--  2.0 unx     2640 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/samples/tracing_open_telemetry.py
+-rw-rw-r--  2.0 unx    30428 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/samples/index_management_async.py
+-rw-rw-r--  2.0 unx    11297 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/samples/container_management.py
+-rw-rw-r--  2.0 unx    30131 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/samples/index_management.py
+-rw-rw-r--  2.0 unx     6438 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/samples/examples.py
+-rw-rw-r--  2.0 unx     3581 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/samples/README.md
+-rw-rw-r--  2.0 unx     9407 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/samples/access_cosmos_with_resource_token.py
+-rw-rw-r--  2.0 unx    11590 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/samples/document_management.py
+-rw-rw-r--  2.0 unx     4258 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/samples/change_feed_management_async.py
+-rw-rw-r--  2.0 unx     4292 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/samples/database_management.py
+-rw-rw-r--  2.0 unx      820 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/samples/config.py
+-rw-rw-r--  2.0 unx    10642 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/samples/access_cosmos_with_resource_token_async.py
+-rw-rw-r--  2.0 unx     2571 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/samples/client_user_configs_async.py
+-rw-rw-r--  2.0 unx     4484 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/samples/access_cosmos_with_aad.py
+-rw-rw-r--  2.0 unx    13013 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/samples/document_management_async.py
+-rw-rw-r--  2.0 unx     3794 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/samples/change_feed_management.py
+-rw-rw-r--  2.0 unx     4083 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/samples/MultiMasterOperations/MultiMasterScenario.py
+-rw-rw-r--  2.0 unx     2843 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/samples/MultiMasterOperations/Worker.py
+-rw-rw-r--  2.0 unx      318 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/samples/MultiMasterOperations/Program.py
+-rw-rw-r--  2.0 unx      402 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/samples/MultiMasterOperations/Configurations.py
+-rw-rw-r--  2.0 unx    35093 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/samples/MultiMasterOperations/ConflictWorker.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 15:33 azure-cosmos-4.4.0b2/azure/cosmos/
+-rw-rw-r--  2.0 unx       81 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 15:33 azure-cosmos-4.4.0b2/azure/cosmos/aio/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 15:33 azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 15:33 azure-cosmos-4.4.0b2/azure/cosmos/_routing/
+-rw-rw-r--  2.0 unx     2603 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/offer.py
+-rw-rw-r--  2.0 unx    19609 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/scripts.py
+-rw-rw-r--  2.0 unx    10529 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_retry_utility.py
+-rw-rw-r--  2.0 unx     1848 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/permission.py
+-rw-rw-r--  2.0 unx     2720 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/diagnostics.py
+-rw-rw-r--  2.0 unx    29424 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_base.py
+-rw-rw-r--  2.0 unx     6575 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_vector_session_token.py
+-rw-rw-r--  2.0 unx     3695 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_timeout_failover_retry_policy.py
+-rw-rw-r--  2.0 unx    12763 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/user.py
+-rw-rw-r--  2.0 unx     2430 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_retry_options.py
+-rw-rw-r--  2.0 unx     2593 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_partition.py
+-rw-rw-r--  2.0 unx     3274 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_default_retry_policy.py
+-rw-rw-r--  2.0 unx    44598 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/container.py
+-rw-rw-r--  2.0 unx     2861 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/partition_key.py
+-rw-rw-r--  2.0 unx    15269 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/documents.py
+-rw-rw-r--  2.0 unx     2302 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_gone_retry_policy.py
+-rw-rw-r--  2.0 unx    39514 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/database.py
+-rw-rw-r--  2.0 unx     3427 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/exceptions.py
+-rw-rw-r--  2.0 unx     4798 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_range_partition_resolver.py
+-rw-rw-r--  2.0 unx    14934 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_location_cache.py
+-rw-rw-r--  2.0 unx    14926 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/http_constants.py
+-rw-rw-r--  2.0 unx     2992 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_resource_throttle_retry_policy.py
+-rw-rw-r--  2.0 unx     6007 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/auth.py
+-rw-rw-r--  2.0 unx     5771 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_session_retry_policy.py
+-rw-rw-r--  2.0 unx    24316 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/cosmos_client.py
+-rw-rw-r--  2.0 unx     2200 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/__init__.py
+-rw-rw-r--  2.0 unx     1142 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_version.py
+-rw-rw-r--  2.0 unx     1696 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_runtime_constants.py
+-rw-rw-r--  2.0 unx     1990 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_utils.py
+-rw-rw-r--  2.0 unx     7909 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_synchronized_request.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/py.typed
+-rw-rw-r--  2.0 unx     3478 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_cosmos_http_logging_policy.py
+-rw-rw-r--  2.0 unx     2258 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_request_object.py
+-rw-rw-r--  2.0 unx     1509 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/errors.py
+-rw-rw-r--  2.0 unx     7801 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_global_endpoint_manager.py
+-rw-rw-r--  2.0 unx     1753 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_constants.py
+-rw-rw-r--  2.0 unx     2806 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_range.py
+-rw-rw-r--  2.0 unx     9656 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_session.py
+-rw-rw-r--  2.0 unx     4685 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_endpoint_discovery_retry_policy.py
+-rw-rw-r--  2.0 unx    97299 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_cosmos_client_connection.py
+-rw-rw-r--  2.0 unx     7198 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_auth_policy.py
+-rw-rw-r--  2.0 unx     3996 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_query_iterable.py
+-rw-rw-r--  2.0 unx    95918 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/aio/_cosmos_client_connection_async.py
+-rw-rw-r--  2.0 unx     7230 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/aio/_asynchronous_request.py
+-rw-rw-r--  2.0 unx    20800 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/aio/_cosmos_client.py
+-rw-rw-r--  2.0 unx    14320 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/aio/_user.py
+-rw-rw-r--  2.0 unx    22102 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/aio/_scripts.py
+-rw-rw-r--  2.0 unx     8185 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/aio/_auth_policy_async.py
+-rw-rw-r--  2.0 unx     9962 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/aio/_retry_utility_async.py
+-rw-rw-r--  2.0 unx     7761 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/aio/_global_endpoint_manager_async.py
+-rw-rw-r--  2.0 unx     1417 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/aio/__init__.py
+-rw-rw-r--  2.0 unx    43363 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/aio/_container.py
+-rw-rw-r--  2.0 unx     4215 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/aio/_query_iterable_async.py
+-rw-rw-r--  2.0 unx    39434 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/aio/_database.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 15:33 azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/aio/
+-rw-rw-r--  2.0 unx     4697 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/query_execution_info.py
+-rw-rw-r--  2.0 unx     7627 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/endpoint_component.py
+-rw-rw-r--  2.0 unx     8091 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/multi_execution_aggregator.py
+-rw-rw-r--  2.0 unx     3295 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/aggregators.py
+-rw-rw-r--  2.0 unx     9096 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/execution_dispatcher.py
+-rw-rw-r--  2.0 unx     1121 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/__init__.py
+-rw-rw-r--  2.0 unx     6113 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/base_execution_context.py
+-rw-rw-r--  2.0 unx     9259 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/document_producer.py
+-rw-rw-r--  2.0 unx     7472 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/aio/endpoint_component.py
+-rw-rw-r--  2.0 unx     8507 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/aio/multi_execution_aggregator.py
+-rw-rw-r--  2.0 unx     8955 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/aio/execution_dispatcher.py
+-rw-rw-r--  2.0 unx     1121 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/aio/__init__.py
+-rw-rw-r--  2.0 unx     6197 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/aio/base_execution_context.py
+-rw-rw-r--  2.0 unx     3220 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/aio/_queue_async_helper.py
+-rw-rw-r--  2.0 unx     9210 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/aio/document_producer.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 15:33 azure-cosmos-4.4.0b2/azure/cosmos/_routing/aio/
+-rw-rw-r--  2.0 unx     7964 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_routing/routing_map_provider.py
+-rw-rw-r--  2.0 unx     4520 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_routing/routing_range.py
+-rw-rw-r--  2.0 unx     1121 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_routing/__init__.py
+-rw-rw-r--  2.0 unx     7528 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_routing/collection_routing_map.py
+-rw-rw-r--  2.0 unx     8085 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_routing/aio/routing_map_provider.py
+-rw-rw-r--  2.0 unx     1121 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_routing/aio/__init__.py
+-rw-rw-r--  2.0 unx        1 b- defN 23-May-22 15:33 azure-cosmos-4.4.0b2/azure_cosmos.egg-info/dependency_links.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-May-22 15:33 azure-cosmos-4.4.0b2/azure_cosmos.egg-info/not-zip-safe
+-rw-rw-r--  2.0 unx     5263 b- defN 23-May-22 15:33 azure-cosmos-4.4.0b2/azure_cosmos.egg-info/SOURCES.txt
+-rw-rw-r--  2.0 unx    55251 b- defN 23-May-22 15:33 azure-cosmos-4.4.0b2/azure_cosmos.egg-info/PKG-INFO
+-rw-rw-r--  2.0 unx       26 b- defN 23-May-22 15:33 azure-cosmos-4.4.0b2/azure_cosmos.egg-info/requires.txt
+-rw-rw-r--  2.0 unx        6 b- defN 23-May-22 15:33 azure-cosmos-4.4.0b2/azure_cosmos.egg-info/top_level.txt
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 15:33 azure-cosmos-4.4.0b2/test/routing/
+-rw-rw-r--  2.0 unx     3985 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_session_token_unit.py
+-rw-rw-r--  2.0 unx   123357 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_crud.py
+-rw-rw-r--  2.0 unx    24366 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_location_cache.py
+-rw-rw-r--  2.0 unx    12416 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_multi_orderby.py
+-rw-rw-r--  2.0 unx    14793 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_ttl.py
+-rw-rw-r--  2.0 unx     2382 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_media.py
+-rw-rw-r--  2.0 unx     4317 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_partition_key.py
+-rw-rw-r--  2.0 unx     7167 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_auto_scale.py
+-rw-rw-r--  2.0 unx   128585 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_crud_async.py
+-rw-rw-r--  2.0 unx     8455 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_config.py
+-rw-rw-r--  2.0 unx     4003 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_routing_map.py
+-rw-rw-r--  2.0 unx     1338 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/cleanup.py
+-rw-rw-r--  2.0 unx     6967 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_user_configs.py
+-rw-rw-r--  2.0 unx     9864 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_aggregate.py
+-rw-rw-r--  2.0 unx     9482 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_globaldb_mock.py
+-rw-rw-r--  2.0 unx     7579 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_auto_scale_async.py
+-rw-rw-r--  2.0 unx    13679 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_analytical_ttl.py
+-rw-rw-r--  2.0 unx     2960 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_encoding.py
+-rw-rw-r--  2.0 unx    15048 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_retry_policy.py
+-rw-rw-r--  2.0 unx     6491 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_cosmos_http_logging_policy.py
+-rw-rw-r--  2.0 unx     4541 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_backwards_compatibility.py
+-rw-rw-r--  2.0 unx    26150 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_globaldb.py
+-rw-rw-r--  2.0 unx     3879 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_headers.py
+-rw-rw-r--  2.0 unx     9224 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_query_execution_context.py
+-rw-rw-r--  2.0 unx     3861 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_session_container.py
+-rw-rw-r--  2.0 unx     5354 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_session.py
+-rw-rw-r--  2.0 unx     5014 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_multimaster.py
+-rw-rw-r--  2.0 unx     4384 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_env.py
+-rw-rw-r--  2.0 unx     1357 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_diagnostics.py
+-rw-rw-r--  2.0 unx     4204 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_proxy.py
+-rw-rw-r--  2.0 unx     4762 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_integrated_cache.py
+-rw-rw-r--  2.0 unx    22619 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_orderby.py
+-rw-rw-r--  2.0 unx     2673 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_correlated_activity_id.py
+-rw-rw-r--  2.0 unx      465 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_base_unit.py
+-rw-rw-r--  2.0 unx     2120 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_utils.py
+-rw-rw-r--  2.0 unx    13949 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_analytical_ttl_async.py
+-rw-rw-r--  2.0 unx     8567 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_streaming_failover.py
+-rw-rw-r--  2.0 unx     1508 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/conftest.py
+-rw-rw-r--  2.0 unx    41041 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_query.py
+-rw-rw-r--  2.0 unx     2335 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_client_user_agent.py
+-rw-rw-r--  2.0 unx     4757 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_partition_split_query.py
+-rw-rw-r--  2.0 unx     7087 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_aad.py
+-rw-rw-r--  2.0 unx    10369 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/routing/test_collection_routing_map.py
+-rw-rw-r--  2.0 unx     1103 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/routing/__init__.py
+-rw-rw-r--  2.0 unx    10381 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/routing/test_routing_map_provider.py
+175 files, 1847877 bytes uncompressed, 420669 bytes compressed:  77.2%
```

## zipnote {}

```diff
@@ -1,523 +1,526 @@
-Filename: azure-cosmos-4.4.0b1/
+Filename: azure-cosmos-4.4.0b2/
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/samples/
+Filename: azure-cosmos-4.4.0b2/samples/
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/
+Filename: azure-cosmos-4.4.0b2/azure/
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/test/
+Filename: azure-cosmos-4.4.0b2/azure_cosmos.egg-info/
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure_cosmos.egg-info/
+Filename: azure-cosmos-4.4.0b2/test/
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/MANIFEST.in
+Filename: azure-cosmos-4.4.0b2/LICENSE
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/pyproject.toml
+Filename: azure-cosmos-4.4.0b2/Contributing.md
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/LICENSE
+Filename: azure-cosmos-4.4.0b2/setup.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/setup.py
+Filename: azure-cosmos-4.4.0b2/CHANGELOG.md
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/PKG-INFO
+Filename: azure-cosmos-4.4.0b2/README.md
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/README.md
+Filename: azure-cosmos-4.4.0b2/setup.cfg
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/Contributing.md
+Filename: azure-cosmos-4.4.0b2/PKG-INFO
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/setup.cfg
+Filename: azure-cosmos-4.4.0b2/pyproject.toml
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/CHANGELOG.md
+Filename: azure-cosmos-4.4.0b2/MANIFEST.in
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/samples/MultiMasterOperations/
+Filename: azure-cosmos-4.4.0b2/samples/MultiMasterOperations/
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/samples/document_management_async.py
+Filename: azure-cosmos-4.4.0b2/samples/examples_async.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/samples/change_feed_management.py
+Filename: azure-cosmos-4.4.0b2/samples/database_management_async.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/samples/container_management.py
+Filename: azure-cosmos-4.4.0b2/samples/access_cosmos_with_aad_async.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/samples/database_management.py
+Filename: azure-cosmos-4.4.0b2/samples/container_management_async.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/samples/examples.py
+Filename: azure-cosmos-4.4.0b2/samples/client_user_configs.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/samples/database_management_async.py
+Filename: azure-cosmos-4.4.0b2/samples/tracing_open_telemetry.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/samples/index_management_async.py
+Filename: azure-cosmos-4.4.0b2/samples/index_management_async.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/samples/access_cosmos_with_aad.py
+Filename: azure-cosmos-4.4.0b2/samples/container_management.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/samples/examples_async.py
+Filename: azure-cosmos-4.4.0b2/samples/index_management.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/samples/access_cosmos_with_resource_token_async.py
+Filename: azure-cosmos-4.4.0b2/samples/examples.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/samples/document_management.py
+Filename: azure-cosmos-4.4.0b2/samples/README.md
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/samples/config.py
+Filename: azure-cosmos-4.4.0b2/samples/access_cosmos_with_resource_token.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/samples/access_cosmos_with_resource_token.py
+Filename: azure-cosmos-4.4.0b2/samples/document_management.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/samples/README.md
+Filename: azure-cosmos-4.4.0b2/samples/change_feed_management_async.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/samples/client_user_configs_async.py
+Filename: azure-cosmos-4.4.0b2/samples/database_management.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/samples/index_management.py
+Filename: azure-cosmos-4.4.0b2/samples/config.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/samples/change_feed_management_async.py
+Filename: azure-cosmos-4.4.0b2/samples/access_cosmos_with_resource_token_async.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/samples/container_management_async.py
+Filename: azure-cosmos-4.4.0b2/samples/client_user_configs_async.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/samples/access_cosmos_with_aad_async.py
+Filename: azure-cosmos-4.4.0b2/samples/access_cosmos_with_aad.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/samples/client_user_configs.py
+Filename: azure-cosmos-4.4.0b2/samples/document_management_async.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/samples/MultiMasterOperations/Configurations.py
+Filename: azure-cosmos-4.4.0b2/samples/change_feed_management.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/samples/MultiMasterOperations/Program.py
+Filename: azure-cosmos-4.4.0b2/samples/MultiMasterOperations/MultiMasterScenario.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/samples/MultiMasterOperations/Worker.py
+Filename: azure-cosmos-4.4.0b2/samples/MultiMasterOperations/Worker.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/samples/MultiMasterOperations/ConflictWorker.py
+Filename: azure-cosmos-4.4.0b2/samples/MultiMasterOperations/Program.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/samples/MultiMasterOperations/MultiMasterScenario.py
+Filename: azure-cosmos-4.4.0b2/samples/MultiMasterOperations/Configurations.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/
+Filename: azure-cosmos-4.4.0b2/samples/MultiMasterOperations/ConflictWorker.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/__init__.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/_execution_context/
+Filename: azure-cosmos-4.4.0b2/azure/__init__.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/_routing/
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/aio/
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/aio/
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/_cosmos_client_connection.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/_routing/
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/_auth_policy.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/offer.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/_retry_options.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/scripts.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/_base.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/_retry_utility.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/user.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/permission.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/_session_retry_policy.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/diagnostics.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/offer.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/_base.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/_resource_throttle_retry_policy.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/_vector_session_token.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/partition_key.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/_timeout_failover_retry_policy.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/http_constants.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/user.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/_default_retry_policy.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/_retry_options.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/_utils.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/_partition.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/_synchronized_request.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/_default_retry_policy.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/_version.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/container.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/database.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/partition_key.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/_constants.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/documents.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/__init__.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/_gone_retry_policy.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/scripts.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/database.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/_range_partition_resolver.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/exceptions.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/_location_cache.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/_range_partition_resolver.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/container.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/_location_cache.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/_session.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/http_constants.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/cosmos_client.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/_resource_throttle_retry_policy.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/exceptions.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/auth.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/_endpoint_discovery_retry_policy.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/_session_retry_policy.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/_partition.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/cosmos_client.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/documents.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/__init__.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/_cosmos_http_logging_policy.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/_version.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/_vector_session_token.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/_runtime_constants.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/_gone_retry_policy.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/_utils.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/_runtime_constants.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/_synchronized_request.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/errors.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/py.typed
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/_request_object.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/_cosmos_http_logging_policy.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/_range.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/_request_object.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/_query_iterable.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/errors.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/permission.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/_global_endpoint_manager.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/py.typed
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/_constants.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/diagnostics.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/_range.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/auth.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/_session.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/_retry_utility.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/_endpoint_discovery_retry_policy.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/_global_endpoint_manager.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/_cosmos_client_connection.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/_timeout_failover_retry_policy.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/_auth_policy.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/_execution_context/aio/
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/_query_iterable.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/_execution_context/execution_dispatcher.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/aio/_cosmos_client_connection_async.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/_execution_context/base_execution_context.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/aio/_asynchronous_request.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/_execution_context/__init__.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/aio/_cosmos_client.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/_execution_context/document_producer.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/aio/_user.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/_execution_context/multi_execution_aggregator.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/aio/_scripts.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/_execution_context/endpoint_component.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/aio/_auth_policy_async.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/_execution_context/aggregators.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/aio/_retry_utility_async.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/_execution_context/query_execution_info.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/aio/_global_endpoint_manager_async.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/_execution_context/aio/execution_dispatcher.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/aio/__init__.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/_execution_context/aio/base_execution_context.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/aio/_container.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/_execution_context/aio/__init__.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/aio/_query_iterable_async.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/_execution_context/aio/_queue_async_helper.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/aio/_database.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/_execution_context/aio/document_producer.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/aio/
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/_execution_context/aio/multi_execution_aggregator.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/query_execution_info.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/_execution_context/aio/endpoint_component.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/endpoint_component.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/_routing/aio/
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/multi_execution_aggregator.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/_routing/collection_routing_map.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/aggregators.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/_routing/__init__.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/execution_dispatcher.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/_routing/routing_map_provider.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/__init__.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/_routing/routing_range.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/base_execution_context.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/_routing/aio/__init__.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/document_producer.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/_routing/aio/routing_map_provider.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/aio/endpoint_component.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/aio/_global_endpoint_manager_async.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/aio/multi_execution_aggregator.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/aio/_scripts.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/aio/execution_dispatcher.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/aio/_retry_utility_async.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/aio/__init__.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/aio/_cosmos_client.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/aio/base_execution_context.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/aio/__init__.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/aio/_queue_async_helper.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/aio/_container.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/aio/document_producer.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/aio/_auth_policy_async.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/_routing/aio/
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/aio/_asynchronous_request.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/_routing/routing_map_provider.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/aio/_cosmos_client_connection_async.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/_routing/routing_range.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/aio/_database.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/_routing/__init__.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/aio/_user.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/_routing/collection_routing_map.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure/cosmos/aio/_query_iterable_async.py
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/_routing/aio/routing_map_provider.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/test/routing/
+Filename: azure-cosmos-4.4.0b2/azure/cosmos/_routing/aio/__init__.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/test/test_session_token_unit.py
+Filename: azure-cosmos-4.4.0b2/azure_cosmos.egg-info/dependency_links.txt
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/test/test_partition_split_query.py
+Filename: azure-cosmos-4.4.0b2/azure_cosmos.egg-info/not-zip-safe
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/test/test_auto_scale.py
+Filename: azure-cosmos-4.4.0b2/azure_cosmos.egg-info/SOURCES.txt
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/test/test_correlated_activity_id.py
+Filename: azure-cosmos-4.4.0b2/azure_cosmos.egg-info/PKG-INFO
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/test/test_aad.py
+Filename: azure-cosmos-4.4.0b2/azure_cosmos.egg-info/requires.txt
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/test/test_orderby.py
+Filename: azure-cosmos-4.4.0b2/azure_cosmos.egg-info/top_level.txt
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/test/test_user_configs.py
+Filename: azure-cosmos-4.4.0b2/test/routing/
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/test/test_analytical_ttl.py
+Filename: azure-cosmos-4.4.0b2/test/test_session_token_unit.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/test/test_session.py
+Filename: azure-cosmos-4.4.0b2/test/test_crud.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/test/test_headers.py
+Filename: azure-cosmos-4.4.0b2/test/test_location_cache.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/test/test_streaming_failover.py
+Filename: azure-cosmos-4.4.0b2/test/test_multi_orderby.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/test/test_media.py
+Filename: azure-cosmos-4.4.0b2/test/test_ttl.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/test/test_query.py
+Filename: azure-cosmos-4.4.0b2/test/test_media.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/test/test_partition_key.py
+Filename: azure-cosmos-4.4.0b2/test/test_partition_key.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/test/test_routing_map.py
+Filename: azure-cosmos-4.4.0b2/test/test_auto_scale.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/test/test_ttl.py
+Filename: azure-cosmos-4.4.0b2/test/test_crud_async.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/test/test_multi_orderby.py
+Filename: azure-cosmos-4.4.0b2/test/test_config.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/test/test_encoding.py
+Filename: azure-cosmos-4.4.0b2/test/test_routing_map.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/test/test_auto_scale_async.py
+Filename: azure-cosmos-4.4.0b2/test/cleanup.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/test/test_crud_async.py
+Filename: azure-cosmos-4.4.0b2/test/test_user_configs.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/test/test_multimaster.py
+Filename: azure-cosmos-4.4.0b2/test/test_aggregate.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/test/cleanup.py
+Filename: azure-cosmos-4.4.0b2/test/test_globaldb_mock.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/test/test_client_user_agent.py
+Filename: azure-cosmos-4.4.0b2/test/test_auto_scale_async.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/test/test_aggregate.py
+Filename: azure-cosmos-4.4.0b2/test/test_analytical_ttl.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/test/test_cosmos_http_logging_policy.py
+Filename: azure-cosmos-4.4.0b2/test/test_encoding.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/test/test_session_container.py
+Filename: azure-cosmos-4.4.0b2/test/test_retry_policy.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/test/test_retry_policy.py
+Filename: azure-cosmos-4.4.0b2/test/test_cosmos_http_logging_policy.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/test/test_analytical_ttl_async.py
+Filename: azure-cosmos-4.4.0b2/test/test_backwards_compatibility.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/test/test_backwards_compatibility.py
+Filename: azure-cosmos-4.4.0b2/test/test_globaldb.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/test/test_env.py
+Filename: azure-cosmos-4.4.0b2/test/test_headers.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/test/test_utils.py
+Filename: azure-cosmos-4.4.0b2/test/test_query_execution_context.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/test/test_location_cache.py
+Filename: azure-cosmos-4.4.0b2/test/test_session_container.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/test/test_query_execution_context.py
+Filename: azure-cosmos-4.4.0b2/test/test_session.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/test/test_config.py
+Filename: azure-cosmos-4.4.0b2/test/test_multimaster.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/test/conftest.py
+Filename: azure-cosmos-4.4.0b2/test/test_env.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/test/test_globaldb_mock.py
+Filename: azure-cosmos-4.4.0b2/test/test_diagnostics.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/test/test_base_unit.py
+Filename: azure-cosmos-4.4.0b2/test/test_proxy.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/test/test_diagnostics.py
+Filename: azure-cosmos-4.4.0b2/test/test_integrated_cache.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/test/test_proxy.py
+Filename: azure-cosmos-4.4.0b2/test/test_orderby.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/test/test_integrated_cache.py
+Filename: azure-cosmos-4.4.0b2/test/test_correlated_activity_id.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/test/test_crud.py
+Filename: azure-cosmos-4.4.0b2/test/test_base_unit.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/test/test_globaldb.py
+Filename: azure-cosmos-4.4.0b2/test/test_utils.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/test/routing/test_routing_map_provider.py
+Filename: azure-cosmos-4.4.0b2/test/test_analytical_ttl_async.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/test/routing/test_collection_routing_map.py
+Filename: azure-cosmos-4.4.0b2/test/test_streaming_failover.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/test/routing/__init__.py
+Filename: azure-cosmos-4.4.0b2/test/conftest.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure_cosmos.egg-info/dependency_links.txt
+Filename: azure-cosmos-4.4.0b2/test/test_query.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure_cosmos.egg-info/requires.txt
+Filename: azure-cosmos-4.4.0b2/test/test_client_user_agent.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure_cosmos.egg-info/PKG-INFO
+Filename: azure-cosmos-4.4.0b2/test/test_partition_split_query.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure_cosmos.egg-info/SOURCES.txt
+Filename: azure-cosmos-4.4.0b2/test/test_aad.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure_cosmos.egg-info/not-zip-safe
+Filename: azure-cosmos-4.4.0b2/test/routing/test_collection_routing_map.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b1/azure_cosmos.egg-info/top_level.txt
+Filename: azure-cosmos-4.4.0b2/test/routing/__init__.py
+Comment: 
+
+Filename: azure-cosmos-4.4.0b2/test/routing/test_routing_map_provider.py
 Comment: 
 
 Zip file comment:
```

## Comparing `azure-cosmos-4.4.0b1/LICENSE` & `azure-cosmos-4.4.0b2/LICENSE`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/setup.py` & `azure-cosmos-4.4.0b2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     license="MIT License",
     author="Microsoft Corporation",
     author_email="askdocdb@microsoft.com",
     maintainer="Microsoft",
     maintainer_email="askdocdb@microsoft.com",
     url="https://github.com/Azure/azure-sdk-for-python",
     classifiers=[
-        "Development Status :: 5 - Production/Stable",
+        "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
```

## Comparing `azure-cosmos-4.4.0b1/PKG-INFO` & `azure-cosmos-4.4.0b2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: azure-cosmos
-Version: 4.4.0b1
+Version: 4.4.0b2
 Summary: Microsoft Azure Cosmos Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: askdocdb@microsoft.com
 Maintainer: Microsoft
 Maintainer-email: askdocdb@microsoft.com
 License: MIT License
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -686,14 +686,25 @@
 However, if you desire to use the CosmosHttpLoggingPolicy to obtain additional information, the `enable_diagnostics_logging` argument needs to be passed in at the client constructor.
 ```python
 # This example enables the CosmosHttpLoggingPolicy and uses it with the `logger` passed in to the `create_database` request.
 client = CosmosClient(URL, credential=KEY, enable_diagnostics_logging=True)
 database = client.create_database(DATABASE_NAME, logger=logger)
 ```
 
+### Telemetry
+Azure Core provides the ability for our Python SDKs to use OpenTelemetry with them. The only packages that need to be installed
+to use this functionality are the following:
+```bash
+pip install azure-core-tracing-opentelemetry
+pip install opentelemetry-sdk
+```
+For more information on this, we recommend taking a look at this [document](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/core/azure-core-tracing-opentelemetry/README.md) 
+from Azure Core describing how to set it up. We have also added a [sample file][telemetry_sample] to show how it can
+be used with our SDK. This works the same way regardless of the Cosmos client you are using.
+
 ## Next steps
 
 For more extensive documentation on the Cosmos DB service, see the [Azure Cosmos DB documentation][cosmos_docs] on docs.microsoft.com.
 
 <!-- LINKS -->
 [azure_cli]: https://docs.microsoft.com/cli/azure
 [azure_portal]: https://portal.azure.com
@@ -726,14 +737,15 @@
 [ref_httpfailure]: https://aka.ms/azsdk-python-cosmos-ref-http-failure
 [sample_database_mgmt]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/cosmos/azure-cosmos/samples/database_management.py
 [sample_document_mgmt]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/cosmos/azure-cosmos/samples/document_management.py
 [sample_examples_misc]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/cosmos/azure-cosmos/samples/examples.py
 [source_code]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/cosmos/azure-cosmos
 [venv]: https://docs.python.org/3/library/venv.html
 [virtualenv]: https://virtualenv.pypa.io
+[telemetry_sample]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/cosmos/azure-cosmos/samples/tracing_open_telemetry.py
 
 ## Contributing
 
 This project welcomes contributions and suggestions.  Most contributions require you to agree to a
 Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
 the rights to use your contribution. For details, visit https://cla.microsoft.com.
 
@@ -744,21 +756,31 @@
 This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
 For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
 contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
 
 
 ## Release History
 
+### 4.4.0b2 (2023-05-22)
+
+#### Features Added
+* Added conditional patching for Patch operations. See [PR 30455](https://github.com/Azure/azure-sdk-for-python/pull/30455).
+
+#### Bugs Fixed
+* Fixed bug with non english locales causing an error with the RFC 1123 Date Format. See [PR 30125](https://github.com/Azure/azure-sdk-for-python/pull/30125).
+
+#### Other Changes
+* Refactoring of our client `connection_timeout` and `request_timeout` configurations. See [PR 30171](https://github.com/Azure/azure-sdk-for-python/pull/30171).
+
 ### 4.4.0b1 (2023-04-11)
 
 #### Features Added
  - Added **preview** delete all items by partition key functionality. See [PR 29186](https://github.com/Azure/azure-sdk-for-python/pull/29186).
  - Added **preview** partial document update (Patch API) functionality and container methods for patching items with operations. See [PR 29497](https://github.com/Azure/azure-sdk-for-python/pull/29497). For more information on Patch, please see [Azure Cosmos DB Partial Document Update](https://learn.microsoft.com/azure/cosmos-db/partial-document-update).
 
-
 #### Bugs Fixed
 * Fixed bug in method `create_container_if_not_exists()` of async database client for unexpected kwargs being passed into `read()` method used internally. See [PR 29136](https://github.com/Azure/azure-sdk-for-python/pull/29136).
 * Fixed bug with method `query_items()` of our async container class, where partition key and cross partition headers would both be set when using partition keys. See [PR 29366](https://github.com/Azure/azure-sdk-for-python/pull/29366/).
 * Fixed bug with client not properly surfacing errors for invalid credentials and identities with insufficient permissions. Users running into 'NoneType has no attribute ConsistencyPolicy' errors when initializing their clients will now see proper authentication exceptions. See [PR 29256](https://github.com/Azure/azure-sdk-for-python/pull/29256).
 
 #### Other Changes
 * Removed use of `six` package within the SDK.
```

## Comparing `azure-cosmos-4.4.0b1/README.md` & `azure-cosmos-4.4.0b2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -660,14 +660,25 @@
 However, if you desire to use the CosmosHttpLoggingPolicy to obtain additional information, the `enable_diagnostics_logging` argument needs to be passed in at the client constructor.
 ```python
 # This example enables the CosmosHttpLoggingPolicy and uses it with the `logger` passed in to the `create_database` request.
 client = CosmosClient(URL, credential=KEY, enable_diagnostics_logging=True)
 database = client.create_database(DATABASE_NAME, logger=logger)
 ```
 
+### Telemetry
+Azure Core provides the ability for our Python SDKs to use OpenTelemetry with them. The only packages that need to be installed
+to use this functionality are the following:
+```bash
+pip install azure-core-tracing-opentelemetry
+pip install opentelemetry-sdk
+```
+For more information on this, we recommend taking a look at this [document](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/core/azure-core-tracing-opentelemetry/README.md) 
+from Azure Core describing how to set it up. We have also added a [sample file][telemetry_sample] to show how it can
+be used with our SDK. This works the same way regardless of the Cosmos client you are using.
+
 ## Next steps
 
 For more extensive documentation on the Cosmos DB service, see the [Azure Cosmos DB documentation][cosmos_docs] on docs.microsoft.com.
 
 <!-- LINKS -->
 [azure_cli]: https://docs.microsoft.com/cli/azure
 [azure_portal]: https://portal.azure.com
@@ -700,14 +711,15 @@
 [ref_httpfailure]: https://aka.ms/azsdk-python-cosmos-ref-http-failure
 [sample_database_mgmt]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/cosmos/azure-cosmos/samples/database_management.py
 [sample_document_mgmt]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/cosmos/azure-cosmos/samples/document_management.py
 [sample_examples_misc]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/cosmos/azure-cosmos/samples/examples.py
 [source_code]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/cosmos/azure-cosmos
 [venv]: https://docs.python.org/3/library/venv.html
 [virtualenv]: https://virtualenv.pypa.io
+[telemetry_sample]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/cosmos/azure-cosmos/samples/tracing_open_telemetry.py
 
 ## Contributing
 
 This project welcomes contributions and suggestions.  Most contributions require you to agree to a
 Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
 the rights to use your contribution. For details, visit https://cla.microsoft.com.
```

## Comparing `azure-cosmos-4.4.0b1/CHANGELOG.md` & `azure-cosmos-4.4.0b2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,26 @@
 ## Release History
 
+### 4.4.0b2 (2023-05-22)
+
+#### Features Added
+* Added conditional patching for Patch operations. See [PR 30455](https://github.com/Azure/azure-sdk-for-python/pull/30455).
+
+#### Bugs Fixed
+* Fixed bug with non english locales causing an error with the RFC 1123 Date Format. See [PR 30125](https://github.com/Azure/azure-sdk-for-python/pull/30125).
+
+#### Other Changes
+* Refactoring of our client `connection_timeout` and `request_timeout` configurations. See [PR 30171](https://github.com/Azure/azure-sdk-for-python/pull/30171).
+
 ### 4.4.0b1 (2023-04-11)
 
 #### Features Added
  - Added **preview** delete all items by partition key functionality. See [PR 29186](https://github.com/Azure/azure-sdk-for-python/pull/29186).
  - Added **preview** partial document update (Patch API) functionality and container methods for patching items with operations. See [PR 29497](https://github.com/Azure/azure-sdk-for-python/pull/29497). For more information on Patch, please see [Azure Cosmos DB Partial Document Update](https://learn.microsoft.com/azure/cosmos-db/partial-document-update).
 
-
 #### Bugs Fixed
 * Fixed bug in method `create_container_if_not_exists()` of async database client for unexpected kwargs being passed into `read()` method used internally. See [PR 29136](https://github.com/Azure/azure-sdk-for-python/pull/29136).
 * Fixed bug with method `query_items()` of our async container class, where partition key and cross partition headers would both be set when using partition keys. See [PR 29366](https://github.com/Azure/azure-sdk-for-python/pull/29366/).
 * Fixed bug with client not properly surfacing errors for invalid credentials and identities with insufficient permissions. Users running into 'NoneType has no attribute ConsistencyPolicy' errors when initializing their clients will now see proper authentication exceptions. See [PR 29256](https://github.com/Azure/azure-sdk-for-python/pull/29256).
 
 #### Other Changes
 * Removed use of `six` package within the SDK.
```

## Comparing `azure-cosmos-4.4.0b1/samples/document_management_async.py` & `azure-cosmos-4.4.0b2/samples/document_management_async.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See LICENSE.txt in the project root for
 # license information.
 # -------------------------------------------------------------------------
 from azure.cosmos.aio import CosmosClient
 import azure.cosmos.exceptions as exceptions
+from azure.cosmos.http_constants import StatusCodes
 from azure.cosmos.partition_key import PartitionKey
 import datetime
 
 import asyncio
 import config
 
 # ----------------------------------------------------------------------------------------------------------
@@ -116,43 +117,62 @@
 
     read_item = await container.read_item(item=doc_id, partition_key=doc_id)
     read_item['subtotal'] = read_item['subtotal'] + 1
     response = await container.upsert_item(body=read_item)
 
     print('Upserted Item\'s Id is {0}, new subtotal={1}'.format(response['id'], response['subtotal']))
 
+async def conditional_patch_item(container, doc_id):
+    print('\n1.7 Patching Item by Id based on filter\n')
+    operations = [
+        {"op": "add", "path": "/favorite_color", "value": "red"},
+        {"op": "remove", "path": "/ttl"},
+        {"op": "replace", "path": "/tax_amount", "value": 14},
+        {"op": "set", "path": "/items/0/discount", "value": 20.0512},
+        {"op": "incr", "path": "/total_due", "value": 5},
+        {"op": "move", "from": "/freight", "path": "/service_addition"}
+    ]
+    filter_predicate = "from c where c.tax_amount = 10"
+
+    print("Filter predicate match failure will result in BadRequestException.")
+    try:
+        await container.patch_item(item=doc_id, partition_key=doc_id,
+                                    patch_operations=operations, filter_predicate=filter_predicate)
+    except exceptions.CosmosHttpResponseError as e:
+        assert(e.status_code == StatusCodes.PRECONDITION_FAILED)
+        print("Failed as expected.")
 async def patch_item(container, doc_id):
-    print('\n1.7 Patching Item by Id\n')
+    print('\n1.8 Patching Item by Id\n')
 
     operations = [
         {"op": "add", "path": "/favorite_color", "value": "red"},
         {"op": "remove", "path": "/ttl"},
         {"op": "replace", "path": "/tax_amount", "value": 14},
         {"op": "set", "path": "/items/0/discount", "value": 20.0512},
         {"op": "incr", "path": "/total_due", "value": 5},
         {"op": "move", "from": "/freight", "path": "/service_addition"}
     ]
 
     response = await container.patch_item(item=doc_id, partition_key=doc_id, patch_operations=operations)
     print('Patched Item\'s Id is {0}, new path favorite color={1}, removed path ttl={2}, replaced path tax_amount={3},'
           ' set path for item at index 0 of discount={4}, increase in path total_due, new total_due={5}, '
           'move from path freight={6} to path service_addition={7}'.format(response["id"], response["favorite_color"],
-                                response.get("ttl"), response["tax_amount"], response["items"].get(0).get("discount"),
+                                response.get("ttl"), response["tax_amount"], response["items"][0].get("discount"),
                                 response["total_due"], response.get("freight"), response["service_addition"]))
 
 async def delete_item(container, doc_id):
-    print('\n1.8 Deleting Item by Id\n')
+    print('\n1.9 Deleting Item by Id\n')
 
     await container.delete_item(item=doc_id, partition_key=doc_id)
 
     print('Deleted item\'s Id is {0}'.format(doc_id))
 
 
 async def delete_all_items_by_partition_key(db, partitionkey):
-    print('\n1.8 Deleting all Items by Partition Key\n')
+    print('\n1.10 Deleting all Items by Partition Key\n')
 
     # A container with a partition key that is different from id is needed
     container = await db.create_container_if_not_exists(id="Partition Key Delete Container",
                                                   partition_key=PartitionKey(path='/company'))
     sales_order_company_A1 = get_sales_order("SalesOrderCompanyA1")
     sales_order_company_A1["company"] = partitionkey
     await container.upsert_item(sales_order_company_A1)
@@ -250,14 +270,15 @@
 
             await create_items(container)
             await read_item(container, 'SalesOrder1')
             await read_items(container)
             await query_items(container, 'SalesOrder1')
             await replace_item(container, 'SalesOrder1')
             await upsert_item(container, 'SalesOrder1')
+            await conditional_patch_item(container, 'SalesOrder1')
             await patch_item(container, 'SalesOrder1')
             await delete_item(container, 'SalesOrder1')
             await delete_all_items_by_partition_key(db, "CompanyA")
 
             # cleanup database after sample
             try:
                 await client.delete_database(db)
```

## Comparing `azure-cosmos-4.4.0b1/samples/change_feed_management.py` & `azure-cosmos-4.4.0b2/samples/change_feed_management.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/samples/container_management.py` & `azure-cosmos-4.4.0b2/samples/container_management.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/samples/database_management.py` & `azure-cosmos-4.4.0b2/samples/database_management.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/samples/examples.py` & `azure-cosmos-4.4.0b2/samples/examples.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/samples/database_management_async.py` & `azure-cosmos-4.4.0b2/samples/database_management_async.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/samples/index_management_async.py` & `azure-cosmos-4.4.0b2/samples/index_management_async.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/samples/access_cosmos_with_aad.py` & `azure-cosmos-4.4.0b2/samples/access_cosmos_with_aad.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/samples/examples_async.py` & `azure-cosmos-4.4.0b2/samples/examples_async.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,20 +163,20 @@
         # [START delete_all_items_by_partition_key]
         container_name = "products"
         container = database.get_container_client(container_name)
         for i in range(1, 10):
             await container.upsert_item(
                 dict(id="item{}".format(i), productName="Gadget", productModel="Model {}".format(i))
             )
-        items = await container.read_all_items()
+        items = container.read_all_items()
         async for item in items:
             print(json.dumps(item, indent=True))
         await container.delete_all_items_by_partition_key("Gadget")
         print("All items in partition {} deleted.".format("Gadget"))
-        items = await container.read_all_items()
+        items = container.read_all_items()
         async for item in items:
             print(json.dumps(item, indent=True))
         # [END delete_all_items_by_partition_key]
 
         await client.delete_database(database_name)
         print("Sample done running!")
```

## Comparing `azure-cosmos-4.4.0b1/samples/access_cosmos_with_resource_token_async.py` & `azure-cosmos-4.4.0b2/samples/access_cosmos_with_resource_token_async.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/samples/document_management.py` & `azure-cosmos-4.4.0b2/samples/document_management.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See LICENSE.txt in the project root for
 # license information.
 # -------------------------------------------------------------------------
 import azure.cosmos.cosmos_client as cosmos_client
 import azure.cosmos.exceptions as exceptions
+from azure.cosmos.http_constants import StatusCodes
 from azure.cosmos.partition_key import PartitionKey
 import datetime
 
 import config
 
 # ----------------------------------------------------------------------------------------------------------
 # Prerequisites -
@@ -98,43 +99,63 @@
 
     read_item = container.read_item(item=doc_id, partition_key=doc_id)
     read_item['subtotal'] = read_item['subtotal'] + 1
     response = container.upsert_item(body=read_item)
 
     print('Upserted Item\'s Id is {0}, new subtotal={1}'.format(response['id'], response['subtotal']))
 
+def conditional_patch_item(container, doc_id):
+    print('\n1.7 Patching Item by Id based on filter\n')
+    operations = [
+        {"op": "add", "path": "/favorite_color", "value": "red"},
+        {"op": "remove", "path": "/ttl"},
+        {"op": "replace", "path": "/tax_amount", "value": 14},
+        {"op": "set", "path": "/items/0/discount", "value": 20.0512},
+        {"op": "incr", "path": "/total_due", "value": 5},
+        {"op": "move", "from": "/freight", "path": "/service_addition"}
+    ]
+    filter_predicate = "from c where c.tax_amount = 10"
+
+    print("Filter predicate match failure will result in BadRequestException.")
+    try:
+        container.patch_item(item=doc_id, partition_key=doc_id,
+                                    patch_operations=operations, filter_predicate=filter_predicate)
+    except exceptions.CosmosHttpResponseError as e:
+        assert(e.status_code == StatusCodes.PRECONDITION_FAILED)
+        print("Failed as expected.")
+
 def patch_item(container, doc_id):
-    print('\n1.7 Patching Item by Id\n')
+    print('\n1.8 Patching Item by Id\n')
 
     operations = [
         {"op": "add", "path": "/favorite_color", "value": "red"},
         {"op": "remove", "path": "/ttl"},
         {"op": "replace", "path": "/tax_amount", "value": 14},
         {"op": "set", "path": "/items/0/discount", "value": 20.0512},
         {"op": "incr", "path": "/total_due", "value": 5},
         {"op": "move", "from": "/freight", "path": "/service_addition"}
     ]
 
     response = container.patch_item(item=doc_id, partition_key=doc_id, patch_operations=operations)
     print('Patched Item\'s Id is {0}, new path favorite color={1}, removed path ttl={2}, replaced path tax_amount={3},'
           ' set path for item at index 0 of discount={4}, increase in path total_due, new total_due={5}, move from path freight={6}'
           ' to path service_addition={7}'.format(response["id"], response["favorite_color"], response.get("ttl"),
-                                                 response["tax_amount"], response["items"].get(0).get("discount"),
+                                                 response["tax_amount"], response["items"][0].get("discount"),
                                                  response["total_due"], response.get("freight"), response["service_addition"]))
 
 def delete_item(container, doc_id):
-    print('\n1.8 Deleting Item by Id\n')
+    print('\n1.9 Deleting Item by Id\n')
 
     response = container.delete_item(item=doc_id, partition_key=doc_id)
 
     print('Deleted item\'s Id is {0}'.format(doc_id))
 
 
 def delete_all_items_by_partition_key(db, partitionkey):
-    print('\n1.8 Deleting all Items by Partition Key\n')
+    print('\n1.10 Deleting all Items by Partition Key\n')
 
     # A container with a partition key that is different from id is needed
     container = db.create_container_if_not_exists(id="Partition Key Delete Container",
                                                   partition_key=PartitionKey(path='/company'))
     sales_order_company_A1 = get_sales_order("SalesOrderCompanyA1")
     sales_order_company_A1["company"] = partitionkey
     container.upsert_item(sales_order_company_A1)
@@ -230,14 +251,15 @@
 
         create_items(container)
         read_item(container, 'SalesOrder1')
         read_items(container)
         query_items(container, 'SalesOrder1')
         replace_item(container, 'SalesOrder1')
         upsert_item(container, 'SalesOrder1')
+        conditional_patch_item(container, 'SalesOrder1')
         patch_item(container, 'SalesOrder1')
         delete_item(container, 'SalesOrder1')
         delete_all_items_by_partition_key(db, "CompanyA")
 
         # cleanup database after sample
         try:
             client.delete_database(db)
```

## Comparing `azure-cosmos-4.4.0b1/samples/config.py` & `azure-cosmos-4.4.0b2/samples/config.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/samples/access_cosmos_with_resource_token.py` & `azure-cosmos-4.4.0b2/samples/access_cosmos_with_resource_token.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/samples/README.md` & `azure-cosmos-4.4.0b2/samples/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -41,14 +41,16 @@
 
 
 * [access_cosmos_with_resource_token.py](https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/cosmos/azure-cosmos/samples/access_cosmos_with_resource_token.py) - Example demontrating how to get and use resource token that allows restricted access to data.
 
 
 * [multi-master operations](https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/cosmos/azure-cosmos/samples/MultiMasterOperations) - Example demonstrating multi-master operations.
 
+* [tracing-open-telemetry](https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/cosmos/azure-cosmos/samples/tracing_open_telemetry.py) - Example demonstrating how to use OpenTelemetry tracing with our SDK.
+
 ## Prerequisites
 * Python 3.6+
 * You must have an [Azure subscription](https://azure.microsoft.com/free/) and an
 [Azure Cosmos DB account](https://docs.microsoft.com/azure/cosmos-db/create-sql-api-python#create-a-database-account) to run these samples.
 
 ## Setup
```

## Comparing `azure-cosmos-4.4.0b1/samples/client_user_configs_async.py` & `azure-cosmos-4.4.0b2/samples/client_user_configs_async.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/samples/index_management.py` & `azure-cosmos-4.4.0b2/samples/index_management.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/samples/change_feed_management_async.py` & `azure-cosmos-4.4.0b2/samples/change_feed_management_async.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/samples/container_management_async.py` & `azure-cosmos-4.4.0b2/samples/container_management_async.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/samples/access_cosmos_with_aad_async.py` & `azure-cosmos-4.4.0b2/samples/access_cosmos_with_aad_async.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/samples/client_user_configs.py` & `azure-cosmos-4.4.0b2/samples/client_user_configs.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/samples/MultiMasterOperations/Worker.py` & `azure-cosmos-4.4.0b2/samples/MultiMasterOperations/Worker.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/samples/MultiMasterOperations/ConflictWorker.py` & `azure-cosmos-4.4.0b2/samples/MultiMasterOperations/ConflictWorker.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/samples/MultiMasterOperations/MultiMasterScenario.py` & `azure-cosmos-4.4.0b2/samples/MultiMasterOperations/MultiMasterScenario.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/_cosmos_client_connection.py` & `azure-cosmos-4.4.0b2/azure/cosmos/_cosmos_client_connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1751,15 +1751,19 @@
         if options is None:
             options = {}
 
         initial_headers = self.default_headers
         headers = base.GetHeaders(self, initial_headers, "patch", path, document_id, typ, options)
         # Patch will use WriteEndpoint since it uses PUT operation
         request_params = _request_object.RequestObject(typ, documents._OperationType.Patch)
-        result, self.last_response_headers = self.__Patch(path, request_params, operations, headers, **kwargs)
+        request_data = {}
+        if options.get("filterPredicate"):
+            request_data["condition"] = options.get("filterPredicate")
+        request_data["operations"] = operations
+        result, self.last_response_headers = self.__Patch(path, request_params, request_data, headers, **kwargs)
 
         # update session for request mutates data on server side
         self._UpdateSessionIfRequired(headers, result, self.last_response_headers)
         return result
 
     def DeleteItem(self, document_link, options=None, **kwargs):
         """Deletes a document.
@@ -2368,20 +2372,20 @@
             connection_policy=self.connection_policy,
             pipeline_client=self.pipeline_client,
             request=request,
             request_data=body,
             **kwargs
         )
 
-    def __Patch(self, path, request_params, operations, req_headers, **kwargs):
+    def __Patch(self, path, request_params, request_data, req_headers, **kwargs):
         """Azure Cosmos 'PATCH' http request.
 
         :params str path:
         :params ~azure.cosmos.RequestObject request_params:
-        :params list operations:
+        :params dict request_data:
         :params dict req_headers:
 
         :return:
             Tuple of (result, headers).
         :rtype:
             tuple of (dict, dict)
 
@@ -2390,15 +2394,15 @@
         return synchronized_request.SynchronizedRequest(
             client=self,
             request_params=request_params,
             global_endpoint_manager=self._global_endpoint_manager,
             connection_policy=self.connection_policy,
             pipeline_client=self.pipeline_client,
             request=request,
-            request_data=operations,
+            request_data=request_data,
             **kwargs
         )
 
     def __Delete(self, path, request_params, req_headers, **kwargs):
         """Azure Cosmos 'DELETE' http request.
 
         :params str url:
```

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/_auth_policy.py` & `azure-cosmos-4.4.0b2/azure/cosmos/_auth_policy.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/_retry_options.py` & `azure-cosmos-4.4.0b2/azure/cosmos/_retry_options.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/_base.py` & `azure-cosmos-4.4.0b2/azure/cosmos/_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Base functions in the Azure Cosmos database service.
 """
 
 import base64
-import datetime
+from email.utils import formatdate
 import json
 import uuid
 import binascii
 from typing import Dict, Any, Union
 
 from urllib.parse import quote as urllib_quote
 from urllib.parse import urlsplit
@@ -220,15 +220,16 @@
     if options.get("enableCrossPartitionQuery"):
         headers[http_constants.HttpHeaders.EnableCrossPartitionQuery] = options["enableCrossPartitionQuery"]
 
     if options.get("populateQueryMetrics"):
         headers[http_constants.HttpHeaders.PopulateQueryMetrics] = options["populateQueryMetrics"]
 
     if cosmos_client_connection.master_key:
-        headers[http_constants.HttpHeaders.XDate] = datetime.datetime.utcnow().strftime("%a, %d %b %Y %H:%M:%S GMT")
+        #formatedate guarantees RFC 1123 date format regardless of current locale
+        headers[http_constants.HttpHeaders.XDate] = formatdate(timeval=None, localtime=False, usegmt=True)
 
     if cosmos_client_connection.master_key or cosmos_client_connection.resource_tokens:
         resource_type = _internal_resourcetype(resource_type)
         authorization = auth._get_authorization_header(
             cosmos_client_connection, verb, path, resource_id, IsNameBased(resource_id), resource_type, headers
         )
         # urllib.quote throws when the input parameter is None
```

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/user.py` & `azure-cosmos-4.4.0b2/azure/cosmos/user.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/_session_retry_policy.py` & `azure-cosmos-4.4.0b2/azure/cosmos/_session_retry_policy.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/offer.py` & `azure-cosmos-4.4.0b2/azure/cosmos/offer.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/_resource_throttle_retry_policy.py` & `azure-cosmos-4.4.0b2/azure/cosmos/_resource_throttle_retry_policy.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/partition_key.py` & `azure-cosmos-4.4.0b2/azure/cosmos/partition_key.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/http_constants.py` & `azure-cosmos-4.4.0b2/azure/cosmos/http_constants.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/_default_retry_policy.py` & `azure-cosmos-4.4.0b2/azure/cosmos/_default_retry_policy.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/_utils.py` & `azure-cosmos-4.4.0b2/azure/cosmos/_utils.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/_synchronized_request.py` & `azure-cosmos-4.4.0b2/azure/cosmos/_synchronized_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     :return: tuple of (result, headers)
     :rtype: tuple of (dict, dict)
 
     """
     # pylint: disable=protected-access
 
     connection_timeout = connection_policy.RequestTimeout
-    connection_timeout = kwargs.pop("connection_timeout", connection_timeout / 1000.0)
+    connection_timeout = kwargs.pop("connection_timeout", connection_timeout)
 
     # Every request tries to perform a refresh
     client_timeout = kwargs.get('timeout')
     start_time = time.time()
     global_endpoint_manager.refresh_endpoint_list(None, **kwargs)
     if client_timeout is not None:
         kwargs['timeout'] = client_timeout - (time.time() - start_time)
```

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/_version.py` & `azure-cosmos-4.4.0b2/azure/cosmos/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,8 +15,8 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-VERSION = "4.4.0b1"
+VERSION = "4.4.0b2"
```

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/database.py` & `azure-cosmos-4.4.0b2/azure/cosmos/database.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/_constants.py` & `azure-cosmos-4.4.0b2/azure/cosmos/_constants.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/__init__.py` & `azure-cosmos-4.4.0b2/azure/cosmos/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/scripts.py` & `azure-cosmos-4.4.0b2/azure/cosmos/scripts.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/_range_partition_resolver.py` & `azure-cosmos-4.4.0b2/azure/cosmos/_range_partition_resolver.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/_location_cache.py` & `azure-cosmos-4.4.0b2/azure/cosmos/_location_cache.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/container.py` & `azure-cosmos-4.4.0b2/azure/cosmos/container.py`

 * *Files 0% similar despite different names*

```diff
@@ -572,27 +572,28 @@
 
     @distributed_trace
     def patch_item(
         self,
         item: Union[str, Dict[str, Any]],
         partition_key: Union[str, int, float, bool],
         patch_operations: List[Dict[str, Any]],
-        **kwargs:Any
+        **kwargs: Any
     ) -> Dict[str, Any]:
         """ **Provisional method** Patches the specified item with the provided operations if it
          exists in the container.
 
         If the item does not already exist in the container, an exception is raised.
 
         :param item: The ID (name) or dict representing item to be patched.
         :type item: Union[str, Dict[str, Any]]
         :param partition_key: The partition key of the object to patch.
         :type partition_key: Union[str, int, float, bool]
         :param patch_operations: The list of patch operations to apply to the item.
         :type patch_operations: List[Dict[str, Any]]
+        :keyword str filter_predicate: conditional filter to apply to Patch operations.
         :keyword str pre_trigger_include: trigger id to be used as pre operation trigger.
         :keyword str post_trigger_include: trigger id to be used as post operation trigger.
         :keyword str session_token: Token for use with Session consistency.
         :keyword dict[str,str] initial_headers: Initial headers to be sent as part of the request.
         :keyword str etag: An ETag value, or the wildcard character (*). Used to check if the resource
             has changed, and act according to the condition specified by the `match_condition` parameter.
         :keyword ~azure.core.MatchConditions match_condition: The match condition to use upon the etag.
@@ -602,14 +603,17 @@
             given id does not exist.
         :rtype: dict[str, Any]
         """
         request_options = build_options(kwargs)
         response_hook = kwargs.pop('response_hook', None)
         request_options["disableAutomaticIdGeneration"] = True
         request_options["partitionKey"] = partition_key
+        filter_predicate = kwargs.pop("filter_predicate", None)
+        if filter_predicate is not None:
+            request_options["filterPredicate"] = filter_predicate
 
         item_link = self._get_document_link(item)
         result = self.client_connection.PatchItem(
             document_link=item_link, operations=patch_operations, options=request_options, **kwargs)
         if response_hook:
             response_hook(self.client_connection.last_response_headers, result)
         return result
```

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/_session.py` & `azure-cosmos-4.4.0b2/azure/cosmos/_session.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/cosmos_client.py` & `azure-cosmos-4.4.0b2/azure/cosmos/cosmos_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,34 +70,34 @@
             " TokenCredential (see azure.identity module for specific implementations such as ClientSecretCredential).")
     return auth
 
 
 def _build_connection_policy(kwargs):
     # type: (Dict[str, Any]) -> ConnectionPolicy
     # pylint: disable=protected-access
-    policy = kwargs.pop('connection_policy', None) or ConnectionPolicy()
+    policy = kwargs.pop('connection_policy', ConnectionPolicy())
 
     # Connection config
-    policy.RequestTimeout = kwargs.pop('request_timeout', None) or \
-        kwargs.pop('connection_timeout', None) or \
-        policy.RequestTimeout
-    policy.ConnectionMode = kwargs.pop('connection_mode', None) or policy.ConnectionMode
-    policy.ProxyConfiguration = kwargs.pop('proxy_config', None) or policy.ProxyConfiguration
-    policy.EnableEndpointDiscovery = kwargs.pop('enable_endpoint_discovery') \
-        if 'enable_endpoint_discovery' in kwargs.keys() else policy.EnableEndpointDiscovery
-    policy.PreferredLocations = kwargs.pop('preferred_locations', None) or policy.PreferredLocations
-    policy.UseMultipleWriteLocations = kwargs.pop('multiple_write_locations', None) or \
-        policy.UseMultipleWriteLocations
+    # `request_timeout` is supported as a legacy parameter later replaced by `connection_timeout`
+    if 'request_timeout' in kwargs:
+        policy.RequestTimeout = kwargs.pop('request_timeout') / 1000.0
+    else:
+        policy.RequestTimeout = kwargs.pop('connection_timeout', policy.RequestTimeout)
+    policy.ConnectionMode = kwargs.pop('connection_mode', policy.ConnectionMode)
+    policy.ProxyConfiguration = kwargs.pop('proxy_config', policy.ProxyConfiguration)
+    policy.EnableEndpointDiscovery = kwargs.pop('enable_endpoint_discovery', policy.EnableEndpointDiscovery)
+    policy.PreferredLocations = kwargs.pop('preferred_locations', policy.PreferredLocations)
+    policy.UseMultipleWriteLocations = kwargs.pop('multiple_write_locations', policy.UseMultipleWriteLocations)
 
     # SSL config
     verify = kwargs.pop('connection_verify', None)
     policy.DisableSSLVerification = not bool(verify if verify is not None else True)
-    ssl = kwargs.pop('ssl_config', None) or policy.SSLConfiguration
+    ssl = kwargs.pop('ssl_config', policy.SSLConfiguration)
     if ssl:
-        ssl.SSLCertFile = kwargs.pop('connection_cert', None) or ssl.SSLCertFile
+        ssl.SSLCertFile = kwargs.pop('connection_cert', ssl.SSLCertFile)
         ssl.SSLCaCerts = verify or ssl.SSLCaCerts
         policy.SSLConfiguration = ssl
 
     # Retry config
     retry_options = kwargs.pop('retry_options', None)
     if retry_options is not None:
         warnings.warn("This option has been deprecated and will be removed from the SDK in a future release.",
@@ -137,15 +137,15 @@
 
     :param str url: The URL of the Cosmos DB account.
     :param credential: Can be the account key, or a dictionary of resource tokens.
     :type credential: Union[str, Dict[str, str], ~azure.core.credentials.TokenCredential]
     :param str consistency_level: Consistency level to use for the session. The default value is None (Account level).
         More on consistency levels and possible values: https://aka.ms/cosmos-consistency-levels
     :keyword int timeout: An absolute timeout in seconds, for the combined HTTP request and response processing.
-    :keyword int request_timeout: The HTTP request timeout in milliseconds.
+    :keyword int connection_timeout: The HTTP request timeout in seconds.
     :keyword str connection_mode: The connection mode for the client - currently only supports 'Gateway'.
     :keyword proxy_config: Connection proxy configuration.
     :paramtype proxy_config: ~azure.cosmos.ProxyConfiguration
     :keyword ssl_config: Connection SSL configuration.
     :paramtype ssl_config: ~azure.cosmos.SSLConfiguration
     :keyword bool connection_verify: Whether to verify the connection, default value is True.
     :keyword str connection_cert: An alternative certificate to verify the connection.
```

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/exceptions.py` & `azure-cosmos-4.4.0b2/azure/cosmos/exceptions.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/_endpoint_discovery_retry_policy.py` & `azure-cosmos-4.4.0b2/azure/cosmos/_endpoint_discovery_retry_policy.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/_partition.py` & `azure-cosmos-4.4.0b2/azure/cosmos/_partition.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/documents.py` & `azure-cosmos-4.4.0b2/azure/cosmos/documents.py`

 * *Files 0% similar despite different names*

```diff
@@ -354,15 +354,15 @@
         database accounts in the Azure Cosmos database service.
     :ivar ConnectionRetryConfiguration:
         Retry Configuration to be used for connection retries.
     :vartype ConnectionRetryConfiguration:
         int or azure.cosmos.ConnectionRetryPolicy or urllib3.util.retry
     """
 
-    __defaultRequestTimeout = 60000  # milliseconds
+    __defaultRequestTimeout = 60  # seconds
 
     def __init__(self):
         self.RequestTimeout = self.__defaultRequestTimeout
         self.ConnectionMode = ConnectionMode.Gateway
         self.SSLConfiguration = None
         self.ProxyConfiguration = None
         self.EnableEndpointDiscovery = True
```

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/_cosmos_http_logging_policy.py` & `azure-cosmos-4.4.0b2/azure/cosmos/_cosmos_http_logging_policy.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/_vector_session_token.py` & `azure-cosmos-4.4.0b2/azure/cosmos/_vector_session_token.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/_gone_retry_policy.py` & `azure-cosmos-4.4.0b2/azure/cosmos/_gone_retry_policy.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/_runtime_constants.py` & `azure-cosmos-4.4.0b2/azure/cosmos/_runtime_constants.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/errors.py` & `azure-cosmos-4.4.0b2/azure/cosmos/errors.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/_request_object.py` & `azure-cosmos-4.4.0b2/azure/cosmos/_request_object.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/_range.py` & `azure-cosmos-4.4.0b2/azure/cosmos/_range.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/_query_iterable.py` & `azure-cosmos-4.4.0b2/azure/cosmos/_query_iterable.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/permission.py` & `azure-cosmos-4.4.0b2/azure/cosmos/permission.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/diagnostics.py` & `azure-cosmos-4.4.0b2/azure/cosmos/diagnostics.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/auth.py` & `azure-cosmos-4.4.0b2/azure/cosmos/auth.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/_retry_utility.py` & `azure-cosmos-4.4.0b2/azure/cosmos/_retry_utility.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/_global_endpoint_manager.py` & `azure-cosmos-4.4.0b2/azure/cosmos/_global_endpoint_manager.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/_timeout_failover_retry_policy.py` & `azure-cosmos-4.4.0b2/azure/cosmos/_timeout_failover_retry_policy.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,42 +19,36 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Internal class for timeout failover retry policy implementation in the Azure
 Cosmos database service.
 """
 from . import http_constants
-from ..cosmos.documents import _OperationType
 
 
 class _TimeoutFailoverRetryPolicy(object):
 
     def __init__(self, connection_policy, global_endpoint_manager, *args):
         self._max_retry_attempt_count = 120
         self._max_service_unavailable_retry_count = 1
         self.retry_after_in_milliseconds = 0
         self.args = args
 
         self.global_endpoint_manager = global_endpoint_manager
         self.failover_retry_count = 0
         self.connection_policy = connection_policy
         self.request = args[0] if args else None
-
         if self.request:
-            self.request.clear_route_to_location()
-
-            # Resolve the endpoint for the request and pin the resolution to the resolved endpoint
-            # This enables marking the endpoint unavailability on endpoint failover/unreachability
             self.location_endpoint = self.global_endpoint_manager.resolve_service_endpoint(self.request)
-            self.request.route_to_location(self.location_endpoint)
 
     def needsRetry(self):
         if self.args:
             if (self.args[3].method == "GET") \
-                    or (http_constants.HttpHeaders.IsQueryPlanRequest in self.args[3].headers):
+                    or http_constants.HttpHeaders.IsQueryPlanRequest in self.args[3].headers\
+                    or http_constants.HttpHeaders.IsQuery in self.args[3].headers:
                 return True
         return False
 
     def ShouldRetry(self, _exception):
         """Returns true if should retry based on the passed-in exception.
 
         :param (exceptions.CosmosHttpResponseError instance) _exception:
@@ -71,31 +65,20 @@
                 self.failover_retry_count >= self._max_service_unavailable_retry_count:
             return False
         if self.failover_retry_count >= self._max_retry_attempt_count:
             return False
 
         self.failover_retry_count += 1
 
-        if self.location_endpoint:
-            if _OperationType.IsReadOnlyOperation(self.request.operation_type):
-                # Mark current read endpoint as unavailable
-                self.global_endpoint_manager.mark_endpoint_unavailable_for_read(self.location_endpoint)
-            else:
-                self.global_endpoint_manager.mark_endpoint_unavailable_for_write(self.location_endpoint)
-
-        # set the refresh_needed flag to ensure that endpoint list is
-        # refreshed with new writable and readable locations
-        self.global_endpoint_manager.refresh_needed = True
-
-        # clear previous location-based routing directive
-        self.request.clear_route_to_location()
-
-        # set location-based routing directive based on retry count
-        # simulating single master writes by ensuring usePreferredLocations
-        # is set to false
-        self.request.route_to_location_with_preferred_location_flag(self.failover_retry_count, False)
-
-        # Resolve the endpoint for the request and pin the resolution to the resolved endpoint
-        # This enables marking the endpoint unavailability on endpoint failover/unreachability
-        self.location_endpoint = self.global_endpoint_manager.resolve_service_endpoint(self.request)
-        self.request.route_to_location(self.location_endpoint)
+        if self.request:
+            # clear previous location-based routing directive
+            self.request.clear_route_to_location()
+
+            # set location-based routing directive based on retry count
+            # ensuring usePreferredLocations is set to True for retry
+            self.request.route_to_location_with_preferred_location_flag(self.failover_retry_count, True)
+
+            # Resolve the endpoint for the request and pin the resolution to the resolved endpoint
+            # This enables marking the endpoint unavailability on endpoint failover/unreachability
+            self.location_endpoint = self.global_endpoint_manager.resolve_service_endpoint(self.request)
+            self.request.route_to_location(self.location_endpoint)
         return True
```

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/_execution_context/execution_dispatcher.py` & `azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/execution_dispatcher.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/_execution_context/base_execution_context.py` & `azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/base_execution_context.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/_execution_context/__init__.py` & `azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/_execution_context/document_producer.py` & `azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/document_producer.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/_execution_context/multi_execution_aggregator.py` & `azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/multi_execution_aggregator.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/_execution_context/endpoint_component.py` & `azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/endpoint_component.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/_execution_context/aggregators.py` & `azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/aggregators.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/_execution_context/query_execution_info.py` & `azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/query_execution_info.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/_execution_context/aio/execution_dispatcher.py` & `azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/aio/execution_dispatcher.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/_execution_context/aio/base_execution_context.py` & `azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/aio/base_execution_context.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/_execution_context/aio/__init__.py` & `azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/_execution_context/aio/_queue_async_helper.py` & `azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/aio/_queue_async_helper.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/_execution_context/aio/document_producer.py` & `azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/aio/document_producer.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/_execution_context/aio/multi_execution_aggregator.py` & `azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/aio/multi_execution_aggregator.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/_execution_context/aio/endpoint_component.py` & `azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/aio/endpoint_component.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/_routing/collection_routing_map.py` & `azure-cosmos-4.4.0b2/azure/cosmos/_routing/collection_routing_map.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/_routing/__init__.py` & `azure-cosmos-4.4.0b2/azure/cosmos/_routing/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/_routing/routing_map_provider.py` & `azure-cosmos-4.4.0b2/azure/cosmos/_routing/routing_map_provider.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/_routing/routing_range.py` & `azure-cosmos-4.4.0b2/azure/cosmos/_routing/routing_range.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/_routing/aio/__init__.py` & `azure-cosmos-4.4.0b2/azure/cosmos/_routing/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/_routing/aio/routing_map_provider.py` & `azure-cosmos-4.4.0b2/azure/cosmos/_routing/aio/routing_map_provider.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/aio/_global_endpoint_manager_async.py` & `azure-cosmos-4.4.0b2/azure/cosmos/aio/_global_endpoint_manager_async.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/aio/_scripts.py` & `azure-cosmos-4.4.0b2/azure/cosmos/aio/_scripts.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/aio/_retry_utility_async.py` & `azure-cosmos-4.4.0b2/azure/cosmos/aio/_retry_utility_async.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/aio/_cosmos_client.py` & `azure-cosmos-4.4.0b2/azure/cosmos/aio/_cosmos_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,39 +41,40 @@
 
 
 def _build_connection_policy(kwargs: Dict[str, Any]) -> ConnectionPolicy:
     # pylint: disable=protected-access
     policy = kwargs.pop('connection_policy', None) or ConnectionPolicy()
 
     # Connection config
-    policy.RequestTimeout = kwargs.pop('request_timeout', None) or \
-                            kwargs.pop('connection_timeout', None) or \
-                            policy.RequestTimeout
-    policy.ConnectionMode = kwargs.pop('connection_mode', None) or policy.ConnectionMode
-    policy.ProxyConfiguration = kwargs.pop('proxy_config', None) or policy.ProxyConfiguration
-    policy.EnableEndpointDiscovery = kwargs.pop('enable_endpoint_discovery', None) or policy.EnableEndpointDiscovery
-    policy.PreferredLocations = kwargs.pop('preferred_locations', None) or policy.PreferredLocations
-    policy.UseMultipleWriteLocations = kwargs.pop('multiple_write_locations', None) or \
-                                       policy.UseMultipleWriteLocations
+    # `request_timeout` is supported as a legacy parameter later replaced by `connection_timeout`
+    if 'request_timeout' in kwargs:
+        policy.RequestTimeout = kwargs.pop('request_timeout') / 1000.0
+    else:
+        policy.RequestTimeout = kwargs.pop('connection_timeout', policy.RequestTimeout)
+    policy.ConnectionMode = kwargs.pop('connection_mode', policy.ConnectionMode)
+    policy.ProxyConfiguration = kwargs.pop('proxy_config', policy.ProxyConfiguration)
+    policy.EnableEndpointDiscovery = kwargs.pop('enable_endpoint_discovery', policy.EnableEndpointDiscovery)
+    policy.PreferredLocations = kwargs.pop('preferred_locations', policy.PreferredLocations)
+    policy.UseMultipleWriteLocations = kwargs.pop('multiple_write_locations', policy.UseMultipleWriteLocations)
 
     # SSL config
     verify = kwargs.pop('connection_verify', None)
     policy.DisableSSLVerification = not bool(verify if verify is not None else True)
     ssl = kwargs.pop('ssl_config', None) or policy.SSLConfiguration
     if ssl:
-        ssl.SSLCertFile = kwargs.pop('connection_cert', None) or ssl.SSLCertFile
+        ssl.SSLCertFile = kwargs.pop('connection_cert', ssl.SSLCertFile)
         ssl.SSLCaCerts = verify or ssl.SSLCaCerts
         policy.SSLConfiguration = ssl
 
     # Retry config
     retry_options = policy.RetryOptions
     total_retries = kwargs.pop('retry_total', None)
     retry_options._max_retry_attempt_count = total_retries or retry_options._max_retry_attempt_count
-    retry_options._fixed_retry_interval_in_milliseconds = kwargs.pop('retry_fixed_interval', None) or \
-        retry_options._fixed_retry_interval_in_milliseconds
+    retry_options._fixed_retry_interval_in_milliseconds = \
+        kwargs.pop('retry_fixed_interval', retry_options._fixed_retry_interval_in_milliseconds)
     max_backoff = kwargs.pop('retry_backoff_max', None)
     retry_options._max_wait_time_in_seconds = max_backoff or retry_options._max_wait_time_in_seconds
     policy.RetryOptions = retry_options
     connection_retry = policy.ConnectionRetryConfiguration
     if not connection_retry:
         connection_retry = _ConnectionRetryPolicy(
             retry_total=total_retries,
@@ -96,15 +97,15 @@
 
     :param str url: The URL of the Cosmos DB account.
     :param credential: Can be the account key, or a dictionary of resource tokens.
     :type credential: Union[str, Dict[str, str], ~azure.core.credentials_async.AsyncTokenCredential]
     :keyword str consistency_level: Consistency level to use for the session. Default value is None (account-level).
         More on consistency levels and possible values: https://aka.ms/cosmos-consistency-levels
     :keyword int timeout: An absolute timeout in seconds, for the combined HTTP request and response processing.
-    :keyword int request_timeout: The HTTP request timeout in milliseconds.
+    :keyword int connection_timeout: The HTTP request timeout in seconds.
     :keyword str connection_mode: The connection mode for the client - currently only supports 'Gateway'.
     :keyword proxy_config: Connection proxy configuration.
     :paramtype proxy_config: ~azure.cosmos.ProxyConfiguration
     :keyword ssl_config: Connection SSL configuration.
     :paramtype ssl_config: ~azure.cosmos.SSLConfiguration
     :keyword bool connection_verify: Whether to verify the connection, default value is True.
     :keyword str connection_cert: An alternative certificate to verify the connection.
```

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/aio/__init__.py` & `azure-cosmos-4.4.0b2/azure/cosmos/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/aio/_container.py` & `azure-cosmos-4.4.0b2/azure/cosmos/aio/_container.py`

 * *Files 2% similar despite different names*

```diff
@@ -537,14 +537,15 @@
 
         :param item: The ID (name) or dict representing item to be patched.
         :type item: Union[str, Dict[str, Any]]
         :param partition_key: The partition key of the object to patch.
         :type partition_key: Union[str, int, float, bool]
         :param patch_operations: The list of patch operations to apply to the item.
         :type patch_operations: List[Dict[str, Any]]
+        :keyword str filter_predicate: conditional filter to apply to Patch operations.
         :keyword str pre_trigger_include: trigger id to be used as pre operation trigger.
         :keyword str post_trigger_include: trigger id to be used as post operation trigger.
         :keyword str session_token: Token for use with Session consistency.
         :keyword dict[str,str] initial_headers: Initial headers to be sent as part of the request.
         :keyword str etag: An ETag value, or the wildcard character (*). Used to check if the resource
             has changed, and act according to the condition specified by the `match_condition` parameter.
         :keyword ~azure.core.MatchConditions match_condition: The match condition to use upon the etag.
@@ -554,14 +555,17 @@
             given id does not exist.
         :rtype: dict[str, Any]
         """
         request_options = _build_options(kwargs)
         response_hook = kwargs.pop('response_hook', None)
         request_options["disableAutomaticIdGeneration"] = True
         request_options["partitionKey"] = partition_key
+        filter_predicate = kwargs.pop("filter_predicate")
+        if filter_predicate is not None:
+            request_options["filterPredicate"] = filter_predicate
 
         item_link = self._get_document_link(item)
         result = await self.client_connection.PatchItem(
             document_link=item_link, operations=patch_operations, options=request_options, **kwargs)
         if response_hook:
             response_hook(self.client_connection.last_response_headers, result)
         return result
@@ -801,15 +805,15 @@
         request_options["partitionKey"] = self._set_partition_key(partition_key)
         result = await self.client_connection.DeleteConflict(
             conflict_link=self._get_conflict_link(conflict), options=request_options, **kwargs
         )
         if response_hook:
             response_hook(self.client_connection.last_response_headers, result)
 
-    @distributed_trace
+    @distributed_trace_async
     async def delete_all_items_by_partition_key(
         self,
         partition_key: Union[str, int, float, bool],
         **kwargs: Any
     ) -> None:
         """Exposes an API to delete all items with a single partition key without the user having
                  to explicitly call delete on each record in the partition key.
```

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/aio/_auth_policy_async.py` & `azure-cosmos-4.4.0b2/azure/cosmos/aio/_auth_policy_async.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/aio/_asynchronous_request.py` & `azure-cosmos-4.4.0b2/azure/cosmos/aio/_asynchronous_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     :return: tuple of (result, headers)
     :rtype: tuple of (dict, dict)
 
     """
     # pylint: disable=protected-access
 
     connection_timeout = connection_policy.RequestTimeout
-    connection_timeout = kwargs.pop("connection_timeout", connection_timeout / 1000.0)
+    connection_timeout = kwargs.pop("connection_timeout", connection_timeout)
 
     # Every request tries to perform a refresh
     client_timeout = kwargs.get('timeout')
     start_time = time.time()
     await global_endpoint_manager.refresh_endpoint_list(None, **kwargs)
     if client_timeout is not None:
         kwargs['timeout'] = client_timeout - (time.time() - start_time)
```

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/aio/_cosmos_client_connection_async.py` & `azure-cosmos-4.4.0b2/azure/cosmos/aio/_cosmos_client_connection_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -1180,15 +1180,19 @@
         if options is None:
             options = {}
 
         initial_headers = self.default_headers
         headers = base.GetHeaders(self, initial_headers, "patch", path, document_id, typ, options)
         # Patch will use WriteEndpoint since it uses PUT operation
         request_params = _request_object.RequestObject(typ, documents._OperationType.Patch)
-        result, self.last_response_headers = await self.__Patch(path, request_params, operations, headers, **kwargs)
+        request_data = {}
+        if options.get("filterPredicate"):
+            request_data["condition"] = options.get("filterPredicate")
+        request_data["operations"] = operations
+        result, self.last_response_headers = await self.__Patch(path, request_params, request_data, headers, **kwargs)
 
         # update session for request mutates data on server side
         self._UpdateSessionIfRequired(headers, result, self.last_response_headers)
         return result
 
     async def ReplaceOffer(self, offer_link, offer, **kwargs):
         """Replaces an offer and returns it.
@@ -1289,20 +1293,20 @@
             connection_policy=self.connection_policy,
             pipeline_client=self.pipeline_client,
             request=request,
             request_data=body,
             **kwargs
         )
 
-    async def __Patch(self, path, request_params, operations, req_headers, **kwargs):
+    async def __Patch(self, path, request_params, request_data, req_headers, **kwargs):
         """Azure Cosmos 'PATCH' http request.
 
         :params str path:
         :params ~azure.cosmos.RequestObject request_params:
-        :params list operations:
+        :params dict request_data:
         :params dict req_headers:
 
         :return:
             Tuple of (result, headers).
         :rtype:
             tuple of (dict, dict)
 
@@ -1311,15 +1315,15 @@
         return await asynchronous_request.AsynchronousRequest(
             client=self,
             request_params=request_params,
             global_endpoint_manager=self._global_endpoint_manager,
             connection_policy=self.connection_policy,
             pipeline_client=self.pipeline_client,
             request=request,
-            request_data=operations,
+            request_data=request_data,
             **kwargs
         )
 
     async def DeleteDatabase(self, database_link, options=None, **kwargs):
         """Deletes a database.
 
         :param str database_link:
```

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/aio/_database.py` & `azure-cosmos-4.4.0b2/azure/cosmos/aio/_database.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/aio/_user.py` & `azure-cosmos-4.4.0b2/azure/cosmos/aio/_user.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure/cosmos/aio/_query_iterable_async.py` & `azure-cosmos-4.4.0b2/azure/cosmos/aio/_query_iterable_async.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/test/test_session_token_unit.py` & `azure-cosmos-4.4.0b2/test/test_session_token_unit.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/test/test_partition_split_query.py` & `azure-cosmos-4.4.0b2/test/test_partition_split_query.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,23 +19,23 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import unittest
 
 import azure.cosmos.cosmos_client as cosmos_client
 from azure.cosmos import PartitionKey
+from azure.cosmos.exceptions import CosmosClientTimeoutError
 import pytest
 import time
 import random
 import uuid
 import test_config
 
 # This test class serves to test partition splits within the query context
 
-pytestmark = pytest.mark.cosmosEmulator
 
 
 @pytest.mark.usefixtures("teardown")
 class TestPartitionSplitQuery(unittest.TestCase):
     configs = test_config._test_config
     host = configs.host
     masterKey = configs.masterKey
@@ -46,30 +46,35 @@
         cls.client = cosmos_client.CosmosClient(cls.host, cls.masterKey)
         cls.database = cls.client.create_database_if_not_exists(id=test_config._test_config.TEST_THROUGHPUT_DATABASE_ID,
                                                                 offer_throughput=cls.throughput)
         cls.container = cls.database.create_container_if_not_exists(
             id=test_config._test_config.TEST_COLLECTION_SINGLE_PARTITION_ID,
             partition_key=PartitionKey(path="/id"))
 
+
+    @pytest.mark.skip # skipping test while staging account issue gets resolved
     def test_partition_split_query(self):
         for i in range(100):
             body = self.get_test_item()
             self.container.create_item(body=body)
 
-        print("created items, changing offer to 11k and starting queries")
-        self.database.replace_throughput(11000)
+        start_time = time.time()
+        print("created items, changing offer to 22k and starting queries")
+        self.database.replace_throughput(22000)
         offer_time = time.time()
         print("changed offer to 11k")
         print("--------------------------------")
         print("now starting queries")
 
         self.run_queries(self.container, 100)  # initial check for queries before partition split
         print("initial check succeeded, now reading offer until replacing is done")
         offer = self.database.get_throughput()
         while True:
+            if time.time() - start_time > 60 * 20: #timeout test at 20 minutes
+                raise CosmosClientTimeoutError()
             if offer.properties['content'].get('isOfferReplacePending', False):
                 time.sleep(10)
                 offer = self.database.get_throughput()
             else:
                 print("offer replaced successfully, took around {} seconds".format(time.time() - offer_time))
                 self.run_queries(self.container, 100)  # check queries work post partition split
                 print("test over")
```

## Comparing `azure-cosmos-4.4.0b1/test/test_auto_scale.py` & `azure-cosmos-4.4.0b2/test/test_auto_scale.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/test/test_correlated_activity_id.py` & `azure-cosmos-4.4.0b2/test/test_correlated_activity_id.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/test/test_aad.py` & `azure-cosmos-4.4.0b2/test/test_aad.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/test/test_orderby.py` & `azure-cosmos-4.4.0b2/test/test_orderby.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/test/test_user_configs.py` & `azure-cosmos-4.4.0b2/test/test_user_configs.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/test/test_analytical_ttl.py` & `azure-cosmos-4.4.0b2/test/test_analytical_ttl.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/test/test_session.py` & `azure-cosmos-4.4.0b2/test/test_session.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/test/test_headers.py` & `azure-cosmos-4.4.0b2/test/test_headers.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/test/test_streaming_failover.py` & `azure-cosmos-4.4.0b2/test/test_streaming_failover.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/test/test_media.py` & `azure-cosmos-4.4.0b2/test/test_media.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/test/test_query.py` & `azure-cosmos-4.4.0b2/test/test_query.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/test/test_partition_key.py` & `azure-cosmos-4.4.0b2/test/test_partition_key.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/test/test_routing_map.py` & `azure-cosmos-4.4.0b2/test/test_routing_map.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/test/test_ttl.py` & `azure-cosmos-4.4.0b2/test/test_ttl.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/test/test_multi_orderby.py` & `azure-cosmos-4.4.0b2/test/test_multi_orderby.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/test/test_encoding.py` & `azure-cosmos-4.4.0b2/test/test_encoding.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/test/test_auto_scale_async.py` & `azure-cosmos-4.4.0b2/test/test_auto_scale_async.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/test/test_crud_async.py` & `azure-cosmos-4.4.0b2/test/test_crud_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -7264,616 +7264,774 @@
 0001c5f0: 5f70 6572 6d69 7373 696f 6e28 6372 6561  _permission(crea
 0001c600: 7465 645f 7065 726d 6973 7369 6f6e 2e70  ted_permission.p
 0001c610: 726f 7065 7274 6965 7329 0a20 2020 2020  roperties).     
 0001c620: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
 0001c630: 7561 6c28 7265 6164 5f70 6572 6d69 7373  ual(read_permiss
 0001c640: 696f 6e2e 6964 2c20 6372 6561 7465 645f  ion.id, created_
 0001c650: 7065 726d 6973 7369 6f6e 2e69 6429 0a0a  permission.id)..
-0001c660: 2020 2020 6173 796e 6320 6465 6620 7465      async def te
-0001c670: 7374 5f64 656c 6574 655f 616c 6c5f 6974  st_delete_all_it
-0001c680: 656d 735f 6279 5f70 6172 7469 7469 6f6e  ems_by_partition
-0001c690: 5f6b 6579 2873 656c 6629 3a0a 2020 2020  _key(self):.    
-0001c6a0: 2020 2020 2320 6372 6561 7465 2064 6174      # create dat
-0001c6b0: 6162 6173 650a 2020 2020 2020 2020 6372  abase.        cr
-0001c6c0: 6561 7465 645f 6462 203d 2073 656c 662e  eated_db = self.
-0001c6d0: 6461 7461 6261 7365 466f 7254 6573 740a  databaseForTest.
-0001c6e0: 0a20 2020 2020 2020 2023 2063 7265 6174  .        # creat
-0001c6f0: 6520 636f 6e74 6169 6e65 720a 2020 2020  e container.    
-0001c700: 2020 2020 6372 6561 7465 645f 636f 6c6c      created_coll
-0001c710: 6563 7469 6f6e 203d 2061 7761 6974 2063  ection = await c
-0001c720: 7265 6174 6564 5f64 622e 6372 6561 7465  reated_db.create
-0001c730: 5f63 6f6e 7461 696e 6572 280a 2020 2020  _container(.    
-0001c740: 2020 2020 2020 2020 6964 3d27 7465 7374          id='test
-0001c750: 5f64 656c 6574 655f 616c 6c5f 6974 656d  _delete_all_item
-0001c760: 735f 6279 5f70 6172 7469 7469 6f6e 5f6b  s_by_partition_k
-0001c770: 6579 2027 202b 2073 7472 2875 7569 642e  ey ' + str(uuid.
-0001c780: 7575 6964 3428 2929 2c0a 2020 2020 2020  uuid4()),.      
-0001c790: 2020 2020 2020 7061 7274 6974 696f 6e5f        partition_
-0001c7a0: 6b65 793d 5061 7274 6974 696f 6e4b 6579  key=PartitionKey
-0001c7b0: 2870 6174 683d 272f 706b 272c 206b 696e  (path='/pk', kin
-0001c7c0: 643d 2748 6173 6827 290a 2020 2020 2020  d='Hash').      
-0001c7d0: 2020 290a 2020 2020 2020 2020 2320 4372    ).        # Cr
-0001c7e0: 6561 7465 2074 776f 2070 6172 7469 7469  eate two partiti
-0001c7f0: 6f6e 206b 6579 730a 2020 2020 2020 2020  on keys.        
-0001c800: 7061 7274 6974 696f 6e5f 6b65 7931 203d  partition_key1 =
-0001c810: 2022 7b7d 2d7b 7d22 2e66 6f72 6d61 7428   "{}-{}".format(
-0001c820: 2250 6172 7469 7469 6f6e 204b 6579 2031  "Partition Key 1
-0001c830: 222c 2073 7472 2875 7569 642e 7575 6964  ", str(uuid.uuid
-0001c840: 3428 2929 290a 2020 2020 2020 2020 7061  4())).        pa
-0001c850: 7274 6974 696f 6e5f 6b65 7932 203d 2022  rtition_key2 = "
-0001c860: 7b7d 2d7b 7d22 2e66 6f72 6d61 7428 2250  {}-{}".format("P
-0001c870: 6172 7469 7469 6f6e 204b 6579 2032 222c  artition Key 2",
-0001c880: 2073 7472 2875 7569 642e 7575 6964 3428   str(uuid.uuid4(
-0001c890: 2929 290a 0a20 2020 2020 2020 2023 2061  )))..        # a
-0001c8a0: 6464 2069 7465 6d73 2066 6f72 2070 6172  dd items for par
-0001c8b0: 7469 7469 6f6e 206b 6579 2031 0a20 2020  tition key 1.   
-0001c8c0: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
-0001c8d0: 6e67 6528 312c 2033 293a 0a20 2020 2020  nge(1, 3):.     
-0001c8e0: 2020 2020 2020 2061 7761 6974 2063 7265         await cre
-0001c8f0: 6174 6564 5f63 6f6c 6c65 6374 696f 6e2e  ated_collection.
-0001c900: 7570 7365 7274 5f69 7465 6d28 0a20 2020  upsert_item(.   
-0001c910: 2020 2020 2020 2020 2020 2020 2064 6963               dic
-0001c920: 7428 6964 3d22 6974 656d 7b7d 222e 666f  t(id="item{}".fo
-0001c930: 726d 6174 2869 292c 2070 6b3d 7061 7274  rmat(i), pk=part
-0001c940: 6974 696f 6e5f 6b65 7931 290a 2020 2020  ition_key1).    
-0001c950: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-0001c960: 2020 2023 2061 6464 2069 7465 6d73 2066     # add items f
-0001c970: 6f72 2070 6172 7469 7469 6f6e 206b 6579  or partition key
-0001c980: 2032 0a20 2020 2020 2020 2070 6b32 5f69   2.        pk2_i
-0001c990: 7465 6d20 3d20 6177 6169 7420 6372 6561  tem = await crea
-0001c9a0: 7465 645f 636f 6c6c 6563 7469 6f6e 2e75  ted_collection.u
-0001c9b0: 7073 6572 745f 6974 656d 2864 6963 7428  psert_item(dict(
-0001c9c0: 6964 3d22 6974 656d 7b7d 222e 666f 726d  id="item{}".form
-0001c9d0: 6174 2833 292c 2070 6b3d 7061 7274 6974  at(3), pk=partit
-0001c9e0: 696f 6e5f 6b65 7932 2929 0a0a 2020 2020  ion_key2))..    
-0001c9f0: 2020 2020 2320 6465 6c65 7465 2061 6c6c      # delete all
-0001ca00: 2069 7465 6d73 2066 6f72 2070 6172 7469   items for parti
-0001ca10: 7469 6f6e 206b 6579 2031 0a20 2020 2020  tion key 1.     
-0001ca20: 2020 2061 7761 6974 2063 7265 6174 6564     await created
-0001ca30: 5f63 6f6c 6c65 6374 696f 6e2e 6465 6c65  _collection.dele
-0001ca40: 7465 5f61 6c6c 5f69 7465 6d73 5f62 795f  te_all_items_by_
-0001ca50: 7061 7274 6974 696f 6e5f 6b65 7928 7061  partition_key(pa
-0001ca60: 7274 6974 696f 6e5f 6b65 7931 290a 0a20  rtition_key1).. 
-0001ca70: 2020 2020 2020 2023 2063 6865 636b 2074         # check t
-0001ca80: 6861 7420 6f6e 6c79 2069 7465 6d73 2066  hat only items f
-0001ca90: 726f 6d20 7061 7274 6974 696f 6e20 6b65  rom partition ke
-0001caa0: 7920 3120 6861 7665 2062 6565 6e20 6465  y 1 have been de
-0001cab0: 6c65 7465 640a 2020 2020 2020 2020 6974  leted.        it
-0001cac0: 656d 7320 3d20 5b69 7465 6d20 6173 796e  ems = [item asyn
-0001cad0: 6320 666f 7220 6974 656d 2069 6e20 6372  c for item in cr
-0001cae0: 6561 7465 645f 636f 6c6c 6563 7469 6f6e  eated_collection
-0001caf0: 2e72 6561 645f 616c 6c5f 6974 656d 7328  .read_all_items(
-0001cb00: 295d 0a0a 2020 2020 2020 2020 2320 6974  )]..        # it
-0001cb10: 656d 7320 7368 6f75 6c64 206f 6e6c 7920  ems should only 
-0001cb20: 6861 7665 2031 2069 7465 6d2c 2061 6e64  have 1 item, and
-0001cb30: 2069 7420 7368 6f75 6c64 2065 7175 616c   it should equal
-0001cb40: 2070 6b32 5f69 7465 6d0a 2020 2020 2020   pk2_item.      
-0001cb50: 2020 7365 6c66 2e61 7373 6572 7444 6963    self.assertDic
-0001cb60: 7445 7175 616c 2870 6b32 5f69 7465 6d2c  tEqual(pk2_item,
-0001cb70: 2069 7465 6d73 5b30 5d29 0a0a 2020 2020   items[0])..    
-0001cb80: 2020 2020 2320 6174 7465 6d70 7469 6e67      # attempting
-0001cb90: 2074 6f20 6465 6c65 7465 2061 206e 6f6e   to delete a non
-0001cba0: 2d65 7869 7374 656e 7420 7061 7274 6974  -existent partit
-0001cbb0: 696f 6e20 6b65 7920 6f72 2070 6173 7369  ion key or passi
-0001cbc0: 6e67 206e 6f6e 6520 7368 6f75 6c64 206e  ng none should n
-0001cbd0: 6f74 2064 656c 6574 650a 2020 2020 2020  ot delete.      
-0001cbe0: 2020 2320 616e 7974 6869 6e67 2061 6e64    # anything and
-0001cbf0: 206c 6561 7665 2074 6869 6e67 7320 756e   leave things un
-0001cc00: 6368 616e 6765 640a 2020 2020 2020 2020  changed.        
-0001cc10: 6177 6169 7420 6372 6561 7465 645f 636f  await created_co
-0001cc20: 6c6c 6563 7469 6f6e 2e64 656c 6574 655f  llection.delete_
-0001cc30: 616c 6c5f 6974 656d 735f 6279 5f70 6172  all_items_by_par
-0001cc40: 7469 7469 6f6e 5f6b 6579 284e 6f6e 6529  tition_key(None)
-0001cc50: 0a0a 2020 2020 2020 2020 2320 6368 6563  ..        # chec
-0001cc60: 6b20 7468 6174 206e 6f20 6368 616e 6765  k that no change
-0001cc70: 7320 7765 7265 206d 6164 6520 6279 2063  s were made by c
-0001cc80: 6865 636b 696e 6720 6966 2074 6865 206f  hecking if the o
-0001cc90: 6e6c 7920 6974 656d 2069 7320 7374 696c  nly item is stil
-0001cca0: 6c20 7468 6572 650a 2020 2020 2020 2020  l there.        
-0001ccb0: 6974 656d 7320 3d20 5b69 7465 6d20 6173  items = [item as
-0001ccc0: 796e 6320 666f 7220 6974 656d 2069 6e20  ync for item in 
-0001ccd0: 6372 6561 7465 645f 636f 6c6c 6563 7469  created_collecti
-0001cce0: 6f6e 2e72 6561 645f 616c 6c5f 6974 656d  on.read_all_item
-0001ccf0: 7328 295d 0a0a 2020 2020 2020 2020 2320  s()]..        # 
-0001cd00: 6974 656d 7320 7368 6f75 6c64 206f 6e6c  items should onl
-0001cd10: 7920 6861 7665 2031 2069 7465 6d2c 2061  y have 1 item, a
-0001cd20: 6e64 2069 7420 7368 6f75 6c64 2065 7175  nd it should equ
-0001cd30: 616c 2070 6b32 5f69 7465 6d0a 2020 2020  al pk2_item.    
-0001cd40: 2020 2020 7365 6c66 2e61 7373 6572 7444      self.assertD
-0001cd50: 6963 7445 7175 616c 2870 6b32 5f69 7465  ictEqual(pk2_ite
-0001cd60: 6d2c 2069 7465 6d73 5b30 5d29 0a0a 2020  m, items[0])..  
-0001cd70: 2020 2020 2020 6177 6169 7420 6372 6561        await crea
-0001cd80: 7465 645f 6462 2e64 656c 6574 655f 636f  ted_db.delete_co
-0001cd90: 6e74 6169 6e65 7228 6372 6561 7465 645f  ntainer(created_
-0001cda0: 636f 6c6c 6563 7469 6f6e 290a 0a20 2020  collection)..   
-0001cdb0: 2061 7379 6e63 2064 6566 2074 6573 745f   async def test_
-0001cdc0: 7061 7463 685f 6f70 6572 6174 696f 6e73  patch_operations
-0001cdd0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0001cde0: 6372 6561 7465 645f 636f 6e74 6169 6e65  created_containe
-0001cdf0: 7220 3d20 6177 6169 7420 7365 6c66 2e64  r = await self.d
-0001ce00: 6174 6162 6173 6546 6f72 5465 7374 2e63  atabaseForTest.c
-0001ce10: 7265 6174 655f 636f 6e74 6169 6e65 725f  reate_container_
-0001ce20: 6966 5f6e 6f74 5f65 7869 7374 7328 6964  if_not_exists(id
-0001ce30: 3d22 7061 7463 685f 636f 6e74 6169 6e65  ="patch_containe
-0001ce40: 7222 2c20 7061 7274 6974 696f 6e5f 6b65  r", partition_ke
-0001ce50: 793d 5061 7274 6974 696f 6e4b 6579 2870  y=PartitionKey(p
-0001ce60: 6174 683d 222f 706b 2229 290a 0a20 2020  ath="/pk"))..   
-0001ce70: 2020 2020 2023 4372 6561 7465 2069 7465       #Create ite
-0001ce80: 6d20 746f 2070 6174 6368 0a20 2020 2020  m to patch.     
-0001ce90: 2020 2069 7465 6d20 3d20 7b0a 2020 2020     item = {.    
-0001cea0: 2020 2020 2020 2020 2269 6422 3a20 2270          "id": "p
-0001ceb0: 6174 6368 5f69 7465 6d22 2c0a 2020 2020  atch_item",.    
-0001cec0: 2020 2020 2020 2020 2270 6b22 3a20 2270          "pk": "p
-0001ced0: 6174 6368 5f69 7465 6d5f 706b 222c 0a20  atch_item_pk",. 
-0001cee0: 2020 2020 2020 2020 2020 2022 7072 6f70             "prop
-0001cef0: 223a 2022 7072 6f70 3122 2c0a 2020 2020  ": "prop1",.    
-0001cf00: 2020 2020 2020 2020 2261 6464 7265 7373          "address
-0001cf10: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
-0001cf20: 2020 2020 2022 6369 7479 223a 2022 5265       "city": "Re
-0001cf30: 646d 6f6e 6422 0a20 2020 2020 2020 2020  dmond".         
-0001cf40: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
-0001cf50: 2020 2263 6f6d 7061 6e79 223a 2022 4d69    "company": "Mi
-0001cf60: 6372 6f73 6f66 7422 2c0a 2020 2020 2020  crosoft",.      
-0001cf70: 2020 2020 2020 226e 756d 6265 7222 3a20        "number": 
-0001cf80: 337d 0a20 2020 2020 2020 2061 7761 6974  3}.        await
-0001cf90: 2063 7265 6174 6564 5f63 6f6e 7461 696e   created_contain
-0001cfa0: 6572 2e63 7265 6174 655f 6974 656d 2869  er.create_item(i
-0001cfb0: 7465 6d29 0a20 2020 2020 2020 2023 4465  tem).        #De
-0001cfc0: 6669 6e65 2061 6e64 2072 756e 2070 6174  fine and run pat
-0001cfd0: 6368 206f 7065 7261 7469 6f6e 730a 2020  ch operations.  
-0001cfe0: 2020 2020 2020 6f70 6572 6174 696f 6e73        operations
-0001cff0: 203d 205b 0a20 2020 2020 2020 2020 2020   = [.           
-0001d000: 207b 226f 7022 3a20 2261 6464 222c 2022   {"op": "add", "
-0001d010: 7061 7468 223a 2022 2f63 6f6c 6f72 222c  path": "/color",
-0001d020: 2022 7661 6c75 6522 3a20 2279 656c 6c6f   "value": "yello
-0001d030: 7722 7d2c 0a20 2020 2020 2020 2020 2020  w"},.           
-0001d040: 207b 226f 7022 3a20 2272 656d 6f76 6522   {"op": "remove"
-0001d050: 2c20 2270 6174 6822 3a20 222f 7072 6f70  , "path": "/prop
-0001d060: 227d 2c0a 2020 2020 2020 2020 2020 2020  "},.            
-0001d070: 7b22 6f70 223a 2022 7265 706c 6163 6522  {"op": "replace"
-0001d080: 2c20 2270 6174 6822 3a20 222f 636f 6d70  , "path": "/comp
-0001d090: 616e 7922 2c20 2276 616c 7565 223a 2022  any", "value": "
-0001d0a0: 436f 736d 6f73 4442 227d 2c0a 2020 2020  CosmosDB"},.    
-0001d0b0: 2020 2020 2020 2020 7b22 6f70 223a 2022          {"op": "
-0001d0c0: 7365 7422 2c20 2270 6174 6822 3a20 222f  set", "path": "/
-0001d0d0: 6164 6472 6573 732f 6e65 775f 6369 7479  address/new_city
-0001d0e0: 222c 2022 7661 6c75 6522 3a20 2241 746c  ", "value": "Atl
-0001d0f0: 616e 7461 227d 2c0a 2020 2020 2020 2020  anta"},.        
-0001d100: 2020 2020 7b22 6f70 223a 2022 696e 6372      {"op": "incr
-0001d110: 222c 2022 7061 7468 223a 2022 2f6e 756d  ", "path": "/num
-0001d120: 6265 7222 2c20 2276 616c 7565 223a 2037  ber", "value": 7
-0001d130: 7d2c 0a20 2020 2020 2020 2020 2020 207b  },.            {
-0001d140: 226f 7022 3a20 226d 6f76 6522 2c20 2266  "op": "move", "f
-0001d150: 726f 6d22 3a20 222f 636f 6c6f 7222 2c20  rom": "/color", 
-0001d160: 2270 6174 6822 3a20 222f 6661 766f 7269  "path": "/favori
-0001d170: 7465 5f63 6f6c 6f72 227d 0a20 2020 2020  te_color"}.     
-0001d180: 2020 205d 0a20 2020 2020 2020 2070 6174     ].        pat
-0001d190: 6368 6564 5f69 7465 6d20 3d20 6177 6169  ched_item = awai
-0001d1a0: 7420 6372 6561 7465 645f 636f 6e74 6169  t created_contai
-0001d1b0: 6e65 722e 7061 7463 685f 6974 656d 2869  ner.patch_item(i
-0001d1c0: 7465 6d3d 2270 6174 6368 5f69 7465 6d22  tem="patch_item"
-0001d1d0: 2c20 7061 7274 6974 696f 6e5f 6b65 793d  , partition_key=
-0001d1e0: 2270 6174 6368 5f69 7465 6d5f 706b 222c  "patch_item_pk",
-0001d1f0: 2070 6174 6368 5f6f 7065 7261 7469 6f6e   patch_operation
-0001d200: 733d 6f70 6572 6174 696f 6e73 290a 2020  s=operations).  
-0001d210: 2020 2020 2020 2356 6572 6966 7920 7265        #Verify re
-0001d220: 7375 6c74 7320 6672 6f6d 2070 6174 6368  sults from patch
-0001d230: 206f 7065 7261 7469 6f6e 730a 2020 2020   operations.    
-0001d240: 2020 2020 7365 6c66 2e61 7373 6572 7454      self.assertT
-0001d250: 7275 6528 7061 7463 6865 645f 6974 656d  rue(patched_item
-0001d260: 2e67 6574 2822 636f 6c6f 7222 2920 6973  .get("color") is
-0001d270: 204e 6f6e 6529 0a20 2020 2020 2020 2073   None).        s
-0001d280: 656c 662e 6173 7365 7274 5472 7565 2870  elf.assertTrue(p
-0001d290: 6174 6368 6564 5f69 7465 6d2e 6765 7428  atched_item.get(
-0001d2a0: 2270 726f 7022 2920 6973 204e 6f6e 6529  "prop") is None)
-0001d2b0: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-0001d2c0: 7365 7274 4571 7561 6c28 7061 7463 6865  sertEqual(patche
-0001d2d0: 645f 6974 656d 2e67 6574 2822 636f 6d70  d_item.get("comp
-0001d2e0: 616e 7922 292c 2022 436f 736d 6f73 4442  any"), "CosmosDB
-0001d2f0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-0001d300: 6173 7365 7274 4571 7561 6c28 7061 7463  assertEqual(patc
-0001d310: 6865 645f 6974 656d 2e67 6574 2822 6164  hed_item.get("ad
-0001d320: 6472 6573 7322 292e 6765 7428 226e 6577  dress").get("new
-0001d330: 5f63 6974 7922 292c 2022 4174 6c61 6e74  _city"), "Atlant
-0001d340: 6122 290a 2020 2020 2020 2020 7365 6c66  a").        self
-0001d350: 2e61 7373 6572 7445 7175 616c 2870 6174  .assertEqual(pat
-0001d360: 6368 6564 5f69 7465 6d2e 6765 7428 226e  ched_item.get("n
-0001d370: 756d 6265 7222 292c 2031 3029 0a20 2020  umber"), 10).   
-0001d380: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-0001d390: 4571 7561 6c28 7061 7463 6865 645f 6974  Equal(patched_it
-0001d3a0: 656d 2e67 6574 2822 6661 766f 7269 7465  em.get("favorite
-0001d3b0: 5f63 6f6c 6f72 2229 2c20 2279 656c 6c6f  _color"), "yello
-0001d3c0: 7722 290a 0a20 2020 2020 2020 2023 4e65  w")..        #Ne
-0001d3d0: 6761 7469 7665 2074 6573 7420 2d20 6174  gative test - at
-0001d3e0: 7465 6d70 7420 746f 2072 6570 6c61 6365  tempt to replace
-0001d3f0: 206e 6f6e 2d65 7869 7374 656e 7420 6669   non-existent fi
-0001d400: 656c 640a 2020 2020 2020 2020 6f70 6572  eld.        oper
-0001d410: 6174 696f 6e73 203d 205b 7b22 6f70 223a  ations = [{"op":
-0001d420: 2022 7265 706c 6163 6522 2c20 2270 6174   "replace", "pat
-0001d430: 6822 3a20 222f 7772 6f6e 675f 6669 656c  h": "/wrong_fiel
-0001d440: 6422 2c20 2276 616c 7565 223a 2022 7772  d", "value": "wr
-0001d450: 6f6e 675f 7661 6c75 6522 7d5d 0a20 2020  ong_value"}].   
-0001d460: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-0001d470: 2020 2020 2020 6177 6169 7420 6372 6561        await crea
-0001d480: 7465 645f 636f 6e74 6169 6e65 722e 7061  ted_container.pa
-0001d490: 7463 685f 6974 656d 2869 7465 6d3d 2270  tch_item(item="p
-0001d4a0: 6174 6368 5f69 7465 6d22 2c20 7061 7274  atch_item", part
-0001d4b0: 6974 696f 6e5f 6b65 793d 2270 6174 6368  ition_key="patch
-0001d4c0: 5f69 7465 6d5f 706b 222c 2070 6174 6368  _item_pk", patch
-0001d4d0: 5f6f 7065 7261 7469 6f6e 733d 6f70 6572  _operations=oper
-0001d4e0: 6174 696f 6e73 290a 2020 2020 2020 2020  ations).        
-0001d4f0: 6578 6365 7074 2065 7863 6570 7469 6f6e  except exception
-0001d500: 732e 436f 736d 6f73 4874 7470 5265 7370  s.CosmosHttpResp
-0001d510: 6f6e 7365 4572 726f 7220 6173 2065 3a0a  onseError as e:.
-0001d520: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0001d530: 2e61 7373 6572 7445 7175 616c 2865 2e73  .assertEqual(e.s
-0001d540: 7461 7475 735f 636f 6465 2c20 5374 6174  tatus_code, Stat
-0001d550: 7573 436f 6465 732e 4241 445f 5245 5155  usCodes.BAD_REQU
-0001d560: 4553 5429 0a0a 2020 2020 2020 2020 234e  EST)..        #N
-0001d570: 6567 6174 6976 6520 7465 7374 202d 2061  egative test - a
-0001d580: 7474 656d 7074 2074 6f20 7265 6d6f 7665  ttempt to remove
-0001d590: 206e 6f6e 2d65 7869 7374 656e 7420 6669   non-existent fi
-0001d5a0: 656c 640a 2020 2020 2020 2020 6f70 6572  eld.        oper
-0001d5b0: 6174 696f 6e73 203d 205b 7b22 6f70 223a  ations = [{"op":
-0001d5c0: 2022 7265 6d6f 7665 222c 2022 7061 7468   "remove", "path
-0001d5d0: 223a 2022 2f77 726f 6e67 5f66 6965 6c64  ": "/wrong_field
-0001d5e0: 227d 5d0a 2020 2020 2020 2020 7472 793a  "}].        try:
-0001d5f0: 0a20 2020 2020 2020 2020 2020 2061 7761  .            awa
-0001d600: 6974 2063 7265 6174 6564 5f63 6f6e 7461  it created_conta
-0001d610: 696e 6572 2e70 6174 6368 5f69 7465 6d28  iner.patch_item(
-0001d620: 6974 656d 3d22 7061 7463 685f 6974 656d  item="patch_item
-0001d630: 222c 2070 6172 7469 7469 6f6e 5f6b 6579  ", partition_key
-0001d640: 3d22 7061 7463 685f 6974 656d 5f70 6b22  ="patch_item_pk"
-0001d650: 2c20 7061 7463 685f 6f70 6572 6174 696f  , patch_operatio
-0001d660: 6e73 3d6f 7065 7261 7469 6f6e 7329 0a20  ns=operations). 
-0001d670: 2020 2020 2020 2065 7863 6570 7420 6578         except ex
-0001d680: 6365 7074 696f 6e73 2e43 6f73 6d6f 7348  ceptions.CosmosH
-0001d690: 7474 7052 6573 706f 6e73 6545 7272 6f72  ttpResponseError
-0001d6a0: 2061 7320 653a 0a20 2020 2020 2020 2020   as e:.         
-0001d6b0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-0001d6c0: 7561 6c28 652e 7374 6174 7573 5f63 6f64  ual(e.status_cod
-0001d6d0: 652c 2053 7461 7475 7343 6f64 6573 2e42  e, StatusCodes.B
-0001d6e0: 4144 5f52 4551 5545 5354 290a 0a20 2020  AD_REQUEST)..   
-0001d6f0: 2020 2020 2023 4e65 6761 7469 7665 2074       #Negative t
-0001d700: 6573 7420 2d20 6174 7465 6d70 7420 746f  est - attempt to
-0001d710: 2069 6e63 7265 6d65 6e74 206e 6f6e 2d6e   increment non-n
-0001d720: 756d 6265 7220 6669 656c 640a 2020 2020  umber field.    
-0001d730: 2020 2020 6f70 6572 6174 696f 6e73 203d      operations =
-0001d740: 205b 7b22 6f70 223a 2022 696e 6372 222c   [{"op": "incr",
-0001d750: 2022 7061 7468 223a 2022 2f63 6f6d 7061   "path": "/compa
-0001d760: 6e79 222c 2022 7661 6c75 6522 3a20 337d  ny", "value": 3}
-0001d770: 5d0a 2020 2020 2020 2020 7472 793a 0a20  ].        try:. 
-0001d780: 2020 2020 2020 2020 2020 2061 7761 6974             await
-0001d790: 2063 7265 6174 6564 5f63 6f6e 7461 696e   created_contain
-0001d7a0: 6572 2e70 6174 6368 5f69 7465 6d28 6974  er.patch_item(it
-0001d7b0: 656d 3d22 7061 7463 685f 6974 656d 222c  em="patch_item",
-0001d7c0: 2070 6172 7469 7469 6f6e 5f6b 6579 3d22   partition_key="
-0001d7d0: 7061 7463 685f 6974 656d 5f70 6b22 2c20  patch_item_pk", 
-0001d7e0: 7061 7463 685f 6f70 6572 6174 696f 6e73  patch_operations
-0001d7f0: 3d6f 7065 7261 7469 6f6e 7329 0a20 2020  =operations).   
-0001d800: 2020 2020 2065 7863 6570 7420 6578 6365       except exce
-0001d810: 7074 696f 6e73 2e43 6f73 6d6f 7348 7474  ptions.CosmosHtt
-0001d820: 7052 6573 706f 6e73 6545 7272 6f72 2061  pResponseError a
-0001d830: 7320 653a 0a20 2020 2020 2020 2020 2020  s e:.           
-0001d840: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-0001d850: 6c28 652e 7374 6174 7573 5f63 6f64 652c  l(e.status_code,
-0001d860: 2053 7461 7475 7343 6f64 6573 2e42 4144   StatusCodes.BAD
-0001d870: 5f52 4551 5545 5354 290a 0a20 2020 2020  _REQUEST)..     
-0001d880: 2020 2023 4e65 6761 7469 7665 2074 6573     #Negative tes
-0001d890: 7420 2d20 6174 7465 6d70 7420 746f 206d  t - attempt to m
-0001d8a0: 6f76 6520 6672 6f6d 206e 6f6e 2d65 7869  ove from non-exi
-0001d8b0: 7374 656e 7420 6669 656c 640a 2020 2020  stent field.    
-0001d8c0: 2020 2020 6f70 6572 6174 696f 6e73 203d      operations =
-0001d8d0: 205b 7b22 6f70 223a 2022 6d6f 7665 222c   [{"op": "move",
-0001d8e0: 2022 6672 6f6d 223a 2022 2f77 726f 6e67   "from": "/wrong
-0001d8f0: 5f66 6965 6c64 222c 2022 7061 7468 223a  _field", "path":
-0001d900: 2022 2f6f 7468 6572 5f66 6965 6c64 227d   "/other_field"}
-0001d910: 5d0a 2020 2020 2020 2020 7472 793a 0a20  ].        try:. 
-0001d920: 2020 2020 2020 2020 2020 2061 7761 6974             await
-0001d930: 2063 7265 6174 6564 5f63 6f6e 7461 696e   created_contain
-0001d940: 6572 2e70 6174 6368 5f69 7465 6d28 6974  er.patch_item(it
-0001d950: 656d 3d22 7061 7463 685f 6974 656d 222c  em="patch_item",
-0001d960: 2070 6172 7469 7469 6f6e 5f6b 6579 3d22   partition_key="
-0001d970: 7061 7463 685f 6974 656d 5f70 6b22 2c20  patch_item_pk", 
-0001d980: 7061 7463 685f 6f70 6572 6174 696f 6e73  patch_operations
-0001d990: 3d6f 7065 7261 7469 6f6e 7329 0a20 2020  =operations).   
-0001d9a0: 2020 2020 2065 7863 6570 7420 6578 6365       except exce
-0001d9b0: 7074 696f 6e73 2e43 6f73 6d6f 7348 7474  ptions.CosmosHtt
-0001d9c0: 7052 6573 706f 6e73 6545 7272 6f72 2061  pResponseError a
-0001d9d0: 7320 653a 0a20 2020 2020 2020 2020 2020  s e:.           
-0001d9e0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-0001d9f0: 6c28 652e 7374 6174 7573 5f63 6f64 652c  l(e.status_code,
-0001da00: 2053 7461 7475 7343 6f64 6573 2e42 4144   StatusCodes.BAD
-0001da10: 5f52 4551 5545 5354 290a 0a20 2020 2023  _REQUEST)..    #
-0001da20: 2054 656d 706f 7261 7269 6c79 2063 6f6d   Temporarily com
-0001da30: 6d65 6e74 696e 6720 616e 616c 7974 6963  menting analytic
-0001da40: 616c 2073 746f 7261 6765 2074 6573 7473  al storage tests
-0001da50: 2075 6e74 696c 2065 6d75 6c61 746f 7220   until emulator 
-0001da60: 7375 7070 6f72 7420 636f 6d65 732e 0a20  support comes.. 
-0001da70: 2020 2023 2064 6566 2074 6573 745f 6372     # def test_cr
-0001da80: 6561 7465 5f63 6f6e 7461 696e 6572 5f77  eate_container_w
-0001da90: 6974 685f 616e 616c 7974 6963 616c 5f73  ith_analytical_s
-0001daa0: 746f 7265 5f6f 6666 2873 656c 6629 3a0a  tore_off(self):.
-0001dab0: 2020 2020 2320 2020 2020 2320 646f 6e27      #     # don'
-0001dac0: 7420 7275 6e20 7465 7374 2c20 666f 7220  t run test, for 
-0001dad0: 7468 6520 7469 6d65 2062 6569 6e67 2c20  the time being, 
-0001dae0: 6966 2072 756e 6e69 6e67 2061 6761 696e  if running again
-0001daf0: 7374 2074 6865 2065 6d75 6c61 746f 720a  st the emulator.
-0001db00: 2020 2020 2320 2020 2020 6966 2027 6c6f      #     if 'lo
-0001db10: 6361 6c68 6f73 7427 2069 6e20 7365 6c66  calhost' in self
-0001db20: 2e68 6f73 7420 6f72 2027 3132 372e 302e  .host or '127.0.
-0001db30: 302e 3127 2069 6e20 7365 6c66 2e68 6f73  0.1' in self.hos
-0001db40: 743a 0a20 2020 2023 2020 2020 2020 2020  t:.    #        
-0001db50: 2072 6574 7572 6e0a 0a20 2020 2023 2020   return..    #  
-0001db60: 2020 2063 7265 6174 6564 5f64 6220 3d20     created_db = 
-0001db70: 7365 6c66 2e64 6174 6162 6173 6546 6f72  self.databaseFor
-0001db80: 5465 7374 0a20 2020 2023 2020 2020 2063  Test.    #     c
-0001db90: 6f6c 6c65 6374 696f 6e5f 6964 203d 2027  ollection_id = '
-0001dba0: 7465 7374 5f63 7265 6174 655f 636f 6e74  test_create_cont
-0001dbb0: 6169 6e65 725f 7769 7468 5f61 6e61 6c79  ainer_with_analy
-0001dbc0: 7469 6361 6c5f 7374 6f72 655f 6f66 665f  tical_store_off_
-0001dbd0: 2720 2b20 7374 7228 7575 6964 2e75 7569  ' + str(uuid.uui
-0001dbe0: 6434 2829 290a 2020 2020 2320 2020 2020  d4()).    #     
-0001dbf0: 636f 6c6c 6563 7469 6f6e 5f69 6e64 6578  collection_index
-0001dc00: 696e 675f 706f 6c69 6379 203d 207b 2769  ing_policy = {'i
-0001dc10: 6e64 6578 696e 674d 6f64 6527 3a20 2763  ndexingMode': 'c
-0001dc20: 6f6e 7369 7374 656e 7427 7d0a 2020 2020  onsistent'}.    
-0001dc30: 2320 2020 2020 6372 6561 7465 645f 7265  #     created_re
-0001dc40: 636f 7264 6572 203d 2052 6563 6f72 6444  corder = RecordD
-0001dc50: 6961 676e 6f73 7469 6373 2829 0a20 2020  iagnostics().   
-0001dc60: 2023 2020 2020 2063 7265 6174 6564 5f63   #     created_c
-0001dc70: 6f6c 6c65 6374 696f 6e20 3d20 6372 6561  ollection = crea
-0001dc80: 7465 645f 6462 2e63 7265 6174 655f 636f  ted_db.create_co
-0001dc90: 6e74 6169 6e65 7228 6964 3d63 6f6c 6c65  ntainer(id=colle
-0001dca0: 6374 696f 6e5f 6964 2c0a 2020 2020 2320  ction_id,.    # 
-0001dcb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dcc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dcd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dce0: 2020 2020 2069 6e64 6578 696e 675f 706f       indexing_po
-0001dcf0: 6c69 6379 3d63 6f6c 6c65 6374 696f 6e5f  licy=collection_
-0001dd00: 696e 6465 7869 6e67 5f70 6f6c 6963 792c  indexing_policy,
-0001dd10: 0a20 2020 2023 2020 2020 2020 2020 2020  .    #          
-0001dd20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dd30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dd40: 2020 2020 2020 2020 2020 2020 7061 7274              part
-0001dd50: 6974 696f 6e5f 6b65 793d 5061 7274 6974  ition_key=Partit
-0001dd60: 696f 6e4b 6579 2870 6174 683d 222f 706b  ionKey(path="/pk
-0001dd70: 222c 206b 696e 643d 2248 6173 6822 292c  ", kind="Hash"),
-0001dd80: 200a 2020 2020 2320 2020 2020 2020 2020   .    #         
-0001dd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ddb0: 2020 2020 2020 2020 2020 2020 2072 6573               res
-0001ddc0: 706f 6e73 655f 686f 6f6b 3d63 7265 6174  ponse_hook=creat
-0001ddd0: 6564 5f72 6563 6f72 6465 7229 0a20 2020  ed_recorder).   
-0001dde0: 2023 2020 2020 2070 726f 7065 7274 6965   #     propertie
-0001ddf0: 7320 3d20 6372 6561 7465 645f 636f 6c6c  s = created_coll
-0001de00: 6563 7469 6f6e 2e72 6561 6428 290a 2020  ection.read().  
-0001de10: 2020 2320 2020 2020 7474 6c5f 6b65 7920    #     ttl_key 
-0001de20: 3d20 2261 6e61 6c79 7469 6361 6c53 746f  = "analyticalSto
-0001de30: 7261 6765 5474 6c22 0a20 2020 2023 2020  rageTtl".    #  
-0001de40: 2020 2073 656c 662e 6173 7365 7274 5472     self.assertTr
-0001de50: 7565 2874 746c 5f6b 6579 206e 6f74 2069  ue(ttl_key not i
-0001de60: 6e20 7072 6f70 6572 7469 6573 206f 7220  n properties or 
-0001de70: 7072 6f70 6572 7469 6573 5b74 746c 5f6b  properties[ttl_k
-0001de80: 6579 5d20 3d3d 204e 6f6e 6529 0a0a 2020  ey] == None)..  
-0001de90: 2020 2320 6465 6620 7465 7374 5f63 7265    # def test_cre
-0001dea0: 6174 655f 636f 6e74 6169 6e65 725f 7769  ate_container_wi
-0001deb0: 7468 5f61 6e61 6c79 7469 6361 6c5f 7374  th_analytical_st
-0001dec0: 6f72 655f 6f6e 2873 656c 6629 3a0a 2020  ore_on(self):.  
-0001ded0: 2020 2320 2020 2020 2320 646f 6e27 7420    #     # don't 
-0001dee0: 7275 6e20 7465 7374 2c20 666f 7220 7468  run test, for th
-0001def0: 6520 7469 6d65 2062 6569 6e67 2c20 6966  e time being, if
-0001df00: 2072 756e 6e69 6e67 2061 6761 696e 7374   running against
-0001df10: 2074 6865 2065 6d75 6c61 746f 720a 2020   the emulator.  
-0001df20: 2020 2320 2020 2020 6966 2027 6c6f 6361    #     if 'loca
-0001df30: 6c68 6f73 7427 2069 6e20 7365 6c66 2e68  lhost' in self.h
-0001df40: 6f73 7420 6f72 2027 3132 372e 302e 302e  ost or '127.0.0.
-0001df50: 3127 2069 6e20 7365 6c66 2e68 6f73 743a  1' in self.host:
-0001df60: 0a20 2020 2023 2020 2020 2020 2020 2072  .    #         r
-0001df70: 6574 7572 6e0a 0a20 2020 2023 2020 2020  eturn..    #    
-0001df80: 2063 7265 6174 6564 5f64 6220 3d20 7365   created_db = se
-0001df90: 6c66 2e64 6174 6162 6173 6546 6f72 5465  lf.databaseForTe
-0001dfa0: 7374 0a20 2020 2023 2020 2020 2063 6f6c  st.    #     col
-0001dfb0: 6c65 6374 696f 6e5f 6964 203d 2027 7465  lection_id = 'te
-0001dfc0: 7374 5f63 7265 6174 655f 636f 6e74 6169  st_create_contai
-0001dfd0: 6e65 725f 7769 7468 5f61 6e61 6c79 7469  ner_with_analyti
-0001dfe0: 6361 6c5f 7374 6f72 655f 6f6e 5f27 202b  cal_store_on_' +
-0001dff0: 2073 7472 2875 7569 642e 7575 6964 3428   str(uuid.uuid4(
-0001e000: 2929 0a20 2020 2023 2020 2020 2063 6f6c  )).    #     col
-0001e010: 6c65 6374 696f 6e5f 696e 6465 7869 6e67  lection_indexing
-0001e020: 5f70 6f6c 6963 7920 3d20 7b27 696e 6465  _policy = {'inde
-0001e030: 7869 6e67 4d6f 6465 273a 2027 636f 6e73  xingMode': 'cons
-0001e040: 6973 7465 6e74 277d 0a20 2020 2023 2020  istent'}.    #  
-0001e050: 2020 2063 7265 6174 6564 5f72 6563 6f72     created_recor
-0001e060: 6465 7220 3d20 5265 636f 7264 4469 6167  der = RecordDiag
-0001e070: 6e6f 7374 6963 7328 290a 2020 2020 2320  nostics().    # 
-0001e080: 2020 2020 6372 6561 7465 645f 636f 6c6c      created_coll
-0001e090: 6563 7469 6f6e 203d 2063 7265 6174 6564  ection = created
-0001e0a0: 5f64 622e 6372 6561 7465 5f63 6f6e 7461  _db.create_conta
-0001e0b0: 696e 6572 2869 643d 636f 6c6c 6563 7469  iner(id=collecti
-0001e0c0: 6f6e 5f69 642c 0a20 2020 2023 2020 2020  on_id,.    #    
-0001e0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e100: 2020 616e 616c 7974 6963 616c 5f73 746f    analytical_sto
-0001e110: 7261 6765 5f74 746c 3d2d 312c 0a20 2020  rage_ttl=-1,.   
-0001e120: 2023 2020 2020 2020 2020 2020 2020 2020   #              
-0001e130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e150: 2020 2020 2020 2020 696e 6465 7869 6e67          indexing
-0001e160: 5f70 6f6c 6963 793d 636f 6c6c 6563 7469  _policy=collecti
-0001e170: 6f6e 5f69 6e64 6578 696e 675f 706f 6c69  on_indexing_poli
-0001e180: 6379 2c0a 2020 2020 2320 2020 2020 2020  cy,.    #       
-0001e190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e1b0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-0001e1c0: 6172 7469 7469 6f6e 5f6b 6579 3d50 6172  artition_key=Par
-0001e1d0: 7469 7469 6f6e 4b65 7928 7061 7468 3d22  titionKey(path="
-0001e1e0: 2f70 6b22 2c20 6b69 6e64 3d22 4861 7368  /pk", kind="Hash
-0001e1f0: 2229 2c20 0a20 2020 2023 2020 2020 2020  "), .    #      
-0001e200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e230: 7265 7370 6f6e 7365 5f68 6f6f 6b3d 6372  response_hook=cr
-0001e240: 6561 7465 645f 7265 636f 7264 6572 290a  eated_recorder).
-0001e250: 2020 2020 2320 2020 2020 7072 6f70 6572      #     proper
-0001e260: 7469 6573 203d 2063 7265 6174 6564 5f63  ties = created_c
-0001e270: 6f6c 6c65 6374 696f 6e2e 7265 6164 2829  ollection.read()
-0001e280: 0a20 2020 2023 2020 2020 2074 746c 5f6b  .    #     ttl_k
-0001e290: 6579 203d 2022 616e 616c 7974 6963 616c  ey = "analytical
-0001e2a0: 5374 6f72 6167 6554 746c 220a 2020 2020  StorageTtl".    
-0001e2b0: 2320 2020 2020 7365 6c66 2e61 7373 6572  #     self.asser
-0001e2c0: 7454 7275 6528 7474 6c5f 6b65 7920 696e  tTrue(ttl_key in
-0001e2d0: 2070 726f 7065 7274 6965 7320 616e 6420   properties and 
-0001e2e0: 7072 6f70 6572 7469 6573 5b74 746c 5f6b  properties[ttl_k
-0001e2f0: 6579 5d20 3d3d 202d 3129 0a0a 2020 2020  ey] == -1)..    
-0001e300: 2320 6465 6620 7465 7374 5f63 7265 6174  # def test_creat
-0001e310: 655f 636f 6e74 6169 6e65 725f 6966 5f6e  e_container_if_n
-0001e320: 6f74 5f65 7869 7374 735f 7769 7468 5f61  ot_exists_with_a
-0001e330: 6e61 6c79 7469 6361 6c5f 7374 6f72 655f  nalytical_store_
-0001e340: 6f6e 2873 656c 6629 3a0a 2020 2020 2320  on(self):.    # 
-0001e350: 2020 2020 2320 646f 6e27 7420 7275 6e20      # don't run 
-0001e360: 7465 7374 2c20 666f 7220 7468 6520 7469  test, for the ti
-0001e370: 6d65 2062 6569 6e67 2c20 6966 2072 756e  me being, if run
-0001e380: 6e69 6e67 2061 6761 696e 7374 2074 6865  ning against the
-0001e390: 2065 6d75 6c61 746f 720a 2020 2020 2320   emulator.    # 
-0001e3a0: 2020 2020 6966 2027 6c6f 6361 6c68 6f73      if 'localhos
-0001e3b0: 7427 2069 6e20 7365 6c66 2e68 6f73 7420  t' in self.host 
-0001e3c0: 6f72 2027 3132 372e 302e 302e 3127 2069  or '127.0.0.1' i
-0001e3d0: 6e20 7365 6c66 2e68 6f73 743a 0a20 2020  n self.host:.   
-0001e3e0: 2023 2020 2020 2020 2020 2072 6574 7572   #         retur
-0001e3f0: 6e0a 0a20 2020 2023 2020 2020 2023 2066  n..    #     # f
-0001e400: 6972 7374 2c20 7472 7920 7768 656e 2077  irst, try when w
-0001e410: 6520 6b6e 6f77 2074 6865 2063 6f6e 7461  e know the conta
-0001e420: 696e 6572 2064 6f65 736e 2774 2065 7869  iner doesn't exi
-0001e430: 7374 2e0a 2020 2020 2320 2020 2020 6372  st..    #     cr
-0001e440: 6561 7465 645f 6462 203d 2073 656c 662e  eated_db = self.
-0001e450: 6461 7461 6261 7365 466f 7254 6573 740a  databaseForTest.
-0001e460: 2020 2020 2320 2020 2020 636f 6c6c 6563      #     collec
-0001e470: 7469 6f6e 5f69 6420 3d20 2774 6573 745f  tion_id = 'test_
-0001e480: 6372 6561 7465 5f63 6f6e 7461 696e 6572  create_container
-0001e490: 5f69 665f 6e6f 745f 6578 6973 7473 5f77  _if_not_exists_w
-0001e4a0: 6974 685f 616e 616c 7974 6963 616c 5f73  ith_analytical_s
-0001e4b0: 746f 7265 5f6f 6e5f 2720 2b20 7374 7228  tore_on_' + str(
-0001e4c0: 7575 6964 2e75 7569 6434 2829 290a 2020  uuid.uuid4()).  
-0001e4d0: 2020 2320 2020 2020 636f 6c6c 6563 7469    #     collecti
-0001e4e0: 6f6e 5f69 6e64 6578 696e 675f 706f 6c69  on_indexing_poli
-0001e4f0: 6379 203d 207b 2769 6e64 6578 696e 674d  cy = {'indexingM
-0001e500: 6f64 6527 3a20 2763 6f6e 7369 7374 656e  ode': 'consisten
-0001e510: 7427 7d0a 2020 2020 2320 2020 2020 6372  t'}.    #     cr
-0001e520: 6561 7465 645f 7265 636f 7264 6572 203d  eated_recorder =
-0001e530: 2052 6563 6f72 6444 6961 676e 6f73 7469   RecordDiagnosti
-0001e540: 6373 2829 0a20 2020 2023 2020 2020 2063  cs().    #     c
-0001e550: 7265 6174 6564 5f63 6f6c 6c65 6374 696f  reated_collectio
-0001e560: 6e20 3d20 6372 6561 7465 645f 6462 2e63  n = created_db.c
-0001e570: 7265 6174 655f 636f 6e74 6169 6e65 725f  reate_container_
-0001e580: 6966 5f6e 6f74 5f65 7869 7374 7328 6964  if_not_exists(id
-0001e590: 3d63 6f6c 6c65 6374 696f 6e5f 6964 2c0a  =collection_id,.
-0001e5a0: 2020 2020 2320 2020 2020 2020 2020 2020      #           
-0001e5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e5e0: 2020 2020 2020 2020 2061 6e61 6c79 7469           analyti
-0001e5f0: 6361 6c5f 7374 6f72 6167 655f 7474 6c3d  cal_storage_ttl=
-0001e600: 2d31 2c0a 2020 2020 2320 2020 2020 2020  -1,.    #       
-0001e610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e640: 2020 2020 2020 2020 2020 2020 2069 6e64               ind
-0001e650: 6578 696e 675f 706f 6c69 6379 3d63 6f6c  exing_policy=col
-0001e660: 6c65 6374 696f 6e5f 696e 6465 7869 6e67  lection_indexing
-0001e670: 5f70 6f6c 6963 792c 0a20 2020 2023 2020  _policy,.    #  
-0001e680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c660: 2020 2020 2320 436f 6d6d 656e 7469 6e67      # Commenting
+0001c670: 206f 7574 2064 656c 6574 6520 616c 6c20   out delete all 
+0001c680: 6974 656d 7320 6279 2070 6b20 756e 7469  items by pk unti
+0001c690: 6c20 7069 7065 6c69 6e65 7320 7375 7070  l pipelines supp
+0001c6a0: 6f72 7420 6974 0a20 2020 2023 2061 7379  ort it.    # asy
+0001c6b0: 6e63 2064 6566 2074 6573 745f 6465 6c65  nc def test_dele
+0001c6c0: 7465 5f61 6c6c 5f69 7465 6d73 5f62 795f  te_all_items_by_
+0001c6d0: 7061 7274 6974 696f 6e5f 6b65 7928 7365  partition_key(se
+0001c6e0: 6c66 293a 0a20 2020 2023 2020 2020 2023  lf):.    #     #
+0001c6f0: 2063 7265 6174 6520 6461 7461 6261 7365   create database
+0001c700: 0a20 2020 2023 2020 2020 2063 7265 6174  .    #     creat
+0001c710: 6564 5f64 6220 3d20 7365 6c66 2e64 6174  ed_db = self.dat
+0001c720: 6162 6173 6546 6f72 5465 7374 0a20 2020  abaseForTest.   
+0001c730: 2023 0a20 2020 2023 2020 2020 2023 2063   #.    #     # c
+0001c740: 7265 6174 6520 636f 6e74 6169 6e65 720a  reate container.
+0001c750: 2020 2020 2320 2020 2020 6372 6561 7465      #     create
+0001c760: 645f 636f 6c6c 6563 7469 6f6e 203d 2061  d_collection = a
+0001c770: 7761 6974 2063 7265 6174 6564 5f64 622e  wait created_db.
+0001c780: 6372 6561 7465 5f63 6f6e 7461 696e 6572  create_container
+0001c790: 280a 2020 2020 2320 2020 2020 2020 2020  (.    #         
+0001c7a0: 6964 3d27 7465 7374 5f64 656c 6574 655f  id='test_delete_
+0001c7b0: 616c 6c5f 6974 656d 735f 6279 5f70 6172  all_items_by_par
+0001c7c0: 7469 7469 6f6e 5f6b 6579 2027 202b 2073  tition_key ' + s
+0001c7d0: 7472 2875 7569 642e 7575 6964 3428 2929  tr(uuid.uuid4())
+0001c7e0: 2c0a 2020 2020 2320 2020 2020 2020 2020  ,.    #         
+0001c7f0: 7061 7274 6974 696f 6e5f 6b65 793d 5061  partition_key=Pa
+0001c800: 7274 6974 696f 6e4b 6579 2870 6174 683d  rtitionKey(path=
+0001c810: 272f 706b 272c 206b 696e 643d 2748 6173  '/pk', kind='Has
+0001c820: 6827 290a 2020 2020 2320 2020 2020 290a  h').    #     ).
+0001c830: 2020 2020 2320 2020 2020 2320 4372 6561      #     # Crea
+0001c840: 7465 2074 776f 2070 6172 7469 7469 6f6e  te two partition
+0001c850: 206b 6579 730a 2020 2020 2320 2020 2020   keys.    #     
+0001c860: 7061 7274 6974 696f 6e5f 6b65 7931 203d  partition_key1 =
+0001c870: 2022 7b7d 2d7b 7d22 2e66 6f72 6d61 7428   "{}-{}".format(
+0001c880: 2250 6172 7469 7469 6f6e 204b 6579 2031  "Partition Key 1
+0001c890: 222c 2073 7472 2875 7569 642e 7575 6964  ", str(uuid.uuid
+0001c8a0: 3428 2929 290a 2020 2020 2320 2020 2020  4())).    #     
+0001c8b0: 7061 7274 6974 696f 6e5f 6b65 7932 203d  partition_key2 =
+0001c8c0: 2022 7b7d 2d7b 7d22 2e66 6f72 6d61 7428   "{}-{}".format(
+0001c8d0: 2250 6172 7469 7469 6f6e 204b 6579 2032  "Partition Key 2
+0001c8e0: 222c 2073 7472 2875 7569 642e 7575 6964  ", str(uuid.uuid
+0001c8f0: 3428 2929 290a 2020 2020 230a 2020 2020  4())).    #.    
+0001c900: 2320 2020 2020 2320 6164 6420 6974 656d  #     # add item
+0001c910: 7320 666f 7220 7061 7274 6974 696f 6e20  s for partition 
+0001c920: 6b65 7920 310a 2020 2020 2320 2020 2020  key 1.    #     
+0001c930: 666f 7220 6920 696e 2072 616e 6765 2831  for i in range(1
+0001c940: 2c20 3329 3a0a 2020 2020 2320 2020 2020  , 3):.    #     
+0001c950: 2020 2020 6177 6169 7420 6372 6561 7465      await create
+0001c960: 645f 636f 6c6c 6563 7469 6f6e 2e75 7073  d_collection.ups
+0001c970: 6572 745f 6974 656d 280a 2020 2020 2320  ert_item(.    # 
+0001c980: 2020 2020 2020 2020 2020 2020 6469 6374              dict
+0001c990: 2869 643d 2269 7465 6d7b 7d22 2e66 6f72  (id="item{}".for
+0001c9a0: 6d61 7428 6929 2c20 706b 3d70 6172 7469  mat(i), pk=parti
+0001c9b0: 7469 6f6e 5f6b 6579 3129 0a20 2020 2023  tion_key1).    #
+0001c9c0: 2020 2020 2020 2020 2029 0a20 2020 2023           ).    #
+0001c9d0: 0a20 2020 2023 2020 2020 2023 2061 6464  .    #     # add
+0001c9e0: 2069 7465 6d73 2066 6f72 2070 6172 7469   items for parti
+0001c9f0: 7469 6f6e 206b 6579 2032 0a20 2020 2023  tion key 2.    #
+0001ca00: 2020 2020 2070 6b32 5f69 7465 6d20 3d20       pk2_item = 
+0001ca10: 6177 6169 7420 6372 6561 7465 645f 636f  await created_co
+0001ca20: 6c6c 6563 7469 6f6e 2e75 7073 6572 745f  llection.upsert_
+0001ca30: 6974 656d 2864 6963 7428 6964 3d22 6974  item(dict(id="it
+0001ca40: 656d 7b7d 222e 666f 726d 6174 2833 292c  em{}".format(3),
+0001ca50: 2070 6b3d 7061 7274 6974 696f 6e5f 6b65   pk=partition_ke
+0001ca60: 7932 2929 0a20 2020 2023 0a20 2020 2023  y2)).    #.    #
+0001ca70: 2020 2020 2023 2064 656c 6574 6520 616c       # delete al
+0001ca80: 6c20 6974 656d 7320 666f 7220 7061 7274  l items for part
+0001ca90: 6974 696f 6e20 6b65 7920 310a 2020 2020  ition key 1.    
+0001caa0: 2320 2020 2020 6177 6169 7420 6372 6561  #     await crea
+0001cab0: 7465 645f 636f 6c6c 6563 7469 6f6e 2e64  ted_collection.d
+0001cac0: 656c 6574 655f 616c 6c5f 6974 656d 735f  elete_all_items_
+0001cad0: 6279 5f70 6172 7469 7469 6f6e 5f6b 6579  by_partition_key
+0001cae0: 2870 6172 7469 7469 6f6e 5f6b 6579 3129  (partition_key1)
+0001caf0: 0a20 2020 2023 0a20 2020 2023 2020 2020  .    #.    #    
+0001cb00: 2023 2063 6865 636b 2074 6861 7420 6f6e   # check that on
+0001cb10: 6c79 2069 7465 6d73 2066 726f 6d20 7061  ly items from pa
+0001cb20: 7274 6974 696f 6e20 6b65 7920 3120 6861  rtition key 1 ha
+0001cb30: 7665 2062 6565 6e20 6465 6c65 7465 640a  ve been deleted.
+0001cb40: 2020 2020 2320 2020 2020 6974 656d 7320      #     items 
+0001cb50: 3d20 5b69 7465 6d20 6173 796e 6320 666f  = [item async fo
+0001cb60: 7220 6974 656d 2069 6e20 6372 6561 7465  r item in create
+0001cb70: 645f 636f 6c6c 6563 7469 6f6e 2e72 6561  d_collection.rea
+0001cb80: 645f 616c 6c5f 6974 656d 7328 295d 0a20  d_all_items()]. 
+0001cb90: 2020 2023 0a20 2020 2023 2020 2020 2023     #.    #     #
+0001cba0: 2069 7465 6d73 2073 686f 756c 6420 6f6e   items should on
+0001cbb0: 6c79 2068 6176 6520 3120 6974 656d 2c20  ly have 1 item, 
+0001cbc0: 616e 6420 6974 2073 686f 756c 6420 6571  and it should eq
+0001cbd0: 7561 6c20 706b 325f 6974 656d 0a20 2020  ual pk2_item.   
+0001cbe0: 2023 2020 2020 2073 656c 662e 6173 7365   #     self.asse
+0001cbf0: 7274 4469 6374 4571 7561 6c28 706b 325f  rtDictEqual(pk2_
+0001cc00: 6974 656d 2c20 6974 656d 735b 305d 290a  item, items[0]).
+0001cc10: 2020 2020 230a 2020 2020 2320 2020 2020      #.    #     
+0001cc20: 2320 6174 7465 6d70 7469 6e67 2074 6f20  # attempting to 
+0001cc30: 6465 6c65 7465 2061 206e 6f6e 2d65 7869  delete a non-exi
+0001cc40: 7374 656e 7420 7061 7274 6974 696f 6e20  stent partition 
+0001cc50: 6b65 7920 6f72 2070 6173 7369 6e67 206e  key or passing n
+0001cc60: 6f6e 6520 7368 6f75 6c64 206e 6f74 2064  one should not d
+0001cc70: 656c 6574 650a 2020 2020 2320 2020 2020  elete.    #     
+0001cc80: 2320 616e 7974 6869 6e67 2061 6e64 206c  # anything and l
+0001cc90: 6561 7665 2074 6869 6e67 7320 756e 6368  eave things unch
+0001cca0: 616e 6765 640a 2020 2020 2320 2020 2020  anged.    #     
+0001ccb0: 6177 6169 7420 6372 6561 7465 645f 636f  await created_co
+0001ccc0: 6c6c 6563 7469 6f6e 2e64 656c 6574 655f  llection.delete_
+0001ccd0: 616c 6c5f 6974 656d 735f 6279 5f70 6172  all_items_by_par
+0001cce0: 7469 7469 6f6e 5f6b 6579 284e 6f6e 6529  tition_key(None)
+0001ccf0: 0a20 2020 2023 0a20 2020 2023 2020 2020  .    #.    #    
+0001cd00: 2023 2063 6865 636b 2074 6861 7420 6e6f   # check that no
+0001cd10: 2063 6861 6e67 6573 2077 6572 6520 6d61   changes were ma
+0001cd20: 6465 2062 7920 6368 6563 6b69 6e67 2069  de by checking i
+0001cd30: 6620 7468 6520 6f6e 6c79 2069 7465 6d20  f the only item 
+0001cd40: 6973 2073 7469 6c6c 2074 6865 7265 0a20  is still there. 
+0001cd50: 2020 2023 2020 2020 2069 7465 6d73 203d     #     items =
+0001cd60: 205b 6974 656d 2061 7379 6e63 2066 6f72   [item async for
+0001cd70: 2069 7465 6d20 696e 2063 7265 6174 6564   item in created
+0001cd80: 5f63 6f6c 6c65 6374 696f 6e2e 7265 6164  _collection.read
+0001cd90: 5f61 6c6c 5f69 7465 6d73 2829 5d0a 2020  _all_items()].  
+0001cda0: 2020 230a 2020 2020 2320 2020 2020 2320    #.    #     # 
+0001cdb0: 6974 656d 7320 7368 6f75 6c64 206f 6e6c  items should onl
+0001cdc0: 7920 6861 7665 2031 2069 7465 6d2c 2061  y have 1 item, a
+0001cdd0: 6e64 2069 7420 7368 6f75 6c64 2065 7175  nd it should equ
+0001cde0: 616c 2070 6b32 5f69 7465 6d0a 2020 2020  al pk2_item.    
+0001cdf0: 2320 2020 2020 7365 6c66 2e61 7373 6572  #     self.asser
+0001ce00: 7444 6963 7445 7175 616c 2870 6b32 5f69  tDictEqual(pk2_i
+0001ce10: 7465 6d2c 2069 7465 6d73 5b30 5d29 0a20  tem, items[0]). 
+0001ce20: 2020 2023 0a20 2020 2023 2020 2020 2061     #.    #     a
+0001ce30: 7761 6974 2063 7265 6174 6564 5f64 622e  wait created_db.
+0001ce40: 6465 6c65 7465 5f63 6f6e 7461 696e 6572  delete_container
+0001ce50: 2863 7265 6174 6564 5f63 6f6c 6c65 6374  (created_collect
+0001ce60: 696f 6e29 0a0a 2020 2020 6173 796e 6320  ion)..    async 
+0001ce70: 6465 6620 7465 7374 5f70 6174 6368 5f6f  def test_patch_o
+0001ce80: 7065 7261 7469 6f6e 7328 7365 6c66 293a  perations(self):
+0001ce90: 0a20 2020 2020 2020 2063 7265 6174 6564  .        created
+0001cea0: 5f63 6f6e 7461 696e 6572 203d 2061 7761  _container = awa
+0001ceb0: 6974 2073 656c 662e 6461 7461 6261 7365  it self.database
+0001cec0: 466f 7254 6573 742e 6372 6561 7465 5f63  ForTest.create_c
+0001ced0: 6f6e 7461 696e 6572 5f69 665f 6e6f 745f  ontainer_if_not_
+0001cee0: 6578 6973 7473 2869 643d 2270 6174 6368  exists(id="patch
+0001cef0: 5f63 6f6e 7461 696e 6572 222c 2070 6172  _container", par
+0001cf00: 7469 7469 6f6e 5f6b 6579 3d50 6172 7469  tition_key=Parti
+0001cf10: 7469 6f6e 4b65 7928 7061 7468 3d22 2f70  tionKey(path="/p
+0001cf20: 6b22 2929 0a0a 2020 2020 2020 2020 2343  k"))..        #C
+0001cf30: 7265 6174 6520 6974 656d 2074 6f20 7061  reate item to pa
+0001cf40: 7463 680a 2020 2020 2020 2020 6974 656d  tch.        item
+0001cf50: 203d 207b 0a20 2020 2020 2020 2020 2020   = {.           
+0001cf60: 2022 6964 223a 2022 7061 7463 685f 6974   "id": "patch_it
+0001cf70: 656d 222c 0a20 2020 2020 2020 2020 2020  em",.           
+0001cf80: 2022 706b 223a 2022 7061 7463 685f 6974   "pk": "patch_it
+0001cf90: 656d 5f70 6b22 2c0a 2020 2020 2020 2020  em_pk",.        
+0001cfa0: 2020 2020 2270 726f 7022 3a20 2270 726f      "prop": "pro
+0001cfb0: 7031 222c 0a20 2020 2020 2020 2020 2020  p1",.           
+0001cfc0: 2022 6164 6472 6573 7322 3a20 7b0a 2020   "address": {.  
+0001cfd0: 2020 2020 2020 2020 2020 2020 2020 2263                "c
+0001cfe0: 6974 7922 3a20 2252 6564 6d6f 6e64 220a  ity": "Redmond".
+0001cff0: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
+0001d000: 2020 2020 2020 2020 2020 2022 636f 6d70             "comp
+0001d010: 616e 7922 3a20 224d 6963 726f 736f 6674  any": "Microsoft
+0001d020: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+0001d030: 6e75 6d62 6572 223a 2033 7d0a 2020 2020  number": 3}.    
+0001d040: 2020 2020 6177 6169 7420 6372 6561 7465      await create
+0001d050: 645f 636f 6e74 6169 6e65 722e 6372 6561  d_container.crea
+0001d060: 7465 5f69 7465 6d28 6974 656d 290a 2020  te_item(item).  
+0001d070: 2020 2020 2020 2344 6566 696e 6520 616e        #Define an
+0001d080: 6420 7275 6e20 7061 7463 6820 6f70 6572  d run patch oper
+0001d090: 6174 696f 6e73 0a20 2020 2020 2020 206f  ations.        o
+0001d0a0: 7065 7261 7469 6f6e 7320 3d20 5b0a 2020  perations = [.  
+0001d0b0: 2020 2020 2020 2020 2020 7b22 6f70 223a            {"op":
+0001d0c0: 2022 6164 6422 2c20 2270 6174 6822 3a20   "add", "path": 
+0001d0d0: 222f 636f 6c6f 7222 2c20 2276 616c 7565  "/color", "value
+0001d0e0: 223a 2022 7965 6c6c 6f77 227d 2c0a 2020  ": "yellow"},.  
+0001d0f0: 2020 2020 2020 2020 2020 7b22 6f70 223a            {"op":
+0001d100: 2022 7265 6d6f 7665 222c 2022 7061 7468   "remove", "path
+0001d110: 223a 2022 2f70 726f 7022 7d2c 0a20 2020  ": "/prop"},.   
+0001d120: 2020 2020 2020 2020 207b 226f 7022 3a20           {"op": 
+0001d130: 2272 6570 6c61 6365 222c 2022 7061 7468  "replace", "path
+0001d140: 223a 2022 2f63 6f6d 7061 6e79 222c 2022  ": "/company", "
+0001d150: 7661 6c75 6522 3a20 2243 6f73 6d6f 7344  value": "CosmosD
+0001d160: 4222 7d2c 0a20 2020 2020 2020 2020 2020  B"},.           
+0001d170: 207b 226f 7022 3a20 2273 6574 222c 2022   {"op": "set", "
+0001d180: 7061 7468 223a 2022 2f61 6464 7265 7373  path": "/address
+0001d190: 2f6e 6577 5f63 6974 7922 2c20 2276 616c  /new_city", "val
+0001d1a0: 7565 223a 2022 4174 6c61 6e74 6122 7d2c  ue": "Atlanta"},
+0001d1b0: 0a20 2020 2020 2020 2020 2020 207b 226f  .            {"o
+0001d1c0: 7022 3a20 2269 6e63 7222 2c20 2270 6174  p": "incr", "pat
+0001d1d0: 6822 3a20 222f 6e75 6d62 6572 222c 2022  h": "/number", "
+0001d1e0: 7661 6c75 6522 3a20 377d 2c0a 2020 2020  value": 7},.    
+0001d1f0: 2020 2020 2020 2020 7b22 6f70 223a 2022          {"op": "
+0001d200: 6d6f 7665 222c 2022 6672 6f6d 223a 2022  move", "from": "
+0001d210: 2f63 6f6c 6f72 222c 2022 7061 7468 223a  /color", "path":
+0001d220: 2022 2f66 6176 6f72 6974 655f 636f 6c6f   "/favorite_colo
+0001d230: 7222 7d0a 2020 2020 2020 2020 5d0a 2020  r"}.        ].  
+0001d240: 2020 2020 2020 7061 7463 6865 645f 6974        patched_it
+0001d250: 656d 203d 2061 7761 6974 2063 7265 6174  em = await creat
+0001d260: 6564 5f63 6f6e 7461 696e 6572 2e70 6174  ed_container.pat
+0001d270: 6368 5f69 7465 6d28 6974 656d 3d22 7061  ch_item(item="pa
+0001d280: 7463 685f 6974 656d 222c 2070 6172 7469  tch_item", parti
+0001d290: 7469 6f6e 5f6b 6579 3d22 7061 7463 685f  tion_key="patch_
+0001d2a0: 6974 656d 5f70 6b22 2c20 7061 7463 685f  item_pk", patch_
+0001d2b0: 6f70 6572 6174 696f 6e73 3d6f 7065 7261  operations=opera
+0001d2c0: 7469 6f6e 7329 0a20 2020 2020 2020 2023  tions).        #
+0001d2d0: 5665 7269 6679 2072 6573 756c 7473 2066  Verify results f
+0001d2e0: 726f 6d20 7061 7463 6820 6f70 6572 6174  rom patch operat
+0001d2f0: 696f 6e73 0a20 2020 2020 2020 2073 656c  ions.        sel
+0001d300: 662e 6173 7365 7274 5472 7565 2870 6174  f.assertTrue(pat
+0001d310: 6368 6564 5f69 7465 6d2e 6765 7428 2263  ched_item.get("c
+0001d320: 6f6c 6f72 2229 2069 7320 4e6f 6e65 290a  olor") is None).
+0001d330: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+0001d340: 6572 7454 7275 6528 7061 7463 6865 645f  ertTrue(patched_
+0001d350: 6974 656d 2e67 6574 2822 7072 6f70 2229  item.get("prop")
+0001d360: 2069 7320 4e6f 6e65 290a 2020 2020 2020   is None).      
+0001d370: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+0001d380: 616c 2870 6174 6368 6564 5f69 7465 6d2e  al(patched_item.
+0001d390: 6765 7428 2263 6f6d 7061 6e79 2229 2c20  get("company"), 
+0001d3a0: 2243 6f73 6d6f 7344 4222 290a 2020 2020  "CosmosDB").    
+0001d3b0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+0001d3c0: 7175 616c 2870 6174 6368 6564 5f69 7465  qual(patched_ite
+0001d3d0: 6d2e 6765 7428 2261 6464 7265 7373 2229  m.get("address")
+0001d3e0: 2e67 6574 2822 6e65 775f 6369 7479 2229  .get("new_city")
+0001d3f0: 2c20 2241 746c 616e 7461 2229 0a20 2020  , "Atlanta").   
+0001d400: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+0001d410: 4571 7561 6c28 7061 7463 6865 645f 6974  Equal(patched_it
+0001d420: 656d 2e67 6574 2822 6e75 6d62 6572 2229  em.get("number")
+0001d430: 2c20 3130 290a 2020 2020 2020 2020 7365  , 10).        se
+0001d440: 6c66 2e61 7373 6572 7445 7175 616c 2870  lf.assertEqual(p
+0001d450: 6174 6368 6564 5f69 7465 6d2e 6765 7428  atched_item.get(
+0001d460: 2266 6176 6f72 6974 655f 636f 6c6f 7222  "favorite_color"
+0001d470: 292c 2022 7965 6c6c 6f77 2229 0a0a 2020  ), "yellow")..  
+0001d480: 2020 2020 2020 234e 6567 6174 6976 6520        #Negative 
+0001d490: 7465 7374 202d 2061 7474 656d 7074 2074  test - attempt t
+0001d4a0: 6f20 7265 706c 6163 6520 6e6f 6e2d 6578  o replace non-ex
+0001d4b0: 6973 7465 6e74 2066 6965 6c64 0a20 2020  istent field.   
+0001d4c0: 2020 2020 206f 7065 7261 7469 6f6e 7320       operations 
+0001d4d0: 3d20 5b7b 226f 7022 3a20 2272 6570 6c61  = [{"op": "repla
+0001d4e0: 6365 222c 2022 7061 7468 223a 2022 2f77  ce", "path": "/w
+0001d4f0: 726f 6e67 5f66 6965 6c64 222c 2022 7661  rong_field", "va
+0001d500: 6c75 6522 3a20 2277 726f 6e67 5f76 616c  lue": "wrong_val
+0001d510: 7565 227d 5d0a 2020 2020 2020 2020 7472  ue"}].        tr
+0001d520: 793a 0a20 2020 2020 2020 2020 2020 2061  y:.            a
+0001d530: 7761 6974 2063 7265 6174 6564 5f63 6f6e  wait created_con
+0001d540: 7461 696e 6572 2e70 6174 6368 5f69 7465  tainer.patch_ite
+0001d550: 6d28 6974 656d 3d22 7061 7463 685f 6974  m(item="patch_it
+0001d560: 656d 222c 2070 6172 7469 7469 6f6e 5f6b  em", partition_k
+0001d570: 6579 3d22 7061 7463 685f 6974 656d 5f70  ey="patch_item_p
+0001d580: 6b22 2c20 7061 7463 685f 6f70 6572 6174  k", patch_operat
+0001d590: 696f 6e73 3d6f 7065 7261 7469 6f6e 7329  ions=operations)
+0001d5a0: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
+0001d5b0: 6578 6365 7074 696f 6e73 2e43 6f73 6d6f  exceptions.Cosmo
+0001d5c0: 7348 7474 7052 6573 706f 6e73 6545 7272  sHttpResponseErr
+0001d5d0: 6f72 2061 7320 653a 0a20 2020 2020 2020  or as e:.       
+0001d5e0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+0001d5f0: 4571 7561 6c28 652e 7374 6174 7573 5f63  Equal(e.status_c
+0001d600: 6f64 652c 2053 7461 7475 7343 6f64 6573  ode, StatusCodes
+0001d610: 2e42 4144 5f52 4551 5545 5354 290a 0a20  .BAD_REQUEST).. 
+0001d620: 2020 2020 2020 2023 4e65 6761 7469 7665         #Negative
+0001d630: 2074 6573 7420 2d20 6174 7465 6d70 7420   test - attempt 
+0001d640: 746f 2072 656d 6f76 6520 6e6f 6e2d 6578  to remove non-ex
+0001d650: 6973 7465 6e74 2066 6965 6c64 0a20 2020  istent field.   
+0001d660: 2020 2020 206f 7065 7261 7469 6f6e 7320       operations 
+0001d670: 3d20 5b7b 226f 7022 3a20 2272 656d 6f76  = [{"op": "remov
+0001d680: 6522 2c20 2270 6174 6822 3a20 222f 7772  e", "path": "/wr
+0001d690: 6f6e 675f 6669 656c 6422 7d5d 0a20 2020  ong_field"}].   
+0001d6a0: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+0001d6b0: 2020 2020 2020 6177 6169 7420 6372 6561        await crea
+0001d6c0: 7465 645f 636f 6e74 6169 6e65 722e 7061  ted_container.pa
+0001d6d0: 7463 685f 6974 656d 2869 7465 6d3d 2270  tch_item(item="p
+0001d6e0: 6174 6368 5f69 7465 6d22 2c20 7061 7274  atch_item", part
+0001d6f0: 6974 696f 6e5f 6b65 793d 2270 6174 6368  ition_key="patch
+0001d700: 5f69 7465 6d5f 706b 222c 2070 6174 6368  _item_pk", patch
+0001d710: 5f6f 7065 7261 7469 6f6e 733d 6f70 6572  _operations=oper
+0001d720: 6174 696f 6e73 290a 2020 2020 2020 2020  ations).        
+0001d730: 6578 6365 7074 2065 7863 6570 7469 6f6e  except exception
+0001d740: 732e 436f 736d 6f73 4874 7470 5265 7370  s.CosmosHttpResp
+0001d750: 6f6e 7365 4572 726f 7220 6173 2065 3a0a  onseError as e:.
+0001d760: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001d770: 2e61 7373 6572 7445 7175 616c 2865 2e73  .assertEqual(e.s
+0001d780: 7461 7475 735f 636f 6465 2c20 5374 6174  tatus_code, Stat
+0001d790: 7573 436f 6465 732e 4241 445f 5245 5155  usCodes.BAD_REQU
+0001d7a0: 4553 5429 0a0a 2020 2020 2020 2020 234e  EST)..        #N
+0001d7b0: 6567 6174 6976 6520 7465 7374 202d 2061  egative test - a
+0001d7c0: 7474 656d 7074 2074 6f20 696e 6372 656d  ttempt to increm
+0001d7d0: 656e 7420 6e6f 6e2d 6e75 6d62 6572 2066  ent non-number f
+0001d7e0: 6965 6c64 0a20 2020 2020 2020 206f 7065  ield.        ope
+0001d7f0: 7261 7469 6f6e 7320 3d20 5b7b 226f 7022  rations = [{"op"
+0001d800: 3a20 2269 6e63 7222 2c20 2270 6174 6822  : "incr", "path"
+0001d810: 3a20 222f 636f 6d70 616e 7922 2c20 2276  : "/company", "v
+0001d820: 616c 7565 223a 2033 7d5d 0a20 2020 2020  alue": 3}].     
+0001d830: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+0001d840: 2020 2020 6177 6169 7420 6372 6561 7465      await create
+0001d850: 645f 636f 6e74 6169 6e65 722e 7061 7463  d_container.patc
+0001d860: 685f 6974 656d 2869 7465 6d3d 2270 6174  h_item(item="pat
+0001d870: 6368 5f69 7465 6d22 2c20 7061 7274 6974  ch_item", partit
+0001d880: 696f 6e5f 6b65 793d 2270 6174 6368 5f69  ion_key="patch_i
+0001d890: 7465 6d5f 706b 222c 2070 6174 6368 5f6f  tem_pk", patch_o
+0001d8a0: 7065 7261 7469 6f6e 733d 6f70 6572 6174  perations=operat
+0001d8b0: 696f 6e73 290a 2020 2020 2020 2020 6578  ions).        ex
+0001d8c0: 6365 7074 2065 7863 6570 7469 6f6e 732e  cept exceptions.
+0001d8d0: 436f 736d 6f73 4874 7470 5265 7370 6f6e  CosmosHttpRespon
+0001d8e0: 7365 4572 726f 7220 6173 2065 3a0a 2020  seError as e:.  
+0001d8f0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+0001d900: 7373 6572 7445 7175 616c 2865 2e73 7461  ssertEqual(e.sta
+0001d910: 7475 735f 636f 6465 2c20 5374 6174 7573  tus_code, Status
+0001d920: 436f 6465 732e 4241 445f 5245 5155 4553  Codes.BAD_REQUES
+0001d930: 5429 0a0a 2020 2020 2020 2020 234e 6567  T)..        #Neg
+0001d940: 6174 6976 6520 7465 7374 202d 2061 7474  ative test - att
+0001d950: 656d 7074 2074 6f20 6d6f 7665 2066 726f  empt to move fro
+0001d960: 6d20 6e6f 6e2d 6578 6973 7465 6e74 2066  m non-existent f
+0001d970: 6965 6c64 0a20 2020 2020 2020 206f 7065  ield.        ope
+0001d980: 7261 7469 6f6e 7320 3d20 5b7b 226f 7022  rations = [{"op"
+0001d990: 3a20 226d 6f76 6522 2c20 2266 726f 6d22  : "move", "from"
+0001d9a0: 3a20 222f 7772 6f6e 675f 6669 656c 6422  : "/wrong_field"
+0001d9b0: 2c20 2270 6174 6822 3a20 222f 6f74 6865  , "path": "/othe
+0001d9c0: 725f 6669 656c 6422 7d5d 0a20 2020 2020  r_field"}].     
+0001d9d0: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+0001d9e0: 2020 2020 6177 6169 7420 6372 6561 7465      await create
+0001d9f0: 645f 636f 6e74 6169 6e65 722e 7061 7463  d_container.patc
+0001da00: 685f 6974 656d 2869 7465 6d3d 2270 6174  h_item(item="pat
+0001da10: 6368 5f69 7465 6d22 2c20 7061 7274 6974  ch_item", partit
+0001da20: 696f 6e5f 6b65 793d 2270 6174 6368 5f69  ion_key="patch_i
+0001da30: 7465 6d5f 706b 222c 2070 6174 6368 5f6f  tem_pk", patch_o
+0001da40: 7065 7261 7469 6f6e 733d 6f70 6572 6174  perations=operat
+0001da50: 696f 6e73 290a 2020 2020 2020 2020 6578  ions).        ex
+0001da60: 6365 7074 2065 7863 6570 7469 6f6e 732e  cept exceptions.
+0001da70: 436f 736d 6f73 4874 7470 5265 7370 6f6e  CosmosHttpRespon
+0001da80: 7365 4572 726f 7220 6173 2065 3a0a 2020  seError as e:.  
+0001da90: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+0001daa0: 7373 6572 7445 7175 616c 2865 2e73 7461  ssertEqual(e.sta
+0001dab0: 7475 735f 636f 6465 2c20 5374 6174 7573  tus_code, Status
+0001dac0: 436f 6465 732e 4241 445f 5245 5155 4553  Codes.BAD_REQUES
+0001dad0: 5429 0a0a 2020 2020 6173 796e 6320 6465  T)..    async de
+0001dae0: 6620 7465 7374 5f63 6f6e 6469 7469 6f6e  f test_condition
+0001daf0: 616c 5f70 6174 6368 696e 6728 7365 6c66  al_patching(self
+0001db00: 293a 0a20 2020 2020 2020 2063 7265 6174  ):.        creat
+0001db10: 6564 5f63 6f6e 7461 696e 6572 203d 2061  ed_container = a
+0001db20: 7761 6974 2073 656c 662e 6461 7461 6261  wait self.databa
+0001db30: 7365 466f 7254 6573 742e 6372 6561 7465  seForTest.create
+0001db40: 5f63 6f6e 7461 696e 6572 5f69 665f 6e6f  _container_if_no
+0001db50: 745f 6578 6973 7473 2869 643d 2270 6174  t_exists(id="pat
+0001db60: 6368 5f66 696c 7465 725f 636f 6e74 6169  ch_filter_contai
+0001db70: 6e65 7222 2c20 7061 7274 6974 696f 6e5f  ner", partition_
+0001db80: 6b65 793d 5061 7274 6974 696f 6e4b 6579  key=PartitionKey
+0001db90: 2870 6174 683d 222f 706b 2229 290a 2020  (path="/pk")).  
+0001dba0: 2020 2020 2020 2343 7265 6174 6520 6974        #Create it
+0001dbb0: 656d 2074 6f20 7061 7463 680a 2020 2020  em to patch.    
+0001dbc0: 2020 2020 6974 656d 203d 207b 0a20 2020      item = {.   
+0001dbd0: 2020 2020 2020 2020 2022 6964 223a 2022           "id": "
+0001dbe0: 636f 6e64 6974 696f 6e61 6c5f 7061 7463  conditional_patc
+0001dbf0: 685f 6974 656d 222c 0a20 2020 2020 2020  h_item",.       
+0001dc00: 2020 2020 2022 706b 223a 2022 7061 7463       "pk": "patc
+0001dc10: 685f 6974 656d 5f70 6b22 2c0a 2020 2020  h_item_pk",.    
+0001dc20: 2020 2020 2020 2020 2270 726f 7022 3a20          "prop": 
+0001dc30: 2270 726f 7031 222c 0a20 2020 2020 2020  "prop1",.       
+0001dc40: 2020 2020 2022 6164 6472 6573 7322 3a20       "address": 
+0001dc50: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+0001dc60: 2020 2263 6974 7922 3a20 2252 6564 6d6f    "city": "Redmo
+0001dc70: 6e64 220a 2020 2020 2020 2020 2020 2020  nd".            
+0001dc80: 7d2c 0a20 2020 2020 2020 2020 2020 2022  },.            "
+0001dc90: 636f 6d70 616e 7922 3a20 224d 6963 726f  company": "Micro
+0001dca0: 736f 6674 222c 0a20 2020 2020 2020 2020  soft",.         
+0001dcb0: 2020 2022 6e75 6d62 6572 223a 2033 7d0a     "number": 3}.
+0001dcc0: 2020 2020 2020 2020 6177 6169 7420 6372          await cr
+0001dcd0: 6561 7465 645f 636f 6e74 6169 6e65 722e  eated_container.
+0001dce0: 6372 6561 7465 5f69 7465 6d28 6974 656d  create_item(item
+0001dcf0: 290a 0a20 2020 2020 2020 2023 4465 6669  )..        #Defi
+0001dd00: 6e65 2070 6174 6368 206f 7065 7261 7469  ne patch operati
+0001dd10: 6f6e 730a 2020 2020 2020 2020 6f70 6572  ons.        oper
+0001dd20: 6174 696f 6e73 203d 205b 0a20 2020 2020  ations = [.     
+0001dd30: 2020 2020 2020 207b 226f 7022 3a20 2261         {"op": "a
+0001dd40: 6464 222c 2022 7061 7468 223a 2022 2f63  dd", "path": "/c
+0001dd50: 6f6c 6f72 222c 2022 7661 6c75 6522 3a20  olor", "value": 
+0001dd60: 2279 656c 6c6f 7722 7d2c 0a20 2020 2020  "yellow"},.     
+0001dd70: 2020 2020 2020 207b 226f 7022 3a20 2272         {"op": "r
+0001dd80: 656d 6f76 6522 2c20 2270 6174 6822 3a20  emove", "path": 
+0001dd90: 222f 7072 6f70 227d 2c0a 2020 2020 2020  "/prop"},.      
+0001dda0: 2020 2020 2020 7b22 6f70 223a 2022 7265        {"op": "re
+0001ddb0: 706c 6163 6522 2c20 2270 6174 6822 3a20  place", "path": 
+0001ddc0: 222f 636f 6d70 616e 7922 2c20 2276 616c  "/company", "val
+0001ddd0: 7565 223a 2022 436f 736d 6f73 4442 227d  ue": "CosmosDB"}
+0001dde0: 2c0a 2020 2020 2020 2020 2020 2020 7b22  ,.            {"
+0001ddf0: 6f70 223a 2022 7365 7422 2c20 2270 6174  op": "set", "pat
+0001de00: 6822 3a20 222f 6164 6472 6573 732f 6e65  h": "/address/ne
+0001de10: 775f 6369 7479 222c 2022 7661 6c75 6522  w_city", "value"
+0001de20: 3a20 2241 746c 616e 7461 227d 2c0a 2020  : "Atlanta"},.  
+0001de30: 2020 2020 2020 2020 2020 7b22 6f70 223a            {"op":
+0001de40: 2022 696e 6372 222c 2022 7061 7468 223a   "incr", "path":
+0001de50: 2022 2f6e 756d 6265 7222 2c20 2276 616c   "/number", "val
+0001de60: 7565 223a 2037 7d2c 0a20 2020 2020 2020  ue": 7},.       
+0001de70: 2020 2020 207b 226f 7022 3a20 226d 6f76       {"op": "mov
+0001de80: 6522 2c20 2266 726f 6d22 3a20 222f 636f  e", "from": "/co
+0001de90: 6c6f 7222 2c20 2270 6174 6822 3a20 222f  lor", "path": "/
+0001dea0: 6661 766f 7269 7465 5f63 6f6c 6f72 227d  favorite_color"}
+0001deb0: 0a20 2020 2020 2020 205d 0a0a 2020 2020  .        ]..    
+0001dec0: 2020 2020 2352 756e 2070 6174 6368 206f      #Run patch o
+0001ded0: 7065 7261 7469 6f6e 7320 7769 7468 2077  perations with w
+0001dee0: 726f 6e67 2066 696c 7465 720a 2020 2020  rong filter.    
+0001def0: 2020 2020 6e75 6d5f 6661 6c73 6520 3d20      num_false = 
+0001df00: 6974 656d 2e67 6574 2822 6e75 6d62 6572  item.get("number
+0001df10: 2229 202b 2031 0a20 2020 2020 2020 2066  ") + 1.        f
+0001df20: 696c 7465 725f 7072 6564 6963 6174 6520  ilter_predicate 
+0001df30: 3d20 2266 726f 6d20 726f 6f74 2077 6865  = "from root whe
+0001df40: 7265 2072 6f6f 742e 6e75 6d62 6572 203d  re root.number =
+0001df50: 2022 202b 2073 7472 286e 756d 5f66 616c   " + str(num_fal
+0001df60: 7365 290a 2020 2020 2020 2020 7472 793a  se).        try:
+0001df70: 0a20 2020 2020 2020 2020 2020 2061 7761  .            awa
+0001df80: 6974 2063 7265 6174 6564 5f63 6f6e 7461  it created_conta
+0001df90: 696e 6572 2e70 6174 6368 5f69 7465 6d28  iner.patch_item(
+0001dfa0: 6974 656d 3d22 636f 6e64 6974 696f 6e61  item="conditiona
+0001dfb0: 6c5f 7061 7463 685f 6974 656d 222c 2070  l_patch_item", p
+0001dfc0: 6172 7469 7469 6f6e 5f6b 6579 3d22 7061  artition_key="pa
+0001dfd0: 7463 685f 6974 656d 5f70 6b22 2c0a 2020  tch_item_pk",.  
+0001dfe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e000: 2020 2020 2020 2070 6174 6368 5f6f 7065         patch_ope
+0001e010: 7261 7469 6f6e 733d 6f70 6572 6174 696f  rations=operatio
+0001e020: 6e73 2c20 6669 6c74 6572 5f70 7265 6469  ns, filter_predi
+0001e030: 6361 7465 3d66 696c 7465 725f 7072 6564  cate=filter_pred
+0001e040: 6963 6174 6529 0a20 2020 2020 2020 2065  icate).        e
+0001e050: 7863 6570 7420 6578 6365 7074 696f 6e73  xcept exceptions
+0001e060: 2e43 6f73 6d6f 7348 7474 7052 6573 706f  .CosmosHttpRespo
+0001e070: 6e73 6545 7272 6f72 2061 7320 653a 0a20  nseError as e:. 
+0001e080: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0001e090: 6173 7365 7274 4571 7561 6c28 652e 7374  assertEqual(e.st
+0001e0a0: 6174 7573 5f63 6f64 652c 2053 7461 7475  atus_code, Statu
+0001e0b0: 7343 6f64 6573 2e50 5245 434f 4e44 4954  sCodes.PRECONDIT
+0001e0c0: 494f 4e5f 4641 494c 4544 290a 0a20 2020  ION_FAILED)..   
+0001e0d0: 2020 2020 2023 5275 6e20 7061 7463 6820       #Run patch 
+0001e0e0: 6f70 6572 6174 696f 6e73 2077 6974 6820  operations with 
+0001e0f0: 636f 7272 6563 7420 6669 6c74 6572 0a20  correct filter. 
+0001e100: 2020 2020 2020 2066 696c 7465 725f 7072         filter_pr
+0001e110: 6564 6963 6174 6520 3d20 2266 726f 6d20  edicate = "from 
+0001e120: 726f 6f74 2077 6865 7265 2072 6f6f 742e  root where root.
+0001e130: 6e75 6d62 6572 203d 2022 202b 2073 7472  number = " + str
+0001e140: 2869 7465 6d2e 6765 7428 226e 756d 6265  (item.get("numbe
+0001e150: 7222 2929 0a20 2020 2020 2020 2070 6174  r")).        pat
+0001e160: 6368 6564 5f69 7465 6d20 3d20 6177 6169  ched_item = awai
+0001e170: 7420 6372 6561 7465 645f 636f 6e74 6169  t created_contai
+0001e180: 6e65 722e 7061 7463 685f 6974 656d 2869  ner.patch_item(i
+0001e190: 7465 6d3d 2263 6f6e 6469 7469 6f6e 616c  tem="conditional
+0001e1a0: 5f70 6174 6368 5f69 7465 6d22 2c20 7061  _patch_item", pa
+0001e1b0: 7274 6974 696f 6e5f 6b65 793d 2270 6174  rtition_key="pat
+0001e1c0: 6368 5f69 7465 6d5f 706b 222c 0a20 2020  ch_item_pk",.   
+0001e1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e200: 2070 6174 6368 5f6f 7065 7261 7469 6f6e   patch_operation
+0001e210: 733d 6f70 6572 6174 696f 6e73 2c20 6669  s=operations, fi
+0001e220: 6c74 6572 5f70 7265 6469 6361 7465 3d66  lter_predicate=f
+0001e230: 696c 7465 725f 7072 6564 6963 6174 6529  ilter_predicate)
+0001e240: 0a20 2020 2020 2020 2023 5665 7269 6679  .        #Verify
+0001e250: 2072 6573 756c 7473 2066 726f 6d20 7061   results from pa
+0001e260: 7463 6820 6f70 6572 6174 696f 6e73 0a20  tch operations. 
+0001e270: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+0001e280: 7274 5472 7565 2870 6174 6368 6564 5f69  rtTrue(patched_i
+0001e290: 7465 6d2e 6765 7428 2263 6f6c 6f72 2229  tem.get("color")
+0001e2a0: 2069 7320 4e6f 6e65 290a 2020 2020 2020   is None).      
+0001e2b0: 2020 7365 6c66 2e61 7373 6572 7454 7275    self.assertTru
+0001e2c0: 6528 7061 7463 6865 645f 6974 656d 2e67  e(patched_item.g
+0001e2d0: 6574 2822 7072 6f70 2229 2069 7320 4e6f  et("prop") is No
+0001e2e0: 6e65 290a 2020 2020 2020 2020 7365 6c66  ne).        self
+0001e2f0: 2e61 7373 6572 7445 7175 616c 2870 6174  .assertEqual(pat
+0001e300: 6368 6564 5f69 7465 6d2e 6765 7428 2263  ched_item.get("c
+0001e310: 6f6d 7061 6e79 2229 2c20 2243 6f73 6d6f  ompany"), "Cosmo
+0001e320: 7344 4222 290a 2020 2020 2020 2020 7365  sDB").        se
+0001e330: 6c66 2e61 7373 6572 7445 7175 616c 2870  lf.assertEqual(p
+0001e340: 6174 6368 6564 5f69 7465 6d2e 6765 7428  atched_item.get(
+0001e350: 2261 6464 7265 7373 2229 2e67 6574 2822  "address").get("
+0001e360: 6e65 775f 6369 7479 2229 2c20 2241 746c  new_city"), "Atl
+0001e370: 616e 7461 2229 0a20 2020 2020 2020 2073  anta").        s
+0001e380: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+0001e390: 7061 7463 6865 645f 6974 656d 2e67 6574  patched_item.get
+0001e3a0: 2822 6e75 6d62 6572 2229 2c20 3130 290a  ("number"), 10).
+0001e3b0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+0001e3c0: 6572 7445 7175 616c 2870 6174 6368 6564  ertEqual(patched
+0001e3d0: 5f69 7465 6d2e 6765 7428 2266 6176 6f72  _item.get("favor
+0001e3e0: 6974 655f 636f 6c6f 7222 292c 2022 7965  ite_color"), "ye
+0001e3f0: 6c6c 6f77 2229 0a0a 2020 2020 2320 5465  llow")..    # Te
+0001e400: 6d70 6f72 6172 696c 7920 636f 6d6d 656e  mporarily commen
+0001e410: 7469 6e67 2061 6e61 6c79 7469 6361 6c20  ting analytical 
+0001e420: 7374 6f72 6167 6520 7465 7374 7320 756e  storage tests un
+0001e430: 7469 6c20 656d 756c 6174 6f72 2073 7570  til emulator sup
+0001e440: 706f 7274 2063 6f6d 6573 2e0a 2020 2020  port comes..    
+0001e450: 2320 6465 6620 7465 7374 5f63 7265 6174  # def test_creat
+0001e460: 655f 636f 6e74 6169 6e65 725f 7769 7468  e_container_with
+0001e470: 5f61 6e61 6c79 7469 6361 6c5f 7374 6f72  _analytical_stor
+0001e480: 655f 6f66 6628 7365 6c66 293a 0a20 2020  e_off(self):.   
+0001e490: 2023 2020 2020 2023 2064 6f6e 2774 2072   #     # don't r
+0001e4a0: 756e 2074 6573 742c 2066 6f72 2074 6865  un test, for the
+0001e4b0: 2074 696d 6520 6265 696e 672c 2069 6620   time being, if 
+0001e4c0: 7275 6e6e 696e 6720 6167 6169 6e73 7420  running against 
+0001e4d0: 7468 6520 656d 756c 6174 6f72 0a20 2020  the emulator.   
+0001e4e0: 2023 2020 2020 2069 6620 276c 6f63 616c   #     if 'local
+0001e4f0: 686f 7374 2720 696e 2073 656c 662e 686f  host' in self.ho
+0001e500: 7374 206f 7220 2731 3237 2e30 2e30 2e31  st or '127.0.0.1
+0001e510: 2720 696e 2073 656c 662e 686f 7374 3a0a  ' in self.host:.
+0001e520: 2020 2020 2320 2020 2020 2020 2020 7265      #         re
+0001e530: 7475 726e 0a0a 2020 2020 2320 2020 2020  turn..    #     
+0001e540: 6372 6561 7465 645f 6462 203d 2073 656c  created_db = sel
+0001e550: 662e 6461 7461 6261 7365 466f 7254 6573  f.databaseForTes
+0001e560: 740a 2020 2020 2320 2020 2020 636f 6c6c  t.    #     coll
+0001e570: 6563 7469 6f6e 5f69 6420 3d20 2774 6573  ection_id = 'tes
+0001e580: 745f 6372 6561 7465 5f63 6f6e 7461 696e  t_create_contain
+0001e590: 6572 5f77 6974 685f 616e 616c 7974 6963  er_with_analytic
+0001e5a0: 616c 5f73 746f 7265 5f6f 6666 5f27 202b  al_store_off_' +
+0001e5b0: 2073 7472 2875 7569 642e 7575 6964 3428   str(uuid.uuid4(
+0001e5c0: 2929 0a20 2020 2023 2020 2020 2063 6f6c  )).    #     col
+0001e5d0: 6c65 6374 696f 6e5f 696e 6465 7869 6e67  lection_indexing
+0001e5e0: 5f70 6f6c 6963 7920 3d20 7b27 696e 6465  _policy = {'inde
+0001e5f0: 7869 6e67 4d6f 6465 273a 2027 636f 6e73  xingMode': 'cons
+0001e600: 6973 7465 6e74 277d 0a20 2020 2023 2020  istent'}.    #  
+0001e610: 2020 2063 7265 6174 6564 5f72 6563 6f72     created_recor
+0001e620: 6465 7220 3d20 5265 636f 7264 4469 6167  der = RecordDiag
+0001e630: 6e6f 7374 6963 7328 290a 2020 2020 2320  nostics().    # 
+0001e640: 2020 2020 6372 6561 7465 645f 636f 6c6c      created_coll
+0001e650: 6563 7469 6f6e 203d 2063 7265 6174 6564  ection = created
+0001e660: 5f64 622e 6372 6561 7465 5f63 6f6e 7461  _db.create_conta
+0001e670: 696e 6572 2869 643d 636f 6c6c 6563 7469  iner(id=collecti
+0001e680: 6f6e 5f69 642c 0a20 2020 2023 2020 2020  on_id,.    #    
 0001e690: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001e6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001e6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e6c0: 2020 7061 7274 6974 696f 6e5f 6b65 793d    partition_key=
-0001e6d0: 5061 7274 6974 696f 6e4b 6579 2870 6174  PartitionKey(pat
-0001e6e0: 683d 222f 706b 222c 206b 696e 643d 2248  h="/pk", kind="H
-0001e6f0: 6173 6822 292c 0a20 2020 2023 2020 2020  ash"),.    #    
+0001e6c0: 2020 696e 6465 7869 6e67 5f70 6f6c 6963    indexing_polic
+0001e6d0: 793d 636f 6c6c 6563 7469 6f6e 5f69 6e64  y=collection_ind
+0001e6e0: 6578 696e 675f 706f 6c69 6379 2c0a 2020  exing_policy,.  
+0001e6f0: 2020 2320 2020 2020 2020 2020 2020 2020    #             
 0001e700: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001e710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e740: 7265 7370 6f6e 7365 5f68 6f6f 6b3d 6372  response_hook=cr
-0001e750: 6561 7465 645f 7265 636f 7264 6572 290a  eated_recorder).
-0001e760: 2020 2020 2320 2020 2020 7072 6f70 6572      #     proper
-0001e770: 7469 6573 203d 2063 7265 6174 6564 5f63  ties = created_c
-0001e780: 6f6c 6c65 6374 696f 6e2e 7265 6164 2829  ollection.read()
-0001e790: 0a20 2020 2023 2020 2020 2074 746c 5f6b  .    #     ttl_k
-0001e7a0: 6579 203d 2022 616e 616c 7974 6963 616c  ey = "analytical
-0001e7b0: 5374 6f72 6167 6554 746c 220a 2020 2020  StorageTtl".    
-0001e7c0: 2320 2020 2020 7365 6c66 2e61 7373 6572  #     self.asser
-0001e7d0: 7454 7275 6528 7474 6c5f 6b65 7920 696e  tTrue(ttl_key in
-0001e7e0: 2070 726f 7065 7274 6965 7320 616e 6420   properties and 
-0001e7f0: 7072 6f70 6572 7469 6573 5b74 746c 5f6b  properties[ttl_k
-0001e800: 6579 5d20 3d3d 202d 3129 0a0a 2020 2020  ey] == -1)..    
-0001e810: 2320 2020 2020 2320 6e65 7874 2c20 7472  #     # next, tr
-0001e820: 7920 7768 656e 2077 6520 6b6e 6f77 2074  y when we know t
-0001e830: 6865 2063 6f6e 7461 696e 6572 2044 4f45  he container DOE
-0001e840: 5320 6578 6973 742e 2054 6869 7320 7761  S exist. This wa
-0001e850: 7920 626f 7468 2063 6f64 6520 7061 7468  y both code path
-0001e860: 7320 6172 6520 7465 7374 6564 2e0a 2020  s are tested..  
-0001e870: 2020 2320 2020 2020 6372 6561 7465 645f    #     created_
-0001e880: 636f 6c6c 6563 7469 6f6e 203d 2063 7265  collection = cre
-0001e890: 6174 6564 5f64 622e 6372 6561 7465 5f63  ated_db.create_c
-0001e8a0: 6f6e 7461 696e 6572 5f69 665f 6e6f 745f  ontainer_if_not_
-0001e8b0: 6578 6973 7473 2869 643d 636f 6c6c 6563  exists(id=collec
-0001e8c0: 7469 6f6e 5f69 642c 0a20 2020 2023 2020  tion_id,.    #  
-0001e8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e910: 2020 616e 616c 7974 6963 616c 5f73 746f    analytical_sto
-0001e920: 7261 6765 5f74 746c 3d2d 312c 0a20 2020  rage_ttl=-1,.   
-0001e930: 2023 2020 2020 2020 2020 2020 2020 2020   #              
-0001e940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e970: 2020 2020 2020 696e 6465 7869 6e67 5f70        indexing_p
-0001e980: 6f6c 6963 793d 636f 6c6c 6563 7469 6f6e  olicy=collection
-0001e990: 5f69 6e64 6578 696e 675f 706f 6c69 6379  _indexing_policy
-0001e9a0: 2c0a 2020 2020 2320 2020 2020 2020 2020  ,.    #         
-0001e9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e9e0: 2020 2020 2020 2020 2020 2070 6172 7469             parti
-0001e9f0: 7469 6f6e 5f6b 6579 3d50 6172 7469 7469  tion_key=Partiti
-0001ea00: 6f6e 4b65 7928 7061 7468 3d22 2f70 6b22  onKey(path="/pk"
-0001ea10: 2c20 6b69 6e64 3d22 4861 7368 2229 2c0a  , kind="Hash"),.
-0001ea20: 2020 2020 2320 2020 2020 2020 2020 2020      #           
-0001ea30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ea40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ea50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ea60: 2020 2020 2020 2020 2072 6573 706f 6e73           respons
-0001ea70: 655f 686f 6f6b 3d63 7265 6174 6564 5f72  e_hook=created_r
-0001ea80: 6563 6f72 6465 7229 0a20 2020 2023 2020  ecorder).    #  
-0001ea90: 2020 2070 726f 7065 7274 6965 7320 3d20     properties = 
-0001eaa0: 6372 6561 7465 645f 636f 6c6c 6563 7469  created_collecti
-0001eab0: 6f6e 2e72 6561 6428 290a 2020 2020 2320  on.read().    # 
-0001eac0: 2020 2020 7474 6c5f 6b65 7920 3d20 2261      ttl_key = "a
-0001ead0: 6e61 6c79 7469 6361 6c53 746f 7261 6765  nalyticalStorage
-0001eae0: 5474 6c22 0a20 2020 2023 2020 2020 2073  Ttl".    #     s
-0001eaf0: 656c 662e 6173 7365 7274 5472 7565 2874  elf.assertTrue(t
-0001eb00: 746c 5f6b 6579 2069 6e20 7072 6f70 6572  tl_key in proper
-0001eb10: 7469 6573 2061 6e64 2070 726f 7065 7274  ties and propert
-0001eb20: 6965 735b 7474 6c5f 6b65 795d 203d 3d20  ies[ttl_key] == 
-0001eb30: 2d31 290a 0a20 2020 2061 7379 6e63 2064  -1)..    async d
-0001eb40: 6566 205f 4d6f 636b 4578 6563 7574 6546  ef _MockExecuteF
-0001eb50: 756e 6374 696f 6e28 7365 6c66 2c20 6675  unction(self, fu
-0001eb60: 6e63 7469 6f6e 2c20 2a61 7267 732c 202a  nction, *args, *
-0001eb70: 2a6b 7761 7267 7329 3a0a 2020 2020 2020  *kwargs):.      
-0001eb80: 2020 7365 6c66 2e6c 6173 745f 6865 6164    self.last_head
-0001eb90: 6572 732e 6170 7065 6e64 2861 7267 735b  ers.append(args[
-0001eba0: 345d 2e68 6561 6465 7273 5b48 7474 7048  4].headers[HttpH
-0001ebb0: 6561 6465 7273 2e50 6172 7469 7469 6f6e  eaders.Partition
-0001ebc0: 4b65 795d 0a20 2020 2020 2020 2020 2020  Key].           
-0001ebd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ebe0: 2020 2020 2020 6966 2048 7474 7048 6561        if HttpHea
-0001ebf0: 6465 7273 2e50 6172 7469 7469 6f6e 4b65  ders.PartitionKe
-0001ec00: 7920 696e 2061 7267 735b 345d 2e68 6561  y in args[4].hea
-0001ec10: 6465 7273 2065 6c73 6520 2727 290a 2020  ders else '').  
-0001ec20: 2020 2020 2020 7265 7475 726e 2061 7761        return awa
-0001ec30: 6974 2073 656c 662e 4f72 6967 696e 616c  it self.Original
-0001ec40: 4578 6563 7574 6546 756e 6374 696f 6e28  ExecuteFunction(
-0001ec50: 6675 6e63 7469 6f6e 2c20 2a61 7267 732c  function, *args,
-0001ec60: 202a 2a6b 7761 7267 7329 0a0a             **kwargs)..
+0001e720: 2020 2020 2020 2020 2070 6172 7469 7469           partiti
+0001e730: 6f6e 5f6b 6579 3d50 6172 7469 7469 6f6e  on_key=Partition
+0001e740: 4b65 7928 7061 7468 3d22 2f70 6b22 2c20  Key(path="/pk", 
+0001e750: 6b69 6e64 3d22 4861 7368 2229 2c20 0a20  kind="Hash"), . 
+0001e760: 2020 2023 2020 2020 2020 2020 2020 2020     #            
+0001e770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e790: 2020 2020 2020 2020 2020 7265 7370 6f6e            respon
+0001e7a0: 7365 5f68 6f6f 6b3d 6372 6561 7465 645f  se_hook=created_
+0001e7b0: 7265 636f 7264 6572 290a 2020 2020 2320  recorder).    # 
+0001e7c0: 2020 2020 7072 6f70 6572 7469 6573 203d      properties =
+0001e7d0: 2063 7265 6174 6564 5f63 6f6c 6c65 6374   created_collect
+0001e7e0: 696f 6e2e 7265 6164 2829 0a20 2020 2023  ion.read().    #
+0001e7f0: 2020 2020 2074 746c 5f6b 6579 203d 2022       ttl_key = "
+0001e800: 616e 616c 7974 6963 616c 5374 6f72 6167  analyticalStorag
+0001e810: 6554 746c 220a 2020 2020 2320 2020 2020  eTtl".    #     
+0001e820: 7365 6c66 2e61 7373 6572 7454 7275 6528  self.assertTrue(
+0001e830: 7474 6c5f 6b65 7920 6e6f 7420 696e 2070  ttl_key not in p
+0001e840: 726f 7065 7274 6965 7320 6f72 2070 726f  roperties or pro
+0001e850: 7065 7274 6965 735b 7474 6c5f 6b65 795d  perties[ttl_key]
+0001e860: 203d 3d20 4e6f 6e65 290a 0a20 2020 2023   == None)..    #
+0001e870: 2064 6566 2074 6573 745f 6372 6561 7465   def test_create
+0001e880: 5f63 6f6e 7461 696e 6572 5f77 6974 685f  _container_with_
+0001e890: 616e 616c 7974 6963 616c 5f73 746f 7265  analytical_store
+0001e8a0: 5f6f 6e28 7365 6c66 293a 0a20 2020 2023  _on(self):.    #
+0001e8b0: 2020 2020 2023 2064 6f6e 2774 2072 756e       # don't run
+0001e8c0: 2074 6573 742c 2066 6f72 2074 6865 2074   test, for the t
+0001e8d0: 696d 6520 6265 696e 672c 2069 6620 7275  ime being, if ru
+0001e8e0: 6e6e 696e 6720 6167 6169 6e73 7420 7468  nning against th
+0001e8f0: 6520 656d 756c 6174 6f72 0a20 2020 2023  e emulator.    #
+0001e900: 2020 2020 2069 6620 276c 6f63 616c 686f       if 'localho
+0001e910: 7374 2720 696e 2073 656c 662e 686f 7374  st' in self.host
+0001e920: 206f 7220 2731 3237 2e30 2e30 2e31 2720   or '127.0.0.1' 
+0001e930: 696e 2073 656c 662e 686f 7374 3a0a 2020  in self.host:.  
+0001e940: 2020 2320 2020 2020 2020 2020 7265 7475    #         retu
+0001e950: 726e 0a0a 2020 2020 2320 2020 2020 6372  rn..    #     cr
+0001e960: 6561 7465 645f 6462 203d 2073 656c 662e  eated_db = self.
+0001e970: 6461 7461 6261 7365 466f 7254 6573 740a  databaseForTest.
+0001e980: 2020 2020 2320 2020 2020 636f 6c6c 6563      #     collec
+0001e990: 7469 6f6e 5f69 6420 3d20 2774 6573 745f  tion_id = 'test_
+0001e9a0: 6372 6561 7465 5f63 6f6e 7461 696e 6572  create_container
+0001e9b0: 5f77 6974 685f 616e 616c 7974 6963 616c  _with_analytical
+0001e9c0: 5f73 746f 7265 5f6f 6e5f 2720 2b20 7374  _store_on_' + st
+0001e9d0: 7228 7575 6964 2e75 7569 6434 2829 290a  r(uuid.uuid4()).
+0001e9e0: 2020 2020 2320 2020 2020 636f 6c6c 6563      #     collec
+0001e9f0: 7469 6f6e 5f69 6e64 6578 696e 675f 706f  tion_indexing_po
+0001ea00: 6c69 6379 203d 207b 2769 6e64 6578 696e  licy = {'indexin
+0001ea10: 674d 6f64 6527 3a20 2763 6f6e 7369 7374  gMode': 'consist
+0001ea20: 656e 7427 7d0a 2020 2020 2320 2020 2020  ent'}.    #     
+0001ea30: 6372 6561 7465 645f 7265 636f 7264 6572  created_recorder
+0001ea40: 203d 2052 6563 6f72 6444 6961 676e 6f73   = RecordDiagnos
+0001ea50: 7469 6373 2829 0a20 2020 2023 2020 2020  tics().    #    
+0001ea60: 2063 7265 6174 6564 5f63 6f6c 6c65 6374   created_collect
+0001ea70: 696f 6e20 3d20 6372 6561 7465 645f 6462  ion = created_db
+0001ea80: 2e63 7265 6174 655f 636f 6e74 6169 6e65  .create_containe
+0001ea90: 7228 6964 3d63 6f6c 6c65 6374 696f 6e5f  r(id=collection_
+0001eaa0: 6964 2c0a 2020 2020 2320 2020 2020 2020  id,.    #       
+0001eab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001eac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ead0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+0001eae0: 6e61 6c79 7469 6361 6c5f 7374 6f72 6167  nalytical_storag
+0001eaf0: 655f 7474 6c3d 2d31 2c0a 2020 2020 2320  e_ttl=-1,.    # 
+0001eb00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001eb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001eb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001eb30: 2020 2020 2069 6e64 6578 696e 675f 706f       indexing_po
+0001eb40: 6c69 6379 3d63 6f6c 6c65 6374 696f 6e5f  licy=collection_
+0001eb50: 696e 6465 7869 6e67 5f70 6f6c 6963 792c  indexing_policy,
+0001eb60: 0a20 2020 2023 2020 2020 2020 2020 2020  .    #          
+0001eb70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001eb80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001eb90: 2020 2020 2020 2020 2020 2020 7061 7274              part
+0001eba0: 6974 696f 6e5f 6b65 793d 5061 7274 6974  ition_key=Partit
+0001ebb0: 696f 6e4b 6579 2870 6174 683d 222f 706b  ionKey(path="/pk
+0001ebc0: 222c 206b 696e 643d 2248 6173 6822 292c  ", kind="Hash"),
+0001ebd0: 200a 2020 2020 2320 2020 2020 2020 2020   .    #         
+0001ebe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ebf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ec00: 2020 2020 2020 2020 2020 2020 2072 6573               res
+0001ec10: 706f 6e73 655f 686f 6f6b 3d63 7265 6174  ponse_hook=creat
+0001ec20: 6564 5f72 6563 6f72 6465 7229 0a20 2020  ed_recorder).   
+0001ec30: 2023 2020 2020 2070 726f 7065 7274 6965   #     propertie
+0001ec40: 7320 3d20 6372 6561 7465 645f 636f 6c6c  s = created_coll
+0001ec50: 6563 7469 6f6e 2e72 6561 6428 290a 2020  ection.read().  
+0001ec60: 2020 2320 2020 2020 7474 6c5f 6b65 7920    #     ttl_key 
+0001ec70: 3d20 2261 6e61 6c79 7469 6361 6c53 746f  = "analyticalSto
+0001ec80: 7261 6765 5474 6c22 0a20 2020 2023 2020  rageTtl".    #  
+0001ec90: 2020 2073 656c 662e 6173 7365 7274 5472     self.assertTr
+0001eca0: 7565 2874 746c 5f6b 6579 2069 6e20 7072  ue(ttl_key in pr
+0001ecb0: 6f70 6572 7469 6573 2061 6e64 2070 726f  operties and pro
+0001ecc0: 7065 7274 6965 735b 7474 6c5f 6b65 795d  perties[ttl_key]
+0001ecd0: 203d 3d20 2d31 290a 0a20 2020 2023 2064   == -1)..    # d
+0001ece0: 6566 2074 6573 745f 6372 6561 7465 5f63  ef test_create_c
+0001ecf0: 6f6e 7461 696e 6572 5f69 665f 6e6f 745f  ontainer_if_not_
+0001ed00: 6578 6973 7473 5f77 6974 685f 616e 616c  exists_with_anal
+0001ed10: 7974 6963 616c 5f73 746f 7265 5f6f 6e28  ytical_store_on(
+0001ed20: 7365 6c66 293a 0a20 2020 2023 2020 2020  self):.    #    
+0001ed30: 2023 2064 6f6e 2774 2072 756e 2074 6573   # don't run tes
+0001ed40: 742c 2066 6f72 2074 6865 2074 696d 6520  t, for the time 
+0001ed50: 6265 696e 672c 2069 6620 7275 6e6e 696e  being, if runnin
+0001ed60: 6720 6167 6169 6e73 7420 7468 6520 656d  g against the em
+0001ed70: 756c 6174 6f72 0a20 2020 2023 2020 2020  ulator.    #    
+0001ed80: 2069 6620 276c 6f63 616c 686f 7374 2720   if 'localhost' 
+0001ed90: 696e 2073 656c 662e 686f 7374 206f 7220  in self.host or 
+0001eda0: 2731 3237 2e30 2e30 2e31 2720 696e 2073  '127.0.0.1' in s
+0001edb0: 656c 662e 686f 7374 3a0a 2020 2020 2320  elf.host:.    # 
+0001edc0: 2020 2020 2020 2020 7265 7475 726e 0a0a          return..
+0001edd0: 2020 2020 2320 2020 2020 2320 6669 7273      #     # firs
+0001ede0: 742c 2074 7279 2077 6865 6e20 7765 206b  t, try when we k
+0001edf0: 6e6f 7720 7468 6520 636f 6e74 6169 6e65  now the containe
+0001ee00: 7220 646f 6573 6e27 7420 6578 6973 742e  r doesn't exist.
+0001ee10: 0a20 2020 2023 2020 2020 2063 7265 6174  .    #     creat
+0001ee20: 6564 5f64 6220 3d20 7365 6c66 2e64 6174  ed_db = self.dat
+0001ee30: 6162 6173 6546 6f72 5465 7374 0a20 2020  abaseForTest.   
+0001ee40: 2023 2020 2020 2063 6f6c 6c65 6374 696f   #     collectio
+0001ee50: 6e5f 6964 203d 2027 7465 7374 5f63 7265  n_id = 'test_cre
+0001ee60: 6174 655f 636f 6e74 6169 6e65 725f 6966  ate_container_if
+0001ee70: 5f6e 6f74 5f65 7869 7374 735f 7769 7468  _not_exists_with
+0001ee80: 5f61 6e61 6c79 7469 6361 6c5f 7374 6f72  _analytical_stor
+0001ee90: 655f 6f6e 5f27 202b 2073 7472 2875 7569  e_on_' + str(uui
+0001eea0: 642e 7575 6964 3428 2929 0a20 2020 2023  d.uuid4()).    #
+0001eeb0: 2020 2020 2063 6f6c 6c65 6374 696f 6e5f       collection_
+0001eec0: 696e 6465 7869 6e67 5f70 6f6c 6963 7920  indexing_policy 
+0001eed0: 3d20 7b27 696e 6465 7869 6e67 4d6f 6465  = {'indexingMode
+0001eee0: 273a 2027 636f 6e73 6973 7465 6e74 277d  ': 'consistent'}
+0001eef0: 0a20 2020 2023 2020 2020 2063 7265 6174  .    #     creat
+0001ef00: 6564 5f72 6563 6f72 6465 7220 3d20 5265  ed_recorder = Re
+0001ef10: 636f 7264 4469 6167 6e6f 7374 6963 7328  cordDiagnostics(
+0001ef20: 290a 2020 2020 2320 2020 2020 6372 6561  ).    #     crea
+0001ef30: 7465 645f 636f 6c6c 6563 7469 6f6e 203d  ted_collection =
+0001ef40: 2063 7265 6174 6564 5f64 622e 6372 6561   created_db.crea
+0001ef50: 7465 5f63 6f6e 7461 696e 6572 5f69 665f  te_container_if_
+0001ef60: 6e6f 745f 6578 6973 7473 2869 643d 636f  not_exists(id=co
+0001ef70: 6c6c 6563 7469 6f6e 5f69 642c 0a20 2020  llection_id,.   
+0001ef80: 2023 2020 2020 2020 2020 2020 2020 2020   #              
+0001ef90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001efa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001efb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001efc0: 2020 2020 2020 616e 616c 7974 6963 616c        analytical
+0001efd0: 5f73 746f 7261 6765 5f74 746c 3d2d 312c  _storage_ttl=-1,
+0001efe0: 0a20 2020 2023 2020 2020 2020 2020 2020  .    #          
+0001eff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f020: 2020 2020 2020 2020 2020 696e 6465 7869            indexi
+0001f030: 6e67 5f70 6f6c 6963 793d 636f 6c6c 6563  ng_policy=collec
+0001f040: 7469 6f6e 5f69 6e64 6578 696e 675f 706f  tion_indexing_po
+0001f050: 6c69 6379 2c0a 2020 2020 2320 2020 2020  licy,.    #     
+0001f060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f090: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0001f0a0: 6172 7469 7469 6f6e 5f6b 6579 3d50 6172  artition_key=Par
+0001f0b0: 7469 7469 6f6e 4b65 7928 7061 7468 3d22  titionKey(path="
+0001f0c0: 2f70 6b22 2c20 6b69 6e64 3d22 4861 7368  /pk", kind="Hash
+0001f0d0: 2229 2c0a 2020 2020 2320 2020 2020 2020  "),.    #       
+0001f0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f110: 2020 2020 2020 2020 2020 2020 2072 6573               res
+0001f120: 706f 6e73 655f 686f 6f6b 3d63 7265 6174  ponse_hook=creat
+0001f130: 6564 5f72 6563 6f72 6465 7229 0a20 2020  ed_recorder).   
+0001f140: 2023 2020 2020 2070 726f 7065 7274 6965   #     propertie
+0001f150: 7320 3d20 6372 6561 7465 645f 636f 6c6c  s = created_coll
+0001f160: 6563 7469 6f6e 2e72 6561 6428 290a 2020  ection.read().  
+0001f170: 2020 2320 2020 2020 7474 6c5f 6b65 7920    #     ttl_key 
+0001f180: 3d20 2261 6e61 6c79 7469 6361 6c53 746f  = "analyticalSto
+0001f190: 7261 6765 5474 6c22 0a20 2020 2023 2020  rageTtl".    #  
+0001f1a0: 2020 2073 656c 662e 6173 7365 7274 5472     self.assertTr
+0001f1b0: 7565 2874 746c 5f6b 6579 2069 6e20 7072  ue(ttl_key in pr
+0001f1c0: 6f70 6572 7469 6573 2061 6e64 2070 726f  operties and pro
+0001f1d0: 7065 7274 6965 735b 7474 6c5f 6b65 795d  perties[ttl_key]
+0001f1e0: 203d 3d20 2d31 290a 0a20 2020 2023 2020   == -1)..    #  
+0001f1f0: 2020 2023 206e 6578 742c 2074 7279 2077     # next, try w
+0001f200: 6865 6e20 7765 206b 6e6f 7720 7468 6520  hen we know the 
+0001f210: 636f 6e74 6169 6e65 7220 444f 4553 2065  container DOES e
+0001f220: 7869 7374 2e20 5468 6973 2077 6179 2062  xist. This way b
+0001f230: 6f74 6820 636f 6465 2070 6174 6873 2061  oth code paths a
+0001f240: 7265 2074 6573 7465 642e 0a20 2020 2023  re tested..    #
+0001f250: 2020 2020 2063 7265 6174 6564 5f63 6f6c       created_col
+0001f260: 6c65 6374 696f 6e20 3d20 6372 6561 7465  lection = create
+0001f270: 645f 6462 2e63 7265 6174 655f 636f 6e74  d_db.create_cont
+0001f280: 6169 6e65 725f 6966 5f6e 6f74 5f65 7869  ainer_if_not_exi
+0001f290: 7374 7328 6964 3d63 6f6c 6c65 6374 696f  sts(id=collectio
+0001f2a0: 6e5f 6964 2c0a 2020 2020 2320 2020 2020  n_id,.    #     
+0001f2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f2e0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+0001f2f0: 6e61 6c79 7469 6361 6c5f 7374 6f72 6167  nalytical_storag
+0001f300: 655f 7474 6c3d 2d31 2c0a 2020 2020 2320  e_ttl=-1,.    # 
+0001f310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f350: 2020 2069 6e64 6578 696e 675f 706f 6c69     indexing_poli
+0001f360: 6379 3d63 6f6c 6c65 6374 696f 6e5f 696e  cy=collection_in
+0001f370: 6465 7869 6e67 5f70 6f6c 6963 792c 0a20  dexing_policy,. 
+0001f380: 2020 2023 2020 2020 2020 2020 2020 2020     #            
+0001f390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f3c0: 2020 2020 2020 2020 7061 7274 6974 696f          partitio
+0001f3d0: 6e5f 6b65 793d 5061 7274 6974 696f 6e4b  n_key=PartitionK
+0001f3e0: 6579 2870 6174 683d 222f 706b 222c 206b  ey(path="/pk", k
+0001f3f0: 696e 643d 2248 6173 6822 292c 0a20 2020  ind="Hash"),.   
+0001f400: 2023 2020 2020 2020 2020 2020 2020 2020   #              
+0001f410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f440: 2020 2020 2020 7265 7370 6f6e 7365 5f68        response_h
+0001f450: 6f6f 6b3d 6372 6561 7465 645f 7265 636f  ook=created_reco
+0001f460: 7264 6572 290a 2020 2020 2320 2020 2020  rder).    #     
+0001f470: 7072 6f70 6572 7469 6573 203d 2063 7265  properties = cre
+0001f480: 6174 6564 5f63 6f6c 6c65 6374 696f 6e2e  ated_collection.
+0001f490: 7265 6164 2829 0a20 2020 2023 2020 2020  read().    #    
+0001f4a0: 2074 746c 5f6b 6579 203d 2022 616e 616c   ttl_key = "anal
+0001f4b0: 7974 6963 616c 5374 6f72 6167 6554 746c  yticalStorageTtl
+0001f4c0: 220a 2020 2020 2320 2020 2020 7365 6c66  ".    #     self
+0001f4d0: 2e61 7373 6572 7454 7275 6528 7474 6c5f  .assertTrue(ttl_
+0001f4e0: 6b65 7920 696e 2070 726f 7065 7274 6965  key in propertie
+0001f4f0: 7320 616e 6420 7072 6f70 6572 7469 6573  s and properties
+0001f500: 5b74 746c 5f6b 6579 5d20 3d3d 202d 3129  [ttl_key] == -1)
+0001f510: 0a0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
+0001f520: 5f4d 6f63 6b45 7865 6375 7465 4675 6e63  _MockExecuteFunc
+0001f530: 7469 6f6e 2873 656c 662c 2066 756e 6374  tion(self, funct
+0001f540: 696f 6e2c 202a 6172 6773 2c20 2a2a 6b77  ion, *args, **kw
+0001f550: 6172 6773 293a 0a20 2020 2020 2020 2073  args):.        s
+0001f560: 656c 662e 6c61 7374 5f68 6561 6465 7273  elf.last_headers
+0001f570: 2e61 7070 656e 6428 6172 6773 5b34 5d2e  .append(args[4].
+0001f580: 6865 6164 6572 735b 4874 7470 4865 6164  headers[HttpHead
+0001f590: 6572 732e 5061 7274 6974 696f 6e4b 6579  ers.PartitionKey
+0001f5a0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+0001f5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f5c0: 2020 2069 6620 4874 7470 4865 6164 6572     if HttpHeader
+0001f5d0: 732e 5061 7274 6974 696f 6e4b 6579 2069  s.PartitionKey i
+0001f5e0: 6e20 6172 6773 5b34 5d2e 6865 6164 6572  n args[4].header
+0001f5f0: 7320 656c 7365 2027 2729 0a20 2020 2020  s else '').     
+0001f600: 2020 2072 6574 7572 6e20 6177 6169 7420     return await 
+0001f610: 7365 6c66 2e4f 7269 6769 6e61 6c45 7865  self.OriginalExe
+0001f620: 6375 7465 4675 6e63 7469 6f6e 2866 756e  cuteFunction(fun
+0001f630: 6374 696f 6e2c 202a 6172 6773 2c20 2a2a  ction, *args, **
+0001f640: 6b77 6172 6773 290a 0a                   kwargs)..
```

## Comparing `azure-cosmos-4.4.0b1/test/test_multimaster.py` & `azure-cosmos-4.4.0b2/test/test_multimaster.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/test/cleanup.py` & `azure-cosmos-4.4.0b2/test/cleanup.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/test/test_client_user_agent.py` & `azure-cosmos-4.4.0b2/test/test_client_user_agent.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/test/test_aggregate.py` & `azure-cosmos-4.4.0b2/test/test_aggregate.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/test/test_cosmos_http_logging_policy.py` & `azure-cosmos-4.4.0b2/test/test_cosmos_http_logging_policy.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/test/test_session_container.py` & `azure-cosmos-4.4.0b2/test/test_session_container.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/test/test_retry_policy.py` & `azure-cosmos-4.4.0b2/test/test_retry_policy.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/test/test_analytical_ttl_async.py` & `azure-cosmos-4.4.0b2/test/test_analytical_ttl_async.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/test/test_backwards_compatibility.py` & `azure-cosmos-4.4.0b2/test/test_backwards_compatibility.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/test/test_env.py` & `azure-cosmos-4.4.0b2/test/test_env.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/test/test_utils.py` & `azure-cosmos-4.4.0b2/test/test_utils.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/test/test_location_cache.py` & `azure-cosmos-4.4.0b2/test/test_location_cache.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/test/test_query_execution_context.py` & `azure-cosmos-4.4.0b2/test/test_query_execution_context.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/test/test_config.py` & `azure-cosmos-4.4.0b2/test/test_config.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/test/conftest.py` & `azure-cosmos-4.4.0b2/test/conftest.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/test/test_globaldb_mock.py` & `azure-cosmos-4.4.0b2/test/test_globaldb_mock.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/test/test_diagnostics.py` & `azure-cosmos-4.4.0b2/test/test_diagnostics.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/test/test_proxy.py` & `azure-cosmos-4.4.0b2/test/test_proxy.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/test/test_integrated_cache.py` & `azure-cosmos-4.4.0b2/test/test_integrated_cache.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/test/test_crud.py` & `azure-cosmos-4.4.0b2/test/test_crud.py`

 * *Files 1% similar despite different names*

```diff
@@ -6935,620 +6935,776 @@
 0001b160: 6564 5f75 7365 722e 6765 745f 7065 726d  ed_user.get_perm
 0001b170: 6973 7369 6f6e 2863 7265 6174 6564 5f70  ission(created_p
 0001b180: 6572 6d69 7373 696f 6e2e 7072 6f70 6572  ermission.proper
 0001b190: 7469 6573 290a 2020 2020 2020 2020 7365  ties).        se
 0001b1a0: 6c66 2e61 7373 6572 7445 7175 616c 2872  lf.assertEqual(r
 0001b1b0: 6561 645f 7065 726d 6973 7369 6f6e 2e69  ead_permission.i
 0001b1c0: 642c 2063 7265 6174 6564 5f70 6572 6d69  d, created_permi
-0001b1d0: 7373 696f 6e2e 6964 290a 0a20 2020 2064  ssion.id)..    d
-0001b1e0: 6566 2074 6573 745f 6465 6c65 7465 5f61  ef test_delete_a
-0001b1f0: 6c6c 5f69 7465 6d73 5f62 795f 7061 7274  ll_items_by_part
-0001b200: 6974 696f 6e5f 6b65 7928 7365 6c66 293a  ition_key(self):
-0001b210: 0a20 2020 2020 2020 2023 2063 7265 6174  .        # creat
-0001b220: 6520 6461 7461 6261 7365 0a20 2020 2020  e database.     
-0001b230: 2020 2063 7265 6174 6564 5f64 6220 3d20     created_db = 
-0001b240: 7365 6c66 2e64 6174 6162 6173 6546 6f72  self.databaseFor
-0001b250: 5465 7374 0a0a 2020 2020 2020 2020 2320  Test..        # 
-0001b260: 6372 6561 7465 2063 6f6e 7461 696e 6572  create container
-0001b270: 0a20 2020 2020 2020 2063 7265 6174 6564  .        created
-0001b280: 5f63 6f6c 6c65 6374 696f 6e20 3d20 6372  _collection = cr
-0001b290: 6561 7465 645f 6462 2e63 7265 6174 655f  eated_db.create_
-0001b2a0: 636f 6e74 6169 6e65 7228 0a20 2020 2020  container(.     
-0001b2b0: 2020 2020 2020 2069 643d 2774 6573 745f         id='test_
-0001b2c0: 6465 6c65 7465 5f61 6c6c 5f69 7465 6d73  delete_all_items
-0001b2d0: 5f62 795f 7061 7274 6974 696f 6e5f 6b65  _by_partition_ke
-0001b2e0: 7920 2720 2b20 7374 7228 7575 6964 2e75  y ' + str(uuid.u
-0001b2f0: 7569 6434 2829 292c 0a20 2020 2020 2020  uid4()),.       
-0001b300: 2020 2020 2070 6172 7469 7469 6f6e 5f6b       partition_k
-0001b310: 6579 3d50 6172 7469 7469 6f6e 4b65 7928  ey=PartitionKey(
-0001b320: 7061 7468 3d27 2f70 6b27 2c20 6b69 6e64  path='/pk', kind
-0001b330: 3d27 4861 7368 2729 0a20 2020 2020 2020  ='Hash').       
-0001b340: 2029 0a20 2020 2020 2020 2023 2043 7265   ).        # Cre
-0001b350: 6174 6520 7477 6f20 7061 7274 6974 696f  ate two partitio
-0001b360: 6e20 6b65 7973 0a20 2020 2020 2020 2070  n keys.        p
-0001b370: 6172 7469 7469 6f6e 5f6b 6579 3120 3d20  artition_key1 = 
-0001b380: 227b 7d2d 7b7d 222e 666f 726d 6174 2822  "{}-{}".format("
-0001b390: 5061 7274 6974 696f 6e20 4b65 7920 3122  Partition Key 1"
-0001b3a0: 2c20 7374 7228 7575 6964 2e75 7569 6434  , str(uuid.uuid4
-0001b3b0: 2829 2929 0a20 2020 2020 2020 2070 6172  ())).        par
-0001b3c0: 7469 7469 6f6e 5f6b 6579 3220 3d20 227b  tition_key2 = "{
-0001b3d0: 7d2d 7b7d 222e 666f 726d 6174 2822 5061  }-{}".format("Pa
-0001b3e0: 7274 6974 696f 6e20 4b65 7920 3222 2c20  rtition Key 2", 
-0001b3f0: 7374 7228 7575 6964 2e75 7569 6434 2829  str(uuid.uuid4()
-0001b400: 2929 0a0a 2020 2020 2020 2020 2320 6164  ))..        # ad
-0001b410: 6420 6974 656d 7320 666f 7220 7061 7274  d items for part
-0001b420: 6974 696f 6e20 6b65 7920 310a 2020 2020  ition key 1.    
-0001b430: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-0001b440: 6765 2831 2c20 3329 3a0a 2020 2020 2020  ge(1, 3):.      
-0001b450: 2020 2020 2020 6372 6561 7465 645f 636f        created_co
-0001b460: 6c6c 6563 7469 6f6e 2e75 7073 6572 745f  llection.upsert_
-0001b470: 6974 656d 280a 2020 2020 2020 2020 2020  item(.          
-0001b480: 2020 2020 2020 6469 6374 2869 643d 2269        dict(id="i
-0001b490: 7465 6d7b 7d22 2e66 6f72 6d61 7428 6929  tem{}".format(i)
-0001b4a0: 2c20 706b 3d70 6172 7469 7469 6f6e 5f6b  , pk=partition_k
-0001b4b0: 6579 3129 0a20 2020 2020 2020 2020 2020  ey1).           
-0001b4c0: 2029 0a0a 2020 2020 2020 2020 2320 6164   )..        # ad
-0001b4d0: 6420 6974 656d 7320 666f 7220 7061 7274  d items for part
-0001b4e0: 6974 696f 6e20 6b65 7920 320a 0a20 2020  ition key 2..   
-0001b4f0: 2020 2020 2070 6b32 5f69 7465 6d20 3d20       pk2_item = 
-0001b500: 6372 6561 7465 645f 636f 6c6c 6563 7469  created_collecti
-0001b510: 6f6e 2e75 7073 6572 745f 6974 656d 2864  on.upsert_item(d
-0001b520: 6963 7428 6964 3d22 6974 656d 7b7d 222e  ict(id="item{}".
-0001b530: 666f 726d 6174 2833 292c 2070 6b3d 7061  format(3), pk=pa
-0001b540: 7274 6974 696f 6e5f 6b65 7932 2929 0a0a  rtition_key2))..
-0001b550: 2020 2020 2020 2020 2320 6465 6c65 7465          # delete
-0001b560: 2061 6c6c 2069 7465 6d73 2066 6f72 2070   all items for p
-0001b570: 6172 7469 7469 6f6e 206b 6579 2031 0a20  artition key 1. 
-0001b580: 2020 2020 2020 2063 7265 6174 6564 5f63         created_c
-0001b590: 6f6c 6c65 6374 696f 6e2e 6465 6c65 7465  ollection.delete
-0001b5a0: 5f61 6c6c 5f69 7465 6d73 5f62 795f 7061  _all_items_by_pa
-0001b5b0: 7274 6974 696f 6e5f 6b65 7928 7061 7274  rtition_key(part
-0001b5c0: 6974 696f 6e5f 6b65 7931 290a 0a20 2020  ition_key1)..   
-0001b5d0: 2020 2020 2023 2063 6865 636b 2074 6861       # check tha
-0001b5e0: 7420 6f6e 6c79 2069 7465 6d73 2066 726f  t only items fro
-0001b5f0: 6d20 7061 7274 6974 696f 6e20 6b65 7920  m partition key 
-0001b600: 3120 6861 7665 2062 6565 6e20 6465 6c65  1 have been dele
-0001b610: 7465 640a 2020 2020 2020 2020 6974 656d  ted.        item
-0001b620: 7320 3d20 6c69 7374 2863 7265 6174 6564  s = list(created
-0001b630: 5f63 6f6c 6c65 6374 696f 6e2e 7265 6164  _collection.read
-0001b640: 5f61 6c6c 5f69 7465 6d73 2829 290a 0a20  _all_items()).. 
-0001b650: 2020 2020 2020 2023 2069 7465 6d73 2073         # items s
-0001b660: 686f 756c 6420 6f6e 6c79 2068 6176 6520  hould only have 
-0001b670: 3120 6974 656d 2061 6e64 2069 7420 7368  1 item and it sh
-0001b680: 6f75 6c64 2065 7175 616c 2070 6b32 5f69  ould equal pk2_i
-0001b690: 7465 6d0a 2020 2020 2020 2020 7365 6c66  tem.        self
-0001b6a0: 2e61 7373 6572 7444 6963 7445 7175 616c  .assertDictEqual
-0001b6b0: 2870 6b32 5f69 7465 6d2c 2069 7465 6d73  (pk2_item, items
-0001b6c0: 5b30 5d29 0a0a 2020 2020 2020 2020 2320  [0])..        # 
-0001b6d0: 6174 7465 6d70 7469 6e67 2074 6f20 6465  attempting to de
-0001b6e0: 6c65 7465 2061 206e 6f6e 2d65 7869 7374  lete a non-exist
-0001b6f0: 656e 7420 7061 7274 6974 696f 6e20 6b65  ent partition ke
-0001b700: 7920 6f72 2070 6173 7369 6e67 206e 6f6e  y or passing non
-0001b710: 6520 7368 6f75 6c64 206e 6f74 2064 656c  e should not del
-0001b720: 6574 650a 2020 2020 2020 2020 2320 616e  ete.        # an
-0001b730: 7974 6869 6e67 2061 6e64 206c 6561 7665  ything and leave
-0001b740: 2074 6869 6e67 7320 756e 6368 616e 6765   things unchange
-0001b750: 640a 2020 2020 2020 2020 6372 6561 7465  d.        create
-0001b760: 645f 636f 6c6c 6563 7469 6f6e 2e64 656c  d_collection.del
-0001b770: 6574 655f 616c 6c5f 6974 656d 735f 6279  ete_all_items_by
-0001b780: 5f70 6172 7469 7469 6f6e 5f6b 6579 284e  _partition_key(N
-0001b790: 6f6e 6529 0a0a 2020 2020 2020 2020 2320  one)..        # 
-0001b7a0: 6368 6563 6b20 7468 6174 206e 6f20 6368  check that no ch
-0001b7b0: 616e 6765 7320 7765 7265 206d 6164 6520  anges were made 
-0001b7c0: 6279 2063 6865 636b 696e 6720 6966 2074  by checking if t
-0001b7d0: 6865 206f 6e6c 7920 6974 656d 2069 7320  he only item is 
-0001b7e0: 7374 696c 6c20 7468 6572 650a 2020 2020  still there.    
-0001b7f0: 2020 2020 6974 656d 7320 3d20 6c69 7374      items = list
-0001b800: 2863 7265 6174 6564 5f63 6f6c 6c65 6374  (created_collect
-0001b810: 696f 6e2e 7265 6164 5f61 6c6c 5f69 7465  ion.read_all_ite
-0001b820: 6d73 2829 290a 0a20 2020 2020 2020 2023  ms())..        #
-0001b830: 2069 7465 6d73 2073 686f 756c 6420 6f6e   items should on
-0001b840: 6c79 2068 6176 6520 3120 6974 656d 2061  ly have 1 item a
-0001b850: 6e64 2069 7420 7368 6f75 6c64 2065 7175  nd it should equ
-0001b860: 616c 2070 6b32 5f69 7465 6d0a 2020 2020  al pk2_item.    
-0001b870: 2020 2020 7365 6c66 2e61 7373 6572 7444      self.assertD
-0001b880: 6963 7445 7175 616c 2870 6b32 5f69 7465  ictEqual(pk2_ite
-0001b890: 6d2c 2069 7465 6d73 5b30 5d29 0a0a 2020  m, items[0])..  
-0001b8a0: 2020 2020 2020 6372 6561 7465 645f 6462        created_db
-0001b8b0: 2e64 656c 6574 655f 636f 6e74 6169 6e65  .delete_containe
-0001b8c0: 7228 6372 6561 7465 645f 636f 6c6c 6563  r(created_collec
-0001b8d0: 7469 6f6e 290a 0a20 2020 2064 6566 2074  tion)..    def t
-0001b8e0: 6573 745f 7061 7463 685f 6f70 6572 6174  est_patch_operat
-0001b8f0: 696f 6e73 2873 656c 6629 3a0a 2020 2020  ions(self):.    
-0001b900: 2020 2020 6372 6561 7465 645f 636f 6e74      created_cont
-0001b910: 6169 6e65 7220 3d20 7365 6c66 2e64 6174  ainer = self.dat
-0001b920: 6162 6173 6546 6f72 5465 7374 2e63 7265  abaseForTest.cre
-0001b930: 6174 655f 636f 6e74 6169 6e65 725f 6966  ate_container_if
-0001b940: 5f6e 6f74 5f65 7869 7374 7328 6964 3d22  _not_exists(id="
-0001b950: 7061 7463 685f 636f 6e74 6169 6e65 7222  patch_container"
-0001b960: 2c20 7061 7274 6974 696f 6e5f 6b65 793d  , partition_key=
-0001b970: 5061 7274 6974 696f 6e4b 6579 2870 6174  PartitionKey(pat
-0001b980: 683d 222f 706b 2229 290a 0a20 2020 2020  h="/pk"))..     
-0001b990: 2020 2023 4372 6561 7465 2069 7465 6d20     #Create item 
-0001b9a0: 746f 2070 6174 6368 0a20 2020 2020 2020  to patch.       
-0001b9b0: 2069 7465 6d20 3d20 7b0a 2020 2020 2020   item = {.      
-0001b9c0: 2020 2020 2020 2269 6422 3a20 2270 6174        "id": "pat
-0001b9d0: 6368 5f69 7465 6d22 2c0a 2020 2020 2020  ch_item",.      
-0001b9e0: 2020 2020 2020 2270 6b22 3a20 2270 6174        "pk": "pat
-0001b9f0: 6368 5f69 7465 6d5f 706b 222c 0a20 2020  ch_item_pk",.   
-0001ba00: 2020 2020 2020 2020 2022 7072 6f70 223a           "prop":
-0001ba10: 2022 7072 6f70 3122 2c0a 2020 2020 2020   "prop1",.      
-0001ba20: 2020 2020 2020 2261 6464 7265 7373 223a        "address":
-0001ba30: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-0001ba40: 2020 2022 6369 7479 223a 2022 5265 646d     "city": "Redm
-0001ba50: 6f6e 6422 0a20 2020 2020 2020 2020 2020  ond".           
-0001ba60: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
-0001ba70: 2263 6f6d 7061 6e79 223a 2022 4d69 6372  "company": "Micr
-0001ba80: 6f73 6f66 7422 2c0a 2020 2020 2020 2020  osoft",.        
-0001ba90: 2020 2020 226e 756d 6265 7222 3a20 337d      "number": 3}
-0001baa0: 0a20 2020 2020 2020 2063 7265 6174 6564  .        created
-0001bab0: 5f63 6f6e 7461 696e 6572 2e63 7265 6174  _container.creat
-0001bac0: 655f 6974 656d 2869 7465 6d29 0a20 2020  e_item(item).   
-0001bad0: 2020 2020 2023 4465 6669 6e65 2061 6e64       #Define and
-0001bae0: 2072 756e 2070 6174 6368 206f 7065 7261   run patch opera
-0001baf0: 7469 6f6e 730a 2020 2020 2020 2020 6f70  tions.        op
-0001bb00: 6572 6174 696f 6e73 203d 205b 0a20 2020  erations = [.   
-0001bb10: 2020 2020 2020 2020 207b 226f 7022 3a20           {"op": 
-0001bb20: 2261 6464 222c 2022 7061 7468 223a 2022  "add", "path": "
-0001bb30: 2f63 6f6c 6f72 222c 2022 7661 6c75 6522  /color", "value"
-0001bb40: 3a20 2279 656c 6c6f 7722 7d2c 0a20 2020  : "yellow"},.   
-0001bb50: 2020 2020 2020 2020 207b 226f 7022 3a20           {"op": 
-0001bb60: 2272 656d 6f76 6522 2c20 2270 6174 6822  "remove", "path"
-0001bb70: 3a20 222f 7072 6f70 227d 2c0a 2020 2020  : "/prop"},.    
-0001bb80: 2020 2020 2020 2020 7b22 6f70 223a 2022          {"op": "
-0001bb90: 7265 706c 6163 6522 2c20 2270 6174 6822  replace", "path"
-0001bba0: 3a20 222f 636f 6d70 616e 7922 2c20 2276  : "/company", "v
-0001bbb0: 616c 7565 223a 2022 436f 736d 6f73 4442  alue": "CosmosDB
-0001bbc0: 227d 2c0a 2020 2020 2020 2020 2020 2020  "},.            
-0001bbd0: 7b22 6f70 223a 2022 7365 7422 2c20 2270  {"op": "set", "p
-0001bbe0: 6174 6822 3a20 222f 6164 6472 6573 732f  ath": "/address/
-0001bbf0: 6e65 775f 6369 7479 222c 2022 7661 6c75  new_city", "valu
-0001bc00: 6522 3a20 2241 746c 616e 7461 227d 2c0a  e": "Atlanta"},.
-0001bc10: 2020 2020 2020 2020 2020 2020 7b22 6f70              {"op
-0001bc20: 223a 2022 696e 6372 222c 2022 7061 7468  ": "incr", "path
-0001bc30: 223a 2022 2f6e 756d 6265 7222 2c20 2276  ": "/number", "v
-0001bc40: 616c 7565 223a 2037 7d2c 0a20 2020 2020  alue": 7},.     
-0001bc50: 2020 2020 2020 207b 226f 7022 3a20 226d         {"op": "m
-0001bc60: 6f76 6522 2c20 2266 726f 6d22 3a20 222f  ove", "from": "/
-0001bc70: 636f 6c6f 7222 2c20 2270 6174 6822 3a20  color", "path": 
-0001bc80: 222f 6661 766f 7269 7465 5f63 6f6c 6f72  "/favorite_color
-0001bc90: 227d 0a20 2020 2020 2020 205d 0a20 2020  "}.        ].   
-0001bca0: 2020 2020 2070 6174 6368 6564 5f69 7465       patched_ite
-0001bcb0: 6d20 3d20 6372 6561 7465 645f 636f 6e74  m = created_cont
-0001bcc0: 6169 6e65 722e 7061 7463 685f 6974 656d  ainer.patch_item
-0001bcd0: 2869 7465 6d3d 2270 6174 6368 5f69 7465  (item="patch_ite
-0001bce0: 6d22 2c20 7061 7274 6974 696f 6e5f 6b65  m", partition_ke
-0001bcf0: 793d 2270 6174 6368 5f69 7465 6d5f 706b  y="patch_item_pk
-0001bd00: 222c 2070 6174 6368 5f6f 7065 7261 7469  ", patch_operati
-0001bd10: 6f6e 733d 6f70 6572 6174 696f 6e73 290a  ons=operations).
-0001bd20: 2020 2020 2020 2020 2356 6572 6966 7920          #Verify 
-0001bd30: 7265 7375 6c74 7320 6672 6f6d 2070 6174  results from pat
-0001bd40: 6368 206f 7065 7261 7469 6f6e 730a 2020  ch operations.  
-0001bd50: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-0001bd60: 7454 7275 6528 7061 7463 6865 645f 6974  tTrue(patched_it
-0001bd70: 656d 2e67 6574 2822 636f 6c6f 7222 2920  em.get("color") 
-0001bd80: 6973 204e 6f6e 6529 0a20 2020 2020 2020  is None).       
-0001bd90: 2073 656c 662e 6173 7365 7274 5472 7565   self.assertTrue
-0001bda0: 2870 6174 6368 6564 5f69 7465 6d2e 6765  (patched_item.ge
-0001bdb0: 7428 2270 726f 7022 2920 6973 204e 6f6e  t("prop") is Non
-0001bdc0: 6529 0a20 2020 2020 2020 2073 656c 662e  e).        self.
-0001bdd0: 6173 7365 7274 4571 7561 6c28 7061 7463  assertEqual(patc
-0001bde0: 6865 645f 6974 656d 2e67 6574 2822 636f  hed_item.get("co
-0001bdf0: 6d70 616e 7922 292c 2022 436f 736d 6f73  mpany"), "Cosmos
-0001be00: 4442 2229 0a20 2020 2020 2020 2073 656c  DB").        sel
-0001be10: 662e 6173 7365 7274 4571 7561 6c28 7061  f.assertEqual(pa
-0001be20: 7463 6865 645f 6974 656d 2e67 6574 2822  tched_item.get("
-0001be30: 6164 6472 6573 7322 292e 6765 7428 226e  address").get("n
-0001be40: 6577 5f63 6974 7922 292c 2022 4174 6c61  ew_city"), "Atla
-0001be50: 6e74 6122 290a 2020 2020 2020 2020 7365  nta").        se
-0001be60: 6c66 2e61 7373 6572 7445 7175 616c 2870  lf.assertEqual(p
-0001be70: 6174 6368 6564 5f69 7465 6d2e 6765 7428  atched_item.get(
-0001be80: 226e 756d 6265 7222 292c 2031 3029 0a20  "number"), 10). 
-0001be90: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-0001bea0: 7274 4571 7561 6c28 7061 7463 6865 645f  rtEqual(patched_
-0001beb0: 6974 656d 2e67 6574 2822 6661 766f 7269  item.get("favori
-0001bec0: 7465 5f63 6f6c 6f72 2229 2c20 2279 656c  te_color"), "yel
-0001bed0: 6c6f 7722 290a 0a20 2020 2020 2020 2023  low")..        #
-0001bee0: 4e65 6761 7469 7665 2074 6573 7420 2d20  Negative test - 
-0001bef0: 6174 7465 6d70 7420 746f 2072 6570 6c61  attempt to repla
-0001bf00: 6365 206e 6f6e 2d65 7869 7374 656e 7420  ce non-existent 
-0001bf10: 6669 656c 640a 2020 2020 2020 2020 6f70  field.        op
-0001bf20: 6572 6174 696f 6e73 203d 205b 7b22 6f70  erations = [{"op
-0001bf30: 223a 2022 7265 706c 6163 6522 2c20 2270  ": "replace", "p
-0001bf40: 6174 6822 3a20 222f 7772 6f6e 675f 6669  ath": "/wrong_fi
-0001bf50: 656c 6422 2c20 2276 616c 7565 223a 2022  eld", "value": "
-0001bf60: 7772 6f6e 675f 7661 6c75 6522 7d5d 0a20  wrong_value"}]. 
-0001bf70: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
-0001bf80: 2020 2020 2020 2020 6372 6561 7465 645f          created_
-0001bf90: 636f 6e74 6169 6e65 722e 7061 7463 685f  container.patch_
-0001bfa0: 6974 656d 2869 7465 6d3d 2270 6174 6368  item(item="patch
-0001bfb0: 5f69 7465 6d22 2c20 7061 7274 6974 696f  _item", partitio
-0001bfc0: 6e5f 6b65 793d 2270 6174 6368 5f69 7465  n_key="patch_ite
-0001bfd0: 6d5f 706b 222c 2070 6174 6368 5f6f 7065  m_pk", patch_ope
-0001bfe0: 7261 7469 6f6e 733d 6f70 6572 6174 696f  rations=operatio
-0001bff0: 6e73 290a 2020 2020 2020 2020 6578 6365  ns).        exce
-0001c000: 7074 2065 7863 6570 7469 6f6e 732e 436f  pt exceptions.Co
-0001c010: 736d 6f73 4874 7470 5265 7370 6f6e 7365  smosHttpResponse
-0001c020: 4572 726f 7220 6173 2065 3a0a 2020 2020  Error as e:.    
-0001c030: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-0001c040: 6572 7445 7175 616c 2865 2e73 7461 7475  ertEqual(e.statu
-0001c050: 735f 636f 6465 2c20 5374 6174 7573 436f  s_code, StatusCo
-0001c060: 6465 732e 4241 445f 5245 5155 4553 5429  des.BAD_REQUEST)
-0001c070: 0a0a 2020 2020 2020 2020 234e 6567 6174  ..        #Negat
-0001c080: 6976 6520 7465 7374 202d 2061 7474 656d  ive test - attem
-0001c090: 7074 2074 6f20 7265 6d6f 7665 206e 6f6e  pt to remove non
-0001c0a0: 2d65 7869 7374 656e 7420 6669 656c 640a  -existent field.
-0001c0b0: 2020 2020 2020 2020 6f70 6572 6174 696f          operatio
-0001c0c0: 6e73 203d 205b 7b22 6f70 223a 2022 7265  ns = [{"op": "re
-0001c0d0: 6d6f 7665 222c 2022 7061 7468 223a 2022  move", "path": "
-0001c0e0: 2f77 726f 6e67 5f66 6965 6c64 227d 5d0a  /wrong_field"}].
-0001c0f0: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
-0001c100: 2020 2020 2020 2020 2063 7265 6174 6564           created
-0001c110: 5f63 6f6e 7461 696e 6572 2e70 6174 6368  _container.patch
-0001c120: 5f69 7465 6d28 6974 656d 3d22 7061 7463  _item(item="patc
-0001c130: 685f 6974 656d 222c 2070 6172 7469 7469  h_item", partiti
-0001c140: 6f6e 5f6b 6579 3d22 7061 7463 685f 6974  on_key="patch_it
-0001c150: 656d 5f70 6b22 2c20 7061 7463 685f 6f70  em_pk", patch_op
-0001c160: 6572 6174 696f 6e73 3d6f 7065 7261 7469  erations=operati
-0001c170: 6f6e 7329 0a20 2020 2020 2020 2065 7863  ons).        exc
-0001c180: 6570 7420 6578 6365 7074 696f 6e73 2e43  ept exceptions.C
-0001c190: 6f73 6d6f 7348 7474 7052 6573 706f 6e73  osmosHttpRespons
-0001c1a0: 6545 7272 6f72 2061 7320 653a 0a20 2020  eError as e:.   
-0001c1b0: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-0001c1c0: 7365 7274 4571 7561 6c28 652e 7374 6174  sertEqual(e.stat
-0001c1d0: 7573 5f63 6f64 652c 2053 7461 7475 7343  us_code, StatusC
-0001c1e0: 6f64 6573 2e42 4144 5f52 4551 5545 5354  odes.BAD_REQUEST
-0001c1f0: 290a 0a20 2020 2020 2020 2023 4e65 6761  )..        #Nega
-0001c200: 7469 7665 2074 6573 7420 2d20 6174 7465  tive test - atte
-0001c210: 6d70 7420 746f 2069 6e63 7265 6d65 6e74  mpt to increment
-0001c220: 206e 6f6e 2d6e 756d 6265 7220 6669 656c   non-number fiel
-0001c230: 640a 2020 2020 2020 2020 6f70 6572 6174  d.        operat
-0001c240: 696f 6e73 203d 205b 7b22 6f70 223a 2022  ions = [{"op": "
-0001c250: 696e 6372 222c 2022 7061 7468 223a 2022  incr", "path": "
-0001c260: 2f63 6f6d 7061 6e79 222c 2022 7661 6c75  /company", "valu
-0001c270: 6522 3a20 337d 5d0a 2020 2020 2020 2020  e": 3}].        
-0001c280: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
-0001c290: 2063 7265 6174 6564 5f63 6f6e 7461 696e   created_contain
-0001c2a0: 6572 2e70 6174 6368 5f69 7465 6d28 6974  er.patch_item(it
-0001c2b0: 656d 3d22 7061 7463 685f 6974 656d 222c  em="patch_item",
-0001c2c0: 2070 6172 7469 7469 6f6e 5f6b 6579 3d22   partition_key="
-0001c2d0: 7061 7463 685f 6974 656d 5f70 6b22 2c20  patch_item_pk", 
-0001c2e0: 7061 7463 685f 6f70 6572 6174 696f 6e73  patch_operations
-0001c2f0: 3d6f 7065 7261 7469 6f6e 7329 0a20 2020  =operations).   
-0001c300: 2020 2020 2065 7863 6570 7420 6578 6365       except exce
-0001c310: 7074 696f 6e73 2e43 6f73 6d6f 7348 7474  ptions.CosmosHtt
-0001c320: 7052 6573 706f 6e73 6545 7272 6f72 2061  pResponseError a
-0001c330: 7320 653a 0a20 2020 2020 2020 2020 2020  s e:.           
-0001c340: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-0001c350: 6c28 652e 7374 6174 7573 5f63 6f64 652c  l(e.status_code,
-0001c360: 2053 7461 7475 7343 6f64 6573 2e42 4144   StatusCodes.BAD
-0001c370: 5f52 4551 5545 5354 290a 0a20 2020 2020  _REQUEST)..     
-0001c380: 2020 2023 4e65 6761 7469 7665 2074 6573     #Negative tes
-0001c390: 7420 2d20 6174 7465 6d70 7420 746f 206d  t - attempt to m
-0001c3a0: 6f76 6520 6672 6f6d 206e 6f6e 2d65 7869  ove from non-exi
-0001c3b0: 7374 656e 7420 6669 656c 640a 2020 2020  stent field.    
-0001c3c0: 2020 2020 6f70 6572 6174 696f 6e73 203d      operations =
-0001c3d0: 205b 7b22 6f70 223a 2022 6d6f 7665 222c   [{"op": "move",
-0001c3e0: 2022 6672 6f6d 223a 2022 2f77 726f 6e67   "from": "/wrong
-0001c3f0: 5f66 6965 6c64 222c 2022 7061 7468 223a  _field", "path":
-0001c400: 2022 2f6f 7468 6572 5f66 6965 6c64 227d   "/other_field"}
-0001c410: 5d0a 2020 2020 2020 2020 7472 793a 0a20  ].        try:. 
-0001c420: 2020 2020 2020 2020 2020 2063 7265 6174             creat
-0001c430: 6564 5f63 6f6e 7461 696e 6572 2e70 6174  ed_container.pat
-0001c440: 6368 5f69 7465 6d28 6974 656d 3d22 7061  ch_item(item="pa
-0001c450: 7463 685f 6974 656d 222c 2070 6172 7469  tch_item", parti
-0001c460: 7469 6f6e 5f6b 6579 3d22 7061 7463 685f  tion_key="patch_
-0001c470: 6974 656d 5f70 6b22 2c20 7061 7463 685f  item_pk", patch_
-0001c480: 6f70 6572 6174 696f 6e73 3d6f 7065 7261  operations=opera
-0001c490: 7469 6f6e 7329 0a20 2020 2020 2020 2065  tions).        e
-0001c4a0: 7863 6570 7420 6578 6365 7074 696f 6e73  xcept exceptions
-0001c4b0: 2e43 6f73 6d6f 7348 7474 7052 6573 706f  .CosmosHttpRespo
-0001c4c0: 6e73 6545 7272 6f72 2061 7320 653a 0a20  nseError as e:. 
-0001c4d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0001c4e0: 6173 7365 7274 4571 7561 6c28 652e 7374  assertEqual(e.st
-0001c4f0: 6174 7573 5f63 6f64 652c 2053 7461 7475  atus_code, Statu
-0001c500: 7343 6f64 6573 2e42 4144 5f52 4551 5545  sCodes.BAD_REQUE
-0001c510: 5354 290a 0a20 2020 2023 2054 656d 706f  ST)..    # Tempo
-0001c520: 7261 7269 6c79 2063 6f6d 6d65 6e74 696e  rarily commentin
-0001c530: 6720 616e 616c 7974 6963 616c 2073 746f  g analytical sto
-0001c540: 7261 6765 2074 6573 7473 2075 6e74 696c  rage tests until
-0001c550: 2065 6d75 6c61 746f 7220 7375 7070 6f72   emulator suppor
-0001c560: 7420 636f 6d65 732e 0a20 2020 2023 2064  t comes..    # d
-0001c570: 6566 2074 6573 745f 6372 6561 7465 5f63  ef test_create_c
-0001c580: 6f6e 7461 696e 6572 5f77 6974 685f 616e  ontainer_with_an
-0001c590: 616c 7974 6963 616c 5f73 746f 7265 5f6f  alytical_store_o
-0001c5a0: 6666 2873 656c 6629 3a0a 2020 2020 2320  ff(self):.    # 
-0001c5b0: 2020 2020 2320 646f 6e27 7420 7275 6e20      # don't run 
-0001c5c0: 7465 7374 2c20 666f 7220 7468 6520 7469  test, for the ti
-0001c5d0: 6d65 2062 6569 6e67 2c20 6966 2072 756e  me being, if run
-0001c5e0: 6e69 6e67 2061 6761 696e 7374 2074 6865  ning against the
-0001c5f0: 2065 6d75 6c61 746f 720a 2020 2020 2320   emulator.    # 
-0001c600: 2020 2020 6966 2027 6c6f 6361 6c68 6f73      if 'localhos
-0001c610: 7427 2069 6e20 7365 6c66 2e68 6f73 7420  t' in self.host 
-0001c620: 6f72 2027 3132 372e 302e 302e 3127 2069  or '127.0.0.1' i
-0001c630: 6e20 7365 6c66 2e68 6f73 743a 0a20 2020  n self.host:.   
-0001c640: 2023 2020 2020 2020 2020 2072 6574 7572   #         retur
-0001c650: 6e0a 0a20 2020 2023 2020 2020 2063 7265  n..    #     cre
-0001c660: 6174 6564 5f64 6220 3d20 7365 6c66 2e64  ated_db = self.d
-0001c670: 6174 6162 6173 6546 6f72 5465 7374 0a20  atabaseForTest. 
-0001c680: 2020 2023 2020 2020 2063 6f6c 6c65 6374     #     collect
-0001c690: 696f 6e5f 6964 203d 2027 7465 7374 5f63  ion_id = 'test_c
-0001c6a0: 7265 6174 655f 636f 6e74 6169 6e65 725f  reate_container_
-0001c6b0: 7769 7468 5f61 6e61 6c79 7469 6361 6c5f  with_analytical_
-0001c6c0: 7374 6f72 655f 6f66 665f 2720 2b20 7374  store_off_' + st
-0001c6d0: 7228 7575 6964 2e75 7569 6434 2829 290a  r(uuid.uuid4()).
-0001c6e0: 2020 2020 2320 2020 2020 636f 6c6c 6563      #     collec
-0001c6f0: 7469 6f6e 5f69 6e64 6578 696e 675f 706f  tion_indexing_po
-0001c700: 6c69 6379 203d 207b 2769 6e64 6578 696e  licy = {'indexin
-0001c710: 674d 6f64 6527 3a20 2763 6f6e 7369 7374  gMode': 'consist
-0001c720: 656e 7427 7d0a 2020 2020 2320 2020 2020  ent'}.    #     
-0001c730: 6372 6561 7465 645f 7265 636f 7264 6572  created_recorder
-0001c740: 203d 2052 6563 6f72 6444 6961 676e 6f73   = RecordDiagnos
-0001c750: 7469 6373 2829 0a20 2020 2023 2020 2020  tics().    #    
-0001c760: 2063 7265 6174 6564 5f63 6f6c 6c65 6374   created_collect
-0001c770: 696f 6e20 3d20 6372 6561 7465 645f 6462  ion = created_db
-0001c780: 2e63 7265 6174 655f 636f 6e74 6169 6e65  .create_containe
-0001c790: 7228 6964 3d63 6f6c 6c65 6374 696f 6e5f  r(id=collection_
-0001c7a0: 6964 2c0a 2020 2020 2320 2020 2020 2020  id,.    #       
-0001c7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c7d0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0001c7e0: 6e64 6578 696e 675f 706f 6c69 6379 3d63  ndexing_policy=c
-0001c7f0: 6f6c 6c65 6374 696f 6e5f 696e 6465 7869  ollection_indexi
-0001c800: 6e67 5f70 6f6c 6963 792c 0a20 2020 2023  ng_policy,.    #
-0001c810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c840: 2020 2020 2020 7061 7274 6974 696f 6e5f        partition_
-0001c850: 6b65 793d 5061 7274 6974 696f 6e4b 6579  key=PartitionKey
-0001c860: 2870 6174 683d 222f 706b 222c 206b 696e  (path="/pk", kin
-0001c870: 643d 2248 6173 6822 292c 200a 2020 2020  d="Hash"), .    
-0001c880: 2320 2020 2020 2020 2020 2020 2020 2020  #               
-0001c890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c8b0: 2020 2020 2020 2072 6573 706f 6e73 655f         response_
-0001c8c0: 686f 6f6b 3d63 7265 6174 6564 5f72 6563  hook=created_rec
-0001c8d0: 6f72 6465 7229 0a20 2020 2023 2020 2020  order).    #    
-0001c8e0: 2070 726f 7065 7274 6965 7320 3d20 6372   properties = cr
-0001c8f0: 6561 7465 645f 636f 6c6c 6563 7469 6f6e  eated_collection
-0001c900: 2e72 6561 6428 290a 2020 2020 2320 2020  .read().    #   
-0001c910: 2020 7474 6c5f 6b65 7920 3d20 2261 6e61    ttl_key = "ana
-0001c920: 6c79 7469 6361 6c53 746f 7261 6765 5474  lyticalStorageTt
-0001c930: 6c22 0a20 2020 2023 2020 2020 2073 656c  l".    #     sel
-0001c940: 662e 6173 7365 7274 5472 7565 2874 746c  f.assertTrue(ttl
-0001c950: 5f6b 6579 206e 6f74 2069 6e20 7072 6f70  _key not in prop
-0001c960: 6572 7469 6573 206f 7220 7072 6f70 6572  erties or proper
-0001c970: 7469 6573 5b74 746c 5f6b 6579 5d20 3d3d  ties[ttl_key] ==
-0001c980: 204e 6f6e 6529 0a0a 2020 2020 2320 6465   None)..    # de
-0001c990: 6620 7465 7374 5f63 7265 6174 655f 636f  f test_create_co
-0001c9a0: 6e74 6169 6e65 725f 7769 7468 5f61 6e61  ntainer_with_ana
-0001c9b0: 6c79 7469 6361 6c5f 7374 6f72 655f 6f6e  lytical_store_on
-0001c9c0: 2873 656c 6629 3a0a 2020 2020 2320 2020  (self):.    #   
-0001c9d0: 2020 2320 646f 6e27 7420 7275 6e20 7465    # don't run te
-0001c9e0: 7374 2c20 666f 7220 7468 6520 7469 6d65  st, for the time
-0001c9f0: 2062 6569 6e67 2c20 6966 2072 756e 6e69   being, if runni
-0001ca00: 6e67 2061 6761 696e 7374 2074 6865 2065  ng against the e
-0001ca10: 6d75 6c61 746f 720a 2020 2020 2320 2020  mulator.    #   
-0001ca20: 2020 6966 2027 6c6f 6361 6c68 6f73 7427    if 'localhost'
-0001ca30: 2069 6e20 7365 6c66 2e68 6f73 7420 6f72   in self.host or
-0001ca40: 2027 3132 372e 302e 302e 3127 2069 6e20   '127.0.0.1' in 
-0001ca50: 7365 6c66 2e68 6f73 743a 0a20 2020 2023  self.host:.    #
-0001ca60: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
-0001ca70: 0a20 2020 2023 2020 2020 2063 7265 6174  .    #     creat
-0001ca80: 6564 5f64 6220 3d20 7365 6c66 2e64 6174  ed_db = self.dat
-0001ca90: 6162 6173 6546 6f72 5465 7374 0a20 2020  abaseForTest.   
-0001caa0: 2023 2020 2020 2063 6f6c 6c65 6374 696f   #     collectio
-0001cab0: 6e5f 6964 203d 2027 7465 7374 5f63 7265  n_id = 'test_cre
-0001cac0: 6174 655f 636f 6e74 6169 6e65 725f 7769  ate_container_wi
-0001cad0: 7468 5f61 6e61 6c79 7469 6361 6c5f 7374  th_analytical_st
-0001cae0: 6f72 655f 6f6e 5f27 202b 2073 7472 2875  ore_on_' + str(u
-0001caf0: 7569 642e 7575 6964 3428 2929 0a20 2020  uid.uuid4()).   
-0001cb00: 2023 2020 2020 2063 6f6c 6c65 6374 696f   #     collectio
-0001cb10: 6e5f 696e 6465 7869 6e67 5f70 6f6c 6963  n_indexing_polic
-0001cb20: 7920 3d20 7b27 696e 6465 7869 6e67 4d6f  y = {'indexingMo
-0001cb30: 6465 273a 2027 636f 6e73 6973 7465 6e74  de': 'consistent
-0001cb40: 277d 0a20 2020 2023 2020 2020 2063 7265  '}.    #     cre
-0001cb50: 6174 6564 5f72 6563 6f72 6465 7220 3d20  ated_recorder = 
-0001cb60: 5265 636f 7264 4469 6167 6e6f 7374 6963  RecordDiagnostic
-0001cb70: 7328 290a 2020 2020 2320 2020 2020 6372  s().    #     cr
-0001cb80: 6561 7465 645f 636f 6c6c 6563 7469 6f6e  eated_collection
-0001cb90: 203d 2063 7265 6174 6564 5f64 622e 6372   = created_db.cr
-0001cba0: 6561 7465 5f63 6f6e 7461 696e 6572 2869  eate_container(i
-0001cbb0: 643d 636f 6c6c 6563 7469 6f6e 5f69 642c  d=collection_id,
-0001cbc0: 0a20 2020 2023 2020 2020 2020 2020 2020  .    #          
-0001cbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cbf0: 2020 2020 2020 2020 2020 2020 616e 616c              anal
-0001cc00: 7974 6963 616c 5f73 746f 7261 6765 5f74  ytical_storage_t
-0001cc10: 746c 3d2d 312c 0a20 2020 2023 2020 2020  tl=-1,.    #    
-0001cc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cc30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cc40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cc50: 2020 696e 6465 7869 6e67 5f70 6f6c 6963    indexing_polic
-0001cc60: 793d 636f 6c6c 6563 7469 6f6e 5f69 6e64  y=collection_ind
-0001cc70: 6578 696e 675f 706f 6c69 6379 2c0a 2020  exing_policy,.  
-0001cc80: 2020 2320 2020 2020 2020 2020 2020 2020    #             
-0001cc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ccb0: 2020 2020 2020 2020 2070 6172 7469 7469           partiti
-0001ccc0: 6f6e 5f6b 6579 3d50 6172 7469 7469 6f6e  on_key=Partition
-0001ccd0: 4b65 7928 7061 7468 3d22 2f70 6b22 2c20  Key(path="/pk", 
-0001cce0: 6b69 6e64 3d22 4861 7368 2229 2c20 0a20  kind="Hash"), . 
-0001ccf0: 2020 2023 2020 2020 2020 2020 2020 2020     #            
-0001cd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cd10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cd20: 2020 2020 2020 2020 2020 7265 7370 6f6e            respon
-0001cd30: 7365 5f68 6f6f 6b3d 6372 6561 7465 645f  se_hook=created_
-0001cd40: 7265 636f 7264 6572 290a 2020 2020 2320  recorder).    # 
-0001cd50: 2020 2020 7072 6f70 6572 7469 6573 203d      properties =
-0001cd60: 2063 7265 6174 6564 5f63 6f6c 6c65 6374   created_collect
-0001cd70: 696f 6e2e 7265 6164 2829 0a20 2020 2023  ion.read().    #
-0001cd80: 2020 2020 2074 746c 5f6b 6579 203d 2022       ttl_key = "
-0001cd90: 616e 616c 7974 6963 616c 5374 6f72 6167  analyticalStorag
-0001cda0: 6554 746c 220a 2020 2020 2320 2020 2020  eTtl".    #     
-0001cdb0: 7365 6c66 2e61 7373 6572 7454 7275 6528  self.assertTrue(
-0001cdc0: 7474 6c5f 6b65 7920 696e 2070 726f 7065  ttl_key in prope
-0001cdd0: 7274 6965 7320 616e 6420 7072 6f70 6572  rties and proper
-0001cde0: 7469 6573 5b74 746c 5f6b 6579 5d20 3d3d  ties[ttl_key] ==
-0001cdf0: 202d 3129 0a0a 2020 2020 2320 6465 6620   -1)..    # def 
-0001ce00: 7465 7374 5f63 7265 6174 655f 636f 6e74  test_create_cont
-0001ce10: 6169 6e65 725f 6966 5f6e 6f74 5f65 7869  ainer_if_not_exi
-0001ce20: 7374 735f 7769 7468 5f61 6e61 6c79 7469  sts_with_analyti
-0001ce30: 6361 6c5f 7374 6f72 655f 6f6e 2873 656c  cal_store_on(sel
-0001ce40: 6629 3a0a 2020 2020 2320 2020 2020 2320  f):.    #     # 
-0001ce50: 646f 6e27 7420 7275 6e20 7465 7374 2c20  don't run test, 
-0001ce60: 666f 7220 7468 6520 7469 6d65 2062 6569  for the time bei
-0001ce70: 6e67 2c20 6966 2072 756e 6e69 6e67 2061  ng, if running a
-0001ce80: 6761 696e 7374 2074 6865 2065 6d75 6c61  gainst the emula
-0001ce90: 746f 720a 2020 2020 2320 2020 2020 6966  tor.    #     if
-0001cea0: 2027 6c6f 6361 6c68 6f73 7427 2069 6e20   'localhost' in 
-0001ceb0: 7365 6c66 2e68 6f73 7420 6f72 2027 3132  self.host or '12
-0001cec0: 372e 302e 302e 3127 2069 6e20 7365 6c66  7.0.0.1' in self
-0001ced0: 2e68 6f73 743a 0a20 2020 2023 2020 2020  .host:.    #    
-0001cee0: 2020 2020 2072 6574 7572 6e0a 0a20 2020       return..   
-0001cef0: 2023 2020 2020 2023 2066 6972 7374 2c20   #     # first, 
-0001cf00: 7472 7920 7768 656e 2077 6520 6b6e 6f77  try when we know
-0001cf10: 2074 6865 2063 6f6e 7461 696e 6572 2064   the container d
-0001cf20: 6f65 736e 2774 2065 7869 7374 2e0a 2020  oesn't exist..  
-0001cf30: 2020 2320 2020 2020 6372 6561 7465 645f    #     created_
-0001cf40: 6462 203d 2073 656c 662e 6461 7461 6261  db = self.databa
-0001cf50: 7365 466f 7254 6573 740a 2020 2020 2320  seForTest.    # 
-0001cf60: 2020 2020 636f 6c6c 6563 7469 6f6e 5f69      collection_i
-0001cf70: 6420 3d20 2774 6573 745f 6372 6561 7465  d = 'test_create
-0001cf80: 5f63 6f6e 7461 696e 6572 5f69 665f 6e6f  _container_if_no
-0001cf90: 745f 6578 6973 7473 5f77 6974 685f 616e  t_exists_with_an
-0001cfa0: 616c 7974 6963 616c 5f73 746f 7265 5f6f  alytical_store_o
-0001cfb0: 6e5f 2720 2b20 7374 7228 7575 6964 2e75  n_' + str(uuid.u
-0001cfc0: 7569 6434 2829 290a 2020 2020 2320 2020  uid4()).    #   
-0001cfd0: 2020 636f 6c6c 6563 7469 6f6e 5f69 6e64    collection_ind
-0001cfe0: 6578 696e 675f 706f 6c69 6379 203d 207b  exing_policy = {
-0001cff0: 2769 6e64 6578 696e 674d 6f64 6527 3a20  'indexingMode': 
-0001d000: 2763 6f6e 7369 7374 656e 7427 7d0a 2020  'consistent'}.  
-0001d010: 2020 2320 2020 2020 6372 6561 7465 645f    #     created_
-0001d020: 7265 636f 7264 6572 203d 2052 6563 6f72  recorder = Recor
-0001d030: 6444 6961 676e 6f73 7469 6373 2829 0a20  dDiagnostics(). 
-0001d040: 2020 2023 2020 2020 2063 7265 6174 6564     #     created
-0001d050: 5f63 6f6c 6c65 6374 696f 6e20 3d20 6372  _collection = cr
-0001d060: 6561 7465 645f 6462 2e63 7265 6174 655f  eated_db.create_
-0001d070: 636f 6e74 6169 6e65 725f 6966 5f6e 6f74  container_if_not
-0001d080: 5f65 7869 7374 7328 6964 3d63 6f6c 6c65  _exists(id=colle
-0001d090: 6374 696f 6e5f 6964 2c0a 2020 2020 2320  ction_id,.    # 
-0001d0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d0e0: 2020 2061 6e61 6c79 7469 6361 6c5f 7374     analytical_st
-0001d0f0: 6f72 6167 655f 7474 6c3d 2d31 2c0a 2020  orage_ttl=-1,.  
-0001d100: 2020 2320 2020 2020 2020 2020 2020 2020    #             
-0001d110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d140: 2020 2020 2020 2069 6e64 6578 696e 675f         indexing_
-0001d150: 706f 6c69 6379 3d63 6f6c 6c65 6374 696f  policy=collectio
-0001d160: 6e5f 696e 6465 7869 6e67 5f70 6f6c 6963  n_indexing_polic
-0001d170: 792c 0a20 2020 2023 2020 2020 2020 2020  y,.    #        
+0001b1d0: 7373 696f 6e2e 6964 290a 0a20 2020 2023  ssion.id)..    #
+0001b1e0: 436f 6d6d 656e 7469 6e67 206f 7574 2064  Commenting out d
+0001b1f0: 656c 6574 6520 6974 656d 7320 6279 2070  elete items by p
+0001b200: 6b20 756e 7469 6c20 7465 7374 2070 6970  k until test pip
+0001b210: 656c 696e 6573 2073 7570 706f 7274 2069  elines support i
+0001b220: 740a 2020 2020 2320 6465 6620 7465 7374  t.    # def test
+0001b230: 5f64 656c 6574 655f 616c 6c5f 6974 656d  _delete_all_item
+0001b240: 735f 6279 5f70 6172 7469 7469 6f6e 5f6b  s_by_partition_k
+0001b250: 6579 2873 656c 6629 3a0a 2020 2020 2320  ey(self):.    # 
+0001b260: 2020 2020 2320 6372 6561 7465 2064 6174      # create dat
+0001b270: 6162 6173 650a 2020 2020 2320 2020 2020  abase.    #     
+0001b280: 6372 6561 7465 645f 6462 203d 2073 656c  created_db = sel
+0001b290: 662e 6461 7461 6261 7365 466f 7254 6573  f.databaseForTes
+0001b2a0: 740a 2020 2020 230a 2020 2020 2320 2020  t.    #.    #   
+0001b2b0: 2020 2320 6372 6561 7465 2063 6f6e 7461    # create conta
+0001b2c0: 696e 6572 0a20 2020 2023 2020 2020 2063  iner.    #     c
+0001b2d0: 7265 6174 6564 5f63 6f6c 6c65 6374 696f  reated_collectio
+0001b2e0: 6e20 3d20 6372 6561 7465 645f 6462 2e63  n = created_db.c
+0001b2f0: 7265 6174 655f 636f 6e74 6169 6e65 7228  reate_container(
+0001b300: 0a20 2020 2023 2020 2020 2020 2020 2069  .    #         i
+0001b310: 643d 2774 6573 745f 6465 6c65 7465 5f61  d='test_delete_a
+0001b320: 6c6c 5f69 7465 6d73 5f62 795f 7061 7274  ll_items_by_part
+0001b330: 6974 696f 6e5f 6b65 7920 2720 2b20 7374  ition_key ' + st
+0001b340: 7228 7575 6964 2e75 7569 6434 2829 292c  r(uuid.uuid4()),
+0001b350: 0a20 2020 2023 2020 2020 2020 2020 2070  .    #         p
+0001b360: 6172 7469 7469 6f6e 5f6b 6579 3d50 6172  artition_key=Par
+0001b370: 7469 7469 6f6e 4b65 7928 7061 7468 3d27  titionKey(path='
+0001b380: 2f70 6b27 2c20 6b69 6e64 3d27 4861 7368  /pk', kind='Hash
+0001b390: 2729 0a20 2020 2023 2020 2020 2029 0a20  ').    #     ). 
+0001b3a0: 2020 2023 2020 2020 2023 2043 7265 6174     #     # Creat
+0001b3b0: 6520 7477 6f20 7061 7274 6974 696f 6e20  e two partition 
+0001b3c0: 6b65 7973 0a20 2020 2023 2020 2020 2070  keys.    #     p
+0001b3d0: 6172 7469 7469 6f6e 5f6b 6579 3120 3d20  artition_key1 = 
+0001b3e0: 227b 7d2d 7b7d 222e 666f 726d 6174 2822  "{}-{}".format("
+0001b3f0: 5061 7274 6974 696f 6e20 4b65 7920 3122  Partition Key 1"
+0001b400: 2c20 7374 7228 7575 6964 2e75 7569 6434  , str(uuid.uuid4
+0001b410: 2829 2929 0a20 2020 2023 2020 2020 2070  ())).    #     p
+0001b420: 6172 7469 7469 6f6e 5f6b 6579 3220 3d20  artition_key2 = 
+0001b430: 227b 7d2d 7b7d 222e 666f 726d 6174 2822  "{}-{}".format("
+0001b440: 5061 7274 6974 696f 6e20 4b65 7920 3222  Partition Key 2"
+0001b450: 2c20 7374 7228 7575 6964 2e75 7569 6434  , str(uuid.uuid4
+0001b460: 2829 2929 0a20 2020 2023 0a20 2020 2023  ())).    #.    #
+0001b470: 2020 2020 2023 2061 6464 2069 7465 6d73       # add items
+0001b480: 2066 6f72 2070 6172 7469 7469 6f6e 206b   for partition k
+0001b490: 6579 2031 0a20 2020 2023 2020 2020 2066  ey 1.    #     f
+0001b4a0: 6f72 2069 2069 6e20 7261 6e67 6528 312c  or i in range(1,
+0001b4b0: 2033 293a 0a20 2020 2023 2020 2020 2020   3):.    #      
+0001b4c0: 2020 2063 7265 6174 6564 5f63 6f6c 6c65     created_colle
+0001b4d0: 6374 696f 6e2e 7570 7365 7274 5f69 7465  ction.upsert_ite
+0001b4e0: 6d28 0a20 2020 2023 2020 2020 2020 2020  m(.    #        
+0001b4f0: 2020 2020 2064 6963 7428 6964 3d22 6974       dict(id="it
+0001b500: 656d 7b7d 222e 666f 726d 6174 2869 292c  em{}".format(i),
+0001b510: 2070 6b3d 7061 7274 6974 696f 6e5f 6b65   pk=partition_ke
+0001b520: 7931 290a 2020 2020 2320 2020 2020 2020  y1).    #       
+0001b530: 2020 290a 2020 2020 230a 2020 2020 2320    ).    #.    # 
+0001b540: 2020 2020 2320 6164 6420 6974 656d 7320      # add items 
+0001b550: 666f 7220 7061 7274 6974 696f 6e20 6b65  for partition ke
+0001b560: 7920 320a 2020 2020 230a 2020 2020 2320  y 2.    #.    # 
+0001b570: 2020 2020 706b 325f 6974 656d 203d 2063      pk2_item = c
+0001b580: 7265 6174 6564 5f63 6f6c 6c65 6374 696f  reated_collectio
+0001b590: 6e2e 7570 7365 7274 5f69 7465 6d28 6469  n.upsert_item(di
+0001b5a0: 6374 2869 643d 2269 7465 6d7b 7d22 2e66  ct(id="item{}".f
+0001b5b0: 6f72 6d61 7428 3329 2c20 706b 3d70 6172  ormat(3), pk=par
+0001b5c0: 7469 7469 6f6e 5f6b 6579 3229 290a 2020  tition_key2)).  
+0001b5d0: 2020 230a 2020 2020 2320 2020 2020 2320    #.    #     # 
+0001b5e0: 6465 6c65 7465 2061 6c6c 2069 7465 6d73  delete all items
+0001b5f0: 2066 6f72 2070 6172 7469 7469 6f6e 206b   for partition k
+0001b600: 6579 2031 0a20 2020 2023 2020 2020 2063  ey 1.    #     c
+0001b610: 7265 6174 6564 5f63 6f6c 6c65 6374 696f  reated_collectio
+0001b620: 6e2e 6465 6c65 7465 5f61 6c6c 5f69 7465  n.delete_all_ite
+0001b630: 6d73 5f62 795f 7061 7274 6974 696f 6e5f  ms_by_partition_
+0001b640: 6b65 7928 7061 7274 6974 696f 6e5f 6b65  key(partition_ke
+0001b650: 7931 290a 2020 2020 230a 2020 2020 2320  y1).    #.    # 
+0001b660: 2020 2020 2320 6368 6563 6b20 7468 6174      # check that
+0001b670: 206f 6e6c 7920 6974 656d 7320 6672 6f6d   only items from
+0001b680: 2070 6172 7469 7469 6f6e 206b 6579 2031   partition key 1
+0001b690: 2068 6176 6520 6265 656e 2064 656c 6574   have been delet
+0001b6a0: 6564 0a20 2020 2023 2020 2020 2069 7465  ed.    #     ite
+0001b6b0: 6d73 203d 206c 6973 7428 6372 6561 7465  ms = list(create
+0001b6c0: 645f 636f 6c6c 6563 7469 6f6e 2e72 6561  d_collection.rea
+0001b6d0: 645f 616c 6c5f 6974 656d 7328 2929 0a20  d_all_items()). 
+0001b6e0: 2020 2023 0a20 2020 2023 2020 2020 2023     #.    #     #
+0001b6f0: 2069 7465 6d73 2073 686f 756c 6420 6f6e   items should on
+0001b700: 6c79 2068 6176 6520 3120 6974 656d 2061  ly have 1 item a
+0001b710: 6e64 2069 7420 7368 6f75 6c64 2065 7175  nd it should equ
+0001b720: 616c 2070 6b32 5f69 7465 6d0a 2020 2020  al pk2_item.    
+0001b730: 2320 2020 2020 7365 6c66 2e61 7373 6572  #     self.asser
+0001b740: 7444 6963 7445 7175 616c 2870 6b32 5f69  tDictEqual(pk2_i
+0001b750: 7465 6d2c 2069 7465 6d73 5b30 5d29 0a20  tem, items[0]). 
+0001b760: 2020 2023 0a20 2020 2023 2020 2020 2023     #.    #     #
+0001b770: 2061 7474 656d 7074 696e 6720 746f 2064   attempting to d
+0001b780: 656c 6574 6520 6120 6e6f 6e2d 6578 6973  elete a non-exis
+0001b790: 7465 6e74 2070 6172 7469 7469 6f6e 206b  tent partition k
+0001b7a0: 6579 206f 7220 7061 7373 696e 6720 6e6f  ey or passing no
+0001b7b0: 6e65 2073 686f 756c 6420 6e6f 7420 6465  ne should not de
+0001b7c0: 6c65 7465 0a20 2020 2023 2020 2020 2023  lete.    #     #
+0001b7d0: 2061 6e79 7468 696e 6720 616e 6420 6c65   anything and le
+0001b7e0: 6176 6520 7468 696e 6773 2075 6e63 6861  ave things uncha
+0001b7f0: 6e67 6564 0a20 2020 2023 2020 2020 2063  nged.    #     c
+0001b800: 7265 6174 6564 5f63 6f6c 6c65 6374 696f  reated_collectio
+0001b810: 6e2e 6465 6c65 7465 5f61 6c6c 5f69 7465  n.delete_all_ite
+0001b820: 6d73 5f62 795f 7061 7274 6974 696f 6e5f  ms_by_partition_
+0001b830: 6b65 7928 4e6f 6e65 290a 2020 2020 230a  key(None).    #.
+0001b840: 2020 2020 2320 2020 2020 2320 6368 6563      #     # chec
+0001b850: 6b20 7468 6174 206e 6f20 6368 616e 6765  k that no change
+0001b860: 7320 7765 7265 206d 6164 6520 6279 2063  s were made by c
+0001b870: 6865 636b 696e 6720 6966 2074 6865 206f  hecking if the o
+0001b880: 6e6c 7920 6974 656d 2069 7320 7374 696c  nly item is stil
+0001b890: 6c20 7468 6572 650a 2020 2020 2320 2020  l there.    #   
+0001b8a0: 2020 6974 656d 7320 3d20 6c69 7374 2863    items = list(c
+0001b8b0: 7265 6174 6564 5f63 6f6c 6c65 6374 696f  reated_collectio
+0001b8c0: 6e2e 7265 6164 5f61 6c6c 5f69 7465 6d73  n.read_all_items
+0001b8d0: 2829 290a 2020 2020 230a 2020 2020 2320  ()).    #.    # 
+0001b8e0: 2020 2020 2320 6974 656d 7320 7368 6f75      # items shou
+0001b8f0: 6c64 206f 6e6c 7920 6861 7665 2031 2069  ld only have 1 i
+0001b900: 7465 6d20 616e 6420 6974 2073 686f 756c  tem and it shoul
+0001b910: 6420 6571 7561 6c20 706b 325f 6974 656d  d equal pk2_item
+0001b920: 0a20 2020 2023 2020 2020 2073 656c 662e  .    #     self.
+0001b930: 6173 7365 7274 4469 6374 4571 7561 6c28  assertDictEqual(
+0001b940: 706b 325f 6974 656d 2c20 6974 656d 735b  pk2_item, items[
+0001b950: 305d 290a 2020 2020 230a 2020 2020 2320  0]).    #.    # 
+0001b960: 2020 2020 6372 6561 7465 645f 6462 2e64      created_db.d
+0001b970: 656c 6574 655f 636f 6e74 6169 6e65 7228  elete_container(
+0001b980: 6372 6561 7465 645f 636f 6c6c 6563 7469  created_collecti
+0001b990: 6f6e 290a 0a20 2020 2064 6566 2074 6573  on)..    def tes
+0001b9a0: 745f 7061 7463 685f 6f70 6572 6174 696f  t_patch_operatio
+0001b9b0: 6e73 2873 656c 6629 3a0a 2020 2020 2020  ns(self):.      
+0001b9c0: 2020 6372 6561 7465 645f 636f 6e74 6169    created_contai
+0001b9d0: 6e65 7220 3d20 7365 6c66 2e64 6174 6162  ner = self.datab
+0001b9e0: 6173 6546 6f72 5465 7374 2e63 7265 6174  aseForTest.creat
+0001b9f0: 655f 636f 6e74 6169 6e65 725f 6966 5f6e  e_container_if_n
+0001ba00: 6f74 5f65 7869 7374 7328 6964 3d22 7061  ot_exists(id="pa
+0001ba10: 7463 685f 636f 6e74 6169 6e65 7222 2c20  tch_container", 
+0001ba20: 7061 7274 6974 696f 6e5f 6b65 793d 5061  partition_key=Pa
+0001ba30: 7274 6974 696f 6e4b 6579 2870 6174 683d  rtitionKey(path=
+0001ba40: 222f 706b 2229 290a 0a20 2020 2020 2020  "/pk"))..       
+0001ba50: 2023 4372 6561 7465 2069 7465 6d20 746f   #Create item to
+0001ba60: 2070 6174 6368 0a20 2020 2020 2020 2069   patch.        i
+0001ba70: 7465 6d20 3d20 7b0a 2020 2020 2020 2020  tem = {.        
+0001ba80: 2020 2020 2269 6422 3a20 2270 6174 6368      "id": "patch
+0001ba90: 5f69 7465 6d22 2c0a 2020 2020 2020 2020  _item",.        
+0001baa0: 2020 2020 2270 6b22 3a20 2270 6174 6368      "pk": "patch
+0001bab0: 5f69 7465 6d5f 706b 222c 0a20 2020 2020  _item_pk",.     
+0001bac0: 2020 2020 2020 2022 7072 6f70 223a 2022         "prop": "
+0001bad0: 7072 6f70 3122 2c0a 2020 2020 2020 2020  prop1",.        
+0001bae0: 2020 2020 2261 6464 7265 7373 223a 207b      "address": {
+0001baf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001bb00: 2022 6369 7479 223a 2022 5265 646d 6f6e   "city": "Redmon
+0001bb10: 6422 0a20 2020 2020 2020 2020 2020 207d  d".            }
+0001bb20: 2c0a 2020 2020 2020 2020 2020 2020 2263  ,.            "c
+0001bb30: 6f6d 7061 6e79 223a 2022 4d69 6372 6f73  ompany": "Micros
+0001bb40: 6f66 7422 2c0a 2020 2020 2020 2020 2020  oft",.          
+0001bb50: 2020 226e 756d 6265 7222 3a20 337d 0a20    "number": 3}. 
+0001bb60: 2020 2020 2020 2063 7265 6174 6564 5f63         created_c
+0001bb70: 6f6e 7461 696e 6572 2e63 7265 6174 655f  ontainer.create_
+0001bb80: 6974 656d 2869 7465 6d29 0a20 2020 2020  item(item).     
+0001bb90: 2020 2023 4465 6669 6e65 2061 6e64 2072     #Define and r
+0001bba0: 756e 2070 6174 6368 206f 7065 7261 7469  un patch operati
+0001bbb0: 6f6e 730a 2020 2020 2020 2020 6f70 6572  ons.        oper
+0001bbc0: 6174 696f 6e73 203d 205b 0a20 2020 2020  ations = [.     
+0001bbd0: 2020 2020 2020 207b 226f 7022 3a20 2261         {"op": "a
+0001bbe0: 6464 222c 2022 7061 7468 223a 2022 2f63  dd", "path": "/c
+0001bbf0: 6f6c 6f72 222c 2022 7661 6c75 6522 3a20  olor", "value": 
+0001bc00: 2279 656c 6c6f 7722 7d2c 0a20 2020 2020  "yellow"},.     
+0001bc10: 2020 2020 2020 207b 226f 7022 3a20 2272         {"op": "r
+0001bc20: 656d 6f76 6522 2c20 2270 6174 6822 3a20  emove", "path": 
+0001bc30: 222f 7072 6f70 227d 2c0a 2020 2020 2020  "/prop"},.      
+0001bc40: 2020 2020 2020 7b22 6f70 223a 2022 7265        {"op": "re
+0001bc50: 706c 6163 6522 2c20 2270 6174 6822 3a20  place", "path": 
+0001bc60: 222f 636f 6d70 616e 7922 2c20 2276 616c  "/company", "val
+0001bc70: 7565 223a 2022 436f 736d 6f73 4442 227d  ue": "CosmosDB"}
+0001bc80: 2c0a 2020 2020 2020 2020 2020 2020 7b22  ,.            {"
+0001bc90: 6f70 223a 2022 7365 7422 2c20 2270 6174  op": "set", "pat
+0001bca0: 6822 3a20 222f 6164 6472 6573 732f 6e65  h": "/address/ne
+0001bcb0: 775f 6369 7479 222c 2022 7661 6c75 6522  w_city", "value"
+0001bcc0: 3a20 2241 746c 616e 7461 227d 2c0a 2020  : "Atlanta"},.  
+0001bcd0: 2020 2020 2020 2020 2020 7b22 6f70 223a            {"op":
+0001bce0: 2022 696e 6372 222c 2022 7061 7468 223a   "incr", "path":
+0001bcf0: 2022 2f6e 756d 6265 7222 2c20 2276 616c   "/number", "val
+0001bd00: 7565 223a 2037 7d2c 0a20 2020 2020 2020  ue": 7},.       
+0001bd10: 2020 2020 207b 226f 7022 3a20 226d 6f76       {"op": "mov
+0001bd20: 6522 2c20 2266 726f 6d22 3a20 222f 636f  e", "from": "/co
+0001bd30: 6c6f 7222 2c20 2270 6174 6822 3a20 222f  lor", "path": "/
+0001bd40: 6661 766f 7269 7465 5f63 6f6c 6f72 227d  favorite_color"}
+0001bd50: 0a20 2020 2020 2020 205d 0a20 2020 2020  .        ].     
+0001bd60: 2020 2070 6174 6368 6564 5f69 7465 6d20     patched_item 
+0001bd70: 3d20 6372 6561 7465 645f 636f 6e74 6169  = created_contai
+0001bd80: 6e65 722e 7061 7463 685f 6974 656d 2869  ner.patch_item(i
+0001bd90: 7465 6d3d 2270 6174 6368 5f69 7465 6d22  tem="patch_item"
+0001bda0: 2c20 7061 7274 6974 696f 6e5f 6b65 793d  , partition_key=
+0001bdb0: 2270 6174 6368 5f69 7465 6d5f 706b 222c  "patch_item_pk",
+0001bdc0: 2070 6174 6368 5f6f 7065 7261 7469 6f6e   patch_operation
+0001bdd0: 733d 6f70 6572 6174 696f 6e73 290a 2020  s=operations).  
+0001bde0: 2020 2020 2020 2356 6572 6966 7920 7265        #Verify re
+0001bdf0: 7375 6c74 7320 6672 6f6d 2070 6174 6368  sults from patch
+0001be00: 206f 7065 7261 7469 6f6e 730a 2020 2020   operations.    
+0001be10: 2020 2020 7365 6c66 2e61 7373 6572 7454      self.assertT
+0001be20: 7275 6528 7061 7463 6865 645f 6974 656d  rue(patched_item
+0001be30: 2e67 6574 2822 636f 6c6f 7222 2920 6973  .get("color") is
+0001be40: 204e 6f6e 6529 0a20 2020 2020 2020 2073   None).        s
+0001be50: 656c 662e 6173 7365 7274 5472 7565 2870  elf.assertTrue(p
+0001be60: 6174 6368 6564 5f69 7465 6d2e 6765 7428  atched_item.get(
+0001be70: 2270 726f 7022 2920 6973 204e 6f6e 6529  "prop") is None)
+0001be80: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+0001be90: 7365 7274 4571 7561 6c28 7061 7463 6865  sertEqual(patche
+0001bea0: 645f 6974 656d 2e67 6574 2822 636f 6d70  d_item.get("comp
+0001beb0: 616e 7922 292c 2022 436f 736d 6f73 4442  any"), "CosmosDB
+0001bec0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+0001bed0: 6173 7365 7274 4571 7561 6c28 7061 7463  assertEqual(patc
+0001bee0: 6865 645f 6974 656d 2e67 6574 2822 6164  hed_item.get("ad
+0001bef0: 6472 6573 7322 292e 6765 7428 226e 6577  dress").get("new
+0001bf00: 5f63 6974 7922 292c 2022 4174 6c61 6e74  _city"), "Atlant
+0001bf10: 6122 290a 2020 2020 2020 2020 7365 6c66  a").        self
+0001bf20: 2e61 7373 6572 7445 7175 616c 2870 6174  .assertEqual(pat
+0001bf30: 6368 6564 5f69 7465 6d2e 6765 7428 226e  ched_item.get("n
+0001bf40: 756d 6265 7222 292c 2031 3029 0a20 2020  umber"), 10).   
+0001bf50: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+0001bf60: 4571 7561 6c28 7061 7463 6865 645f 6974  Equal(patched_it
+0001bf70: 656d 2e67 6574 2822 6661 766f 7269 7465  em.get("favorite
+0001bf80: 5f63 6f6c 6f72 2229 2c20 2279 656c 6c6f  _color"), "yello
+0001bf90: 7722 290a 0a20 2020 2020 2020 2023 4e65  w")..        #Ne
+0001bfa0: 6761 7469 7665 2074 6573 7420 2d20 6174  gative test - at
+0001bfb0: 7465 6d70 7420 746f 2072 6570 6c61 6365  tempt to replace
+0001bfc0: 206e 6f6e 2d65 7869 7374 656e 7420 6669   non-existent fi
+0001bfd0: 656c 640a 2020 2020 2020 2020 6f70 6572  eld.        oper
+0001bfe0: 6174 696f 6e73 203d 205b 7b22 6f70 223a  ations = [{"op":
+0001bff0: 2022 7265 706c 6163 6522 2c20 2270 6174   "replace", "pat
+0001c000: 6822 3a20 222f 7772 6f6e 675f 6669 656c  h": "/wrong_fiel
+0001c010: 6422 2c20 2276 616c 7565 223a 2022 7772  d", "value": "wr
+0001c020: 6f6e 675f 7661 6c75 6522 7d5d 0a20 2020  ong_value"}].   
+0001c030: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+0001c040: 2020 2020 2020 6372 6561 7465 645f 636f        created_co
+0001c050: 6e74 6169 6e65 722e 7061 7463 685f 6974  ntainer.patch_it
+0001c060: 656d 2869 7465 6d3d 2270 6174 6368 5f69  em(item="patch_i
+0001c070: 7465 6d22 2c20 7061 7274 6974 696f 6e5f  tem", partition_
+0001c080: 6b65 793d 2270 6174 6368 5f69 7465 6d5f  key="patch_item_
+0001c090: 706b 222c 2070 6174 6368 5f6f 7065 7261  pk", patch_opera
+0001c0a0: 7469 6f6e 733d 6f70 6572 6174 696f 6e73  tions=operations
+0001c0b0: 290a 2020 2020 2020 2020 6578 6365 7074  ).        except
+0001c0c0: 2065 7863 6570 7469 6f6e 732e 436f 736d   exceptions.Cosm
+0001c0d0: 6f73 4874 7470 5265 7370 6f6e 7365 4572  osHttpResponseEr
+0001c0e0: 726f 7220 6173 2065 3a0a 2020 2020 2020  ror as e:.      
+0001c0f0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+0001c100: 7445 7175 616c 2865 2e73 7461 7475 735f  tEqual(e.status_
+0001c110: 636f 6465 2c20 5374 6174 7573 436f 6465  code, StatusCode
+0001c120: 732e 4241 445f 5245 5155 4553 5429 0a0a  s.BAD_REQUEST)..
+0001c130: 2020 2020 2020 2020 234e 6567 6174 6976          #Negativ
+0001c140: 6520 7465 7374 202d 2061 7474 656d 7074  e test - attempt
+0001c150: 2074 6f20 7265 6d6f 7665 206e 6f6e 2d65   to remove non-e
+0001c160: 7869 7374 656e 7420 6669 656c 640a 2020  xistent field.  
+0001c170: 2020 2020 2020 6f70 6572 6174 696f 6e73        operations
+0001c180: 203d 205b 7b22 6f70 223a 2022 7265 6d6f   = [{"op": "remo
+0001c190: 7665 222c 2022 7061 7468 223a 2022 2f77  ve", "path": "/w
+0001c1a0: 726f 6e67 5f66 6965 6c64 227d 5d0a 2020  rong_field"}].  
+0001c1b0: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
+0001c1c0: 2020 2020 2020 2063 7265 6174 6564 5f63         created_c
+0001c1d0: 6f6e 7461 696e 6572 2e70 6174 6368 5f69  ontainer.patch_i
+0001c1e0: 7465 6d28 6974 656d 3d22 7061 7463 685f  tem(item="patch_
+0001c1f0: 6974 656d 222c 2070 6172 7469 7469 6f6e  item", partition
+0001c200: 5f6b 6579 3d22 7061 7463 685f 6974 656d  _key="patch_item
+0001c210: 5f70 6b22 2c20 7061 7463 685f 6f70 6572  _pk", patch_oper
+0001c220: 6174 696f 6e73 3d6f 7065 7261 7469 6f6e  ations=operation
+0001c230: 7329 0a20 2020 2020 2020 2065 7863 6570  s).        excep
+0001c240: 7420 6578 6365 7074 696f 6e73 2e43 6f73  t exceptions.Cos
+0001c250: 6d6f 7348 7474 7052 6573 706f 6e73 6545  mosHttpResponseE
+0001c260: 7272 6f72 2061 7320 653a 0a20 2020 2020  rror as e:.     
+0001c270: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+0001c280: 7274 4571 7561 6c28 652e 7374 6174 7573  rtEqual(e.status
+0001c290: 5f63 6f64 652c 2053 7461 7475 7343 6f64  _code, StatusCod
+0001c2a0: 6573 2e42 4144 5f52 4551 5545 5354 290a  es.BAD_REQUEST).
+0001c2b0: 0a20 2020 2020 2020 2023 4e65 6761 7469  .        #Negati
+0001c2c0: 7665 2074 6573 7420 2d20 6174 7465 6d70  ve test - attemp
+0001c2d0: 7420 746f 2069 6e63 7265 6d65 6e74 206e  t to increment n
+0001c2e0: 6f6e 2d6e 756d 6265 7220 6669 656c 640a  on-number field.
+0001c2f0: 2020 2020 2020 2020 6f70 6572 6174 696f          operatio
+0001c300: 6e73 203d 205b 7b22 6f70 223a 2022 696e  ns = [{"op": "in
+0001c310: 6372 222c 2022 7061 7468 223a 2022 2f63  cr", "path": "/c
+0001c320: 6f6d 7061 6e79 222c 2022 7661 6c75 6522  ompany", "value"
+0001c330: 3a20 337d 5d0a 2020 2020 2020 2020 7472  : 3}].        tr
+0001c340: 793a 0a20 2020 2020 2020 2020 2020 2063  y:.            c
+0001c350: 7265 6174 6564 5f63 6f6e 7461 696e 6572  reated_container
+0001c360: 2e70 6174 6368 5f69 7465 6d28 6974 656d  .patch_item(item
+0001c370: 3d22 7061 7463 685f 6974 656d 222c 2070  ="patch_item", p
+0001c380: 6172 7469 7469 6f6e 5f6b 6579 3d22 7061  artition_key="pa
+0001c390: 7463 685f 6974 656d 5f70 6b22 2c20 7061  tch_item_pk", pa
+0001c3a0: 7463 685f 6f70 6572 6174 696f 6e73 3d6f  tch_operations=o
+0001c3b0: 7065 7261 7469 6f6e 7329 0a20 2020 2020  perations).     
+0001c3c0: 2020 2065 7863 6570 7420 6578 6365 7074     except except
+0001c3d0: 696f 6e73 2e43 6f73 6d6f 7348 7474 7052  ions.CosmosHttpR
+0001c3e0: 6573 706f 6e73 6545 7272 6f72 2061 7320  esponseError as 
+0001c3f0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0001c400: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+0001c410: 652e 7374 6174 7573 5f63 6f64 652c 2053  e.status_code, S
+0001c420: 7461 7475 7343 6f64 6573 2e42 4144 5f52  tatusCodes.BAD_R
+0001c430: 4551 5545 5354 290a 0a20 2020 2020 2020  EQUEST)..       
+0001c440: 2023 4e65 6761 7469 7665 2074 6573 7420   #Negative test 
+0001c450: 2d20 6174 7465 6d70 7420 746f 206d 6f76  - attempt to mov
+0001c460: 6520 6672 6f6d 206e 6f6e 2d65 7869 7374  e from non-exist
+0001c470: 656e 7420 6669 656c 640a 2020 2020 2020  ent field.      
+0001c480: 2020 6f70 6572 6174 696f 6e73 203d 205b    operations = [
+0001c490: 7b22 6f70 223a 2022 6d6f 7665 222c 2022  {"op": "move", "
+0001c4a0: 6672 6f6d 223a 2022 2f77 726f 6e67 5f66  from": "/wrong_f
+0001c4b0: 6965 6c64 222c 2022 7061 7468 223a 2022  ield", "path": "
+0001c4c0: 2f6f 7468 6572 5f66 6965 6c64 227d 5d0a  /other_field"}].
+0001c4d0: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
+0001c4e0: 2020 2020 2020 2020 2063 7265 6174 6564           created
+0001c4f0: 5f63 6f6e 7461 696e 6572 2e70 6174 6368  _container.patch
+0001c500: 5f69 7465 6d28 6974 656d 3d22 7061 7463  _item(item="patc
+0001c510: 685f 6974 656d 222c 2070 6172 7469 7469  h_item", partiti
+0001c520: 6f6e 5f6b 6579 3d22 7061 7463 685f 6974  on_key="patch_it
+0001c530: 656d 5f70 6b22 2c20 7061 7463 685f 6f70  em_pk", patch_op
+0001c540: 6572 6174 696f 6e73 3d6f 7065 7261 7469  erations=operati
+0001c550: 6f6e 7329 0a20 2020 2020 2020 2065 7863  ons).        exc
+0001c560: 6570 7420 6578 6365 7074 696f 6e73 2e43  ept exceptions.C
+0001c570: 6f73 6d6f 7348 7474 7052 6573 706f 6e73  osmosHttpRespons
+0001c580: 6545 7272 6f72 2061 7320 653a 0a20 2020  eError as e:.   
+0001c590: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+0001c5a0: 7365 7274 4571 7561 6c28 652e 7374 6174  sertEqual(e.stat
+0001c5b0: 7573 5f63 6f64 652c 2053 7461 7475 7343  us_code, StatusC
+0001c5c0: 6f64 6573 2e42 4144 5f52 4551 5545 5354  odes.BAD_REQUEST
+0001c5d0: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
+0001c5e0: 636f 6e64 6974 696f 6e61 6c5f 7061 7463  conditional_patc
+0001c5f0: 6869 6e67 2873 656c 6629 3a0a 2020 2020  hing(self):.    
+0001c600: 2020 2020 6372 6561 7465 645f 636f 6e74      created_cont
+0001c610: 6169 6e65 7220 3d20 7365 6c66 2e64 6174  ainer = self.dat
+0001c620: 6162 6173 6546 6f72 5465 7374 2e63 7265  abaseForTest.cre
+0001c630: 6174 655f 636f 6e74 6169 6e65 725f 6966  ate_container_if
+0001c640: 5f6e 6f74 5f65 7869 7374 7328 6964 3d22  _not_exists(id="
+0001c650: 7061 7463 685f 6669 6c74 6572 5f63 6f6e  patch_filter_con
+0001c660: 7461 696e 6572 222c 2070 6172 7469 7469  tainer", partiti
+0001c670: 6f6e 5f6b 6579 3d50 6172 7469 7469 6f6e  on_key=Partition
+0001c680: 4b65 7928 7061 7468 3d22 2f70 6b22 2929  Key(path="/pk"))
+0001c690: 0a20 2020 2020 2020 2023 4372 6561 7465  .        #Create
+0001c6a0: 2069 7465 6d20 746f 2070 6174 6368 0a20   item to patch. 
+0001c6b0: 2020 2020 2020 2069 7465 6d20 3d20 7b0a         item = {.
+0001c6c0: 2020 2020 2020 2020 2020 2020 2269 6422              "id"
+0001c6d0: 3a20 2263 6f6e 6469 7469 6f6e 616c 5f70  : "conditional_p
+0001c6e0: 6174 6368 5f69 7465 6d22 2c0a 2020 2020  atch_item",.    
+0001c6f0: 2020 2020 2020 2020 2270 6b22 3a20 2270          "pk": "p
+0001c700: 6174 6368 5f69 7465 6d5f 706b 222c 0a20  atch_item_pk",. 
+0001c710: 2020 2020 2020 2020 2020 2022 7072 6f70             "prop
+0001c720: 223a 2022 7072 6f70 3122 2c0a 2020 2020  ": "prop1",.    
+0001c730: 2020 2020 2020 2020 2261 6464 7265 7373          "address
+0001c740: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
+0001c750: 2020 2020 2022 6369 7479 223a 2022 5265       "city": "Re
+0001c760: 646d 6f6e 6422 0a20 2020 2020 2020 2020  dmond".         
+0001c770: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
+0001c780: 2020 2263 6f6d 7061 6e79 223a 2022 4d69    "company": "Mi
+0001c790: 6372 6f73 6f66 7422 2c0a 2020 2020 2020  crosoft",.      
+0001c7a0: 2020 2020 2020 226e 756d 6265 7222 3a20        "number": 
+0001c7b0: 337d 0a20 2020 2020 2020 2063 7265 6174  3}.        creat
+0001c7c0: 6564 5f63 6f6e 7461 696e 6572 2e63 7265  ed_container.cre
+0001c7d0: 6174 655f 6974 656d 2869 7465 6d29 0a0a  ate_item(item)..
+0001c7e0: 2020 2020 2020 2020 2344 6566 696e 6520          #Define 
+0001c7f0: 7061 7463 6820 6f70 6572 6174 696f 6e73  patch operations
+0001c800: 0a20 2020 2020 2020 206f 7065 7261 7469  .        operati
+0001c810: 6f6e 7320 3d20 5b0a 2020 2020 2020 2020  ons = [.        
+0001c820: 2020 2020 7b22 6f70 223a 2022 6164 6422      {"op": "add"
+0001c830: 2c20 2270 6174 6822 3a20 222f 636f 6c6f  , "path": "/colo
+0001c840: 7222 2c20 2276 616c 7565 223a 2022 7965  r", "value": "ye
+0001c850: 6c6c 6f77 227d 2c0a 2020 2020 2020 2020  llow"},.        
+0001c860: 2020 2020 7b22 6f70 223a 2022 7265 6d6f      {"op": "remo
+0001c870: 7665 222c 2022 7061 7468 223a 2022 2f70  ve", "path": "/p
+0001c880: 726f 7022 7d2c 0a20 2020 2020 2020 2020  rop"},.         
+0001c890: 2020 207b 226f 7022 3a20 2272 6570 6c61     {"op": "repla
+0001c8a0: 6365 222c 2022 7061 7468 223a 2022 2f63  ce", "path": "/c
+0001c8b0: 6f6d 7061 6e79 222c 2022 7661 6c75 6522  ompany", "value"
+0001c8c0: 3a20 2243 6f73 6d6f 7344 4222 7d2c 0a20  : "CosmosDB"},. 
+0001c8d0: 2020 2020 2020 2020 2020 207b 226f 7022             {"op"
+0001c8e0: 3a20 2273 6574 222c 2022 7061 7468 223a  : "set", "path":
+0001c8f0: 2022 2f61 6464 7265 7373 2f6e 6577 5f63   "/address/new_c
+0001c900: 6974 7922 2c20 2276 616c 7565 223a 2022  ity", "value": "
+0001c910: 4174 6c61 6e74 6122 7d2c 0a20 2020 2020  Atlanta"},.     
+0001c920: 2020 2020 2020 207b 226f 7022 3a20 2269         {"op": "i
+0001c930: 6e63 7222 2c20 2270 6174 6822 3a20 222f  ncr", "path": "/
+0001c940: 6e75 6d62 6572 222c 2022 7661 6c75 6522  number", "value"
+0001c950: 3a20 377d 2c0a 2020 2020 2020 2020 2020  : 7},.          
+0001c960: 2020 7b22 6f70 223a 2022 6d6f 7665 222c    {"op": "move",
+0001c970: 2022 6672 6f6d 223a 2022 2f63 6f6c 6f72   "from": "/color
+0001c980: 222c 2022 7061 7468 223a 2022 2f66 6176  ", "path": "/fav
+0001c990: 6f72 6974 655f 636f 6c6f 7222 7d0a 2020  orite_color"}.  
+0001c9a0: 2020 2020 2020 5d0a 0a20 2020 2020 2020        ]..       
+0001c9b0: 2023 5275 6e20 7061 7463 6820 6f70 6572   #Run patch oper
+0001c9c0: 6174 696f 6e73 2077 6974 6820 7772 6f6e  ations with wron
+0001c9d0: 6720 6669 6c74 6572 0a20 2020 2020 2020  g filter.       
+0001c9e0: 206e 756d 5f66 616c 7365 203d 2069 7465   num_false = ite
+0001c9f0: 6d2e 6765 7428 226e 756d 6265 7222 2920  m.get("number") 
+0001ca00: 2b20 310a 2020 2020 2020 2020 6669 6c74  + 1.        filt
+0001ca10: 6572 5f70 7265 6469 6361 7465 203d 2022  er_predicate = "
+0001ca20: 6672 6f6d 2072 6f6f 7420 7768 6572 6520  from root where 
+0001ca30: 726f 6f74 2e6e 756d 6265 7220 3d20 2220  root.number = " 
+0001ca40: 2b20 7374 7228 6e75 6d5f 6661 6c73 6529  + str(num_false)
+0001ca50: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
+0001ca60: 2020 2020 2020 2020 2020 6372 6561 7465            create
+0001ca70: 645f 636f 6e74 6169 6e65 722e 7061 7463  d_container.patc
+0001ca80: 685f 6974 656d 2869 7465 6d3d 2263 6f6e  h_item(item="con
+0001ca90: 6469 7469 6f6e 616c 5f70 6174 6368 5f69  ditional_patch_i
+0001caa0: 7465 6d22 2c20 7061 7274 6974 696f 6e5f  tem", partition_
+0001cab0: 6b65 793d 2270 6174 6368 5f69 7465 6d5f  key="patch_item_
+0001cac0: 706b 222c 0a20 2020 2020 2020 2020 2020  pk",.           
+0001cad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cae0: 2020 2020 2020 2020 2020 2020 2020 7061                pa
+0001caf0: 7463 685f 6f70 6572 6174 696f 6e73 3d6f  tch_operations=o
+0001cb00: 7065 7261 7469 6f6e 732c 2066 696c 7465  perations, filte
+0001cb10: 725f 7072 6564 6963 6174 653d 6669 6c74  r_predicate=filt
+0001cb20: 6572 5f70 7265 6469 6361 7465 290a 2020  er_predicate).  
+0001cb30: 2020 2020 2020 6578 6365 7074 2065 7863        except exc
+0001cb40: 6570 7469 6f6e 732e 436f 736d 6f73 4874  eptions.CosmosHt
+0001cb50: 7470 5265 7370 6f6e 7365 4572 726f 7220  tpResponseError 
+0001cb60: 6173 2065 3a0a 2020 2020 2020 2020 2020  as e:.          
+0001cb70: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+0001cb80: 616c 2865 2e73 7461 7475 735f 636f 6465  al(e.status_code
+0001cb90: 2c20 5374 6174 7573 436f 6465 732e 5052  , StatusCodes.PR
+0001cba0: 4543 4f4e 4449 5449 4f4e 5f46 4149 4c45  ECONDITION_FAILE
+0001cbb0: 4429 0a0a 2020 2020 2020 2020 2352 756e  D)..        #Run
+0001cbc0: 2070 6174 6368 206f 7065 7261 7469 6f6e   patch operation
+0001cbd0: 7320 7769 7468 2063 6f72 7265 6374 2066  s with correct f
+0001cbe0: 696c 7465 720a 2020 2020 2020 2020 6669  ilter.        fi
+0001cbf0: 6c74 6572 5f70 7265 6469 6361 7465 203d  lter_predicate =
+0001cc00: 2022 6672 6f6d 2072 6f6f 7420 7768 6572   "from root wher
+0001cc10: 6520 726f 6f74 2e6e 756d 6265 7220 3d20  e root.number = 
+0001cc20: 2220 2b20 7374 7228 6974 656d 2e67 6574  " + str(item.get
+0001cc30: 2822 6e75 6d62 6572 2229 290a 2020 2020  ("number")).    
+0001cc40: 2020 2020 7061 7463 6865 645f 6974 656d      patched_item
+0001cc50: 203d 2063 7265 6174 6564 5f63 6f6e 7461   = created_conta
+0001cc60: 696e 6572 2e70 6174 6368 5f69 7465 6d28  iner.patch_item(
+0001cc70: 6974 656d 3d22 636f 6e64 6974 696f 6e61  item="conditiona
+0001cc80: 6c5f 7061 7463 685f 6974 656d 222c 2070  l_patch_item", p
+0001cc90: 6172 7469 7469 6f6e 5f6b 6579 3d22 7061  artition_key="pa
+0001cca0: 7463 685f 6974 656d 5f70 6b22 2c0a 2020  tch_item_pk",.  
+0001ccb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ccc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ccd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cce0: 2020 7061 7463 685f 6f70 6572 6174 696f    patch_operatio
+0001ccf0: 6e73 3d6f 7065 7261 7469 6f6e 732c 2066  ns=operations, f
+0001cd00: 696c 7465 725f 7072 6564 6963 6174 653d  ilter_predicate=
+0001cd10: 6669 6c74 6572 5f70 7265 6469 6361 7465  filter_predicate
+0001cd20: 290a 2020 2020 2020 2020 2356 6572 6966  ).        #Verif
+0001cd30: 7920 7265 7375 6c74 7320 6672 6f6d 2070  y results from p
+0001cd40: 6174 6368 206f 7065 7261 7469 6f6e 730a  atch operations.
+0001cd50: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+0001cd60: 6572 7454 7275 6528 7061 7463 6865 645f  ertTrue(patched_
+0001cd70: 6974 656d 2e67 6574 2822 636f 6c6f 7222  item.get("color"
+0001cd80: 2920 6973 204e 6f6e 6529 0a20 2020 2020  ) is None).     
+0001cd90: 2020 2073 656c 662e 6173 7365 7274 5472     self.assertTr
+0001cda0: 7565 2870 6174 6368 6564 5f69 7465 6d2e  ue(patched_item.
+0001cdb0: 6765 7428 2270 726f 7022 2920 6973 204e  get("prop") is N
+0001cdc0: 6f6e 6529 0a20 2020 2020 2020 2073 656c  one).        sel
+0001cdd0: 662e 6173 7365 7274 4571 7561 6c28 7061  f.assertEqual(pa
+0001cde0: 7463 6865 645f 6974 656d 2e67 6574 2822  tched_item.get("
+0001cdf0: 636f 6d70 616e 7922 292c 2022 436f 736d  company"), "Cosm
+0001ce00: 6f73 4442 2229 0a20 2020 2020 2020 2073  osDB").        s
+0001ce10: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+0001ce20: 7061 7463 6865 645f 6974 656d 2e67 6574  patched_item.get
+0001ce30: 2822 6164 6472 6573 7322 292e 6765 7428  ("address").get(
+0001ce40: 226e 6577 5f63 6974 7922 292c 2022 4174  "new_city"), "At
+0001ce50: 6c61 6e74 6122 290a 2020 2020 2020 2020  lanta").        
+0001ce60: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+0001ce70: 2870 6174 6368 6564 5f69 7465 6d2e 6765  (patched_item.ge
+0001ce80: 7428 226e 756d 6265 7222 292c 2031 3029  t("number"), 10)
+0001ce90: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+0001cea0: 7365 7274 4571 7561 6c28 7061 7463 6865  sertEqual(patche
+0001ceb0: 645f 6974 656d 2e67 6574 2822 6661 766f  d_item.get("favo
+0001cec0: 7269 7465 5f63 6f6c 6f72 2229 2c20 2279  rite_color"), "y
+0001ced0: 656c 6c6f 7722 290a 0a20 2020 2023 2054  ellow")..    # T
+0001cee0: 656d 706f 7261 7269 6c79 2063 6f6d 6d65  emporarily comme
+0001cef0: 6e74 696e 6720 616e 616c 7974 6963 616c  nting analytical
+0001cf00: 2073 746f 7261 6765 2074 6573 7473 2075   storage tests u
+0001cf10: 6e74 696c 2065 6d75 6c61 746f 7220 7375  ntil emulator su
+0001cf20: 7070 6f72 7420 636f 6d65 732e 0a20 2020  pport comes..   
+0001cf30: 2023 2064 6566 2074 6573 745f 6372 6561   # def test_crea
+0001cf40: 7465 5f63 6f6e 7461 696e 6572 5f77 6974  te_container_wit
+0001cf50: 685f 616e 616c 7974 6963 616c 5f73 746f  h_analytical_sto
+0001cf60: 7265 5f6f 6666 2873 656c 6629 3a0a 2020  re_off(self):.  
+0001cf70: 2020 2320 2020 2020 2320 646f 6e27 7420    #     # don't 
+0001cf80: 7275 6e20 7465 7374 2c20 666f 7220 7468  run test, for th
+0001cf90: 6520 7469 6d65 2062 6569 6e67 2c20 6966  e time being, if
+0001cfa0: 2072 756e 6e69 6e67 2061 6761 696e 7374   running against
+0001cfb0: 2074 6865 2065 6d75 6c61 746f 720a 2020   the emulator.  
+0001cfc0: 2020 2320 2020 2020 6966 2027 6c6f 6361    #     if 'loca
+0001cfd0: 6c68 6f73 7427 2069 6e20 7365 6c66 2e68  lhost' in self.h
+0001cfe0: 6f73 7420 6f72 2027 3132 372e 302e 302e  ost or '127.0.0.
+0001cff0: 3127 2069 6e20 7365 6c66 2e68 6f73 743a  1' in self.host:
+0001d000: 0a20 2020 2023 2020 2020 2020 2020 2072  .    #         r
+0001d010: 6574 7572 6e0a 0a20 2020 2023 2020 2020  eturn..    #    
+0001d020: 2063 7265 6174 6564 5f64 6220 3d20 7365   created_db = se
+0001d030: 6c66 2e64 6174 6162 6173 6546 6f72 5465  lf.databaseForTe
+0001d040: 7374 0a20 2020 2023 2020 2020 2063 6f6c  st.    #     col
+0001d050: 6c65 6374 696f 6e5f 6964 203d 2027 7465  lection_id = 'te
+0001d060: 7374 5f63 7265 6174 655f 636f 6e74 6169  st_create_contai
+0001d070: 6e65 725f 7769 7468 5f61 6e61 6c79 7469  ner_with_analyti
+0001d080: 6361 6c5f 7374 6f72 655f 6f66 665f 2720  cal_store_off_' 
+0001d090: 2b20 7374 7228 7575 6964 2e75 7569 6434  + str(uuid.uuid4
+0001d0a0: 2829 290a 2020 2020 2320 2020 2020 636f  ()).    #     co
+0001d0b0: 6c6c 6563 7469 6f6e 5f69 6e64 6578 696e  llection_indexin
+0001d0c0: 675f 706f 6c69 6379 203d 207b 2769 6e64  g_policy = {'ind
+0001d0d0: 6578 696e 674d 6f64 6527 3a20 2763 6f6e  exingMode': 'con
+0001d0e0: 7369 7374 656e 7427 7d0a 2020 2020 2320  sistent'}.    # 
+0001d0f0: 2020 2020 6372 6561 7465 645f 7265 636f      created_reco
+0001d100: 7264 6572 203d 2052 6563 6f72 6444 6961  rder = RecordDia
+0001d110: 676e 6f73 7469 6373 2829 0a20 2020 2023  gnostics().    #
+0001d120: 2020 2020 2063 7265 6174 6564 5f63 6f6c       created_col
+0001d130: 6c65 6374 696f 6e20 3d20 6372 6561 7465  lection = create
+0001d140: 645f 6462 2e63 7265 6174 655f 636f 6e74  d_db.create_cont
+0001d150: 6169 6e65 7228 6964 3d63 6f6c 6c65 6374  ainer(id=collect
+0001d160: 696f 6e5f 6964 2c0a 2020 2020 2320 2020  ion_id,.    #   
+0001d170: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001d180: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001d190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d1b0: 2020 2020 2020 2020 2020 2020 7061 7274              part
-0001d1c0: 6974 696f 6e5f 6b65 793d 5061 7274 6974  ition_key=Partit
-0001d1d0: 696f 6e4b 6579 2870 6174 683d 222f 706b  ionKey(path="/pk
-0001d1e0: 222c 206b 696e 643d 2248 6173 6822 292c  ", kind="Hash"),
-0001d1f0: 0a20 2020 2023 2020 2020 2020 2020 2020  .    #          
-0001d200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d230: 2020 2020 2020 2020 2020 7265 7370 6f6e            respon
-0001d240: 7365 5f68 6f6f 6b3d 6372 6561 7465 645f  se_hook=created_
-0001d250: 7265 636f 7264 6572 290a 2020 2020 2320  recorder).    # 
-0001d260: 2020 2020 7072 6f70 6572 7469 6573 203d      properties =
-0001d270: 2063 7265 6174 6564 5f63 6f6c 6c65 6374   created_collect
-0001d280: 696f 6e2e 7265 6164 2829 0a20 2020 2023  ion.read().    #
-0001d290: 2020 2020 2074 746c 5f6b 6579 203d 2022       ttl_key = "
-0001d2a0: 616e 616c 7974 6963 616c 5374 6f72 6167  analyticalStorag
-0001d2b0: 6554 746c 220a 2020 2020 2320 2020 2020  eTtl".    #     
-0001d2c0: 7365 6c66 2e61 7373 6572 7454 7275 6528  self.assertTrue(
-0001d2d0: 7474 6c5f 6b65 7920 696e 2070 726f 7065  ttl_key in prope
-0001d2e0: 7274 6965 7320 616e 6420 7072 6f70 6572  rties and proper
-0001d2f0: 7469 6573 5b74 746c 5f6b 6579 5d20 3d3d  ties[ttl_key] ==
-0001d300: 202d 3129 0a0a 2020 2020 2320 2020 2020   -1)..    #     
-0001d310: 2320 6e65 7874 2c20 7472 7920 7768 656e  # next, try when
-0001d320: 2077 6520 6b6e 6f77 2074 6865 2063 6f6e   we know the con
-0001d330: 7461 696e 6572 2044 4f45 5320 6578 6973  tainer DOES exis
-0001d340: 742e 2054 6869 7320 7761 7920 626f 7468  t. This way both
-0001d350: 2063 6f64 6520 7061 7468 7320 6172 6520   code paths are 
-0001d360: 7465 7374 6564 2e0a 2020 2020 2320 2020  tested..    #   
-0001d370: 2020 6372 6561 7465 645f 636f 6c6c 6563    created_collec
-0001d380: 7469 6f6e 203d 2063 7265 6174 6564 5f64  tion = created_d
-0001d390: 622e 6372 6561 7465 5f63 6f6e 7461 696e  b.create_contain
-0001d3a0: 6572 5f69 665f 6e6f 745f 6578 6973 7473  er_if_not_exists
-0001d3b0: 2869 643d 636f 6c6c 6563 7469 6f6e 5f69  (id=collection_i
-0001d3c0: 642c 0a20 2020 2023 2020 2020 2020 2020  d,.    #        
-0001d3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d400: 2020 2020 2020 2020 2020 2020 616e 616c              anal
-0001d410: 7974 6963 616c 5f73 746f 7261 6765 5f74  ytical_storage_t
-0001d420: 746c 3d2d 312c 0a20 2020 2023 2020 2020  tl=-1,.    #    
-0001d430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d470: 696e 6465 7869 6e67 5f70 6f6c 6963 793d  indexing_policy=
-0001d480: 636f 6c6c 6563 7469 6f6e 5f69 6e64 6578  collection_index
-0001d490: 696e 675f 706f 6c69 6379 2c0a 2020 2020  ing_policy,.    
-0001d4a0: 2320 2020 2020 2020 2020 2020 2020 2020  #               
-0001d4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d4e0: 2020 2020 2070 6172 7469 7469 6f6e 5f6b       partition_k
-0001d4f0: 6579 3d50 6172 7469 7469 6f6e 4b65 7928  ey=PartitionKey(
-0001d500: 7061 7468 3d22 2f70 6b22 2c20 6b69 6e64  path="/pk", kind
-0001d510: 3d22 4861 7368 2229 2c0a 2020 2020 2320  ="Hash"),.    # 
-0001d520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d560: 2020 2072 6573 706f 6e73 655f 686f 6f6b     response_hook
-0001d570: 3d63 7265 6174 6564 5f72 6563 6f72 6465  =created_recorde
-0001d580: 7229 0a20 2020 2023 2020 2020 2070 726f  r).    #     pro
-0001d590: 7065 7274 6965 7320 3d20 6372 6561 7465  perties = create
-0001d5a0: 645f 636f 6c6c 6563 7469 6f6e 2e72 6561  d_collection.rea
-0001d5b0: 6428 290a 2020 2020 2320 2020 2020 7474  d().    #     tt
-0001d5c0: 6c5f 6b65 7920 3d20 2261 6e61 6c79 7469  l_key = "analyti
-0001d5d0: 6361 6c53 746f 7261 6765 5474 6c22 0a20  calStorageTtl". 
-0001d5e0: 2020 2023 2020 2020 2073 656c 662e 6173     #     self.as
-0001d5f0: 7365 7274 5472 7565 2874 746c 5f6b 6579  sertTrue(ttl_key
-0001d600: 2069 6e20 7072 6f70 6572 7469 6573 2061   in properties a
-0001d610: 6e64 2070 726f 7065 7274 6965 735b 7474  nd properties[tt
-0001d620: 6c5f 6b65 795d 203d 3d20 2d31 290a 0a20  l_key] == -1).. 
-0001d630: 2020 2064 6566 205f 4d6f 636b 4578 6563     def _MockExec
-0001d640: 7574 6546 756e 6374 696f 6e28 7365 6c66  uteFunction(self
-0001d650: 2c20 6675 6e63 7469 6f6e 2c20 2a61 7267  , function, *arg
-0001d660: 732c 202a 2a6b 7761 7267 7329 3a0a 2020  s, **kwargs):.  
-0001d670: 2020 2020 2020 7365 6c66 2e6c 6173 745f        self.last_
-0001d680: 6865 6164 6572 732e 6170 7065 6e64 2861  headers.append(a
-0001d690: 7267 735b 345d 2e68 6561 6465 7273 5b48  rgs[4].headers[H
-0001d6a0: 7474 7048 6561 6465 7273 2e50 6172 7469  ttpHeaders.Parti
-0001d6b0: 7469 6f6e 4b65 795d 0a20 2020 2020 2020  tionKey].       
+0001d1a0: 2020 2069 6e64 6578 696e 675f 706f 6c69     indexing_poli
+0001d1b0: 6379 3d63 6f6c 6c65 6374 696f 6e5f 696e  cy=collection_in
+0001d1c0: 6465 7869 6e67 5f70 6f6c 6963 792c 0a20  dexing_policy,. 
+0001d1d0: 2020 2023 2020 2020 2020 2020 2020 2020     #            
+0001d1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d200: 2020 2020 2020 2020 2020 7061 7274 6974            partit
+0001d210: 696f 6e5f 6b65 793d 5061 7274 6974 696f  ion_key=Partitio
+0001d220: 6e4b 6579 2870 6174 683d 222f 706b 222c  nKey(path="/pk",
+0001d230: 206b 696e 643d 2248 6173 6822 292c 200a   kind="Hash"), .
+0001d240: 2020 2020 2320 2020 2020 2020 2020 2020      #           
+0001d250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d270: 2020 2020 2020 2020 2020 2072 6573 706f             respo
+0001d280: 6e73 655f 686f 6f6b 3d63 7265 6174 6564  nse_hook=created
+0001d290: 5f72 6563 6f72 6465 7229 0a20 2020 2023  _recorder).    #
+0001d2a0: 2020 2020 2070 726f 7065 7274 6965 7320       properties 
+0001d2b0: 3d20 6372 6561 7465 645f 636f 6c6c 6563  = created_collec
+0001d2c0: 7469 6f6e 2e72 6561 6428 290a 2020 2020  tion.read().    
+0001d2d0: 2320 2020 2020 7474 6c5f 6b65 7920 3d20  #     ttl_key = 
+0001d2e0: 2261 6e61 6c79 7469 6361 6c53 746f 7261  "analyticalStora
+0001d2f0: 6765 5474 6c22 0a20 2020 2023 2020 2020  geTtl".    #    
+0001d300: 2073 656c 662e 6173 7365 7274 5472 7565   self.assertTrue
+0001d310: 2874 746c 5f6b 6579 206e 6f74 2069 6e20  (ttl_key not in 
+0001d320: 7072 6f70 6572 7469 6573 206f 7220 7072  properties or pr
+0001d330: 6f70 6572 7469 6573 5b74 746c 5f6b 6579  operties[ttl_key
+0001d340: 5d20 3d3d 204e 6f6e 6529 0a0a 2020 2020  ] == None)..    
+0001d350: 2320 6465 6620 7465 7374 5f63 7265 6174  # def test_creat
+0001d360: 655f 636f 6e74 6169 6e65 725f 7769 7468  e_container_with
+0001d370: 5f61 6e61 6c79 7469 6361 6c5f 7374 6f72  _analytical_stor
+0001d380: 655f 6f6e 2873 656c 6629 3a0a 2020 2020  e_on(self):.    
+0001d390: 2320 2020 2020 2320 646f 6e27 7420 7275  #     # don't ru
+0001d3a0: 6e20 7465 7374 2c20 666f 7220 7468 6520  n test, for the 
+0001d3b0: 7469 6d65 2062 6569 6e67 2c20 6966 2072  time being, if r
+0001d3c0: 756e 6e69 6e67 2061 6761 696e 7374 2074  unning against t
+0001d3d0: 6865 2065 6d75 6c61 746f 720a 2020 2020  he emulator.    
+0001d3e0: 2320 2020 2020 6966 2027 6c6f 6361 6c68  #     if 'localh
+0001d3f0: 6f73 7427 2069 6e20 7365 6c66 2e68 6f73  ost' in self.hos
+0001d400: 7420 6f72 2027 3132 372e 302e 302e 3127  t or '127.0.0.1'
+0001d410: 2069 6e20 7365 6c66 2e68 6f73 743a 0a20   in self.host:. 
+0001d420: 2020 2023 2020 2020 2020 2020 2072 6574     #         ret
+0001d430: 7572 6e0a 0a20 2020 2023 2020 2020 2063  urn..    #     c
+0001d440: 7265 6174 6564 5f64 6220 3d20 7365 6c66  reated_db = self
+0001d450: 2e64 6174 6162 6173 6546 6f72 5465 7374  .databaseForTest
+0001d460: 0a20 2020 2023 2020 2020 2063 6f6c 6c65  .    #     colle
+0001d470: 6374 696f 6e5f 6964 203d 2027 7465 7374  ction_id = 'test
+0001d480: 5f63 7265 6174 655f 636f 6e74 6169 6e65  _create_containe
+0001d490: 725f 7769 7468 5f61 6e61 6c79 7469 6361  r_with_analytica
+0001d4a0: 6c5f 7374 6f72 655f 6f6e 5f27 202b 2073  l_store_on_' + s
+0001d4b0: 7472 2875 7569 642e 7575 6964 3428 2929  tr(uuid.uuid4())
+0001d4c0: 0a20 2020 2023 2020 2020 2063 6f6c 6c65  .    #     colle
+0001d4d0: 6374 696f 6e5f 696e 6465 7869 6e67 5f70  ction_indexing_p
+0001d4e0: 6f6c 6963 7920 3d20 7b27 696e 6465 7869  olicy = {'indexi
+0001d4f0: 6e67 4d6f 6465 273a 2027 636f 6e73 6973  ngMode': 'consis
+0001d500: 7465 6e74 277d 0a20 2020 2023 2020 2020  tent'}.    #    
+0001d510: 2063 7265 6174 6564 5f72 6563 6f72 6465   created_recorde
+0001d520: 7220 3d20 5265 636f 7264 4469 6167 6e6f  r = RecordDiagno
+0001d530: 7374 6963 7328 290a 2020 2020 2320 2020  stics().    #   
+0001d540: 2020 6372 6561 7465 645f 636f 6c6c 6563    created_collec
+0001d550: 7469 6f6e 203d 2063 7265 6174 6564 5f64  tion = created_d
+0001d560: 622e 6372 6561 7465 5f63 6f6e 7461 696e  b.create_contain
+0001d570: 6572 2869 643d 636f 6c6c 6563 7469 6f6e  er(id=collection
+0001d580: 5f69 642c 0a20 2020 2023 2020 2020 2020  _id,.    #      
+0001d590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d5c0: 616e 616c 7974 6963 616c 5f73 746f 7261  analytical_stora
+0001d5d0: 6765 5f74 746c 3d2d 312c 0a20 2020 2023  ge_ttl=-1,.    #
+0001d5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d610: 2020 2020 2020 696e 6465 7869 6e67 5f70        indexing_p
+0001d620: 6f6c 6963 793d 636f 6c6c 6563 7469 6f6e  olicy=collection
+0001d630: 5f69 6e64 6578 696e 675f 706f 6c69 6379  _indexing_policy
+0001d640: 2c0a 2020 2020 2320 2020 2020 2020 2020  ,.    #         
+0001d650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d670: 2020 2020 2020 2020 2020 2020 2070 6172               par
+0001d680: 7469 7469 6f6e 5f6b 6579 3d50 6172 7469  tition_key=Parti
+0001d690: 7469 6f6e 4b65 7928 7061 7468 3d22 2f70  tionKey(path="/p
+0001d6a0: 6b22 2c20 6b69 6e64 3d22 4861 7368 2229  k", kind="Hash")
+0001d6b0: 2c20 0a20 2020 2023 2020 2020 2020 2020  , .    #        
 0001d6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d6d0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0001d6e0: 4874 7470 4865 6164 6572 732e 5061 7274  HttpHeaders.Part
-0001d6f0: 6974 696f 6e4b 6579 2069 6e20 6172 6773  itionKey in args
-0001d700: 5b34 5d2e 6865 6164 6572 7320 656c 7365  [4].headers else
-0001d710: 2027 2729 0a20 2020 2020 2020 2072 6574   '').        ret
-0001d720: 7572 6e20 7365 6c66 2e4f 7269 6769 6e61  urn self.Origina
-0001d730: 6c45 7865 6375 7465 4675 6e63 7469 6f6e  lExecuteFunction
-0001d740: 2866 756e 6374 696f 6e2c 202a 6172 6773  (function, *args
-0001d750: 2c20 2a2a 6b77 6172 6773 290a 0a69 6620  , **kwargs)..if 
-0001d760: 5f5f 6e61 6d65 5f5f 203d 3d20 275f 5f6d  __name__ == '__m
-0001d770: 6169 6e5f 5f27 3a0a 2020 2020 7472 793a  ain__':.    try:
-0001d780: 0a20 2020 2020 2020 2075 6e69 7474 6573  .        unittes
-0001d790: 742e 6d61 696e 2829 0a20 2020 2065 7863  t.main().    exc
-0001d7a0: 6570 7420 5379 7374 656d 4578 6974 2061  ept SystemExit a
-0001d7b0: 7320 696e 7374 3a0a 2020 2020 2020 2020  s inst:.        
-0001d7c0: 6966 2069 6e73 742e 6172 6773 5b30 5d20  if inst.args[0] 
-0001d7d0: 6973 2054 7275 653a 2020 2320 7261 6973  is True:  # rais
-0001d7e0: 6564 2062 7920 7379 732e 6578 6974 2854  ed by sys.exit(T
-0001d7f0: 7275 6529 2077 6865 6e20 7465 7374 7320  rue) when tests 
-0001d800: 6661 696c 6564 0a20 2020 2020 2020 2020  failed.         
-0001d810: 2020 2072 6169 7365 0a                      raise.
+0001d6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d6e0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+0001d6f0: 7370 6f6e 7365 5f68 6f6f 6b3d 6372 6561  sponse_hook=crea
+0001d700: 7465 645f 7265 636f 7264 6572 290a 2020  ted_recorder).  
+0001d710: 2020 2320 2020 2020 7072 6f70 6572 7469    #     properti
+0001d720: 6573 203d 2063 7265 6174 6564 5f63 6f6c  es = created_col
+0001d730: 6c65 6374 696f 6e2e 7265 6164 2829 0a20  lection.read(). 
+0001d740: 2020 2023 2020 2020 2074 746c 5f6b 6579     #     ttl_key
+0001d750: 203d 2022 616e 616c 7974 6963 616c 5374   = "analyticalSt
+0001d760: 6f72 6167 6554 746c 220a 2020 2020 2320  orageTtl".    # 
+0001d770: 2020 2020 7365 6c66 2e61 7373 6572 7454      self.assertT
+0001d780: 7275 6528 7474 6c5f 6b65 7920 696e 2070  rue(ttl_key in p
+0001d790: 726f 7065 7274 6965 7320 616e 6420 7072  roperties and pr
+0001d7a0: 6f70 6572 7469 6573 5b74 746c 5f6b 6579  operties[ttl_key
+0001d7b0: 5d20 3d3d 202d 3129 0a0a 2020 2020 2320  ] == -1)..    # 
+0001d7c0: 6465 6620 7465 7374 5f63 7265 6174 655f  def test_create_
+0001d7d0: 636f 6e74 6169 6e65 725f 6966 5f6e 6f74  container_if_not
+0001d7e0: 5f65 7869 7374 735f 7769 7468 5f61 6e61  _exists_with_ana
+0001d7f0: 6c79 7469 6361 6c5f 7374 6f72 655f 6f6e  lytical_store_on
+0001d800: 2873 656c 6629 3a0a 2020 2020 2320 2020  (self):.    #   
+0001d810: 2020 2320 646f 6e27 7420 7275 6e20 7465    # don't run te
+0001d820: 7374 2c20 666f 7220 7468 6520 7469 6d65  st, for the time
+0001d830: 2062 6569 6e67 2c20 6966 2072 756e 6e69   being, if runni
+0001d840: 6e67 2061 6761 696e 7374 2074 6865 2065  ng against the e
+0001d850: 6d75 6c61 746f 720a 2020 2020 2320 2020  mulator.    #   
+0001d860: 2020 6966 2027 6c6f 6361 6c68 6f73 7427    if 'localhost'
+0001d870: 2069 6e20 7365 6c66 2e68 6f73 7420 6f72   in self.host or
+0001d880: 2027 3132 372e 302e 302e 3127 2069 6e20   '127.0.0.1' in 
+0001d890: 7365 6c66 2e68 6f73 743a 0a20 2020 2023  self.host:.    #
+0001d8a0: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+0001d8b0: 0a20 2020 2023 2020 2020 2023 2066 6972  .    #     # fir
+0001d8c0: 7374 2c20 7472 7920 7768 656e 2077 6520  st, try when we 
+0001d8d0: 6b6e 6f77 2074 6865 2063 6f6e 7461 696e  know the contain
+0001d8e0: 6572 2064 6f65 736e 2774 2065 7869 7374  er doesn't exist
+0001d8f0: 2e0a 2020 2020 2320 2020 2020 6372 6561  ..    #     crea
+0001d900: 7465 645f 6462 203d 2073 656c 662e 6461  ted_db = self.da
+0001d910: 7461 6261 7365 466f 7254 6573 740a 2020  tabaseForTest.  
+0001d920: 2020 2320 2020 2020 636f 6c6c 6563 7469    #     collecti
+0001d930: 6f6e 5f69 6420 3d20 2774 6573 745f 6372  on_id = 'test_cr
+0001d940: 6561 7465 5f63 6f6e 7461 696e 6572 5f69  eate_container_i
+0001d950: 665f 6e6f 745f 6578 6973 7473 5f77 6974  f_not_exists_wit
+0001d960: 685f 616e 616c 7974 6963 616c 5f73 746f  h_analytical_sto
+0001d970: 7265 5f6f 6e5f 2720 2b20 7374 7228 7575  re_on_' + str(uu
+0001d980: 6964 2e75 7569 6434 2829 290a 2020 2020  id.uuid4()).    
+0001d990: 2320 2020 2020 636f 6c6c 6563 7469 6f6e  #     collection
+0001d9a0: 5f69 6e64 6578 696e 675f 706f 6c69 6379  _indexing_policy
+0001d9b0: 203d 207b 2769 6e64 6578 696e 674d 6f64   = {'indexingMod
+0001d9c0: 6527 3a20 2763 6f6e 7369 7374 656e 7427  e': 'consistent'
+0001d9d0: 7d0a 2020 2020 2320 2020 2020 6372 6561  }.    #     crea
+0001d9e0: 7465 645f 7265 636f 7264 6572 203d 2052  ted_recorder = R
+0001d9f0: 6563 6f72 6444 6961 676e 6f73 7469 6373  ecordDiagnostics
+0001da00: 2829 0a20 2020 2023 2020 2020 2063 7265  ().    #     cre
+0001da10: 6174 6564 5f63 6f6c 6c65 6374 696f 6e20  ated_collection 
+0001da20: 3d20 6372 6561 7465 645f 6462 2e63 7265  = created_db.cre
+0001da30: 6174 655f 636f 6e74 6169 6e65 725f 6966  ate_container_if
+0001da40: 5f6e 6f74 5f65 7869 7374 7328 6964 3d63  _not_exists(id=c
+0001da50: 6f6c 6c65 6374 696f 6e5f 6964 2c0a 2020  ollection_id,.  
+0001da60: 2020 2320 2020 2020 2020 2020 2020 2020    #             
+0001da70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001da80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001da90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001daa0: 2020 2020 2020 2061 6e61 6c79 7469 6361         analytica
+0001dab0: 6c5f 7374 6f72 6167 655f 7474 6c3d 2d31  l_storage_ttl=-1
+0001dac0: 2c0a 2020 2020 2320 2020 2020 2020 2020  ,.    #         
+0001dad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001daf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001db00: 2020 2020 2020 2020 2020 2069 6e64 6578             index
+0001db10: 696e 675f 706f 6c69 6379 3d63 6f6c 6c65  ing_policy=colle
+0001db20: 6374 696f 6e5f 696e 6465 7869 6e67 5f70  ction_indexing_p
+0001db30: 6f6c 6963 792c 0a20 2020 2023 2020 2020  olicy,.    #    
+0001db40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001db50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001db60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001db70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001db80: 7061 7274 6974 696f 6e5f 6b65 793d 5061  partition_key=Pa
+0001db90: 7274 6974 696f 6e4b 6579 2870 6174 683d  rtitionKey(path=
+0001dba0: 222f 706b 222c 206b 696e 643d 2248 6173  "/pk", kind="Has
+0001dbb0: 6822 292c 0a20 2020 2023 2020 2020 2020  h"),.    #      
+0001dbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dbf0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+0001dc00: 7370 6f6e 7365 5f68 6f6f 6b3d 6372 6561  sponse_hook=crea
+0001dc10: 7465 645f 7265 636f 7264 6572 290a 2020  ted_recorder).  
+0001dc20: 2020 2320 2020 2020 7072 6f70 6572 7469    #     properti
+0001dc30: 6573 203d 2063 7265 6174 6564 5f63 6f6c  es = created_col
+0001dc40: 6c65 6374 696f 6e2e 7265 6164 2829 0a20  lection.read(). 
+0001dc50: 2020 2023 2020 2020 2074 746c 5f6b 6579     #     ttl_key
+0001dc60: 203d 2022 616e 616c 7974 6963 616c 5374   = "analyticalSt
+0001dc70: 6f72 6167 6554 746c 220a 2020 2020 2320  orageTtl".    # 
+0001dc80: 2020 2020 7365 6c66 2e61 7373 6572 7454      self.assertT
+0001dc90: 7275 6528 7474 6c5f 6b65 7920 696e 2070  rue(ttl_key in p
+0001dca0: 726f 7065 7274 6965 7320 616e 6420 7072  roperties and pr
+0001dcb0: 6f70 6572 7469 6573 5b74 746c 5f6b 6579  operties[ttl_key
+0001dcc0: 5d20 3d3d 202d 3129 0a0a 2020 2020 2320  ] == -1)..    # 
+0001dcd0: 2020 2020 2320 6e65 7874 2c20 7472 7920      # next, try 
+0001dce0: 7768 656e 2077 6520 6b6e 6f77 2074 6865  when we know the
+0001dcf0: 2063 6f6e 7461 696e 6572 2044 4f45 5320   container DOES 
+0001dd00: 6578 6973 742e 2054 6869 7320 7761 7920  exist. This way 
+0001dd10: 626f 7468 2063 6f64 6520 7061 7468 7320  both code paths 
+0001dd20: 6172 6520 7465 7374 6564 2e0a 2020 2020  are tested..    
+0001dd30: 2320 2020 2020 6372 6561 7465 645f 636f  #     created_co
+0001dd40: 6c6c 6563 7469 6f6e 203d 2063 7265 6174  llection = creat
+0001dd50: 6564 5f64 622e 6372 6561 7465 5f63 6f6e  ed_db.create_con
+0001dd60: 7461 696e 6572 5f69 665f 6e6f 745f 6578  tainer_if_not_ex
+0001dd70: 6973 7473 2869 643d 636f 6c6c 6563 7469  ists(id=collecti
+0001dd80: 6f6e 5f69 642c 0a20 2020 2023 2020 2020  on_id,.    #    
+0001dd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ddb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ddc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ddd0: 616e 616c 7974 6963 616c 5f73 746f 7261  analytical_stora
+0001dde0: 6765 5f74 746c 3d2d 312c 0a20 2020 2023  ge_ttl=-1,.    #
+0001ddf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001de00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001de10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001de20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001de30: 2020 2020 696e 6465 7869 6e67 5f70 6f6c      indexing_pol
+0001de40: 6963 793d 636f 6c6c 6563 7469 6f6e 5f69  icy=collection_i
+0001de50: 6e64 6578 696e 675f 706f 6c69 6379 2c0a  ndexing_policy,.
+0001de60: 2020 2020 2320 2020 2020 2020 2020 2020      #           
+0001de70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001de80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001de90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dea0: 2020 2020 2020 2020 2070 6172 7469 7469           partiti
+0001deb0: 6f6e 5f6b 6579 3d50 6172 7469 7469 6f6e  on_key=Partition
+0001dec0: 4b65 7928 7061 7468 3d22 2f70 6b22 2c20  Key(path="/pk", 
+0001ded0: 6b69 6e64 3d22 4861 7368 2229 2c0a 2020  kind="Hash"),.  
+0001dee0: 2020 2320 2020 2020 2020 2020 2020 2020    #             
+0001def0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001df00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001df10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001df20: 2020 2020 2020 2072 6573 706f 6e73 655f         response_
+0001df30: 686f 6f6b 3d63 7265 6174 6564 5f72 6563  hook=created_rec
+0001df40: 6f72 6465 7229 0a20 2020 2023 2020 2020  order).    #    
+0001df50: 2070 726f 7065 7274 6965 7320 3d20 6372   properties = cr
+0001df60: 6561 7465 645f 636f 6c6c 6563 7469 6f6e  eated_collection
+0001df70: 2e72 6561 6428 290a 2020 2020 2320 2020  .read().    #   
+0001df80: 2020 7474 6c5f 6b65 7920 3d20 2261 6e61    ttl_key = "ana
+0001df90: 6c79 7469 6361 6c53 746f 7261 6765 5474  lyticalStorageTt
+0001dfa0: 6c22 0a20 2020 2023 2020 2020 2073 656c  l".    #     sel
+0001dfb0: 662e 6173 7365 7274 5472 7565 2874 746c  f.assertTrue(ttl
+0001dfc0: 5f6b 6579 2069 6e20 7072 6f70 6572 7469  _key in properti
+0001dfd0: 6573 2061 6e64 2070 726f 7065 7274 6965  es and propertie
+0001dfe0: 735b 7474 6c5f 6b65 795d 203d 3d20 2d31  s[ttl_key] == -1
+0001dff0: 290a 0a20 2020 2064 6566 205f 4d6f 636b  )..    def _Mock
+0001e000: 4578 6563 7574 6546 756e 6374 696f 6e28  ExecuteFunction(
+0001e010: 7365 6c66 2c20 6675 6e63 7469 6f6e 2c20  self, function, 
+0001e020: 2a61 7267 732c 202a 2a6b 7761 7267 7329  *args, **kwargs)
+0001e030: 3a0a 2020 2020 2020 2020 7365 6c66 2e6c  :.        self.l
+0001e040: 6173 745f 6865 6164 6572 732e 6170 7065  ast_headers.appe
+0001e050: 6e64 2861 7267 735b 345d 2e68 6561 6465  nd(args[4].heade
+0001e060: 7273 5b48 7474 7048 6561 6465 7273 2e50  rs[HttpHeaders.P
+0001e070: 6172 7469 7469 6f6e 4b65 795d 0a20 2020  artitionKey].   
+0001e080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e0a0: 2069 6620 4874 7470 4865 6164 6572 732e   if HttpHeaders.
+0001e0b0: 5061 7274 6974 696f 6e4b 6579 2069 6e20  PartitionKey in 
+0001e0c0: 6172 6773 5b34 5d2e 6865 6164 6572 7320  args[4].headers 
+0001e0d0: 656c 7365 2027 2729 0a20 2020 2020 2020  else '').       
+0001e0e0: 2072 6574 7572 6e20 7365 6c66 2e4f 7269   return self.Ori
+0001e0f0: 6769 6e61 6c45 7865 6375 7465 4675 6e63  ginalExecuteFunc
+0001e100: 7469 6f6e 2866 756e 6374 696f 6e2c 202a  tion(function, *
+0001e110: 6172 6773 2c20 2a2a 6b77 6172 6773 290a  args, **kwargs).
+0001e120: 0a69 6620 5f5f 6e61 6d65 5f5f 203d 3d20  .if __name__ == 
+0001e130: 275f 5f6d 6169 6e5f 5f27 3a0a 2020 2020  '__main__':.    
+0001e140: 7472 793a 0a20 2020 2020 2020 2075 6e69  try:.        uni
+0001e150: 7474 6573 742e 6d61 696e 2829 0a20 2020  ttest.main().   
+0001e160: 2065 7863 6570 7420 5379 7374 656d 4578   except SystemEx
+0001e170: 6974 2061 7320 696e 7374 3a0a 2020 2020  it as inst:.    
+0001e180: 2020 2020 6966 2069 6e73 742e 6172 6773      if inst.args
+0001e190: 5b30 5d20 6973 2054 7275 653a 2020 2320  [0] is True:  # 
+0001e1a0: 7261 6973 6564 2062 7920 7379 732e 6578  raised by sys.ex
+0001e1b0: 6974 2854 7275 6529 2077 6865 6e20 7465  it(True) when te
+0001e1c0: 7374 7320 6661 696c 6564 0a20 2020 2020  sts failed.     
+0001e1d0: 2020 2020 2020 2072 6169 7365 0a                raise.
```

## Comparing `azure-cosmos-4.4.0b1/test/test_globaldb.py` & `azure-cosmos-4.4.0b2/test/test_globaldb.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/test/routing/test_routing_map_provider.py` & `azure-cosmos-4.4.0b2/test/routing/test_routing_map_provider.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/test/routing/test_collection_routing_map.py` & `azure-cosmos-4.4.0b2/test/routing/test_collection_routing_map.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/test/routing/__init__.py` & `azure-cosmos-4.4.0b2/test/routing/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b1/azure_cosmos.egg-info/PKG-INFO` & `azure-cosmos-4.4.0b2/azure_cosmos.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: azure-cosmos
-Version: 4.4.0b1
+Version: 4.4.0b2
 Summary: Microsoft Azure Cosmos Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: askdocdb@microsoft.com
 Maintainer: Microsoft
 Maintainer-email: askdocdb@microsoft.com
 License: MIT License
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -686,14 +686,25 @@
 However, if you desire to use the CosmosHttpLoggingPolicy to obtain additional information, the `enable_diagnostics_logging` argument needs to be passed in at the client constructor.
 ```python
 # This example enables the CosmosHttpLoggingPolicy and uses it with the `logger` passed in to the `create_database` request.
 client = CosmosClient(URL, credential=KEY, enable_diagnostics_logging=True)
 database = client.create_database(DATABASE_NAME, logger=logger)
 ```
 
+### Telemetry
+Azure Core provides the ability for our Python SDKs to use OpenTelemetry with them. The only packages that need to be installed
+to use this functionality are the following:
+```bash
+pip install azure-core-tracing-opentelemetry
+pip install opentelemetry-sdk
+```
+For more information on this, we recommend taking a look at this [document](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/core/azure-core-tracing-opentelemetry/README.md) 
+from Azure Core describing how to set it up. We have also added a [sample file][telemetry_sample] to show how it can
+be used with our SDK. This works the same way regardless of the Cosmos client you are using.
+
 ## Next steps
 
 For more extensive documentation on the Cosmos DB service, see the [Azure Cosmos DB documentation][cosmos_docs] on docs.microsoft.com.
 
 <!-- LINKS -->
 [azure_cli]: https://docs.microsoft.com/cli/azure
 [azure_portal]: https://portal.azure.com
@@ -726,14 +737,15 @@
 [ref_httpfailure]: https://aka.ms/azsdk-python-cosmos-ref-http-failure
 [sample_database_mgmt]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/cosmos/azure-cosmos/samples/database_management.py
 [sample_document_mgmt]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/cosmos/azure-cosmos/samples/document_management.py
 [sample_examples_misc]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/cosmos/azure-cosmos/samples/examples.py
 [source_code]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/cosmos/azure-cosmos
 [venv]: https://docs.python.org/3/library/venv.html
 [virtualenv]: https://virtualenv.pypa.io
+[telemetry_sample]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/cosmos/azure-cosmos/samples/tracing_open_telemetry.py
 
 ## Contributing
 
 This project welcomes contributions and suggestions.  Most contributions require you to agree to a
 Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
 the rights to use your contribution. For details, visit https://cla.microsoft.com.
 
@@ -744,21 +756,31 @@
 This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
 For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
 contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
 
 
 ## Release History
 
+### 4.4.0b2 (2023-05-22)
+
+#### Features Added
+* Added conditional patching for Patch operations. See [PR 30455](https://github.com/Azure/azure-sdk-for-python/pull/30455).
+
+#### Bugs Fixed
+* Fixed bug with non english locales causing an error with the RFC 1123 Date Format. See [PR 30125](https://github.com/Azure/azure-sdk-for-python/pull/30125).
+
+#### Other Changes
+* Refactoring of our client `connection_timeout` and `request_timeout` configurations. See [PR 30171](https://github.com/Azure/azure-sdk-for-python/pull/30171).
+
 ### 4.4.0b1 (2023-04-11)
 
 #### Features Added
  - Added **preview** delete all items by partition key functionality. See [PR 29186](https://github.com/Azure/azure-sdk-for-python/pull/29186).
  - Added **preview** partial document update (Patch API) functionality and container methods for patching items with operations. See [PR 29497](https://github.com/Azure/azure-sdk-for-python/pull/29497). For more information on Patch, please see [Azure Cosmos DB Partial Document Update](https://learn.microsoft.com/azure/cosmos-db/partial-document-update).
 
-
 #### Bugs Fixed
 * Fixed bug in method `create_container_if_not_exists()` of async database client for unexpected kwargs being passed into `read()` method used internally. See [PR 29136](https://github.com/Azure/azure-sdk-for-python/pull/29136).
 * Fixed bug with method `query_items()` of our async container class, where partition key and cross partition headers would both be set when using partition keys. See [PR 29366](https://github.com/Azure/azure-sdk-for-python/pull/29366/).
 * Fixed bug with client not properly surfacing errors for invalid credentials and identities with insufficient permissions. Users running into 'NoneType has no attribute ConsistencyPolicy' errors when initializing their clients will now see proper authentication exceptions. See [PR 29256](https://github.com/Azure/azure-sdk-for-python/pull/29256).
 
 #### Other Changes
 * Removed use of `six` package within the SDK.
```

## Comparing `azure-cosmos-4.4.0b1/azure_cosmos.egg-info/SOURCES.txt` & `azure-cosmos-4.4.0b2/azure_cosmos.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -103,14 +103,15 @@
 samples/database_management_async.py
 samples/document_management.py
 samples/document_management_async.py
 samples/examples.py
 samples/examples_async.py
 samples/index_management.py
 samples/index_management_async.py
+samples/tracing_open_telemetry.py
 samples/MultiMasterOperations/Configurations.py
 samples/MultiMasterOperations/ConflictWorker.py
 samples/MultiMasterOperations/MultiMasterScenario.py
 samples/MultiMasterOperations/Program.py
 samples/MultiMasterOperations/Worker.py
 test/cleanup.py
 test/conftest.py
```

